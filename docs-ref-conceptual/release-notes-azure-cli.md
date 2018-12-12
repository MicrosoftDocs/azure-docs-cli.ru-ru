---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/20/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 7a2ab41dd6696d658d05ab76e44abf97626761aa
ms.sourcegitcommit: 14aa16beeec59e51890a6cba4906bdc8e19b94d0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2018
ms.locfileid: "52892689"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="f6a4d-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f6a4d-103">Azure CLI release notes</span></span>
## <a name="december-4-2018"></a><span data-ttu-id="f6a4d-104">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-104">December 4, 2018</span></span>

<span data-ttu-id="f6a4d-105">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="f6a4d-105">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="f6a4d-106">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-106">Core</span></span>
* <span data-ttu-id="f6a4d-107">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-107">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="f6a4d-108">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-108">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-109">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f6a4d-109">Appservice</span></span>
* <span data-ttu-id="f6a4d-110">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-110">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="f6a4d-111">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-111">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-112">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-112">Network</span></span>
* <span data-ttu-id="f6a4d-113">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-113">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="f6a4d-114">Роль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-114">Role</span></span>
* <span data-ttu-id="f6a4d-115">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-115">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="f6a4d-116">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-116">VM</span></span>
* <span data-ttu-id="f6a4d-117">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` устарел.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-117">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="f6a4d-118">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-118">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="f6a4d-119">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-119">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="f6a4d-120">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-120">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="f6a4d-121">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-121">November 20, 2018</span></span>

<span data-ttu-id="f6a4d-122">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="f6a4d-122">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="f6a4d-123">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-123">Core</span></span>
* <span data-ttu-id="f6a4d-124">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-124">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="f6a4d-125">ACR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-125">ACR</span></span>
* <span data-ttu-id="f6a4d-126">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-126">Added context token to task step</span></span>
* <span data-ttu-id="f6a4d-127">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-127">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="f6a4d-128">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-128">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-129">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f6a4d-129">Appservice</span></span>
* <span data-ttu-id="f6a4d-130">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-130">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="f6a4d-131">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-131">Updated the default `node_version`.</span></span> <span data-ttu-id="f6a4d-132">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-132">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="f6a4d-133">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-133">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="f6a4d-134">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-134">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="f6a4d-135">IotCentral</span><span class="sxs-lookup"><span data-stu-id="f6a4d-135">IotCentral</span></span>
* <span data-ttu-id="f6a4d-136">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-136">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6a4d-137">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-137">KeyVault</span></span>
* <span data-ttu-id="f6a4d-138">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-138">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-139">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-139">Network</span></span>
* <span data-ttu-id="f6a4d-140">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-140">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="f6a4d-141">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-141">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="f6a4d-142">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-142">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="f6a4d-143">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-143">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6a4d-144">Rdbms</span><span class="sxs-lookup"><span data-stu-id="f6a4d-144">Rdbms</span></span>
* <span data-ttu-id="f6a4d-145">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-145">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="f6a4d-146">RBAC:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-146">Rbac</span></span>
* <span data-ttu-id="f6a4d-147">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-147">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="f6a4d-148">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-148">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="f6a4d-149">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-149">Storage</span></span>
* <span data-ttu-id="f6a4d-150">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-150">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="f6a4d-151">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-151">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="f6a4d-152">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-152">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="f6a4d-153">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-153">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-154">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-154">VM</span></span>
* <span data-ttu-id="f6a4d-155">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-155">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="f6a4d-156">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-156">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="f6a4d-157">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-157">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="f6a4d-158">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-158">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="f6a4d-159">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-159">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="f6a4d-160">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-160">Added `snapshot wait` command</span></span>
* <span data-ttu-id="f6a4d-161">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-161">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="f6a4d-162">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-162">November 6, 2018</span></span>

<span data-ttu-id="f6a4d-163">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="f6a4d-163">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-164">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-164">Core</span></span>
* <span data-ttu-id="f6a4d-165">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-165">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="f6a4d-166">ACR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-166">ACR</span></span>
* <span data-ttu-id="f6a4d-167">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-167">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="f6a4d-168">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-168">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-169">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-169">ACS</span></span>
* <span data-ttu-id="f6a4d-170">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-170">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="f6a4d-171">Помощник</span><span class="sxs-lookup"><span data-stu-id="f6a4d-171">Advisor</span></span>
* <span data-ttu-id="f6a4d-172">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="f6a4d-172">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="f6a4d-173">AMS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-173">AMS</span></span>
* <span data-ttu-id="f6a4d-174">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-174">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="f6a4d-175">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-175">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="f6a4d-176">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-176">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="f6a4d-177">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-177">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="f6a4d-178">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-178">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="f6a4d-179">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-179">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="f6a4d-180">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-180">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="f6a4d-181">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-181">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="f6a4d-182">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-182">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="f6a4d-183">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-183">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="f6a4d-184">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-184">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="f6a4d-185">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-185">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="f6a4d-186">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-186">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="f6a4d-187">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-187">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="f6a4d-188">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-188">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="f6a4d-189">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-189">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="f6a4d-190">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-190">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-191">AppService</span><span class="sxs-lookup"><span data-stu-id="f6a4d-191">AppService</span></span>
* <span data-ttu-id="f6a4d-192">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-192">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="f6a4d-193">Настройка</span><span class="sxs-lookup"><span data-stu-id="f6a4d-193">Configure</span></span>
* <span data-ttu-id="f6a4d-194">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-194">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="f6a4d-195">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-195">Container</span></span>
* <span data-ttu-id="f6a4d-196">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-196">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="f6a4d-197">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-197">EventHub</span></span>
* <span data-ttu-id="f6a4d-198">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-198">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="f6a4d-199">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6a4d-199">Interactive</span></span>
* <span data-ttu-id="f6a4d-200">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-200">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="f6a4d-201">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f6a4d-201">Monitor</span></span>
* <span data-ttu-id="f6a4d-202">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-202">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-203">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-203">Network</span></span>
* <span data-ttu-id="f6a4d-204">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-204">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="f6a4d-205">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-205">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="f6a4d-206">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-206">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="f6a4d-207">Профиль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-207">Profile</span></span>
* <span data-ttu-id="f6a4d-208">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-208">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6a4d-209">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="f6a4d-209">RDBMS</span></span>
* <span data-ttu-id="f6a4d-210">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-210">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="f6a4d-211">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f6a4d-211">Resource</span></span>
* <span data-ttu-id="f6a4d-212">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-212">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="f6a4d-213">Роль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-213">Role</span></span>
* <span data-ttu-id="f6a4d-214">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-214">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="f6a4d-215">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-215">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="f6a4d-216">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-216">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-217">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-217">Storage</span></span>
* <span data-ttu-id="f6a4d-218">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-218">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-219">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-219">VM</span></span>
* <span data-ttu-id="f6a4d-220">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-220">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="f6a4d-221">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-221">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="f6a4d-222">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-222">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="f6a4d-223">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-223">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="f6a4d-224">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-224">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="f6a4d-225">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-225">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="f6a4d-226">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-226">October 23, 2018</span></span>

<span data-ttu-id="f6a4d-227">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="f6a4d-227">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-228">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-228">Core</span></span>
* <span data-ttu-id="f6a4d-229">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-229">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="f6a4d-230">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-230">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="f6a4d-231">ACR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-231">ACR</span></span>
* <span data-ttu-id="f6a4d-232">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-232">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="f6a4d-233">CDN</span><span class="sxs-lookup"><span data-stu-id="f6a4d-233">CDN</span></span>
* <span data-ttu-id="f6a4d-234">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-234">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="f6a4d-235">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-235">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="f6a4d-236">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-236">Container</span></span>
* <span data-ttu-id="f6a4d-237">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-237">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="f6a4d-238">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-238">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="f6a4d-239">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-239">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="f6a4d-240">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-240">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="f6a4d-241">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-241">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="f6a4d-242">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-242">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="f6a4d-243">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-243">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6a4d-244">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6a4d-244">CosmosDB</span></span>
* <span data-ttu-id="f6a4d-245">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-245">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="f6a4d-246">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6a4d-246">Interactive</span></span>
* <span data-ttu-id="f6a4d-247">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-247">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="f6a4d-248">IoT Central</span><span class="sxs-lookup"><span data-stu-id="f6a4d-248">IoT Central</span></span>
* <span data-ttu-id="f6a4d-249">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-249">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="f6a4d-250">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-250">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="f6a4d-251">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f6a4d-251">Monitor</span></span>
* <span data-ttu-id="f6a4d-252">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-252">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="f6a4d-253">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-253">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="f6a4d-254">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-254">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="f6a4d-255">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-255">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="f6a4d-256">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-256">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="f6a4d-257">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-257">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="f6a4d-258">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-258">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="f6a4d-259">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-259">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="f6a4d-260">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-260">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="f6a4d-261">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-261">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-262">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-262">Network</span></span>
* <span data-ttu-id="f6a4d-263">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-263">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="f6a4d-264">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-264">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="f6a4d-265">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="f6a4d-265">ServiceBus</span></span>
* <span data-ttu-id="f6a4d-266">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="f6a4d-266">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="f6a4d-267">SQL</span><span class="sxs-lookup"><span data-stu-id="f6a4d-267">SQL</span></span>
* <span data-ttu-id="f6a4d-268">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-268">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-269">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-269">Storage</span></span>
* <span data-ttu-id="f6a4d-270">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-270">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="f6a4d-271">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-271">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-272">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-272">VM</span></span>
* <span data-ttu-id="f6a4d-273">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-273">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="f6a4d-274">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-274">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="f6a4d-275">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="f6a4d-275">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="f6a4d-276">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-276">October 16, 2018</span></span>

<span data-ttu-id="f6a4d-277">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="f6a4d-277">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-278">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-278">VM</span></span>
* <span data-ttu-id="f6a4d-279">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-279">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="f6a4d-280">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-280">October 9, 2018</span></span>

<span data-ttu-id="f6a4d-281">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="f6a4d-281">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-282">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-282">Core</span></span>
* <span data-ttu-id="f6a4d-283">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-283">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="f6a4d-284">ACR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-284">ACR</span></span>
* <span data-ttu-id="f6a4d-285">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-285">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-286">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-286">ACS</span></span>
* <span data-ttu-id="f6a4d-287">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-287">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="f6a4d-288">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-288">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="f6a4d-289">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-289">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="f6a4d-290">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-290">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="f6a4d-291">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-291">Container</span></span>
* <span data-ttu-id="f6a4d-292">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-292">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="f6a4d-293">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-293">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="f6a4d-294">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="f6a4d-294">Event Hub</span></span>
* <span data-ttu-id="f6a4d-295">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-295">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="f6a4d-296">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-296">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="f6a4d-297">расширения.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-297">Extensions</span></span>
* <span data-ttu-id="f6a4d-298">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-298">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6a4d-299">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6a4d-299">HDInsight</span></span>
* <span data-ttu-id="f6a4d-300">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="f6a4d-300">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="f6a4d-301">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-301">IoT</span></span>
* <span data-ttu-id="f6a4d-302">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-302">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6a4d-303">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-303">KeyVault</span></span>
* <span data-ttu-id="f6a4d-304">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-304">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-305">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-305">Network</span></span>
* <span data-ttu-id="f6a4d-306">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-306">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="f6a4d-307">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-307">See #6052</span></span>
* <span data-ttu-id="f6a4d-308">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-308">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="f6a4d-309">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-309">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="f6a4d-310">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-310">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="f6a4d-311">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-311">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="f6a4d-312">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-312">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="f6a4d-313">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-313">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="f6a4d-314">Роль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-314">Role</span></span>
* <span data-ttu-id="f6a4d-315">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-315">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="f6a4d-316">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-316">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="f6a4d-317">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-317">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="f6a4d-318">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-318">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="f6a4d-319">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="f6a4d-319">Service Bus</span></span>
* <span data-ttu-id="f6a4d-320">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-320">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-321">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-321">VM</span></span>
* <span data-ttu-id="f6a4d-322">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-322">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="f6a4d-323">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-323">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="f6a4d-324">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-324">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="f6a4d-325">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-325">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="f6a4d-326">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-326">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="f6a4d-327">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-327">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="f6a4d-328">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-328">September 21, 2018</span></span>

<span data-ttu-id="f6a4d-329">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="f6a4d-329">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="f6a4d-330">ACR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-330">ACR</span></span>
* <span data-ttu-id="f6a4d-331">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-331">Added ACR Task commands</span></span>
* <span data-ttu-id="f6a4d-332">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-332">Added quick run command</span></span>
* <span data-ttu-id="f6a4d-333">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-333">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="f6a4d-334">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-334">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="f6a4d-335">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-335">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="f6a4d-336">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-336">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-337">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-337">ACS</span></span>
* <span data-ttu-id="f6a4d-338">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-338">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="f6a4d-339">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-339">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-340">AppService</span><span class="sxs-lookup"><span data-stu-id="f6a4d-340">AppService</span></span>

* <span data-ttu-id="f6a4d-341">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-341">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="f6a4d-342">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-342">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="f6a4d-343">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-343">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="f6a4d-344">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-344">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="f6a4d-345">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="f6a4d-345">Batch</span></span>
* <span data-ttu-id="f6a4d-346">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-346">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="f6a4d-347">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-347">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="f6a4d-348">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-348">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="f6a4d-349">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-349">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f6a4d-350">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="f6a4d-350">Batch AI</span></span> 
* <span data-ttu-id="f6a4d-351">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-351">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f6a4d-352">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f6a4d-352">Cognitive Services</span></span>
* <span data-ttu-id="f6a4d-353">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-353">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="f6a4d-354">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-354">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="f6a4d-355">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-355">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="f6a4d-356">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-356">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="f6a4d-357">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-357">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="f6a4d-358">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-358">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="f6a4d-359">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-359">Container</span></span>
* <span data-ttu-id="f6a4d-360">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-360">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="f6a4d-361">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-361">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="f6a4d-362">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-362">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="f6a4d-363">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-363">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="f6a4d-364">Data Lake</span><span class="sxs-lookup"><span data-stu-id="f6a4d-364">Datalake</span></span>
* <span data-ttu-id="f6a4d-365">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-365">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="f6a4d-366">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="f6a4d-366">Interactive Shell</span></span>
* <span data-ttu-id="f6a4d-367">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-367">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="f6a4d-368">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-368">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="f6a4d-369">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-369">IoT</span></span>
* <span data-ttu-id="f6a4d-370">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-370">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="f6a4d-371">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f6a4d-371">Key Vault</span></span>
* <span data-ttu-id="f6a4d-372">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-372">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-373">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-373">Network</span></span>
* <span data-ttu-id="f6a4d-374">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-374">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="f6a4d-375">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-375">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="f6a4d-376">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="f6a4d-376">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="f6a4d-377">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-377">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="f6a4d-378">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-378">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="f6a4d-379">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-379">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="f6a4d-380">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-380">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="f6a4d-381">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-381">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="f6a4d-382">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-382">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="f6a4d-383">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-383">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="f6a4d-384">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-384">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="f6a4d-385">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-385">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="f6a4d-386">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры`--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-386">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="f6a4d-387">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-387">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="f6a4d-388">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-388">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="f6a4d-389">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-389">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="f6a4d-390">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-390">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="f6a4d-391">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-391">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6a4d-392">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="f6a4d-392">RDBMS</span></span>
* <span data-ttu-id="f6a4d-393">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-393">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="f6a4d-394">резервирование.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-394">Reservation</span></span>
* <span data-ttu-id="f6a4d-395">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-395">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="f6a4d-396">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-396">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="f6a4d-397">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="f6a4d-397">Manage App</span></span>
* <span data-ttu-id="f6a4d-398">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-398">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="f6a4d-399">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-399">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="f6a4d-400">Роль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-400">Role</span></span>
* <span data-ttu-id="f6a4d-401">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-401">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="f6a4d-402">SignalR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-402">SignalR</span></span>
* <span data-ttu-id="f6a4d-403">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="f6a4d-403">First release</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-404">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-404">Storage</span></span>
* <span data-ttu-id="f6a4d-405">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-405">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="f6a4d-406">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-406">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-407">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-407">VM</span></span>
* <span data-ttu-id="f6a4d-408">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-408">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="f6a4d-409">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-409">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="f6a4d-410">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-410">August 28, 2018</span></span>

<span data-ttu-id="f6a4d-411">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="f6a4d-411">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-412">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-412">Core</span></span>

* <span data-ttu-id="f6a4d-413">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-413">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="f6a4d-414">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-414">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="f6a4d-415">ACR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-415">ACR</span></span>

* <span data-ttu-id="f6a4d-416">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-416">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="f6a4d-417">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-417">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-418">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-418">ACS</span></span>

* <span data-ttu-id="f6a4d-419">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-419">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="f6a4d-420">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-420">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-421">AppService</span><span class="sxs-lookup"><span data-stu-id="f6a4d-421">AppService</span></span>

* <span data-ttu-id="f6a4d-422">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-422">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="f6a4d-423">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-423">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="f6a4d-424">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-424">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="f6a4d-425">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="f6a4d-425">Backup</span></span>

* <span data-ttu-id="f6a4d-426">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-426">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="f6a4d-427">Служба Bot Service</span><span class="sxs-lookup"><span data-stu-id="f6a4d-427">Bot Service</span></span>

* <span data-ttu-id="f6a4d-428">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="f6a4d-428">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f6a4d-429">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f6a4d-429">Cognitive Services</span></span>

* <span data-ttu-id="f6a4d-430">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-430">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="f6a4d-431">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-431">IoT</span></span>

* <span data-ttu-id="f6a4d-432">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-432">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="f6a4d-433">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f6a4d-433">Monitor</span></span>

* <span data-ttu-id="f6a4d-434">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-434">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="f6a4d-435">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-435">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-436">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-436">Network</span></span>

* <span data-ttu-id="f6a4d-437">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-437">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="f6a4d-438">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f6a4d-438">Resource</span></span>

* <span data-ttu-id="f6a4d-439">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-439">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-440">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-440">Storage</span></span>

* <span data-ttu-id="f6a4d-441">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-441">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-442">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-442">VM</span></span>

* <span data-ttu-id="f6a4d-443">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-443">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="f6a4d-444">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-444">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="f6a4d-445">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-445">Auguest 14, 2018</span></span>

<span data-ttu-id="f6a4d-446">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="f6a4d-446">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-447">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-447">Core</span></span>

* <span data-ttu-id="f6a4d-448">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-448">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="f6a4d-449">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-449">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="f6a4d-450">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="f6a4d-450">Telemetry</span></span>

* <span data-ttu-id="f6a4d-451">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-451">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="f6a4d-452">ACR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-452">ACR</span></span>

* <span data-ttu-id="f6a4d-453">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-453">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="f6a4d-454">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-454">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-455">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-455">ACS</span></span>

* <span data-ttu-id="f6a4d-456">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-456">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="f6a4d-457">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-457">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="f6a4d-458">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-458">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="f6a4d-459">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-459">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="f6a4d-460">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-460">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="f6a4d-461">AppService</span><span class="sxs-lookup"><span data-stu-id="f6a4d-461">AppService</span></span>

* <span data-ttu-id="f6a4d-462">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-462">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="f6a4d-463">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-463">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="f6a4d-464">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f6a4d-464">BatchAI</span></span>

* <span data-ttu-id="f6a4d-465">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-465">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="f6a4d-466">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-466">Container</span></span>

* <span data-ttu-id="f6a4d-467">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-467">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="f6a4d-468">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-468">IoT</span></span>

* <span data-ttu-id="f6a4d-469">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-469">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="f6a4d-470">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-470">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="f6a4d-471">IoT Central</span><span class="sxs-lookup"><span data-stu-id="f6a4d-471">Iot Central</span></span>

* <span data-ttu-id="f6a4d-472">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="f6a4d-472">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6a4d-473">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-473">KeyVault</span></span>


* <span data-ttu-id="f6a4d-474">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-474">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="f6a4d-475">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-475">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="f6a4d-476">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-476">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="f6a4d-477">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-477">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="f6a4d-478">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-478">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="f6a4d-479">Передача</span><span class="sxs-lookup"><span data-stu-id="f6a4d-479">Relay</span></span>

* <span data-ttu-id="f6a4d-480">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="f6a4d-480">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="f6a4d-481">SQL</span><span class="sxs-lookup"><span data-stu-id="f6a4d-481">Sql</span></span>

* <span data-ttu-id="f6a4d-482">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-482">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-483">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-483">Storage</span></span>

* <span data-ttu-id="f6a4d-484">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-484">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="f6a4d-485">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-485">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="f6a4d-486">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-486">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="f6a4d-487">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-487">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="f6a4d-488">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-488">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-489">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-489">VM</span></span>

* <span data-ttu-id="f6a4d-490">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-490">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="f6a4d-491">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-491">July 31, 2018</span></span>

<span data-ttu-id="f6a4d-492">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="f6a4d-492">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="f6a4d-493">ACR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-493">ACR</span></span>

* <span data-ttu-id="f6a4d-494">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-494">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="f6a4d-495">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-495">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-496">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-496">ACS</span></span>

* <span data-ttu-id="f6a4d-497">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-497">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="f6a4d-498">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="f6a4d-498">Batch</span></span>

* <span data-ttu-id="f6a4d-499">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-499">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="f6a4d-500">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-500">Container</span></span>

* <span data-ttu-id="f6a4d-501">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-501">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-502">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-502">Network</span></span>

* <span data-ttu-id="f6a4d-503">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-503">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="f6a4d-504">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f6a4d-504">Resource</span></span>

* <span data-ttu-id="f6a4d-505">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-505">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="f6a4d-506">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-506">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="f6a4d-507">Роль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-507">Role</span></span>

* <span data-ttu-id="f6a4d-508">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-508">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="f6a4d-509">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-509">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="f6a4d-510">поиска</span><span class="sxs-lookup"><span data-stu-id="f6a4d-510">Search</span></span>

* <span data-ttu-id="f6a4d-511">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="f6a4d-511">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="f6a4d-512">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="f6a4d-512">Service Bus</span></span>

* <span data-ttu-id="f6a4d-513">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="f6a4d-513">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="f6a4d-514">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-514">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="f6a4d-515">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="f6a4d-515">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="f6a4d-516">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-516">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-517">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-517">Storage</span></span>

* <span data-ttu-id="f6a4d-518">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-518">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="f6a4d-519">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-519">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-520">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-520">VM</span></span>

* <span data-ttu-id="f6a4d-521">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-521">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="f6a4d-522">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-522">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="f6a4d-523">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-523">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="f6a4d-524">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-524">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="f6a4d-525">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-525">July 18, 2018</span></span>

<span data-ttu-id="f6a4d-526">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="f6a4d-526">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-527">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-527">Core</span></span>

* <span data-ttu-id="f6a4d-528">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-528">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="f6a4d-529">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-529">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="f6a4d-530">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-530">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="f6a4d-531">ACR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-531">ACR</span></span>

* <span data-ttu-id="f6a4d-532">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-532">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="f6a4d-533">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-533">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="f6a4d-534">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-534">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="f6a4d-535">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-535">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-536">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-536">ACS</span></span>

* <span data-ttu-id="f6a4d-537">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-537">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-538">AppService</span><span class="sxs-lookup"><span data-stu-id="f6a4d-538">AppService</span></span>

* <span data-ttu-id="f6a4d-539">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-539">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="f6a4d-540">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="f6a4d-540">Batch</span></span>

* <span data-ttu-id="f6a4d-541">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-541">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="f6a4d-542">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-542">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f6a4d-543">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="f6a4d-543">Batch AI</span></span>

* <span data-ttu-id="f6a4d-544">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-544">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="f6a4d-545">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-545">Container</span></span>

* <span data-ttu-id="f6a4d-546">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-546">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="f6a4d-547">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-547">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-548">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-548">Network</span></span>

* <span data-ttu-id="f6a4d-549">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-549">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="f6a4d-550">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-550">Added `network nic wait`</span></span>
* <span data-ttu-id="f6a4d-551">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-551">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="f6a4d-552">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-552">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="f6a4d-553">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f6a4d-553">Resource</span></span>

* <span data-ttu-id="f6a4d-554">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-554">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="f6a4d-555">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-555">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="f6a4d-556">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-556">Added `deployment wait` command</span></span>
* <span data-ttu-id="f6a4d-557">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-557">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="f6a4d-558">SQL</span><span class="sxs-lookup"><span data-stu-id="f6a4d-558">SQL</span></span>

* <span data-ttu-id="f6a4d-559">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-559">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="f6a4d-560">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-560">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="f6a4d-561">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-561">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-562">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-562">Storage</span></span>

* <span data-ttu-id="f6a4d-563">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-563">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-564">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-564">VM</span></span>

* <span data-ttu-id="f6a4d-565">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-565">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="f6a4d-566">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-566">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="f6a4d-567">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-567">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="f6a4d-568">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-568">July 3, 2018</span></span>

<span data-ttu-id="f6a4d-569">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="f6a4d-569">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="f6a4d-570">AKS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-570">AKS</span></span>

* <span data-ttu-id="f6a4d-571">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-571">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="f6a4d-572">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-572">July 3, 2018</span></span>

<span data-ttu-id="f6a4d-573">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="f6a4d-573">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-574">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-574">Core</span></span>

* <span data-ttu-id="f6a4d-575">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-575">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="f6a4d-576">ACR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-576">ACR</span></span>

* <span data-ttu-id="f6a4d-577">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-577">Added polling build status</span></span>
* <span data-ttu-id="f6a4d-578">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-578">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="f6a4d-579">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-579">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-580">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-580">ACS</span></span>

* <span data-ttu-id="f6a4d-581">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-581">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="f6a4d-582">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-582">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="f6a4d-583">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-583">Updated options for `aks browse` command.</span></span> <span data-ttu-id="f6a4d-584">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-584">Added `--listen-port` support</span></span>
* <span data-ttu-id="f6a4d-585">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-585">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="f6a4d-586">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-586">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="f6a4d-587">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-587">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-588">AppService</span><span class="sxs-lookup"><span data-stu-id="f6a4d-588">AppService</span></span>

* <span data-ttu-id="f6a4d-589">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-589">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="f6a4d-590">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-590">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="f6a4d-591">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="f6a4d-591">Backup</span></span>

* <span data-ttu-id="f6a4d-592">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-592">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="f6a4d-593">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f6a4d-593">BatchAI</span></span>

* <span data-ttu-id="f6a4d-594">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-594">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="f6a4d-595">Облако</span><span class="sxs-lookup"><span data-stu-id="f6a4d-595">Cloud</span></span>

* <span data-ttu-id="f6a4d-596">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-596">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="f6a4d-597">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-597">Container</span></span>

* <span data-ttu-id="f6a4d-598">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-598">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="f6a4d-599">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-599">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="f6a4d-600">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-600">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="f6a4d-601">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-601">Extension</span></span>

* <span data-ttu-id="f6a4d-602">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-602">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-603">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-603">Network</span></span>

* <span data-ttu-id="f6a4d-604">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-604">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6a4d-605">Rdbms</span><span class="sxs-lookup"><span data-stu-id="f6a4d-605">Rdbms</span></span>

* <span data-ttu-id="f6a4d-606">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-606">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="f6a4d-607">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f6a4d-607">Resource</span></span>

* <span data-ttu-id="f6a4d-608">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-608">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-609">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-609">VM</span></span>

* <span data-ttu-id="f6a4d-610">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-610">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="f6a4d-611">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-611">June 25, 2018</span></span>

<span data-ttu-id="f6a4d-612">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="f6a4d-612">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="f6a4d-613">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="f6a4d-613">CLI</span></span>

* <span data-ttu-id="f6a4d-614">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-614">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="f6a4d-615">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-615">June 19, 2018</span></span>

<span data-ttu-id="f6a4d-616">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="f6a4d-616">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-617">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-617">Core</span></span>

* <span data-ttu-id="f6a4d-618">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-618">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="f6a4d-619">ACR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-619">ACR</span></span>

* <span data-ttu-id="f6a4d-620">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-620">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="f6a4d-621">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-621">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-622">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-622">ACS</span></span>

* <span data-ttu-id="f6a4d-623">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-623">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="f6a4d-624">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-624">Added `--update` support</span></span>
* <span data-ttu-id="f6a4d-625">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-625">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="f6a4d-626">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-626">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="f6a4d-627">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-627">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="f6a4d-628">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-628">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="f6a4d-629">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-629">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="f6a4d-630">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-630">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-631">AppService</span><span class="sxs-lookup"><span data-stu-id="f6a4d-631">AppService</span></span>

* <span data-ttu-id="f6a4d-632">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-632">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="f6a4d-633">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-633">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="f6a4d-634">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="f6a4d-634">Batch</span></span>

* <span data-ttu-id="f6a4d-635">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-635">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f6a4d-636">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="f6a4d-636">Batch AI</span></span>

* <span data-ttu-id="f6a4d-637">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-637">Added support for workspaces.</span></span> <span data-ttu-id="f6a4d-638">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-638">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="f6a4d-639">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-639">Added support for experiments.</span></span> <span data-ttu-id="f6a4d-640">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-640">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="f6a4d-641">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-641">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="f6a4d-642">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-642">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="f6a4d-643">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-643">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="f6a4d-644">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-644">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="f6a4d-645">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-645">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="f6a4d-646">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-646">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="f6a4d-647">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-647">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="f6a4d-648">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-648">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="f6a4d-649">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-649">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="f6a4d-650">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-650">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="f6a4d-651">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-651">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="f6a4d-652">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-652">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="f6a4d-653">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-653">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="f6a4d-654">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-654">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="f6a4d-655">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="f6a4d-655">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="f6a4d-656">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="f6a4d-656">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="f6a4d-657">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="f6a4d-657">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="f6a4d-658">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="f6a4d-658">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="f6a4d-659">Карты</span><span class="sxs-lookup"><span data-stu-id="f6a4d-659">Maps</span></span>

* <span data-ttu-id="f6a4d-660">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-660">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-661">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-661">Network</span></span>

* <span data-ttu-id="f6a4d-662">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-662">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="f6a4d-663">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-663">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="f6a4d-664">#6502</span><span class="sxs-lookup"><span data-stu-id="f6a4d-664">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="f6a4d-665">Резервирование</span><span class="sxs-lookup"><span data-stu-id="f6a4d-665">Reservations</span></span>

* <span data-ttu-id="f6a4d-666">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-666">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="f6a4d-667">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-667">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="f6a4d-668">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-668">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="f6a4d-669">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-669">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="f6a4d-670">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-670">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="f6a4d-671">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-671">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="f6a4d-672">Роль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-672">Role</span></span>

* <span data-ttu-id="f6a4d-673">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-673">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="f6a4d-674">SQL</span><span class="sxs-lookup"><span data-stu-id="f6a4d-674">SQL</span></span>

* <span data-ttu-id="f6a4d-675">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-675">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-676">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-676">Storage</span></span>

* <span data-ttu-id="f6a4d-677">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-677">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-678">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-678">VM</span></span>

* <span data-ttu-id="f6a4d-679">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-679">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="f6a4d-680">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-680">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="f6a4d-681">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-681">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="f6a4d-682">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-682">June 13, 2018</span></span>

<span data-ttu-id="f6a4d-683">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="f6a4d-683">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-684">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-684">Core</span></span>

* <span data-ttu-id="f6a4d-685">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-685">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="f6a4d-686">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-686">June 13, 2018</span></span>

<span data-ttu-id="f6a4d-687">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="f6a4d-687">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="f6a4d-688">AKS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-688">AKS</span></span>

* <span data-ttu-id="f6a4d-689">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-689">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="f6a4d-690">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-690">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="f6a4d-691">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-691">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="f6a4d-692">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-692">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="f6a4d-693">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-693">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-694">AppService</span><span class="sxs-lookup"><span data-stu-id="f6a4d-694">AppService</span></span>

* <span data-ttu-id="f6a4d-695">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-695">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="f6a4d-696">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-696">June 5, 2018</span></span>

<span data-ttu-id="f6a4d-697">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="f6a4d-697">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="f6a4d-698">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6a4d-698">Interactive</span></span>

* <span data-ttu-id="f6a4d-699">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-699">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="f6a4d-700">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-700">June 5, 2018</span></span>

<span data-ttu-id="f6a4d-701">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="f6a4d-701">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-702">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-702">Core</span></span>

* <span data-ttu-id="f6a4d-703">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-703">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="f6a4d-704">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-704">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="f6a4d-705">ACR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-705">ACR</span></span>

* <span data-ttu-id="f6a4d-706">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-706">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="f6a4d-707">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-707">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="f6a4d-708">AKS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-708">AKS</span></span>

* <span data-ttu-id="f6a4d-709">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-709">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="f6a4d-710">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="f6a4d-710">Batch</span></span>

* <span data-ttu-id="f6a4d-711">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="f6a4d-711">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="f6a4d-712">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-712">IOT</span></span>

* <span data-ttu-id="f6a4d-713">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="f6a4d-713">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-714">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-714">Network</span></span>

* <span data-ttu-id="f6a4d-715">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-715">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="f6a4d-716">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="f6a4d-716">Policy Insights</span></span>

* <span data-ttu-id="f6a4d-717">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="f6a4d-717">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="f6a4d-718">ARM</span><span class="sxs-lookup"><span data-stu-id="f6a4d-718">ARM</span></span>

* <span data-ttu-id="f6a4d-719">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-719">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="f6a4d-720">SQL</span><span class="sxs-lookup"><span data-stu-id="f6a4d-720">SQL</span></span>

* <span data-ttu-id="f6a4d-721">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-721">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="f6a4d-722">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-722">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="f6a4d-723">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-723">Storage</span></span>

* <span data-ttu-id="f6a4d-724">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-724">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-725">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-725">VM</span></span>

* <span data-ttu-id="f6a4d-726">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-726">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="f6a4d-727">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-727">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="f6a4d-728">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-728">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="f6a4d-729">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-729">May 22, 2018</span></span>

<span data-ttu-id="f6a4d-730">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="f6a4d-730">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-731">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-731">Core</span></span>

* <span data-ttu-id="f6a4d-732">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-732">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-733">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-733">ACS</span></span>

* <span data-ttu-id="f6a4d-734">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-734">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="f6a4d-735">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-735">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-736">AppService</span><span class="sxs-lookup"><span data-stu-id="f6a4d-736">AppService</span></span>

* <span data-ttu-id="f6a4d-737">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-737">Improved generic update commands</span></span>
* <span data-ttu-id="f6a4d-738">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-738">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="f6a4d-739">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-739">Container</span></span>

* <span data-ttu-id="f6a4d-740">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-740">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="f6a4d-741">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-741">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="f6a4d-742">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-742">Extension</span></span>

* <span data-ttu-id="f6a4d-743">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-743">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="f6a4d-744">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6a4d-744">Interactive</span></span>

* <span data-ttu-id="f6a4d-745">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-745">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="f6a4d-746">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-746">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6a4d-747">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-747">KeyVault</span></span>

* <span data-ttu-id="f6a4d-748">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-748">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-749">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-749">Network</span></span>

* <span data-ttu-id="f6a4d-750">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="f6a4d-750">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="f6a4d-751">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="f6a4d-751">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="f6a4d-752">SQL</span><span class="sxs-lookup"><span data-stu-id="f6a4d-752">SQL</span></span>

* <span data-ttu-id="f6a4d-753">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-753">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="f6a4d-754">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-754">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="f6a4d-755">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-755">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="f6a4d-756">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-756">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="f6a4d-757">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-757">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="f6a4d-758">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-758">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="f6a4d-759">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-759">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="f6a4d-760">`edition`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-760">`edition`.</span></span> <span data-ttu-id="f6a4d-761">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-761">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="f6a4d-762">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-762">`elasticPoolName`.</span></span> <span data-ttu-id="f6a4d-763">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-763">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="f6a4d-764">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-764">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="f6a4d-765">`edition`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-765">`edition`.</span></span> <span data-ttu-id="f6a4d-766">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-766">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="f6a4d-767">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-767">`dtu`.</span></span> <span data-ttu-id="f6a4d-768">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-768">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="f6a4d-769">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-769">`databaseDtuMin`.</span></span> <span data-ttu-id="f6a4d-770">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-770">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="f6a4d-771">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-771">`databaseDtuMax`.</span></span> <span data-ttu-id="f6a4d-772">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-772">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="f6a4d-773">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-773">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="f6a4d-774">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-774">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-775">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-775">Storage</span></span>

* <span data-ttu-id="f6a4d-776">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-776">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="f6a4d-777">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-777">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-778">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-778">VM</span></span>

* <span data-ttu-id="f6a4d-779">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-779">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="f6a4d-780">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-780">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="f6a4d-781">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-781">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="f6a4d-782">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-782">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="f6a4d-783">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-783">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="f6a4d-784">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-784">May 7, 2018</span></span>

<span data-ttu-id="f6a4d-785">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="f6a4d-785">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-786">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-786">Core</span></span>

* <span data-ttu-id="f6a4d-787">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-787">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="f6a4d-788">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-788">Added limited support for positional arguments</span></span>
* <span data-ttu-id="f6a4d-789">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-789">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="f6a4d-790">#5591</span><span class="sxs-lookup"><span data-stu-id="f6a4d-790">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="f6a4d-791">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-791">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="f6a4d-792">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-792">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="f6a4d-793">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-793">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="f6a4d-794">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-794">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="f6a4d-795">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-795">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="f6a4d-796">ACR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-796">ACR</span></span>

* <span data-ttu-id="f6a4d-797">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-797">Added ACR Build commands</span></span>
* <span data-ttu-id="f6a4d-798">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-798">Improved resource not found error messages</span></span>
* <span data-ttu-id="f6a4d-799">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-799">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="f6a4d-800">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-800">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="f6a4d-801">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-801">Improved repository commands error messages</span></span>
* <span data-ttu-id="f6a4d-802">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-802">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-803">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-803">ACS</span></span>

* <span data-ttu-id="f6a4d-804">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-804">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="f6a4d-805">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-805">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="f6a4d-806">AMS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-806">AMS</span></span>

* <span data-ttu-id="f6a4d-807">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-807">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-808">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f6a4d-808">Appservice</span></span>

* <span data-ttu-id="f6a4d-809">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-809">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="f6a4d-810">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-810">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="f6a4d-811">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-811">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="f6a4d-812">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-812">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f6a4d-813">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="f6a4d-813">Batch AI</span></span>

* <span data-ttu-id="f6a4d-814">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-814">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f6a4d-815">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f6a4d-815">Cognitive Services</span></span>

* <span data-ttu-id="f6a4d-816">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-816">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="f6a4d-817">Потребление</span><span class="sxs-lookup"><span data-stu-id="f6a4d-817">Consumption</span></span>

* <span data-ttu-id="f6a4d-818">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-818">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="f6a4d-819">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-819">Container</span></span>

* <span data-ttu-id="f6a4d-820">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-820">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="f6a4d-821">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="f6a4d-821">Cosmos DB</span></span>

* <span data-ttu-id="f6a4d-822">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6a4d-822">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="f6a4d-823">DMS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-823">DMS</span></span>

* <span data-ttu-id="f6a4d-824">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-824">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="f6a4d-825">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-825">Extension</span></span>

* <span data-ttu-id="f6a4d-826">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-826">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="f6a4d-827">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6a4d-827">Interactive</span></span>

* <span data-ttu-id="f6a4d-828">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-828">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="f6a4d-829">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-829">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="f6a4d-830">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-830">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="f6a4d-831">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-831">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="f6a4d-832">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="f6a4d-832">Lab</span></span>

* <span data-ttu-id="f6a4d-833">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-833">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-834">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-834">Network</span></span>

* <span data-ttu-id="f6a4d-835">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-835">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="f6a4d-836">Профиль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-836">Profile</span></span>

* <span data-ttu-id="f6a4d-837">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-837">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="f6a4d-838">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-838">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="f6a4d-839">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-839">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="f6a4d-840">Redis</span><span class="sxs-lookup"><span data-stu-id="f6a4d-840">Redis</span></span>

* <span data-ttu-id="f6a4d-841">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-841">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="f6a4d-842">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-842">Deprecated `redis list-all`.</span></span> <span data-ttu-id="f6a4d-843">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-843">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="f6a4d-844">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-844">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="f6a4d-845">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-845">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="f6a4d-846">Роль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-846">Role</span></span>

* <span data-ttu-id="f6a4d-847">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-847">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-848">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-848">Storage</span></span>

* <span data-ttu-id="f6a4d-849">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-849">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="f6a4d-850">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-850">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="f6a4d-851">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-851">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="f6a4d-852">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="f6a4d-852">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="f6a4d-853">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="f6a4d-853">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-854">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-854">VM</span></span>

* <span data-ttu-id="f6a4d-855">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-855">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="f6a4d-856">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-856">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="f6a4d-857">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-857">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="f6a4d-858">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-858">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="f6a4d-859">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-859">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="f6a4d-860">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-860">Added write accelerator support</span></span>
* <span data-ttu-id="f6a4d-861">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-861">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="f6a4d-862">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-862">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="f6a4d-863">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-863">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="f6a4d-864">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-864">April 10, 2018</span></span>

<span data-ttu-id="f6a4d-865">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="f6a4d-865">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="f6a4d-866">ACR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-866">ACR</span></span>

* <span data-ttu-id="f6a4d-867">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-867">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-868">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-868">ACS</span></span>

* <span data-ttu-id="f6a4d-869">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-869">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-870">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f6a4d-870">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="f6a4d-872">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-872">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="f6a4d-873">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f6a4d-873">BatchAI</span></span>

* <span data-ttu-id="f6a4d-874">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-874">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="f6a4d-875">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-875">Job level mounting</span></span>
  - <span data-ttu-id="f6a4d-876">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-876">Environment variables with secret values</span></span>
  - <span data-ttu-id="f6a4d-877">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="f6a4d-877">Performance counters settings</span></span>
  - <span data-ttu-id="f6a4d-878">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-878">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="f6a4d-879">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-879">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="f6a4d-880">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-880">Usage and limits reporting</span></span>
  - <span data-ttu-id="f6a4d-881">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-881">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="f6a4d-882">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-882">Support for custom images</span></span>
  - <span data-ttu-id="f6a4d-883">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-883">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="f6a4d-884">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-884">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="f6a4d-885">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-885">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="f6a4d-886">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-886">National clouds are supported</span></span>
* <span data-ttu-id="f6a4d-887">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-887">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="f6a4d-888">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-888">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="f6a4d-889">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-889">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="f6a4d-890">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-890">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="f6a4d-891">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-891">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="f6a4d-892">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-892">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="f6a4d-893">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-893">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="f6a4d-894">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-894">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="f6a4d-895">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-895">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="f6a4d-896">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-896">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="f6a4d-897">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-897">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="f6a4d-898">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-898">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="f6a4d-899">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-899">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="f6a4d-900">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="f6a4d-900">Billing</span></span>

* <span data-ttu-id="f6a4d-901">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-901">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="f6a4d-902">Потребление</span><span class="sxs-lookup"><span data-stu-id="f6a4d-902">Consumption</span></span>

* <span data-ttu-id="f6a4d-903">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-903">Added `marketplace` commands</span></span>
* <span data-ttu-id="f6a4d-904">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-904">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="f6a4d-905">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-905">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="f6a4d-906">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-906">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="f6a4d-907">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-907">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="f6a4d-908">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-908">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="f6a4d-909">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-909">Container</span></span>

* <span data-ttu-id="f6a4d-910">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-910">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="f6a4d-911">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-911">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="f6a4d-912">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-912">Extension</span></span>

* <span data-ttu-id="f6a4d-913">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-913">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="f6a4d-914">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6a4d-914">Interactive</span></span>

* <span data-ttu-id="f6a4d-915">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-915">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="f6a4d-916">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-916">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="f6a4d-917">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-917">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-918">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-918">Network</span></span>

* <span data-ttu-id="f6a4d-919">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-919">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="f6a4d-920">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-920">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="f6a4d-921">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-921">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="f6a4d-922">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-922">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="f6a4d-923">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-923">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="f6a4d-924">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-924">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="f6a4d-925">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-925">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="f6a4d-926">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-926">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="f6a4d-927">Профиль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-927">Profile</span></span>

* <span data-ttu-id="f6a4d-928">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-928">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="f6a4d-929">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-929">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6a4d-930">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="f6a4d-930">RDBMS</span></span>

* <span data-ttu-id="f6a4d-931">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-931">Added `georestore` command</span></span>
* <span data-ttu-id="f6a4d-932">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-932">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="f6a4d-933">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f6a4d-933">Resource</span></span>

* <span data-ttu-id="f6a4d-934">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-934">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="f6a4d-935">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-935">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="f6a4d-936">SQL</span><span class="sxs-lookup"><span data-stu-id="f6a4d-936">SQL</span></span>

* <span data-ttu-id="f6a4d-937">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-937">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-938">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-938">Storage</span></span>

* <span data-ttu-id="f6a4d-939">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-939">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-940">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-940">VM</span></span>

* <span data-ttu-id="f6a4d-941">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-941">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="f6a4d-942">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-942">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="f6a4d-944">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-944">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="f6a4d-945">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-945">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="f6a4d-946">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-946">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="f6a4d-947">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-947">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="f6a4d-948">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-948">March 27, 2018</span></span>

<span data-ttu-id="f6a4d-949">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="f6a4d-949">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-950">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-950">Core</span></span>

* <span data-ttu-id="f6a4d-951">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-951">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-952">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-952">ACS</span></span>

* <span data-ttu-id="f6a4d-953">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-953">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-954">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f6a4d-954">Appservice</span></span>

* <span data-ttu-id="f6a4d-955">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-955">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="f6a4d-956">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-956">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="f6a4d-957">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="f6a4d-957">Backup</span></span>

* <span data-ttu-id="f6a4d-958">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-958">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="f6a4d-959">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-959">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="f6a4d-960">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-960">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="f6a4d-961">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-961">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="f6a4d-962">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-962">Container</span></span>

* <span data-ttu-id="f6a4d-963">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-963">Added `container exec` command.</span></span> <span data-ttu-id="f6a4d-964">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-964">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="f6a4d-965">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-965">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="f6a4d-966">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-966">Extension</span></span>

* <span data-ttu-id="f6a4d-967">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-967">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="f6a4d-968">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-968">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="f6a4d-969">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-969">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="f6a4d-970">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6a4d-970">Interactive</span></span>

* <span data-ttu-id="f6a4d-971">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-971">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="f6a4d-972">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-972">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="f6a4d-973">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-973">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="f6a4d-974">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-974">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="f6a4d-975">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="f6a4d-975">Lab</span></span>

* <span data-ttu-id="f6a4d-976">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-976">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="f6a4d-977">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f6a4d-977">Monitor</span></span>

* <span data-ttu-id="f6a4d-978">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-978">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="f6a4d-979">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-979">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="f6a4d-980">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-980">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-981">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-981">Network</span></span>

* <span data-ttu-id="f6a4d-982">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-982">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="f6a4d-983">Профиль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-983">Profile</span></span>

* <span data-ttu-id="f6a4d-984">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-984">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6a4d-985">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="f6a4d-985">RDBMS</span></span>

* <span data-ttu-id="f6a4d-986">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-986">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="f6a4d-987">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f6a4d-987">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="f6a4d-989">Роль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-989">Role</span></span>

* <span data-ttu-id="f6a4d-990">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-990">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="f6a4d-991">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-991">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="f6a4d-992">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-992">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="f6a4d-993">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-993">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="f6a4d-994">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-994">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-995">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-995">Storage</span></span>

* <span data-ttu-id="f6a4d-996">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-996">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="f6a4d-997">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049): проблемы, когда при отправке добавочного большого двоичного объекта игнорируются параметры условия.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-997">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-998">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-998">VM</span></span>

* <span data-ttu-id="f6a4d-999">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-999">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="f6a4d-1000">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1000">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="f6a4d-1001">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1001">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="f6a4d-1002">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1002">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="f6a4d-1003">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1003">March 13, 2018</span></span>

<span data-ttu-id="f6a4d-1004">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1004">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="f6a4d-1005">ACR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1005">ACR</span></span>

* <span data-ttu-id="f6a4d-1006">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1006">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="f6a4d-1007">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1007">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="f6a4d-1008">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1008">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-1009">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1009">ACS</span></span>

* <span data-ttu-id="f6a4d-1010">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1010">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="f6a4d-1011">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1011">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="f6a4d-1012">Помощник</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1012">Advisor</span></span>

* <span data-ttu-id="f6a4d-1013">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1013">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="f6a4d-1014">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1014">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="f6a4d-1015">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1015">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="f6a4d-1016">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1016">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="f6a4d-1017">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1017">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-1018">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1018">Appservice</span></span>

* <span data-ttu-id="f6a4d-1019">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1019">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="f6a4d-1020">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1020">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="f6a4d-1021">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1021">Eventhubs</span></span>

* <span data-ttu-id="f6a4d-1022">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1022">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="f6a4d-1023">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1023">Extension</span></span>

* <span data-ttu-id="f6a4d-1024">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1024">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="f6a4d-1025">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1025">Interactive</span></span>

* <span data-ttu-id="f6a4d-1026">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625): теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1026">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="f6a4d-1027">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016): при использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1027">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="f6a4d-1028">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688): если при загрузке таблицы команд возникало исключение, опережающий ввод не выполнялся.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1028">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="f6a4d-1029">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1029">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="f6a4d-1030">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1030">Monitor</span></span>

* <span data-ttu-id="f6a4d-1031">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1031">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="f6a4d-1032">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1032">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="f6a4d-1033">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1033">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="f6a4d-1034">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1034">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-1035">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1035">Network</span></span>

* <span data-ttu-id="f6a4d-1036">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1036">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="f6a4d-1037">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1037">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="f6a4d-1038">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1038">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="f6a4d-1039">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1039">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="f6a4d-1040">Профиль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1040">Profile</span></span>

* <span data-ttu-id="f6a4d-1041">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1041">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="f6a4d-1042">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1042">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6a4d-1043">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1043">RDBMS</span></span>

* <span data-ttu-id="f6a4d-1044">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1044">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="f6a4d-1045">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1045">Service Bus</span></span>

* <span data-ttu-id="f6a4d-1046">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1046">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-1047">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1047">Storage</span></span>

* <span data-ttu-id="f6a4d-1048">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1048">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="f6a4d-1049">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286): при пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1049">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-1050">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1050">VM</span></span>

* <span data-ttu-id="f6a4d-1051">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1051">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="f6a4d-1052">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1052">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="f6a4d-1053">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1053">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="f6a4d-1054">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1054">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="f6a4d-1055">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1055">February 27, 2018</span></span>

<span data-ttu-id="f6a4d-1056">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1056">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-1057">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1057">Core</span></span>

* <span data-ttu-id="f6a4d-1058">Исправлена ошибка с установкой Homebrew [#5184](https://github.com/Azure/azure-cli/issues/5184).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1058">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="f6a4d-1059">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1059">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="f6a4d-1060">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1060">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-1061">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1061">ACS</span></span>

* <span data-ttu-id="f6a4d-1062">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1062">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="f6a4d-1063">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1063">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="f6a4d-1064">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1064">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="f6a4d-1065">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1065">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-1066">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1066">Appservice</span></span>

* <span data-ttu-id="f6a4d-1067">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1067">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="f6a4d-1068">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1068">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f6a4d-1069">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1069">Cognitive Services</span></span>

* <span data-ttu-id="f6a4d-1070">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1070">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="f6a4d-1071">Потребление</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1071">Consumption</span></span>

* <span data-ttu-id="f6a4d-1072">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1072">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="f6a4d-1073">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1073">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="f6a4d-1074">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1074">Container</span></span>

* <span data-ttu-id="f6a4d-1075">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1075">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-1076">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1076">Network</span></span>

* <span data-ttu-id="f6a4d-1077">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559): отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1077">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="f6a4d-1078">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1078">Resource</span></span>

* <span data-ttu-id="f6a4d-1079">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1079">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="f6a4d-1080">Роль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1080">Role</span></span>

* <span data-ttu-id="f6a4d-1081">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1081">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="f6a4d-1082">SQL</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1082">SQL</span></span>

* <span data-ttu-id="f6a4d-1083">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1083">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-1084">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1084">Storage</span></span>

* <span data-ttu-id="f6a4d-1085">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1085">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-1086">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1086">VM</span></span>

* <span data-ttu-id="f6a4d-1087">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1087">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="f6a4d-1088">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1088">February 13, 2018</span></span>

<span data-ttu-id="f6a4d-1089">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1089">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-1090">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1090">Core</span></span>

* <span data-ttu-id="f6a4d-1091">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1091">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-1092">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1092">ACS</span></span>

* <span data-ttu-id="f6a4d-1093">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1093">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="f6a4d-1094">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1094">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="f6a4d-1095">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1095">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="f6a4d-1096">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1096">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="f6a4d-1097">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1097">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="f6a4d-1098">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1098">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="f6a4d-1099">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1099">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="f6a4d-1100">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1100">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-1101">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1101">Appservice</span></span>

* <span data-ttu-id="f6a4d-1102">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1102">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="f6a4d-1103">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1103">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="f6a4d-1104">CDN</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1104">CDN</span></span>

* <span data-ttu-id="f6a4d-1105">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1105">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="f6a4d-1106">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1106">Container</span></span>

* <span data-ttu-id="f6a4d-1107">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1107">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="f6a4d-1108">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1108">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6a4d-1109">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1109">CosmosDB</span></span>

* <span data-ttu-id="f6a4d-1110">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1110">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="f6a4d-1111">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1111">Extension</span></span>

* <span data-ttu-id="f6a4d-1112">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1112">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="f6a4d-1113">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1113">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="f6a4d-1114">Отзыв</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1114">Feedback</span></span>

* <span data-ttu-id="f6a4d-1115">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1115">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="f6a4d-1116">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1116">Interactive</span></span>

* <span data-ttu-id="f6a4d-1117">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1117">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="f6a4d-1118">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1118">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="f6a4d-1119">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1119">IoT</span></span>

* <span data-ttu-id="f6a4d-1120">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1120">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="f6a4d-1121">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1121">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="f6a4d-1122">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1122">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="f6a4d-1123">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1123">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="f6a4d-1124">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1124">Monitor</span></span>

* <span data-ttu-id="f6a4d-1125">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1125">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-1126">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1126">Network</span></span>

* <span data-ttu-id="f6a4d-1127">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1127">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="f6a4d-1128">Профиль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1128">Profile</span></span>

* <span data-ttu-id="f6a4d-1129">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1129">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="f6a4d-1130">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1130">Resource</span></span>

* <span data-ttu-id="f6a4d-1131">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1131">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="f6a4d-1132">Роль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1132">Role</span></span>

* <span data-ttu-id="f6a4d-1133">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1133">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="f6a4d-1134">SQL</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1134">SQL</span></span>

* <span data-ttu-id="f6a4d-1135">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1135">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="f6a4d-1136">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1136">Added `sql db rename`</span></span>
* <span data-ttu-id="f6a4d-1137">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1137">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-1138">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1138">Storage</span></span>

* <span data-ttu-id="f6a4d-1139">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1139">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-1140">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1140">VM</span></span>

* <span data-ttu-id="f6a4d-1141">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1141">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="f6a4d-1142">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1142">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="f6a4d-1143">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1143">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="f6a4d-1144">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1144">January 31, 2018</span></span>

<span data-ttu-id="f6a4d-1145">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1145">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-1146">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1146">Core</span></span>

* <span data-ttu-id="f6a4d-1147">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1147">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="f6a4d-1148">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1148">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="f6a4d-1149">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1149">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="f6a4d-1150">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1150">Use `--verbose` to see</span></span>
* <span data-ttu-id="f6a4d-1151">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1151">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-1152">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1152">ACS</span></span>

* <span data-ttu-id="f6a4d-1153">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1153">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="f6a4d-1154">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1154">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-1155">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1155">Appservice</span></span>

* <span data-ttu-id="f6a4d-1156">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1156">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="f6a4d-1157">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1157">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="f6a4d-1158">CDN</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1158">CDN</span></span>

* <span data-ttu-id="f6a4d-1159">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1159">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6a4d-1160">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1160">CosmosDB</span></span>

* <span data-ttu-id="f6a4d-1161">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1161">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="f6a4d-1162">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1162">Interactive</span></span>

* <span data-ttu-id="f6a4d-1163">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1163">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-1164">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1164">Network</span></span>

* <span data-ttu-id="f6a4d-1165">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1165">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="f6a4d-1166">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1166">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="f6a4d-1167">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1167">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="f6a4d-1168">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1168">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="f6a4d-1169">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1169">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="f6a4d-1170">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1170">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="f6a4d-1171">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1171">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="f6a4d-1172">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1172">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="f6a4d-1173">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1173">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="f6a4d-1174">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1174">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="f6a4d-1175">Профиль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1175">Profile</span></span>

* <span data-ttu-id="f6a4d-1176">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1176">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="f6a4d-1177">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1177">Resource</span></span>

* <span data-ttu-id="f6a4d-1178">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1178">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-1179">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1179">Storage</span></span>

* <span data-ttu-id="f6a4d-1180">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1180">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="f6a4d-1181">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1181">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="f6a4d-1182">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1182">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="f6a4d-1183">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1183">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="f6a4d-1184">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1184">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-1185">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1185">VM</span></span>

* <span data-ttu-id="f6a4d-1186">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1186">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="f6a4d-1187">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1187">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="f6a4d-1188">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1188">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="f6a4d-1189">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1189">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="f6a4d-1190">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1190">January 17, 2018</span></span>

<span data-ttu-id="f6a4d-1191">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1191">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="f6a4d-1192">ACR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1192">ACR</span></span>

* <span data-ttu-id="f6a4d-1193">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1193">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="f6a4d-1194">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1194">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-1195">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1195">ACS</span></span>

* <span data-ttu-id="f6a4d-1196">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1196">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="f6a4d-1197">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1197">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-1198">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1198">Appservice</span></span>

* <span data-ttu-id="f6a4d-1199">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1199">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="f6a4d-1200">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1200">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="f6a4d-1201">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1201">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="f6a4d-1202">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1202">Backup</span></span>

* <span data-ttu-id="f6a4d-1203">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1203">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="f6a4d-1204">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1204">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="f6a4d-1205">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1205">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="f6a4d-1206">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1206">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="f6a4d-1207">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1207">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="f6a4d-1208">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1208">Batch</span></span>

* <span data-ttu-id="f6a4d-1209">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1209">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="f6a4d-1210">Облако</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1210">Cloud</span></span>

* <span data-ttu-id="f6a4d-1211">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1211">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="f6a4d-1212">Потребление</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1212">Consumption</span></span>

* <span data-ttu-id="f6a4d-1213">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1213">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="f6a4d-1214">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1214">Event Grid</span></span>

* <span data-ttu-id="f6a4d-1215">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1215">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="f6a4d-1216">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1216">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="f6a4d-1217">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1217">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="f6a4d-1218">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1218">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="f6a4d-1219">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1219">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="f6a4d-1220">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1220">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="f6a4d-1221">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1221">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="f6a4d-1222">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1222">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="f6a4d-1223">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1223">Interactive</span></span>

* <span data-ttu-id="f6a4d-1224">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1224">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="f6a4d-1225">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1225">Fixed errors on startup</span></span>
* <span data-ttu-id="f6a4d-1226">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1226">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="f6a4d-1227">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1227">IoT</span></span>

* <span data-ttu-id="f6a4d-1228">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1228">Added support for device provisioning service</span></span>
* <span data-ttu-id="f6a4d-1229">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1229">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="f6a4d-1230">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1230">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="f6a4d-1231">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1231">Monitor</span></span>

* <span data-ttu-id="f6a4d-1232">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1232">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="f6a4d-1233">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1233">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="f6a4d-1234">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1234">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-1235">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1235">Network</span></span>

* <span data-ttu-id="f6a4d-1236">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1236">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="f6a4d-1237">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1237">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="f6a4d-1238">Профиль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1238">Profile</span></span>

* <span data-ttu-id="f6a4d-1239">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1239">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="f6a4d-1240">Роль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1240">Role</span></span>

* <span data-ttu-id="f6a4d-1241">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1241">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f6a4d-1242">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1242">Service Fabric</span></span>

* <span data-ttu-id="f6a4d-1243">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1243">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="f6a4d-1244">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1244">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-1245">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1245">VM</span></span>

* <span data-ttu-id="f6a4d-1246">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1246">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="f6a4d-1247">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1247">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="f6a4d-1248">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1248">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="f6a4d-1249">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1249">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="f6a4d-1250">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1250">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="f6a4d-1251">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1251">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="f6a4d-1252">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1252">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="f6a4d-1253">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1253">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="f6a4d-1254">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1254">December 19, 2017</span></span>

<span data-ttu-id="f6a4d-1255">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1255">Version 2.0.23</span></span>

* <span data-ttu-id="f6a4d-1256">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1256">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="f6a4d-1257">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1257">Container</span></span>

* <span data-ttu-id="f6a4d-1258">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1258">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-1259">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1259">Network</span></span>

* <span data-ttu-id="f6a4d-1260">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1260">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="f6a4d-1261">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1261">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-1262">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1262">Storage</span></span>

* <span data-ttu-id="f6a4d-1263">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1263">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-1264">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1264">VM</span></span>

* <span data-ttu-id="f6a4d-1265">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1265">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="f6a4d-1266">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1266">December 5, 2017</span></span>

<span data-ttu-id="f6a4d-1267">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1267">Version 2.0.22</span></span>

* <span data-ttu-id="f6a4d-1268">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1268">Removed `az component` commands.</span></span> <span data-ttu-id="f6a4d-1269">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1269">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-1270">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1270">Core</span></span>
* <span data-ttu-id="f6a4d-1271">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1271">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="f6a4d-1272">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1272">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-1273">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1273">ACS</span></span>

* <span data-ttu-id="f6a4d-1274">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1274">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="f6a4d-1275">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1275">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="f6a4d-1276">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1276">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="f6a4d-1277">Помощник</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1277">Advisor</span></span>

* <span data-ttu-id="f6a4d-1278">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1278">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-1279">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1279">Appservice</span></span>

* <span data-ttu-id="f6a4d-1280">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1280">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="f6a4d-1281">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1281">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="f6a4d-1282">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1282">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="f6a4d-1283">Потребление</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1283">Consumption</span></span>

* <span data-ttu-id="f6a4d-1284">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1284">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="f6a4d-1285">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1285">Container</span></span>

* <span data-ttu-id="f6a4d-1286">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1286">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="f6a4d-1287">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1287">Monitor</span></span>

* <span data-ttu-id="f6a4d-1288">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1288">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="f6a4d-1289">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1289">Resource</span></span>

* <span data-ttu-id="f6a4d-1290">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1290">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="f6a4d-1291">Роль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1291">Role</span></span>

* <span data-ttu-id="f6a4d-1292">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1292">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="f6a4d-1293">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1293">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="f6a4d-1294">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1294">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="f6a4d-1295">SQL</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1295">SQL</span></span>

* <span data-ttu-id="f6a4d-1296">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1296">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="f6a4d-1297">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1297">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-1298">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1298">VM</span></span>

* <span data-ttu-id="f6a4d-1299">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1299">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="f6a4d-1300">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1300">November 14, 2017</span></span>

<span data-ttu-id="f6a4d-1301">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1301">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="f6a4d-1302">ACR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1302">ACR</span></span>

* <span data-ttu-id="f6a4d-1303">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1303">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="f6a4d-1304">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1304">ACS</span></span>

* <span data-ttu-id="f6a4d-1305">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1305">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="f6a4d-1306">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1306">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="f6a4d-1307">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1307">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="f6a4d-1308">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1308">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="f6a4d-1309">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1309">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-1310">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1310">Appservice</span></span>

* <span data-ttu-id="f6a4d-1311">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1311">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="f6a4d-1312">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1312">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="f6a4d-1313">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1313">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="f6a4d-1314">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1314">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="f6a4d-1315">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1315">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="f6a4d-1316">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1316">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="f6a4d-1317">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1317">Batch</span></span>

* <span data-ttu-id="f6a4d-1318">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1318">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="f6a4d-1319">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1319">Batchai</span></span>

* <span data-ttu-id="f6a4d-1320">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1320">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="f6a4d-1321">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1321">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="f6a4d-1322">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1322">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="f6a4d-1323">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1323">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="f6a4d-1324">Облако</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1324">Cloud</span></span>

* <span data-ttu-id="f6a4d-1325">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1325">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="f6a4d-1326">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1326">Container</span></span>

* <span data-ttu-id="f6a4d-1327">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1327">Added support to open multiple ports</span></span>
* <span data-ttu-id="f6a4d-1328">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1328">Added container group restart policy</span></span>
* <span data-ttu-id="f6a4d-1329">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1329">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="f6a4d-1330">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1330">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f6a4d-1331">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1331">Data Lake Analytics</span></span>

* <span data-ttu-id="f6a4d-1332">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1332">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f6a4d-1333">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1333">Data Lake Store</span></span>

* <span data-ttu-id="f6a4d-1334">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1334">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="f6a4d-1335">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1335">Extension</span></span>

* <span data-ttu-id="f6a4d-1336">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1336">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="f6a4d-1337">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1337">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="f6a4d-1338">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1338">IoT</span></span>

* <span data-ttu-id="f6a4d-1339">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1339">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="f6a4d-1340">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1340">Monitor</span></span>

* <span data-ttu-id="f6a4d-1341">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1341">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-1342">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1342">Network</span></span>

* <span data-ttu-id="f6a4d-1343">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1343">Added support for CAA DNS records</span></span>
* <span data-ttu-id="f6a4d-1344">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1344">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="f6a4d-1345">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1345">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="f6a4d-1346">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1346">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="f6a4d-1347">Резервирование</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1347">Reservations</span></span>

* <span data-ttu-id="f6a4d-1348">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1348">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="f6a4d-1349">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1349">Resource</span></span>

* <span data-ttu-id="f6a4d-1350">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1350">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="f6a4d-1351">SQL</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1351">SQL</span></span>

* <span data-ttu-id="f6a4d-1352">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1352">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-1353">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1353">Storage</span></span>

* <span data-ttu-id="f6a4d-1354">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1354">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="f6a4d-1355">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1355">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="f6a4d-1356">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1356">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="f6a4d-1357">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1357">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="f6a4d-1358">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1358">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="f6a4d-1359">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1359">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="f6a4d-1360">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1360">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-1361">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1361">VM</span></span>

* <span data-ttu-id="f6a4d-1362">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1362">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="f6a4d-1363">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1363">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="f6a4d-1364">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1364">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="f6a4d-1365">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1365">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="f6a4d-1366">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1366">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="f6a4d-1367">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1367">October 24, 2017</span></span>

<span data-ttu-id="f6a4d-1368">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1368">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-1369">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1369">Core</span></span>

* <span data-ttu-id="f6a4d-1370">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1370">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="f6a4d-1371">ACR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1371">ACR</span></span>

* <span data-ttu-id="f6a4d-1372">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1372">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="f6a4d-1373">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1373">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="f6a4d-1374">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1374">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-1375">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1375">ACS</span></span>

* <span data-ttu-id="f6a4d-1376">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1376">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="f6a4d-1377">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1377">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-1378">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1378">Appservice</span></span>

* <span data-ttu-id="f6a4d-1379">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1379">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="f6a4d-1380">Компонент</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1380">Component</span></span>

* <span data-ttu-id="f6a4d-1381">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1381">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="f6a4d-1382">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1382">Monitor</span></span>

* <span data-ttu-id="f6a4d-1383">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1383">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="f6a4d-1384">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1384">Resource</span></span>

* <span data-ttu-id="f6a4d-1385">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1385">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="f6a4d-1386">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1386">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-1387">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1387">VM</span></span>

* <span data-ttu-id="f6a4d-1388">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1388">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="f6a4d-1389">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1389">October 9, 2017</span></span>

<span data-ttu-id="f6a4d-1390">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1390">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-1391">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1391">Core</span></span>

* <span data-ttu-id="f6a4d-1392">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1392">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-1393">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1393">Appservice</span></span>

* <span data-ttu-id="f6a4d-1394">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1394">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="f6a4d-1395">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1395">Batch</span></span>

* <span data-ttu-id="f6a4d-1396">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1396">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="f6a4d-1397">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1397">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="f6a4d-1398">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1398">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="f6a4d-1399">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1399">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="f6a4d-1400">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1400">Batchai</span></span>

* <span data-ttu-id="f6a4d-1401">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1401">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6a4d-1402">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1402">Keyvault</span></span>

* <span data-ttu-id="f6a4d-1403">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1403">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="f6a4d-1404">(#4448)</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1404">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="f6a4d-1405">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1405">Network</span></span>

* <span data-ttu-id="f6a4d-1406">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1406">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="f6a4d-1407">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1407">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="f6a4d-1408">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1408">Resource</span></span>

* <span data-ttu-id="f6a4d-1409">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1409">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="f6a4d-1410">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1410">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="f6a4d-1411">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1411">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="f6a4d-1412">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1412">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="f6a4d-1413">SQL</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1413">Sql</span></span>

* <span data-ttu-id="f6a4d-1414">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1414">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="f6a4d-1415">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1415">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="f6a4d-1416">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1416">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-1417">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1417">Storage</span></span>

* <span data-ttu-id="f6a4d-1418">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1418">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-1419">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1419">Vm</span></span>

* <span data-ttu-id="f6a4d-1420">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1420">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="f6a4d-1421">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1421">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="f6a4d-1422">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1422">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="f6a4d-1423">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1423">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="f6a4d-1424">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1424">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="f6a4d-1425">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1425">September 22, 2017</span></span>

<span data-ttu-id="f6a4d-1426">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1426">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="f6a4d-1427">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1427">Resource</span></span>

* <span data-ttu-id="f6a4d-1428">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1428">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="f6a4d-1429">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1429">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="f6a4d-1430">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1430">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="f6a4d-1431">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1431">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-1432">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1432">Network</span></span>

* <span data-ttu-id="f6a4d-1433">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1433">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="f6a4d-1434">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1434">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="f6a4d-1435">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1435">Added `asg` application security group commands</span></span>
* <span data-ttu-id="f6a4d-1436">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1436">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="f6a4d-1437">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1437">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="f6a4d-1438">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1438">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="f6a4d-1439">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1439">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-1440">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1440">Storage</span></span>

* <span data-ttu-id="f6a4d-1441">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1441">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="f6a4d-1442">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1442">Eventgrid</span></span>

* <span data-ttu-id="f6a4d-1443">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1443">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="f6a4d-1444">SQL</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1444">SQL</span></span>

* <span data-ttu-id="f6a4d-1445">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1445">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="f6a4d-1446">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1446">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="f6a4d-1447">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1447">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6a4d-1448">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1448">Keyvault</span></span>

* <span data-ttu-id="f6a4d-1449">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1449">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-1450">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1450">VM</span></span>

* <span data-ttu-id="f6a4d-1451">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1451">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="f6a4d-1452">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1452">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="f6a4d-1453">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1453">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="f6a4d-1454">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1454">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="f6a4d-1455">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1455">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="f6a4d-1456">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1456">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-1457">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1457">ACS</span></span>

* <span data-ttu-id="f6a4d-1458">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1458">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-1459">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1459">Appservice</span></span>

* <span data-ttu-id="f6a4d-1460">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1460">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="f6a4d-1461">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1461">Backup</span></span>

* <span data-ttu-id="f6a4d-1462">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1462">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="f6a4d-1463">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1463">September 11, 2017</span></span>

<span data-ttu-id="f6a4d-1464">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1464">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="f6a4d-1465">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1465">Core</span></span>

* <span data-ttu-id="f6a4d-1466">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1466">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="f6a4d-1467">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1467">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-1468">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1468">Acs</span></span>

* <span data-ttu-id="f6a4d-1469">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1469">Added `acs list-locations` command</span></span>
* <span data-ttu-id="f6a4d-1470">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1470">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-1471">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1471">Appservice</span></span>

* <span data-ttu-id="f6a4d-1472">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1472">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="f6a4d-1473">CDN</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1473">CDN</span></span>

* <span data-ttu-id="f6a4d-1474">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1474">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="f6a4d-1475">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1475">Extension</span></span>

* <span data-ttu-id="f6a4d-1476">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1476">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6a4d-1477">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1477">Keyvault</span></span>

* <span data-ttu-id="f6a4d-1478">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1478">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-1479">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1479">Network</span></span>

* <span data-ttu-id="f6a4d-1480">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1480">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="f6a4d-1481">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1481">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="f6a4d-1482">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1482">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="f6a4d-1483">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1483">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="f6a4d-1484">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1484">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="f6a4d-1485">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1485">Resource</span></span>

* <span data-ttu-id="f6a4d-1486">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1486">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="f6a4d-1487">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1487">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="f6a4d-1488">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1488">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="f6a4d-1489">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1489">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="f6a4d-1490">SQL</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1490">SQL</span></span>

* <span data-ttu-id="f6a4d-1491">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1491">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-1492">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1492">VM</span></span>

* <span data-ttu-id="f6a4d-1493">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1493">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="f6a4d-1494">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1494">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="f6a4d-1495">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1495">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="f6a4d-1496">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1496">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="f6a4d-1497">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1497">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="f6a4d-1498">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1498">August 31, 2017</span></span>

<span data-ttu-id="f6a4d-1499">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1499">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6a4d-1500">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1500">Keyvault</span></span>

* <span data-ttu-id="f6a4d-1501">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1501">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="f6a4d-1502">Sf</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1502">Sf</span></span>

* <span data-ttu-id="f6a4d-1503">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1503">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-1504">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1504">Storage</span></span>

* <span data-ttu-id="f6a4d-1505">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1505">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="f6a4d-1506">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1506">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="f6a4d-1507">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1507">August 28, 2017</span></span>

<span data-ttu-id="f6a4d-1508">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1508">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="f6a4d-1509">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1509">CLI</span></span>

* <span data-ttu-id="f6a4d-1510">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1510">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-1511">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1511">ACS</span></span>

* <span data-ttu-id="f6a4d-1512">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1512">Corrected preview regions</span></span>
* <span data-ttu-id="f6a4d-1513">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1513">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="f6a4d-1514">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1514">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-1515">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1515">Appservice</span></span>

* <span data-ttu-id="f6a4d-1516">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1516">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="f6a4d-1517">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1517">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="f6a4d-1518">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1518">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="f6a4d-1519">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1519">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="f6a4d-1520">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1520">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="f6a4d-1521">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1521">IoT</span></span>

* <span data-ttu-id="f6a4d-1522">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1522">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-1523">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1523">Network</span></span>

* <span data-ttu-id="f6a4d-1524">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1524">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="f6a4d-1525">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1525">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="f6a4d-1526">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1526">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="f6a4d-1527">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1527">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="f6a4d-1528">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1528">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="f6a4d-1529">Профиль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1529">Profile</span></span>

* <span data-ttu-id="f6a4d-1530">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1530">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f6a4d-1531">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1531">Service Fabric</span></span>

* <span data-ttu-id="f6a4d-1532">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1532">Preview release</span></span>
* <span data-ttu-id="f6a4d-1533">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1533">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="f6a4d-1534">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1534">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="f6a4d-1535">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1535">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-1536">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1536">Storage</span></span>

* <span data-ttu-id="f6a4d-1537">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1537">Enabled setting blob tier</span></span>
* <span data-ttu-id="f6a4d-1538">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1538">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="f6a4d-1539">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1539">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="f6a4d-1540">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1540">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="f6a4d-1541">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1541">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="f6a4d-1542">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1542">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-1543">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1543">VM</span></span>

* <span data-ttu-id="f6a4d-1544">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1544">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="f6a4d-1545">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1545">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="f6a4d-1546">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1546">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="f6a4d-1547">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1547">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="f6a4d-1548">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1548">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="f6a4d-1549">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1549">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="f6a4d-1550">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1550">August 15, 2017</span></span>

<span data-ttu-id="f6a4d-1551">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1551">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-1552">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1552">ACS</span></span>

* <span data-ttu-id="f6a4d-1553">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1553">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-1554">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1554">Appservice</span></span>

* <span data-ttu-id="f6a4d-1555">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1555">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="f6a4d-1556">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1556">Event Grid</span></span>

* <span data-ttu-id="f6a4d-1557">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1557">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="f6a4d-1558">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1558">August 11, 2017</span></span>

<span data-ttu-id="f6a4d-1559">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1559">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-1560">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1560">ACS</span></span>

* <span data-ttu-id="f6a4d-1561">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1561">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="f6a4d-1562">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1562">Batch</span></span>

* <span data-ttu-id="f6a4d-1563">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1563">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="f6a4d-1564">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1564">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="f6a4d-1565">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1565">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="f6a4d-1566">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1566">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="f6a4d-1567">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1567">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="f6a4d-1568">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1568">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="f6a4d-1569">Компонент</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1569">Component</span></span>

* <span data-ttu-id="f6a4d-1570">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1570">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="f6a4d-1571">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1571">Container</span></span>

* <span data-ttu-id="f6a4d-1572">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1572">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="f6a4d-1573">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1573">Data Lake Store</span></span>

* <span data-ttu-id="f6a4d-1574">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1574">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="f6a4d-1575">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1575">Event Grid</span></span>

* <span data-ttu-id="f6a4d-1576">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1576">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-1577">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1577">Network</span></span>

* <span data-ttu-id="f6a4d-1578">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1578">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="f6a4d-1579">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1579">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="f6a4d-1580">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1580">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="f6a4d-1581">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1581">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="f6a4d-1582">Профиль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1582">Profile</span></span>

* <span data-ttu-id="f6a4d-1583">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1583">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-1584">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1584">Storage</span></span>

* <span data-ttu-id="f6a4d-1585">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1585">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-1586">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1586">VM</span></span>

* <span data-ttu-id="f6a4d-1587">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1587">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="f6a4d-1588">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1588">Exposed `list-skus` command</span></span>
* <span data-ttu-id="f6a4d-1589">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1589">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="f6a4d-1590">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1590">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="f6a4d-1591">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1591">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="f6a4d-1592">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1592">July 28, 2017</span></span>

<span data-ttu-id="f6a4d-1593">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1593">Version 2.0.12</span></span>

* <span data-ttu-id="f6a4d-1594">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1594">Added container commands</span></span>
* <span data-ttu-id="f6a4d-1595">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1595">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="f6a4d-1596">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1596">Core</span></span>

* <span data-ttu-id="f6a4d-1597">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1597">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="f6a4d-1598">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1598">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="f6a4d-1599">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1599">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="f6a4d-1600">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1600">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="f6a4d-1601">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1601">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="f6a4d-1602">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1602">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="f6a4d-1603">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1603">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="f6a4d-1604">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1604">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="f6a4d-1605">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1605">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="f6a4d-1606">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1606">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="f6a4d-1607">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1607">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="f6a4d-1608">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1608">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="f6a4d-1609">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1609">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="f6a4d-1610">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1610">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="f6a4d-1611">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1611">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="f6a4d-1612">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1612">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="f6a4d-1613">ACR</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1613">ACR</span></span>

* <span data-ttu-id="f6a4d-1614">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1614">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="f6a4d-1615">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1615">Support SKU update for managed registries</span></span>
* <span data-ttu-id="f6a4d-1616">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1616">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="f6a4d-1617">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1617">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="f6a4d-1618">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1618">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="f6a4d-1619">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1619">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-1620">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1620">ACS</span></span>

* <span data-ttu-id="f6a4d-1621">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1621">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-1622">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1622">Appservice</span></span>

* <span data-ttu-id="f6a4d-1623">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1623">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="f6a4d-1624">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1624">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="f6a4d-1625">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1625">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="f6a4d-1626">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1626">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="f6a4d-1627">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1627">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="f6a4d-1628">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1628">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="f6a4d-1629">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1629">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="f6a4d-1630">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1630">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="f6a4d-1631">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1631">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="f6a4d-1632">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1632">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="f6a4d-1633">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1633">Batch</span></span>

* <span data-ttu-id="f6a4d-1634">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1634">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="f6a4d-1635">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1635">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="f6a4d-1636">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1636">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="f6a4d-1637">CDN</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1637">CDN</span></span>

* <span data-ttu-id="f6a4d-1638">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1638">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="f6a4d-1639">Облако</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1639">Cloud</span></span>

* <span data-ttu-id="f6a4d-1640">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1640">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="f6a4d-1641">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1641">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="f6a4d-1642">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1642">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="f6a4d-1643">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1643">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="f6a4d-1644">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1644">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6a4d-1645">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1645">CosmosDB</span></span>

* <span data-ttu-id="f6a4d-1646">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1646">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="f6a4d-1647">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1647">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f6a4d-1648">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1648">Data Lake Analytics</span></span>

* <span data-ttu-id="f6a4d-1649">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1649">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="f6a4d-1650">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1650">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="f6a4d-1651">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1651">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f6a4d-1652">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1652">Data Lake Store</span></span>

* <span data-ttu-id="f6a4d-1653">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1653">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="f6a4d-1654">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1654">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="f6a4d-1655">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1655">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="f6a4d-1656">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1656">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="f6a4d-1657">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1657">Interactive</span></span>

* <span data-ttu-id="f6a4d-1658">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1658">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="f6a4d-1659">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1659">Increased test coverage</span></span>
* <span data-ttu-id="f6a4d-1660">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1660">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="f6a4d-1661">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1661">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="f6a4d-1662">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1662">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="f6a4d-1663">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1663">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="f6a4d-1664">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1664">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="f6a4d-1665">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1665">Added `--progress` flag</span></span>
* <span data-ttu-id="f6a4d-1666">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1666">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="f6a4d-1667">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1667">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="f6a4d-1668">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1668">IoT</span></span>

* <span data-ttu-id="f6a4d-1669">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1669">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="f6a4d-1670">(3934).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1670">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="f6a4d-1671">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1671">Key vault</span></span>

* <span data-ttu-id="f6a4d-1672">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1672">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="f6a4d-1673">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1673">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="f6a4d-1674">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1674">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="f6a4d-1675">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1675">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="f6a4d-1676">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1676">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="f6a4d-1677">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1677">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="f6a4d-1678">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1678">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="f6a4d-1679">(3307).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1679">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="f6a4d-1680">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1680">Lab</span></span>

* <span data-ttu-id="f6a4d-1681">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1681">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="f6a4d-1682">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1682">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="f6a4d-1683">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1683">Monitor</span></span>

* <span data-ttu-id="f6a4d-1684">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1684">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="f6a4d-1685">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1685">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="f6a4d-1686">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1686">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="f6a4d-1687">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1687">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="f6a4d-1688">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1688">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="f6a4d-1689">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1689">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="f6a4d-1690">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1690">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="f6a4d-1691">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1691">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="f6a4d-1692">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1692">`location` no longer required</span></span>
  * <span data-ttu-id="f6a4d-1693">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1693">Add name and ID support for target</span></span>
  * <span data-ttu-id="f6a4d-1694">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1694">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="f6a4d-1695">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1695">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="f6a4d-1696">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1696">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="f6a4d-1697">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1697">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="f6a4d-1698">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1698">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="f6a4d-1699">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1699">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-1700">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1700">Network</span></span>

* <span data-ttu-id="f6a4d-1701">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1701">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="f6a4d-1702">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1702">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="f6a4d-1703">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1703">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="f6a4d-1704">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1704">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="f6a4d-1705">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1705">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="f6a4d-1706">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1706">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="f6a4d-1707">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1707">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="f6a4d-1708">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1708">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="f6a4d-1709">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1709">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="f6a4d-1710">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1710">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="f6a4d-1711">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1711">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="f6a4d-1712">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1712">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="f6a4d-1713">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1713">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="f6a4d-1714">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1714">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="f6a4d-1715">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1715">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="f6a4d-1716">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1716">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="f6a4d-1717">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1717">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="f6a4d-1718">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1718">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="f6a4d-1719">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1719">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="f6a4d-1720">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1720">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="f6a4d-1721">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1721">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="f6a4d-1722">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1722">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="f6a4d-1723">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1723">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="f6a4d-1724">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1724">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="f6a4d-1725">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1725">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="f6a4d-1726">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1726">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="f6a4d-1727">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1727">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="f6a4d-1728">Профиль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1728">Profile</span></span>

* <span data-ttu-id="f6a4d-1729">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1729">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="f6a4d-1730">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1730">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="f6a4d-1731">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1731">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="f6a4d-1732">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1732">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="f6a4d-1733">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1733">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6a4d-1734">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1734">RDBMS</span></span>

* <span data-ttu-id="f6a4d-1735">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1735">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="f6a4d-1736">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1736">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="f6a4d-1737">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1737">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="f6a4d-1738">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1738">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="f6a4d-1739">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1739">Resource</span></span>

* <span data-ttu-id="f6a4d-1740">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1740">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="f6a4d-1741">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1741">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="f6a4d-1742">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1742">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="f6a4d-1743">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1743">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="f6a4d-1744">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1744">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="f6a4d-1745">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1745">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="f6a4d-1746">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1746">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="f6a4d-1747">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1747">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="f6a4d-1748">Роль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1748">Role</span></span>

* <span data-ttu-id="f6a4d-1749">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1749">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="f6a4d-1750">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1750">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="f6a4d-1751">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1751">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="f6a4d-1752">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1752">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="f6a4d-1753">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1753">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f6a4d-1754">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1754">Service Fabric</span></span>
* <span data-ttu-id="f6a4d-1755">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1755">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="f6a4d-1756">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1756">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="f6a4d-1757">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1757">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="f6a4d-1758">SQL</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1758">SQL</span></span>

* <span data-ttu-id="f6a4d-1759">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1759">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="f6a4d-1760">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1760">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="f6a4d-1761">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1761">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-1762">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1762">Storage</span></span>

* <span data-ttu-id="f6a4d-1763">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1763">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="f6a4d-1764">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1764">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="f6a4d-1765">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1765">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="f6a4d-1766">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1766">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="f6a4d-1767">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1767">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="f6a4d-1768">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1768">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-1769">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1769">VM</span></span>

* <span data-ttu-id="f6a4d-1770">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1770">Support configuring nsg</span></span>
* <span data-ttu-id="f6a4d-1771">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1771">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="f6a4d-1772">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1772">Support managed service identities</span></span>
* <span data-ttu-id="f6a4d-1773">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1773">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="f6a4d-1774">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1774">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="f6a4d-1775">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1775">May 10, 2017</span></span>

<span data-ttu-id="f6a4d-1776">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1776">Version 2.0.6</span></span>

* <span data-ttu-id="f6a4d-1777">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1777">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="f6a4d-1778">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1778">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="f6a4d-1779">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1779">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="f6a4d-1780">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1780">Include Cognitive Services module</span></span>
* <span data-ttu-id="f6a4d-1781">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1781">Include Service Fabric module</span></span>
* <span data-ttu-id="f6a4d-1782">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1782">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="f6a4d-1783">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1783">Add support for CDN commands</span></span>
* <span data-ttu-id="f6a4d-1784">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1784">Remove Container module</span></span>
* <span data-ttu-id="f6a4d-1785">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1785">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="f6a4d-1786">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1786">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="f6a4d-1787">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1787">Core</span></span>

* <span data-ttu-id="f6a4d-1788">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1788">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="f6a4d-1789">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1789">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="f6a4d-1790">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1790">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="f6a4d-1791">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1791">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="f6a4d-1792">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1792">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="f6a4d-1793">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1793">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="f6a4d-1794">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1794">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="f6a4d-1795">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1795">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="f6a4d-1796">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1796">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="f6a4d-1797">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1797">core: Improved performance</span></span>
* <span data-ttu-id="f6a4d-1798">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1798">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="f6a4d-1799">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1799">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-1800">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1800">ACS</span></span>

* <span data-ttu-id="f6a4d-1801">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1801">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="f6a4d-1802">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1802">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="f6a4d-1803">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1803">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="f6a4d-1804">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1804">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-1805">AppService</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1805">AppService</span></span>

* <span data-ttu-id="f6a4d-1806">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1806">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="f6a4d-1807">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1807">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="f6a4d-1808">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1808">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="f6a4d-1809">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1809">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="f6a4d-1810">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1810">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="f6a4d-1811">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1811">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="f6a4d-1812">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1812">support slot swap with preview</span></span>
* <span data-ttu-id="f6a4d-1813">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1813">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="f6a4d-1814">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1814">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6a4d-1815">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1815">CosmosDB</span></span>

* <span data-ttu-id="f6a4d-1816">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1816">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="f6a4d-1817">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1817">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="f6a4d-1818">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1818">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="f6a4d-1819">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1819">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f6a4d-1820">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1820">Data Lake Analytics</span></span>

* <span data-ttu-id="f6a4d-1821">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1821">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="f6a4d-1822">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1822">Add support for new catalog item type: package.</span></span> <span data-ttu-id="f6a4d-1823">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1823">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="f6a4d-1824">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1824">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="f6a4d-1825">Таблица</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1825">Table</span></span>
  * <span data-ttu-id="f6a4d-1826">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1826">Table valued function</span></span>
  * <span data-ttu-id="f6a4d-1827">Просмотр</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1827">View</span></span>
  * <span data-ttu-id="f6a4d-1828">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1828">Table Statistics.</span></span> <span data-ttu-id="f6a4d-1829">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1829">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f6a4d-1830">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1830">Data Lake Store</span></span>

* <span data-ttu-id="f6a4d-1831">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1831">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="f6a4d-1832">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1832">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="f6a4d-1833">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1833">missed help for access show.</span></span> <span data-ttu-id="f6a4d-1834">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1834">adding it.</span></span> <span data-ttu-id="f6a4d-1835">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1835">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="f6a4d-1836">Поиск</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1836">Find</span></span>

* <span data-ttu-id="f6a4d-1837">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1837">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6a4d-1838">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1838">KeyVault</span></span>

* <span data-ttu-id="f6a4d-1839">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1839">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="f6a4d-1840">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1840">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="f6a4d-1841">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1841">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="f6a4d-1842">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1842">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="f6a4d-1843">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1843">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="f6a4d-1844">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1844">Lab</span></span>

* <span data-ttu-id="f6a4d-1845">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1845">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="f6a4d-1846">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1846">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="f6a4d-1847">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1847">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="f6a4d-1848">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1848">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="f6a4d-1849">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1849">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="f6a4d-1850">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1850">Monitor</span></span>

* <span data-ttu-id="f6a4d-1851">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1851">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="f6a4d-1852">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1852">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="f6a4d-1853">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1853">Network</span></span>

* <span data-ttu-id="f6a4d-1854">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1854">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="f6a4d-1855">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1855">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="f6a4d-1856">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1856">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="f6a4d-1857">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1857">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="f6a4d-1858">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1858">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="f6a4d-1859">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1859">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="f6a4d-1860">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1860">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="f6a4d-1861">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1861">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="f6a4d-1862">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1862">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="f6a4d-1863">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1863">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="f6a4d-1864">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1864">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="f6a4d-1865">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1865">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="f6a4d-1866">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1866">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="f6a4d-1867">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1867">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="f6a4d-1868">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1868">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="f6a4d-1869">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1869">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="f6a4d-1870">Профиль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1870">Profile</span></span>

* <span data-ttu-id="f6a4d-1871">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1871">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="f6a4d-1872">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1872">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="f6a4d-1873">Redis</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1873">Redis</span></span>

* <span data-ttu-id="f6a4d-1874">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1874">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="f6a4d-1875">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1875">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="f6a4d-1876">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1876">Resource</span></span>

* <span data-ttu-id="f6a4d-1877">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1877">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="f6a4d-1878">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1878">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="f6a4d-1879">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1879">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="f6a4d-1880">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1880">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="f6a4d-1881">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1881">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="f6a4d-1882">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1882">Add docs for az lock update.</span></span> <span data-ttu-id="f6a4d-1883">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1883">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="f6a4d-1884">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1884">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="f6a4d-1885">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1885">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="f6a4d-1886">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1886">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="f6a4d-1887">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1887">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="f6a4d-1888">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1888">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="f6a4d-1889">Роль</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1889">Role</span></span>

* <span data-ttu-id="f6a4d-1890">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1890">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="f6a4d-1891">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1891">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="f6a4d-1892">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1892">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="f6a4d-1893">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1893">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="f6a4d-1894">SQL</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1894">SQL</span></span>

* <span data-ttu-id="f6a4d-1895">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1895">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="f6a4d-1896">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1896">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="f6a4d-1897">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1897">Storage</span></span>

* <span data-ttu-id="f6a4d-1898">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1898">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="f6a4d-1899">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1899">Add support for incremental blob copy</span></span>
* <span data-ttu-id="f6a4d-1900">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1900">Add support for large block blob upload</span></span>
* <span data-ttu-id="f6a4d-1901">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1901">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-1902">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1902">VM</span></span>

* <span data-ttu-id="f6a4d-1903">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1903">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="f6a4d-1904">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1904">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="f6a4d-1905">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1905">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="f6a4d-1906">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1906">az vm/vmss disk</span></span>
  3. <span data-ttu-id="f6a4d-1907">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1907">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="f6a4d-1908">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1908">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="f6a4d-1909">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1909">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="f6a4d-1910">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1910">April 3, 2017</span></span>

<span data-ttu-id="f6a4d-1911">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1911">Version 2.0.2</span></span>

<span data-ttu-id="f6a4d-1912">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1912">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="f6a4d-1913">Core</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1913">Core</span></span>

* <span data-ttu-id="f6a4d-1914">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1914">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="f6a4d-1915">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1915">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="f6a4d-1916">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1916">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="f6a4d-1917">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1917">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="f6a4d-1918">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1918">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="f6a4d-1919">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1919">Add prompting for missing template parameters.</span></span> <span data-ttu-id="f6a4d-1920">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1920">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="f6a4d-1921">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1921">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="f6a4d-1922">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1922">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="f6a4d-1923">ACS</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1923">ACS</span></span>

* <span data-ttu-id="f6a4d-1924">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1924">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="f6a4d-1925">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1925">Add support for ssh key password prompting.</span></span> <span data-ttu-id="f6a4d-1926">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1926">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="f6a4d-1927">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1927">Add support for windows clusters.</span></span> <span data-ttu-id="f6a4d-1928">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1928">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="f6a4d-1929">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1929">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="f6a4d-1930">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1930">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="f6a4d-1931">AppService</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1931">AppService</span></span>

* <span data-ttu-id="f6a4d-1932">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1932">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="f6a4d-1933">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1933">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="f6a4d-1934">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1934">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="f6a4d-1935">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1935">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="f6a4d-1936">Data Lake</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1936">DataLake</span></span>

* <span data-ttu-id="f6a4d-1937">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1937">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="f6a4d-1938">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1938">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="f6a4d-1939">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1939">DocuemntDB</span></span>

* <span data-ttu-id="f6a4d-1940">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1940">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="f6a4d-1941">ВМ</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1941">VM</span></span>

* <span data-ttu-id="f6a4d-1942">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1942">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="f6a4d-1943">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1943">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="f6a4d-1944">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1944">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="f6a4d-1945">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1945">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="f6a4d-1946">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1946">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="f6a4d-1947">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1947">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="f6a4d-1948">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1948">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="f6a4d-1949">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1949">February 27, 2017</span></span>

<span data-ttu-id="f6a4d-1950">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1950">Version 2.0.0</span></span>

<span data-ttu-id="f6a4d-1951">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1951">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="f6a4d-1952">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1952">Container Service (acs)</span></span>
- <span data-ttu-id="f6a4d-1953">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1953">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="f6a4d-1954">Сеть</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1954">Networking</span></span>
- <span data-ttu-id="f6a4d-1955">Хранилище</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1955">Storage</span></span>

<span data-ttu-id="f6a4d-1956">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1956">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="f6a4d-1957">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1957">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="f6a4d-1958">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1958">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="f6a4d-1959">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1959">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="f6a4d-1960">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1960">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="f6a4d-1961">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1961">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="f6a4d-1962">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1962">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="f6a4d-1963">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1963">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="f6a4d-1964">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="f6a4d-1964">Provide feedback from the command line with the `az feedback` command</span></span>

