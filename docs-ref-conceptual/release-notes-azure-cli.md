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
ms.openlocfilehash: 36b57d52a5851275fd317240e5c2c95171a99e7e
ms.sourcegitcommit: 22b73d56602c1c4e647ed2c5af3d596a2f6a7ed5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2018
ms.locfileid: "52267336"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="ef10c-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="ef10c-103">Azure CLI release notes</span></span>
## <a name="november-20-2018"></a><span data-ttu-id="ef10c-104">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-104">November 20, 2018</span></span>

<span data-ttu-id="ef10c-105">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="ef10c-105">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="ef10c-106">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-106">Core</span></span>
* <span data-ttu-id="ef10c-107">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="ef10c-107">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="ef10c-108">ACR</span><span class="sxs-lookup"><span data-stu-id="ef10c-108">ACR</span></span>
* <span data-ttu-id="ef10c-109">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="ef10c-109">Added context token to task step</span></span>
* <span data-ttu-id="ef10c-110">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="ef10c-110">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="ef10c-111">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-111">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-112">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ef10c-112">Appservice</span></span>
* <span data-ttu-id="ef10c-113">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="ef10c-113">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="ef10c-114">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ef10c-114">Updated the default `node_version`.</span></span> <span data-ttu-id="ef10c-115">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="ef10c-115">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="ef10c-116">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="ef10c-116">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="ef10c-117">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="ef10c-117">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="ef10c-118">IotCentral</span><span class="sxs-lookup"><span data-stu-id="ef10c-118">IotCentral</span></span>
* <span data-ttu-id="ef10c-119">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="ef10c-119">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="ef10c-120">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ef10c-120">KeyVault</span></span>
* <span data-ttu-id="ef10c-121">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="ef10c-121">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-122">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-122">Network</span></span>
* <span data-ttu-id="ef10c-123">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-123">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="ef10c-124">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-124">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="ef10c-125">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="ef10c-125">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="ef10c-126">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-126">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="ef10c-127">Rdbms</span><span class="sxs-lookup"><span data-stu-id="ef10c-127">Rdbms</span></span>
* <span data-ttu-id="ef10c-128">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="ef10c-128">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="ef10c-129">RBAC:</span><span class="sxs-lookup"><span data-stu-id="ef10c-129">Rbac</span></span>
* <span data-ttu-id="ef10c-130">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-130">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="ef10c-131">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="ef10c-131">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="ef10c-132">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-132">Storage</span></span>
* <span data-ttu-id="ef10c-133">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="ef10c-133">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="ef10c-134">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-134">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="ef10c-135">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="ef10c-135">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="ef10c-136">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-136">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-137">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-137">VM</span></span>
* <span data-ttu-id="ef10c-138">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="ef10c-138">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="ef10c-139">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-139">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="ef10c-140">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-140">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="ef10c-141">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="ef10c-141">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="ef10c-142">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-142">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="ef10c-143">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-143">Added `snapshot wait` command</span></span>
* <span data-ttu-id="ef10c-144">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-144">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="ef10c-145">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-145">November 6, 2018</span></span>

<span data-ttu-id="ef10c-146">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="ef10c-146">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-147">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-147">Core</span></span>
* <span data-ttu-id="ef10c-148">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="ef10c-148">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="ef10c-149">ACR</span><span class="sxs-lookup"><span data-stu-id="ef10c-149">ACR</span></span>
* <span data-ttu-id="ef10c-150">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="ef10c-150">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="ef10c-151">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="ef10c-151">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-152">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-152">ACS</span></span>
* <span data-ttu-id="ef10c-153">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ef10c-153">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="ef10c-154">Помощник</span><span class="sxs-lookup"><span data-stu-id="ef10c-154">Advisor</span></span>
* <span data-ttu-id="ef10c-155">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="ef10c-155">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="ef10c-156">AMS</span><span class="sxs-lookup"><span data-stu-id="ef10c-156">AMS</span></span>
* <span data-ttu-id="ef10c-157">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="ef10c-157">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="ef10c-158">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="ef10c-158">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="ef10c-159">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-159">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="ef10c-160">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="ef10c-160">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="ef10c-161">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-161">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="ef10c-162">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-162">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="ef10c-163">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-163">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="ef10c-164">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-164">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="ef10c-165">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-165">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="ef10c-166">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-166">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="ef10c-167">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-167">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="ef10c-168">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-168">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="ef10c-169">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="ef10c-169">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="ef10c-170">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="ef10c-170">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="ef10c-171">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-171">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="ef10c-172">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="ef10c-172">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="ef10c-173">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="ef10c-173">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-174">AppService</span><span class="sxs-lookup"><span data-stu-id="ef10c-174">AppService</span></span>
* <span data-ttu-id="ef10c-175">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="ef10c-175">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="ef10c-176">Настройка</span><span class="sxs-lookup"><span data-stu-id="ef10c-176">Configure</span></span>
* <span data-ttu-id="ef10c-177">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="ef10c-177">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="ef10c-178">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ef10c-178">Container</span></span>
* <span data-ttu-id="ef10c-179">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="ef10c-179">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="ef10c-180">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="ef10c-180">EventHub</span></span>
* <span data-ttu-id="ef10c-181">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-181">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="ef10c-182">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef10c-182">Interactive</span></span>
* <span data-ttu-id="ef10c-183">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="ef10c-183">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="ef10c-184">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ef10c-184">Monitor</span></span>
* <span data-ttu-id="ef10c-185">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-185">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-186">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-186">Network</span></span>
* <span data-ttu-id="ef10c-187">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-187">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="ef10c-188">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="ef10c-188">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="ef10c-189">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-189">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="ef10c-190">Профиль</span><span class="sxs-lookup"><span data-stu-id="ef10c-190">Profile</span></span>
* <span data-ttu-id="ef10c-191">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-191">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="ef10c-192">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ef10c-192">RDBMS</span></span>
* <span data-ttu-id="ef10c-193">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="ef10c-193">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="ef10c-194">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ef10c-194">Resource</span></span>
* <span data-ttu-id="ef10c-195">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-195">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="ef10c-196">Роль</span><span class="sxs-lookup"><span data-stu-id="ef10c-196">Role</span></span>
* <span data-ttu-id="ef10c-197">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="ef10c-197">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="ef10c-198">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="ef10c-198">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="ef10c-199">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="ef10c-199">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-200">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-200">Storage</span></span>
* <span data-ttu-id="ef10c-201">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-201">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-202">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-202">VM</span></span>
* <span data-ttu-id="ef10c-203">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="ef10c-203">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="ef10c-204">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="ef10c-204">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="ef10c-205">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="ef10c-205">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="ef10c-206">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="ef10c-206">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="ef10c-207">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="ef10c-207">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="ef10c-208">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-208">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="ef10c-209">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-209">October 23, 2018</span></span>

<span data-ttu-id="ef10c-210">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="ef10c-210">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-211">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-211">Core</span></span>
* <span data-ttu-id="ef10c-212">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-212">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="ef10c-213">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-213">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="ef10c-214">ACR</span><span class="sxs-lookup"><span data-stu-id="ef10c-214">ACR</span></span>
* <span data-ttu-id="ef10c-215">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="ef10c-215">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="ef10c-216">CDN</span><span class="sxs-lookup"><span data-stu-id="ef10c-216">CDN</span></span>
* <span data-ttu-id="ef10c-217">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ef10c-217">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="ef10c-218">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="ef10c-218">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="ef10c-219">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ef10c-219">Container</span></span>
* <span data-ttu-id="ef10c-220">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="ef10c-220">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="ef10c-221">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="ef10c-221">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="ef10c-222">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-222">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="ef10c-223">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ef10c-223">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="ef10c-224">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="ef10c-224">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="ef10c-225">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="ef10c-225">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="ef10c-226">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-226">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ef10c-227">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ef10c-227">CosmosDB</span></span>
* <span data-ttu-id="ef10c-228">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-228">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="ef10c-229">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef10c-229">Interactive</span></span>
* <span data-ttu-id="ef10c-230">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="ef10c-230">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="ef10c-231">IoT Central</span><span class="sxs-lookup"><span data-stu-id="ef10c-231">IoT Central</span></span>
* <span data-ttu-id="ef10c-232">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="ef10c-232">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="ef10c-233">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="ef10c-233">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="ef10c-234">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ef10c-234">Monitor</span></span>
* <span data-ttu-id="ef10c-235">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="ef10c-235">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="ef10c-236">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="ef10c-236">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="ef10c-237">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="ef10c-237">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="ef10c-238">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="ef10c-238">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="ef10c-239">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-239">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="ef10c-240">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="ef10c-240">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="ef10c-241">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="ef10c-241">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="ef10c-242">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="ef10c-242">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="ef10c-243">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="ef10c-243">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="ef10c-244">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-244">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-245">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-245">Network</span></span>
* <span data-ttu-id="ef10c-246">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="ef10c-246">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="ef10c-247">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="ef10c-247">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="ef10c-248">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="ef10c-248">ServiceBus</span></span>
* <span data-ttu-id="ef10c-249">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="ef10c-249">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="ef10c-250">SQL</span><span class="sxs-lookup"><span data-stu-id="ef10c-250">SQL</span></span>
* <span data-ttu-id="ef10c-251">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="ef10c-251">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-252">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-252">Storage</span></span>
* <span data-ttu-id="ef10c-253">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="ef10c-253">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="ef10c-254">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="ef10c-254">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-255">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-255">VM</span></span>
* <span data-ttu-id="ef10c-256">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="ef10c-256">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="ef10c-257">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="ef10c-257">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="ef10c-258">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="ef10c-258">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="ef10c-259">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-259">October 16, 2018</span></span>

<span data-ttu-id="ef10c-260">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="ef10c-260">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-261">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-261">VM</span></span>
* <span data-ttu-id="ef10c-262">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="ef10c-262">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="ef10c-263">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-263">October 9, 2018</span></span>

<span data-ttu-id="ef10c-264">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="ef10c-264">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-265">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-265">Core</span></span>
* <span data-ttu-id="ef10c-266">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="ef10c-266">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="ef10c-267">ACR</span><span class="sxs-lookup"><span data-stu-id="ef10c-267">ACR</span></span>
* <span data-ttu-id="ef10c-268">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="ef10c-268">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-269">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-269">ACS</span></span>
* <span data-ttu-id="ef10c-270">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="ef10c-270">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="ef10c-271">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="ef10c-271">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="ef10c-272">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-272">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="ef10c-273">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="ef10c-273">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="ef10c-274">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ef10c-274">Container</span></span>
* <span data-ttu-id="ef10c-275">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="ef10c-275">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="ef10c-276">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="ef10c-276">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="ef10c-277">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="ef10c-277">Event Hub</span></span>
* <span data-ttu-id="ef10c-278">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-278">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="ef10c-279">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="ef10c-279">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="ef10c-280">расширения.</span><span class="sxs-lookup"><span data-stu-id="ef10c-280">Extensions</span></span>
* <span data-ttu-id="ef10c-281">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="ef10c-281">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="ef10c-282">HDInsight</span><span class="sxs-lookup"><span data-stu-id="ef10c-282">HDInsight</span></span>
* <span data-ttu-id="ef10c-283">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ef10c-283">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="ef10c-284">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ef10c-284">IoT</span></span>
* <span data-ttu-id="ef10c-285">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="ef10c-285">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="ef10c-286">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ef10c-286">KeyVault</span></span>
* <span data-ttu-id="ef10c-287">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="ef10c-287">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-288">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-288">Network</span></span>
* <span data-ttu-id="ef10c-289">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ef10c-289">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="ef10c-290">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="ef10c-290">See #6052</span></span>
* <span data-ttu-id="ef10c-291">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-291">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="ef10c-292">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="ef10c-292">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="ef10c-293">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-293">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="ef10c-294">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-294">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="ef10c-295">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-295">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="ef10c-296">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-296">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="ef10c-297">Роль</span><span class="sxs-lookup"><span data-stu-id="ef10c-297">Role</span></span>
* <span data-ttu-id="ef10c-298">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-298">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="ef10c-299">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-299">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="ef10c-300">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="ef10c-300">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="ef10c-301">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="ef10c-301">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="ef10c-302">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="ef10c-302">Service Bus</span></span>
* <span data-ttu-id="ef10c-303">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="ef10c-303">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-304">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-304">VM</span></span>
* <span data-ttu-id="ef10c-305">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-305">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="ef10c-306">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="ef10c-306">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="ef10c-307">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-307">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="ef10c-308">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-308">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="ef10c-309">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="ef10c-309">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="ef10c-310">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="ef10c-310">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="ef10c-311">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-311">September 21, 2018</span></span>

<span data-ttu-id="ef10c-312">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="ef10c-312">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="ef10c-313">ACR</span><span class="sxs-lookup"><span data-stu-id="ef10c-313">ACR</span></span>
* <span data-ttu-id="ef10c-314">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="ef10c-314">Added ACR Task commands</span></span>
* <span data-ttu-id="ef10c-315">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="ef10c-315">Added quick run command</span></span>
* <span data-ttu-id="ef10c-316">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="ef10c-316">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="ef10c-317">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="ef10c-317">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="ef10c-318">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="ef10c-318">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="ef10c-319">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="ef10c-319">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-320">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-320">ACS</span></span>
* <span data-ttu-id="ef10c-321">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="ef10c-321">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="ef10c-322">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="ef10c-322">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-323">AppService</span><span class="sxs-lookup"><span data-stu-id="ef10c-323">AppService</span></span>

* <span data-ttu-id="ef10c-324">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="ef10c-324">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="ef10c-325">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="ef10c-325">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="ef10c-326">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="ef10c-326">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="ef10c-327">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="ef10c-327">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="ef10c-328">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ef10c-328">Batch</span></span>
* <span data-ttu-id="ef10c-329">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="ef10c-329">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="ef10c-330">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-330">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="ef10c-331">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-331">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="ef10c-332">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="ef10c-332">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ef10c-333">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ef10c-333">Batch AI</span></span> 
* <span data-ttu-id="ef10c-334">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-334">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ef10c-335">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ef10c-335">Cognitive Services</span></span>
* <span data-ttu-id="ef10c-336">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-336">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="ef10c-337">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-337">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="ef10c-338">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-338">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="ef10c-339">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-339">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="ef10c-340">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="ef10c-340">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="ef10c-341">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-341">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="ef10c-342">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ef10c-342">Container</span></span>
* <span data-ttu-id="ef10c-343">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ef10c-343">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="ef10c-344">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="ef10c-344">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="ef10c-345">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="ef10c-345">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="ef10c-346">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ef10c-346">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="ef10c-347">Data Lake</span><span class="sxs-lookup"><span data-stu-id="ef10c-347">Datalake</span></span>
* <span data-ttu-id="ef10c-348">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="ef10c-348">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="ef10c-349">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="ef10c-349">Interactive Shell</span></span>
* <span data-ttu-id="ef10c-350">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="ef10c-350">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="ef10c-351">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-351">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="ef10c-352">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ef10c-352">IoT</span></span>
* <span data-ttu-id="ef10c-353">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="ef10c-353">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="ef10c-354">Key Vault</span><span class="sxs-lookup"><span data-stu-id="ef10c-354">Key Vault</span></span>
* <span data-ttu-id="ef10c-355">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="ef10c-355">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-356">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-356">Network</span></span>
* <span data-ttu-id="ef10c-357">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-357">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="ef10c-358">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="ef10c-358">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="ef10c-359">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="ef10c-359">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="ef10c-360">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-360">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="ef10c-361">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-361">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="ef10c-362">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-362">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="ef10c-363">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="ef10c-363">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="ef10c-364">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-364">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="ef10c-365">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-365">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="ef10c-366">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-366">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="ef10c-367">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-367">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="ef10c-368">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-368">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="ef10c-369">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры`--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-369">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="ef10c-370">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="ef10c-370">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="ef10c-371">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-371">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="ef10c-372">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="ef10c-372">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="ef10c-373">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="ef10c-373">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="ef10c-374">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="ef10c-374">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="ef10c-375">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ef10c-375">RDBMS</span></span>
* <span data-ttu-id="ef10c-376">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="ef10c-376">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="ef10c-377">резервирование.</span><span class="sxs-lookup"><span data-stu-id="ef10c-377">Reservation</span></span>
* <span data-ttu-id="ef10c-378">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-378">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="ef10c-379">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="ef10c-379">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="ef10c-380">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="ef10c-380">Manage App</span></span>
* <span data-ttu-id="ef10c-381">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ef10c-381">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="ef10c-382">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="ef10c-382">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="ef10c-383">Роль</span><span class="sxs-lookup"><span data-stu-id="ef10c-383">Role</span></span>
* <span data-ttu-id="ef10c-384">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="ef10c-384">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="ef10c-385">SignalR</span><span class="sxs-lookup"><span data-stu-id="ef10c-385">SignalR</span></span>
* <span data-ttu-id="ef10c-386">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ef10c-386">First release</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-387">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-387">Storage</span></span>
* <span data-ttu-id="ef10c-388">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="ef10c-388">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="ef10c-389">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="ef10c-389">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-390">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-390">VM</span></span>
* <span data-ttu-id="ef10c-391">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="ef10c-391">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="ef10c-392">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-392">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="ef10c-393">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-393">August 28, 2018</span></span>

<span data-ttu-id="ef10c-394">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="ef10c-394">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-395">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-395">Core</span></span>

* <span data-ttu-id="ef10c-396">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="ef10c-396">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="ef10c-397">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="ef10c-397">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="ef10c-398">ACR</span><span class="sxs-lookup"><span data-stu-id="ef10c-398">ACR</span></span>

* <span data-ttu-id="ef10c-399">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="ef10c-399">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="ef10c-400">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-400">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-401">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-401">ACS</span></span>

* <span data-ttu-id="ef10c-402">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-402">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="ef10c-403">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="ef10c-403">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-404">AppService</span><span class="sxs-lookup"><span data-stu-id="ef10c-404">AppService</span></span>

* <span data-ttu-id="ef10c-405">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="ef10c-405">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="ef10c-406">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="ef10c-406">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="ef10c-407">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="ef10c-407">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="ef10c-408">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="ef10c-408">Backup</span></span>

* <span data-ttu-id="ef10c-409">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="ef10c-409">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="ef10c-410">Служба Bot Service</span><span class="sxs-lookup"><span data-stu-id="ef10c-410">Bot Service</span></span>

* <span data-ttu-id="ef10c-411">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="ef10c-411">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ef10c-412">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ef10c-412">Cognitive Services</span></span>

* <span data-ttu-id="ef10c-413">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="ef10c-413">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="ef10c-414">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ef10c-414">IoT</span></span>

* <span data-ttu-id="ef10c-415">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="ef10c-415">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="ef10c-416">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ef10c-416">Monitor</span></span>

* <span data-ttu-id="ef10c-417">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="ef10c-417">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="ef10c-418">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="ef10c-418">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-419">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-419">Network</span></span>

* <span data-ttu-id="ef10c-420">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="ef10c-420">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="ef10c-421">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ef10c-421">Resource</span></span>

* <span data-ttu-id="ef10c-422">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="ef10c-422">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-423">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-423">Storage</span></span>

* <span data-ttu-id="ef10c-424">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="ef10c-424">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-425">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-425">VM</span></span>

* <span data-ttu-id="ef10c-426">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="ef10c-426">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="ef10c-427">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-427">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="ef10c-428">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-428">Auguest 14, 2018</span></span>

<span data-ttu-id="ef10c-429">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="ef10c-429">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-430">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-430">Core</span></span>

* <span data-ttu-id="ef10c-431">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-431">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="ef10c-432">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="ef10c-432">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="ef10c-433">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="ef10c-433">Telemetry</span></span>

* <span data-ttu-id="ef10c-434">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="ef10c-434">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="ef10c-435">ACR</span><span class="sxs-lookup"><span data-stu-id="ef10c-435">ACR</span></span>

* <span data-ttu-id="ef10c-436">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-436">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="ef10c-437">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-437">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-438">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-438">ACS</span></span>

* <span data-ttu-id="ef10c-439">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="ef10c-439">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="ef10c-440">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="ef10c-440">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="ef10c-441">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="ef10c-441">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="ef10c-442">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="ef10c-442">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="ef10c-443">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="ef10c-443">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="ef10c-444">AppService</span><span class="sxs-lookup"><span data-stu-id="ef10c-444">AppService</span></span>

* <span data-ttu-id="ef10c-445">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-445">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="ef10c-446">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="ef10c-446">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="ef10c-447">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ef10c-447">BatchAI</span></span>

* <span data-ttu-id="ef10c-448">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="ef10c-448">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="ef10c-449">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ef10c-449">Container</span></span>

* <span data-ttu-id="ef10c-450">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="ef10c-450">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="ef10c-451">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ef10c-451">IoT</span></span>

* <span data-ttu-id="ef10c-452">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="ef10c-452">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="ef10c-453">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-453">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="ef10c-454">IoT Central</span><span class="sxs-lookup"><span data-stu-id="ef10c-454">Iot Central</span></span>

* <span data-ttu-id="ef10c-455">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="ef10c-455">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="ef10c-456">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ef10c-456">KeyVault</span></span>


* <span data-ttu-id="ef10c-457">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="ef10c-457">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="ef10c-458">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="ef10c-458">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="ef10c-459">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="ef10c-459">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="ef10c-460">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="ef10c-460">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="ef10c-461">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="ef10c-461">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="ef10c-462">Передача</span><span class="sxs-lookup"><span data-stu-id="ef10c-462">Relay</span></span>

* <span data-ttu-id="ef10c-463">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ef10c-463">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="ef10c-464">SQL</span><span class="sxs-lookup"><span data-stu-id="ef10c-464">Sql</span></span>

* <span data-ttu-id="ef10c-465">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-465">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-466">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-466">Storage</span></span>

* <span data-ttu-id="ef10c-467">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="ef10c-467">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="ef10c-468">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="ef10c-468">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="ef10c-469">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="ef10c-469">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="ef10c-470">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="ef10c-470">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="ef10c-471">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="ef10c-471">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-472">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-472">VM</span></span>

* <span data-ttu-id="ef10c-473">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="ef10c-473">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="ef10c-474">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-474">July 31, 2018</span></span>

<span data-ttu-id="ef10c-475">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="ef10c-475">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="ef10c-476">ACR</span><span class="sxs-lookup"><span data-stu-id="ef10c-476">ACR</span></span>

* <span data-ttu-id="ef10c-477">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-477">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="ef10c-478">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-478">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-479">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-479">ACS</span></span>

* <span data-ttu-id="ef10c-480">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="ef10c-480">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="ef10c-481">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ef10c-481">Batch</span></span>

* <span data-ttu-id="ef10c-482">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="ef10c-482">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="ef10c-483">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ef10c-483">Container</span></span>

* <span data-ttu-id="ef10c-484">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="ef10c-484">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-485">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-485">Network</span></span>

* <span data-ttu-id="ef10c-486">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="ef10c-486">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="ef10c-487">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ef10c-487">Resource</span></span>

* <span data-ttu-id="ef10c-488">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="ef10c-488">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="ef10c-489">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="ef10c-489">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="ef10c-490">Роль</span><span class="sxs-lookup"><span data-stu-id="ef10c-490">Role</span></span>

* <span data-ttu-id="ef10c-491">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="ef10c-491">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="ef10c-492">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="ef10c-492">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="ef10c-493">поиска</span><span class="sxs-lookup"><span data-stu-id="ef10c-493">Search</span></span>

* <span data-ttu-id="ef10c-494">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="ef10c-494">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="ef10c-495">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="ef10c-495">Service Bus</span></span>

* <span data-ttu-id="ef10c-496">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="ef10c-496">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="ef10c-497">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="ef10c-497">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="ef10c-498">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="ef10c-498">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="ef10c-499">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-499">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-500">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-500">Storage</span></span>

* <span data-ttu-id="ef10c-501">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="ef10c-501">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="ef10c-502">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="ef10c-502">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-503">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-503">VM</span></span>

* <span data-ttu-id="ef10c-504">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="ef10c-504">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="ef10c-505">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-505">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="ef10c-506">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="ef10c-506">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="ef10c-507">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="ef10c-507">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="ef10c-508">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-508">July 18, 2018</span></span>

<span data-ttu-id="ef10c-509">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="ef10c-509">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-510">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-510">Core</span></span>

* <span data-ttu-id="ef10c-511">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="ef10c-511">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="ef10c-512">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="ef10c-512">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="ef10c-513">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="ef10c-513">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="ef10c-514">ACR</span><span class="sxs-lookup"><span data-stu-id="ef10c-514">ACR</span></span>

* <span data-ttu-id="ef10c-515">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="ef10c-515">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="ef10c-516">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-516">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="ef10c-517">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="ef10c-517">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="ef10c-518">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="ef10c-518">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-519">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-519">ACS</span></span>

* <span data-ttu-id="ef10c-520">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="ef10c-520">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-521">AppService</span><span class="sxs-lookup"><span data-stu-id="ef10c-521">AppService</span></span>

* <span data-ttu-id="ef10c-522">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="ef10c-522">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="ef10c-523">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ef10c-523">Batch</span></span>

* <span data-ttu-id="ef10c-524">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="ef10c-524">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="ef10c-525">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="ef10c-525">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ef10c-526">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ef10c-526">Batch AI</span></span>

* <span data-ttu-id="ef10c-527">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-527">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="ef10c-528">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ef10c-528">Container</span></span>

* <span data-ttu-id="ef10c-529">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="ef10c-529">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="ef10c-530">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="ef10c-530">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-531">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-531">Network</span></span>

* <span data-ttu-id="ef10c-532">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-532">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="ef10c-533">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-533">Added `network nic wait`</span></span>
* <span data-ttu-id="ef10c-534">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="ef10c-534">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="ef10c-535">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="ef10c-535">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="ef10c-536">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ef10c-536">Resource</span></span>

* <span data-ttu-id="ef10c-537">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-537">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="ef10c-538">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-538">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="ef10c-539">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-539">Added `deployment wait` command</span></span>
* <span data-ttu-id="ef10c-540">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="ef10c-540">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="ef10c-541">SQL</span><span class="sxs-lookup"><span data-stu-id="ef10c-541">SQL</span></span>

* <span data-ttu-id="ef10c-542">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-542">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="ef10c-543">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-543">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="ef10c-544">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-544">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-545">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-545">Storage</span></span>

* <span data-ttu-id="ef10c-546">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-546">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-547">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-547">VM</span></span>

* <span data-ttu-id="ef10c-548">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ef10c-548">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="ef10c-549">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-549">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="ef10c-550">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-550">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="ef10c-551">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-551">July 3, 2018</span></span>

<span data-ttu-id="ef10c-552">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="ef10c-552">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="ef10c-553">AKS</span><span class="sxs-lookup"><span data-stu-id="ef10c-553">AKS</span></span>

* <span data-ttu-id="ef10c-554">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="ef10c-554">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="ef10c-555">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-555">July 3, 2018</span></span>

<span data-ttu-id="ef10c-556">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="ef10c-556">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-557">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-557">Core</span></span>

* <span data-ttu-id="ef10c-558">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="ef10c-558">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="ef10c-559">ACR</span><span class="sxs-lookup"><span data-stu-id="ef10c-559">ACR</span></span>

* <span data-ttu-id="ef10c-560">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="ef10c-560">Added polling build status</span></span>
* <span data-ttu-id="ef10c-561">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="ef10c-561">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="ef10c-562">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-562">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-563">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-563">ACS</span></span>

* <span data-ttu-id="ef10c-564">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ef10c-564">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="ef10c-565">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ef10c-565">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="ef10c-566">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-566">Updated options for `aks browse` command.</span></span> <span data-ttu-id="ef10c-567">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-567">Added `--listen-port` support</span></span>
* <span data-ttu-id="ef10c-568">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-568">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="ef10c-569">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="ef10c-569">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="ef10c-570">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-570">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-571">AppService</span><span class="sxs-lookup"><span data-stu-id="ef10c-571">AppService</span></span>

* <span data-ttu-id="ef10c-572">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-572">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="ef10c-573">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="ef10c-573">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="ef10c-574">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="ef10c-574">Backup</span></span>

* <span data-ttu-id="ef10c-575">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="ef10c-575">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="ef10c-576">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ef10c-576">BatchAI</span></span>

* <span data-ttu-id="ef10c-577">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-577">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="ef10c-578">Облако</span><span class="sxs-lookup"><span data-stu-id="ef10c-578">Cloud</span></span>

* <span data-ttu-id="ef10c-579">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-579">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="ef10c-580">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ef10c-580">Container</span></span>

* <span data-ttu-id="ef10c-581">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="ef10c-581">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="ef10c-582">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-582">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="ef10c-583">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="ef10c-583">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="ef10c-584">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ef10c-584">Extension</span></span>

* <span data-ttu-id="ef10c-585">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="ef10c-585">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-586">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-586">Network</span></span>

* <span data-ttu-id="ef10c-587">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-587">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="ef10c-588">Rdbms</span><span class="sxs-lookup"><span data-stu-id="ef10c-588">Rdbms</span></span>

* <span data-ttu-id="ef10c-589">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-589">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="ef10c-590">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ef10c-590">Resource</span></span>

* <span data-ttu-id="ef10c-591">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-591">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-592">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-592">VM</span></span>

* <span data-ttu-id="ef10c-593">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="ef10c-593">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="ef10c-594">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-594">June 25, 2018</span></span>

<span data-ttu-id="ef10c-595">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="ef10c-595">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="ef10c-596">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="ef10c-596">CLI</span></span>

* <span data-ttu-id="ef10c-597">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="ef10c-597">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="ef10c-598">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-598">June 19, 2018</span></span>

<span data-ttu-id="ef10c-599">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="ef10c-599">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-600">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-600">Core</span></span>

* <span data-ttu-id="ef10c-601">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="ef10c-601">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="ef10c-602">ACR</span><span class="sxs-lookup"><span data-stu-id="ef10c-602">ACR</span></span>

* <span data-ttu-id="ef10c-603">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-603">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="ef10c-604">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="ef10c-604">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-605">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-605">ACS</span></span>

* <span data-ttu-id="ef10c-606">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-606">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="ef10c-607">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-607">Added `--update` support</span></span>
* <span data-ttu-id="ef10c-608">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-608">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="ef10c-609">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-609">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="ef10c-610">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-610">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="ef10c-611">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-611">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="ef10c-612">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-612">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="ef10c-613">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-613">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-614">AppService</span><span class="sxs-lookup"><span data-stu-id="ef10c-614">AppService</span></span>

* <span data-ttu-id="ef10c-615">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="ef10c-615">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="ef10c-616">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-616">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="ef10c-617">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ef10c-617">Batch</span></span>

* <span data-ttu-id="ef10c-618">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-618">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ef10c-619">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ef10c-619">Batch AI</span></span>

* <span data-ttu-id="ef10c-620">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="ef10c-620">Added support for workspaces.</span></span> <span data-ttu-id="ef10c-621">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-621">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="ef10c-622">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-622">Added support for experiments.</span></span> <span data-ttu-id="ef10c-623">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="ef10c-623">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="ef10c-624">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="ef10c-624">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="ef10c-625">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-625">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="ef10c-626">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-626">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="ef10c-627">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-627">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="ef10c-628">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="ef10c-628">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="ef10c-629">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-629">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="ef10c-630">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-630">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="ef10c-631">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-631">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="ef10c-632">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-632">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="ef10c-633">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-633">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="ef10c-634">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-634">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="ef10c-635">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="ef10c-635">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="ef10c-636">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-636">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="ef10c-637">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="ef10c-637">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="ef10c-638">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="ef10c-638">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="ef10c-639">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="ef10c-639">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="ef10c-640">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="ef10c-640">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="ef10c-641">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="ef10c-641">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="ef10c-642">Карты</span><span class="sxs-lookup"><span data-stu-id="ef10c-642">Maps</span></span>

* <span data-ttu-id="ef10c-643">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-643">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-644">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-644">Network</span></span>

* <span data-ttu-id="ef10c-645">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="ef10c-645">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="ef10c-646">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="ef10c-646">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="ef10c-647">#6502</span><span class="sxs-lookup"><span data-stu-id="ef10c-647">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="ef10c-648">Резервирование</span><span class="sxs-lookup"><span data-stu-id="ef10c-648">Reservations</span></span>

* <span data-ttu-id="ef10c-649">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-649">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="ef10c-650">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-650">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="ef10c-651">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-651">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="ef10c-652">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-652">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="ef10c-653">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-653">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="ef10c-654">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-654">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="ef10c-655">Роль</span><span class="sxs-lookup"><span data-stu-id="ef10c-655">Role</span></span>

* <span data-ttu-id="ef10c-656">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="ef10c-656">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="ef10c-657">SQL</span><span class="sxs-lookup"><span data-stu-id="ef10c-657">SQL</span></span>

* <span data-ttu-id="ef10c-658">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="ef10c-658">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-659">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-659">Storage</span></span>

* <span data-ttu-id="ef10c-660">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="ef10c-660">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-661">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-661">VM</span></span>

* <span data-ttu-id="ef10c-662">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-662">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="ef10c-663">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-663">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="ef10c-664">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="ef10c-664">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="ef10c-665">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-665">June 13, 2018</span></span>

<span data-ttu-id="ef10c-666">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="ef10c-666">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-667">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-667">Core</span></span>

* <span data-ttu-id="ef10c-668">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="ef10c-668">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="ef10c-669">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-669">June 13, 2018</span></span>

<span data-ttu-id="ef10c-670">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="ef10c-670">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="ef10c-671">AKS</span><span class="sxs-lookup"><span data-stu-id="ef10c-671">AKS</span></span>

* <span data-ttu-id="ef10c-672">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="ef10c-672">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="ef10c-673">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="ef10c-673">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="ef10c-674">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="ef10c-674">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="ef10c-675">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="ef10c-675">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="ef10c-676">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ef10c-676">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-677">AppService</span><span class="sxs-lookup"><span data-stu-id="ef10c-677">AppService</span></span>

* <span data-ttu-id="ef10c-678">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="ef10c-678">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="ef10c-679">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-679">June 5, 2018</span></span>

<span data-ttu-id="ef10c-680">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="ef10c-680">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="ef10c-681">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef10c-681">Interactive</span></span>

* <span data-ttu-id="ef10c-682">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="ef10c-682">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="ef10c-683">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-683">June 5, 2018</span></span>

<span data-ttu-id="ef10c-684">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="ef10c-684">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-685">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-685">Core</span></span>

* <span data-ttu-id="ef10c-686">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="ef10c-686">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="ef10c-687">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="ef10c-687">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="ef10c-688">ACR</span><span class="sxs-lookup"><span data-stu-id="ef10c-688">ACR</span></span>

* <span data-ttu-id="ef10c-689">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="ef10c-689">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="ef10c-690">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-690">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="ef10c-691">AKS</span><span class="sxs-lookup"><span data-stu-id="ef10c-691">AKS</span></span>

* <span data-ttu-id="ef10c-692">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="ef10c-692">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="ef10c-693">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ef10c-693">Batch</span></span>

* <span data-ttu-id="ef10c-694">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="ef10c-694">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="ef10c-695">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ef10c-695">IOT</span></span>

* <span data-ttu-id="ef10c-696">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="ef10c-696">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-697">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-697">Network</span></span>

* <span data-ttu-id="ef10c-698">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-698">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="ef10c-699">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="ef10c-699">Policy Insights</span></span>

* <span data-ttu-id="ef10c-700">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ef10c-700">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="ef10c-701">ARM</span><span class="sxs-lookup"><span data-stu-id="ef10c-701">ARM</span></span>

* <span data-ttu-id="ef10c-702">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-702">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="ef10c-703">SQL</span><span class="sxs-lookup"><span data-stu-id="ef10c-703">SQL</span></span>

* <span data-ttu-id="ef10c-704">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="ef10c-704">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="ef10c-705">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="ef10c-705">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="ef10c-706">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-706">Storage</span></span>

* <span data-ttu-id="ef10c-707">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-707">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-708">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-708">VM</span></span>

* <span data-ttu-id="ef10c-709">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-709">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="ef10c-710">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-710">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="ef10c-711">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-711">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="ef10c-712">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-712">May 22, 2018</span></span>

<span data-ttu-id="ef10c-713">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="ef10c-713">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-714">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-714">Core</span></span>

* <span data-ttu-id="ef10c-715">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-715">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-716">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-716">ACS</span></span>

* <span data-ttu-id="ef10c-717">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-717">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="ef10c-718">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="ef10c-718">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-719">AppService</span><span class="sxs-lookup"><span data-stu-id="ef10c-719">AppService</span></span>

* <span data-ttu-id="ef10c-720">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="ef10c-720">Improved generic update commands</span></span>
* <span data-ttu-id="ef10c-721">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-721">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="ef10c-722">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ef10c-722">Container</span></span>

* <span data-ttu-id="ef10c-723">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="ef10c-723">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="ef10c-724">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ef10c-724">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="ef10c-725">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ef10c-725">Extension</span></span>

* <span data-ttu-id="ef10c-726">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="ef10c-726">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="ef10c-727">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef10c-727">Interactive</span></span>

* <span data-ttu-id="ef10c-728">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="ef10c-728">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="ef10c-729">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="ef10c-729">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="ef10c-730">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ef10c-730">KeyVault</span></span>

* <span data-ttu-id="ef10c-731">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="ef10c-731">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-732">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-732">Network</span></span>

* <span data-ttu-id="ef10c-733">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="ef10c-733">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="ef10c-734">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="ef10c-734">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="ef10c-735">SQL</span><span class="sxs-lookup"><span data-stu-id="ef10c-735">SQL</span></span>

* <span data-ttu-id="ef10c-736">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="ef10c-736">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="ef10c-737">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-737">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="ef10c-738">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-738">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="ef10c-739">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="ef10c-739">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="ef10c-740">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="ef10c-740">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="ef10c-741">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-741">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="ef10c-742">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-742">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="ef10c-743">`edition`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-743">`edition`.</span></span> <span data-ttu-id="ef10c-744">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-744">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="ef10c-745">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-745">`elasticPoolName`.</span></span> <span data-ttu-id="ef10c-746">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-746">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="ef10c-747">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="ef10c-747">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="ef10c-748">`edition`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-748">`edition`.</span></span> <span data-ttu-id="ef10c-749">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-749">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="ef10c-750">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-750">`dtu`.</span></span> <span data-ttu-id="ef10c-751">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-751">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="ef10c-752">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-752">`databaseDtuMin`.</span></span> <span data-ttu-id="ef10c-753">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-753">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="ef10c-754">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-754">`databaseDtuMax`.</span></span> <span data-ttu-id="ef10c-755">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-755">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="ef10c-756">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-756">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="ef10c-757">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-757">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-758">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-758">Storage</span></span>

* <span data-ttu-id="ef10c-759">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-759">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="ef10c-760">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-760">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-761">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-761">VM</span></span>

* <span data-ttu-id="ef10c-762">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-762">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="ef10c-763">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-763">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="ef10c-764">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-764">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="ef10c-765">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="ef10c-765">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="ef10c-766">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-766">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="ef10c-767">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-767">May 7, 2018</span></span>

<span data-ttu-id="ef10c-768">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="ef10c-768">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-769">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-769">Core</span></span>

* <span data-ttu-id="ef10c-770">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="ef10c-770">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="ef10c-771">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-771">Added limited support for positional arguments</span></span>
* <span data-ttu-id="ef10c-772">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-772">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="ef10c-773">#5591</span><span class="sxs-lookup"><span data-stu-id="ef10c-773">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="ef10c-774">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-774">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="ef10c-775">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="ef10c-775">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="ef10c-776">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="ef10c-776">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="ef10c-777">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-777">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="ef10c-778">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="ef10c-778">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="ef10c-779">ACR</span><span class="sxs-lookup"><span data-stu-id="ef10c-779">ACR</span></span>

* <span data-ttu-id="ef10c-780">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="ef10c-780">Added ACR Build commands</span></span>
* <span data-ttu-id="ef10c-781">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="ef10c-781">Improved resource not found error messages</span></span>
* <span data-ttu-id="ef10c-782">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="ef10c-782">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="ef10c-783">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="ef10c-783">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="ef10c-784">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="ef10c-784">Improved repository commands error messages</span></span>
* <span data-ttu-id="ef10c-785">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="ef10c-785">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-786">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-786">ACS</span></span>

* <span data-ttu-id="ef10c-787">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="ef10c-787">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="ef10c-788">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="ef10c-788">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="ef10c-789">AMS</span><span class="sxs-lookup"><span data-stu-id="ef10c-789">AMS</span></span>

* <span data-ttu-id="ef10c-790">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="ef10c-790">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-791">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ef10c-791">Appservice</span></span>

* <span data-ttu-id="ef10c-792">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="ef10c-792">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="ef10c-793">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-793">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="ef10c-794">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="ef10c-794">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="ef10c-795">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ef10c-795">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ef10c-796">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ef10c-796">Batch AI</span></span>

* <span data-ttu-id="ef10c-797">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="ef10c-797">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ef10c-798">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ef10c-798">Cognitive Services</span></span>

* <span data-ttu-id="ef10c-799">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="ef10c-799">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="ef10c-800">Потребление</span><span class="sxs-lookup"><span data-stu-id="ef10c-800">Consumption</span></span>

* <span data-ttu-id="ef10c-801">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="ef10c-801">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="ef10c-802">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ef10c-802">Container</span></span>

* <span data-ttu-id="ef10c-803">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="ef10c-803">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="ef10c-804">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="ef10c-804">Cosmos DB</span></span>

* <span data-ttu-id="ef10c-805">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ef10c-805">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="ef10c-806">DMS</span><span class="sxs-lookup"><span data-stu-id="ef10c-806">DMS</span></span>

* <span data-ttu-id="ef10c-807">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="ef10c-807">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="ef10c-808">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ef10c-808">Extension</span></span>

* <span data-ttu-id="ef10c-809">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="ef10c-809">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="ef10c-810">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef10c-810">Interactive</span></span>

* <span data-ttu-id="ef10c-811">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="ef10c-811">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="ef10c-812">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="ef10c-812">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="ef10c-813">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="ef10c-813">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="ef10c-814">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="ef10c-814">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="ef10c-815">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="ef10c-815">Lab</span></span>

* <span data-ttu-id="ef10c-816">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="ef10c-816">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-817">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-817">Network</span></span>

* <span data-ttu-id="ef10c-818">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="ef10c-818">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="ef10c-819">Профиль</span><span class="sxs-lookup"><span data-stu-id="ef10c-819">Profile</span></span>

* <span data-ttu-id="ef10c-820">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-820">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="ef10c-821">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="ef10c-821">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="ef10c-822">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-822">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="ef10c-823">Redis</span><span class="sxs-lookup"><span data-stu-id="ef10c-823">Redis</span></span>

* <span data-ttu-id="ef10c-824">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-824">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="ef10c-825">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="ef10c-825">Deprecated `redis list-all`.</span></span> <span data-ttu-id="ef10c-826">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-826">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="ef10c-827">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-827">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="ef10c-828">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="ef10c-828">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="ef10c-829">Роль</span><span class="sxs-lookup"><span data-stu-id="ef10c-829">Role</span></span>

* <span data-ttu-id="ef10c-830">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="ef10c-830">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-831">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-831">Storage</span></span>

* <span data-ttu-id="ef10c-832">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="ef10c-832">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="ef10c-833">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="ef10c-833">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="ef10c-834">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="ef10c-834">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="ef10c-835">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="ef10c-835">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="ef10c-836">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="ef10c-836">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-837">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-837">VM</span></span>

* <span data-ttu-id="ef10c-838">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="ef10c-838">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="ef10c-839">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="ef10c-839">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="ef10c-840">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="ef10c-840">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="ef10c-841">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-841">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="ef10c-842">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="ef10c-842">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="ef10c-843">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="ef10c-843">Added write accelerator support</span></span>
* <span data-ttu-id="ef10c-844">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-844">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="ef10c-845">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="ef10c-845">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="ef10c-846">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="ef10c-846">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="ef10c-847">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-847">April 10, 2018</span></span>

<span data-ttu-id="ef10c-848">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="ef10c-848">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="ef10c-849">ACR</span><span class="sxs-lookup"><span data-stu-id="ef10c-849">ACR</span></span>

* <span data-ttu-id="ef10c-850">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="ef10c-850">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-851">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-851">ACS</span></span>

* <span data-ttu-id="ef10c-852">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="ef10c-852">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-853">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ef10c-853">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="ef10c-855">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="ef10c-855">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="ef10c-856">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ef10c-856">BatchAI</span></span>

* <span data-ttu-id="ef10c-857">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="ef10c-857">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="ef10c-858">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="ef10c-858">Job level mounting</span></span>
  - <span data-ttu-id="ef10c-859">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-859">Environment variables with secret values</span></span>
  - <span data-ttu-id="ef10c-860">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="ef10c-860">Performance counters settings</span></span>
  - <span data-ttu-id="ef10c-861">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="ef10c-861">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="ef10c-862">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-862">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="ef10c-863">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="ef10c-863">Usage and limits reporting</span></span>
  - <span data-ttu-id="ef10c-864">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-864">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="ef10c-865">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-865">Support for custom images</span></span>
  - <span data-ttu-id="ef10c-866">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="ef10c-866">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="ef10c-867">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="ef10c-867">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="ef10c-868">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-868">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="ef10c-869">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="ef10c-869">National clouds are supported</span></span>
* <span data-ttu-id="ef10c-870">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="ef10c-870">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="ef10c-871">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="ef10c-871">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="ef10c-872">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="ef10c-872">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="ef10c-873">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="ef10c-873">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="ef10c-874">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="ef10c-874">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="ef10c-875">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="ef10c-875">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="ef10c-876">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-876">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="ef10c-877">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="ef10c-877">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="ef10c-878">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="ef10c-878">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="ef10c-879">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-879">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="ef10c-880">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="ef10c-880">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="ef10c-881">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-881">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="ef10c-882">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-882">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="ef10c-883">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="ef10c-883">Billing</span></span>

* <span data-ttu-id="ef10c-884">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="ef10c-884">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="ef10c-885">Потребление</span><span class="sxs-lookup"><span data-stu-id="ef10c-885">Consumption</span></span>

* <span data-ttu-id="ef10c-886">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-886">Added `marketplace` commands</span></span>
* <span data-ttu-id="ef10c-887">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-887">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="ef10c-888">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-888">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="ef10c-889">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-889">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="ef10c-890">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-890">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="ef10c-891">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-891">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="ef10c-892">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ef10c-892">Container</span></span>

* <span data-ttu-id="ef10c-893">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-893">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="ef10c-894">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="ef10c-894">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="ef10c-895">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ef10c-895">Extension</span></span>

* <span data-ttu-id="ef10c-896">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="ef10c-896">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="ef10c-897">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef10c-897">Interactive</span></span>

* <span data-ttu-id="ef10c-898">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="ef10c-898">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="ef10c-899">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="ef10c-899">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="ef10c-900">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-900">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-901">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-901">Network</span></span>

* <span data-ttu-id="ef10c-902">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-902">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="ef10c-903">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-903">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="ef10c-904">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="ef10c-904">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="ef10c-905">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="ef10c-905">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="ef10c-906">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="ef10c-906">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="ef10c-907">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-907">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="ef10c-908">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-908">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="ef10c-909">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="ef10c-909">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="ef10c-910">Профиль</span><span class="sxs-lookup"><span data-stu-id="ef10c-910">Profile</span></span>

* <span data-ttu-id="ef10c-911">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-911">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="ef10c-912">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-912">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="ef10c-913">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ef10c-913">RDBMS</span></span>

* <span data-ttu-id="ef10c-914">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-914">Added `georestore` command</span></span>
* <span data-ttu-id="ef10c-915">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="ef10c-915">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="ef10c-916">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ef10c-916">Resource</span></span>

* <span data-ttu-id="ef10c-917">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-917">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="ef10c-918">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-918">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="ef10c-919">SQL</span><span class="sxs-lookup"><span data-stu-id="ef10c-919">SQL</span></span>

* <span data-ttu-id="ef10c-920">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-920">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-921">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-921">Storage</span></span>

* <span data-ttu-id="ef10c-922">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="ef10c-922">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-923">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-923">VM</span></span>

* <span data-ttu-id="ef10c-924">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="ef10c-924">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="ef10c-925">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="ef10c-925">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="ef10c-927">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-927">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="ef10c-928">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="ef10c-928">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="ef10c-929">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="ef10c-929">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="ef10c-930">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="ef10c-930">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="ef10c-931">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-931">March 27, 2018</span></span>

<span data-ttu-id="ef10c-932">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="ef10c-932">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-933">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-933">Core</span></span>

* <span data-ttu-id="ef10c-934">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="ef10c-934">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-935">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-935">ACS</span></span>

* <span data-ttu-id="ef10c-936">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="ef10c-936">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-937">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ef10c-937">Appservice</span></span>

* <span data-ttu-id="ef10c-938">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-938">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="ef10c-939">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-939">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="ef10c-940">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="ef10c-940">Backup</span></span>

* <span data-ttu-id="ef10c-941">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-941">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="ef10c-942">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="ef10c-942">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="ef10c-943">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="ef10c-943">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="ef10c-944">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-944">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="ef10c-945">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ef10c-945">Container</span></span>

* <span data-ttu-id="ef10c-946">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-946">Added `container exec` command.</span></span> <span data-ttu-id="ef10c-947">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ef10c-947">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="ef10c-948">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ef10c-948">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="ef10c-949">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ef10c-949">Extension</span></span>

* <span data-ttu-id="ef10c-950">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="ef10c-950">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="ef10c-951">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-951">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="ef10c-952">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ef10c-952">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="ef10c-953">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef10c-953">Interactive</span></span>

* <span data-ttu-id="ef10c-954">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="ef10c-954">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="ef10c-955">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-955">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="ef10c-956">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="ef10c-956">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="ef10c-957">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="ef10c-957">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="ef10c-958">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="ef10c-958">Lab</span></span>

* <span data-ttu-id="ef10c-959">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-959">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="ef10c-960">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ef10c-960">Monitor</span></span>

* <span data-ttu-id="ef10c-961">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="ef10c-961">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="ef10c-962">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="ef10c-962">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="ef10c-963">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="ef10c-963">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-964">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-964">Network</span></span>

* <span data-ttu-id="ef10c-965">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="ef10c-965">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="ef10c-966">Профиль</span><span class="sxs-lookup"><span data-stu-id="ef10c-966">Profile</span></span>

* <span data-ttu-id="ef10c-967">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-967">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="ef10c-968">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ef10c-968">RDBMS</span></span>

* <span data-ttu-id="ef10c-969">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="ef10c-969">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="ef10c-970">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ef10c-970">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="ef10c-972">Роль</span><span class="sxs-lookup"><span data-stu-id="ef10c-972">Role</span></span>

* <span data-ttu-id="ef10c-973">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-973">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="ef10c-974">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="ef10c-974">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="ef10c-975">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="ef10c-975">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="ef10c-976">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-976">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="ef10c-977">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-977">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-978">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-978">Storage</span></span>

* <span data-ttu-id="ef10c-979">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="ef10c-979">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="ef10c-980">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049): проблемы, когда при отправке добавочного большого двоичного объекта игнорируются параметры условия.</span><span class="sxs-lookup"><span data-stu-id="ef10c-980">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-981">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-981">VM</span></span>

* <span data-ttu-id="ef10c-982">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="ef10c-982">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="ef10c-983">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-983">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="ef10c-984">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="ef10c-984">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="ef10c-985">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="ef10c-985">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="ef10c-986">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-986">March 13, 2018</span></span>

<span data-ttu-id="ef10c-987">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="ef10c-987">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="ef10c-988">ACR</span><span class="sxs-lookup"><span data-stu-id="ef10c-988">ACR</span></span>

* <span data-ttu-id="ef10c-989">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-989">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="ef10c-990">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="ef10c-990">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="ef10c-991">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="ef10c-991">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-992">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-992">ACS</span></span>

* <span data-ttu-id="ef10c-993">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="ef10c-993">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="ef10c-994">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="ef10c-994">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="ef10c-995">Помощник</span><span class="sxs-lookup"><span data-stu-id="ef10c-995">Advisor</span></span>

* <span data-ttu-id="ef10c-996">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-996">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="ef10c-997">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-997">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="ef10c-998">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-998">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="ef10c-999">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-999">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="ef10c-1000">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1000">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-1001">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ef10c-1001">Appservice</span></span>

* <span data-ttu-id="ef10c-1002">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1002">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="ef10c-1003">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1003">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="ef10c-1004">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="ef10c-1004">Eventhubs</span></span>

* <span data-ttu-id="ef10c-1005">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ef10c-1005">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="ef10c-1006">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ef10c-1006">Extension</span></span>

* <span data-ttu-id="ef10c-1007">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1007">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="ef10c-1008">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef10c-1008">Interactive</span></span>

* <span data-ttu-id="ef10c-1009">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625): теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1009">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="ef10c-1010">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016): при использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1010">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="ef10c-1011">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688): если при загрузке таблицы команд возникало исключение, опережающий ввод не выполнялся.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1011">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="ef10c-1012">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1012">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="ef10c-1013">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ef10c-1013">Monitor</span></span>

* <span data-ttu-id="ef10c-1014">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1014">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="ef10c-1015">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1015">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="ef10c-1016">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1016">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="ef10c-1017">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1017">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-1018">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-1018">Network</span></span>

* <span data-ttu-id="ef10c-1019">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1019">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="ef10c-1020">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="ef10c-1020">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="ef10c-1021">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1021">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="ef10c-1022">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1022">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="ef10c-1023">Профиль</span><span class="sxs-lookup"><span data-stu-id="ef10c-1023">Profile</span></span>

* <span data-ttu-id="ef10c-1024">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1024">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="ef10c-1025">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1025">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="ef10c-1026">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ef10c-1026">RDBMS</span></span>

* <span data-ttu-id="ef10c-1027">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1027">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="ef10c-1028">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="ef10c-1028">Service Bus</span></span>

* <span data-ttu-id="ef10c-1029">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ef10c-1029">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-1030">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-1030">Storage</span></span>

* <span data-ttu-id="ef10c-1031">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1031">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="ef10c-1032">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286): при пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1032">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-1033">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-1033">VM</span></span>

* <span data-ttu-id="ef10c-1034">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1034">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="ef10c-1035">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1035">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="ef10c-1036">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1036">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="ef10c-1037">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1037">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="ef10c-1038">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="ef10c-1038">February 27, 2018</span></span>

<span data-ttu-id="ef10c-1039">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="ef10c-1039">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-1040">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-1040">Core</span></span>

* <span data-ttu-id="ef10c-1041">Исправлена ошибка с установкой Homebrew [#5184](https://github.com/Azure/azure-cli/issues/5184).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1041">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="ef10c-1042">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1042">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="ef10c-1043">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1043">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-1044">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-1044">ACS</span></span>

* <span data-ttu-id="ef10c-1045">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1045">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="ef10c-1046">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1046">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="ef10c-1047">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1047">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="ef10c-1048">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1048">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-1049">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ef10c-1049">Appservice</span></span>

* <span data-ttu-id="ef10c-1050">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="ef10c-1050">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="ef10c-1051">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1051">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ef10c-1052">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ef10c-1052">Cognitive Services</span></span>

* <span data-ttu-id="ef10c-1053">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1053">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="ef10c-1054">Потребление</span><span class="sxs-lookup"><span data-stu-id="ef10c-1054">Consumption</span></span>

* <span data-ttu-id="ef10c-1055">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1055">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="ef10c-1056">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1056">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="ef10c-1057">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ef10c-1057">Container</span></span>

* <span data-ttu-id="ef10c-1058">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1058">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-1059">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-1059">Network</span></span>

* <span data-ttu-id="ef10c-1060">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559): отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1060">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="ef10c-1061">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ef10c-1061">Resource</span></span>

* <span data-ttu-id="ef10c-1062">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1062">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="ef10c-1063">Роль</span><span class="sxs-lookup"><span data-stu-id="ef10c-1063">Role</span></span>

* <span data-ttu-id="ef10c-1064">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1064">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="ef10c-1065">SQL</span><span class="sxs-lookup"><span data-stu-id="ef10c-1065">SQL</span></span>

* <span data-ttu-id="ef10c-1066">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1066">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-1067">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-1067">Storage</span></span>

* <span data-ttu-id="ef10c-1068">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1068">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-1069">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-1069">VM</span></span>

* <span data-ttu-id="ef10c-1070">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1070">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="ef10c-1071">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1071">February 13, 2018</span></span>

<span data-ttu-id="ef10c-1072">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="ef10c-1072">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-1073">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-1073">Core</span></span>

* <span data-ttu-id="ef10c-1074">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1074">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-1075">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-1075">ACS</span></span>

* <span data-ttu-id="ef10c-1076">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1076">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="ef10c-1077">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1077">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="ef10c-1078">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1078">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="ef10c-1079">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1079">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="ef10c-1080">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1080">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="ef10c-1081">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1081">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="ef10c-1082">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1082">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="ef10c-1083">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1083">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-1084">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ef10c-1084">Appservice</span></span>

* <span data-ttu-id="ef10c-1085">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1085">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="ef10c-1086">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1086">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="ef10c-1087">CDN</span><span class="sxs-lookup"><span data-stu-id="ef10c-1087">CDN</span></span>

* <span data-ttu-id="ef10c-1088">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1088">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="ef10c-1089">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ef10c-1089">Container</span></span>

* <span data-ttu-id="ef10c-1090">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1090">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="ef10c-1091">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1091">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ef10c-1092">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ef10c-1092">CosmosDB</span></span>

* <span data-ttu-id="ef10c-1093">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1093">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="ef10c-1094">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ef10c-1094">Extension</span></span>

* <span data-ttu-id="ef10c-1095">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1095">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="ef10c-1096">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1096">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="ef10c-1097">Отзыв</span><span class="sxs-lookup"><span data-stu-id="ef10c-1097">Feedback</span></span>

* <span data-ttu-id="ef10c-1098">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1098">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="ef10c-1099">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef10c-1099">Interactive</span></span>

* <span data-ttu-id="ef10c-1100">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1100">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="ef10c-1101">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1101">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="ef10c-1102">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ef10c-1102">IoT</span></span>

* <span data-ttu-id="ef10c-1103">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="ef10c-1103">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="ef10c-1104">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="ef10c-1104">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="ef10c-1105">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1105">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="ef10c-1106">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1106">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="ef10c-1107">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ef10c-1107">Monitor</span></span>

* <span data-ttu-id="ef10c-1108">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1108">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-1109">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-1109">Network</span></span>

* <span data-ttu-id="ef10c-1110">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="ef10c-1110">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="ef10c-1111">Профиль</span><span class="sxs-lookup"><span data-stu-id="ef10c-1111">Profile</span></span>

* <span data-ttu-id="ef10c-1112">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1112">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="ef10c-1113">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ef10c-1113">Resource</span></span>

* <span data-ttu-id="ef10c-1114">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1114">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="ef10c-1115">Роль</span><span class="sxs-lookup"><span data-stu-id="ef10c-1115">Role</span></span>

* <span data-ttu-id="ef10c-1116">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1116">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="ef10c-1117">SQL</span><span class="sxs-lookup"><span data-stu-id="ef10c-1117">SQL</span></span>

* <span data-ttu-id="ef10c-1118">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1118">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="ef10c-1119">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1119">Added `sql db rename`</span></span>
* <span data-ttu-id="ef10c-1120">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1120">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-1121">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-1121">Storage</span></span>

* <span data-ttu-id="ef10c-1122">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1122">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-1123">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-1123">VM</span></span>

* <span data-ttu-id="ef10c-1124">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1124">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="ef10c-1125">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1125">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="ef10c-1126">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1126">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="ef10c-1127">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1127">January 31, 2018</span></span>

<span data-ttu-id="ef10c-1128">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="ef10c-1128">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-1129">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-1129">Core</span></span>

* <span data-ttu-id="ef10c-1130">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1130">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="ef10c-1131">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1131">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="ef10c-1132">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1132">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="ef10c-1133">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1133">Use `--verbose` to see</span></span>
* <span data-ttu-id="ef10c-1134">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1134">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-1135">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-1135">ACS</span></span>

* <span data-ttu-id="ef10c-1136">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1136">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="ef10c-1137">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1137">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-1138">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ef10c-1138">Appservice</span></span>

* <span data-ttu-id="ef10c-1139">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1139">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="ef10c-1140">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1140">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="ef10c-1141">CDN</span><span class="sxs-lookup"><span data-stu-id="ef10c-1141">CDN</span></span>

* <span data-ttu-id="ef10c-1142">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1142">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ef10c-1143">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ef10c-1143">CosmosDB</span></span>

* <span data-ttu-id="ef10c-1144">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1144">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="ef10c-1145">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef10c-1145">Interactive</span></span>

* <span data-ttu-id="ef10c-1146">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1146">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-1147">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-1147">Network</span></span>

* <span data-ttu-id="ef10c-1148">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1148">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="ef10c-1149">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1149">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="ef10c-1150">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1150">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="ef10c-1151">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1151">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="ef10c-1152">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1152">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="ef10c-1153">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="ef10c-1153">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="ef10c-1154">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1154">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="ef10c-1155">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1155">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="ef10c-1156">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1156">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="ef10c-1157">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1157">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="ef10c-1158">Профиль</span><span class="sxs-lookup"><span data-stu-id="ef10c-1158">Profile</span></span>

* <span data-ttu-id="ef10c-1159">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1159">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="ef10c-1160">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ef10c-1160">Resource</span></span>

* <span data-ttu-id="ef10c-1161">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1161">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-1162">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-1162">Storage</span></span>

* <span data-ttu-id="ef10c-1163">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1163">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="ef10c-1164">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1164">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="ef10c-1165">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1165">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="ef10c-1166">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1166">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="ef10c-1167">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1167">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-1168">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-1168">VM</span></span>

* <span data-ttu-id="ef10c-1169">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1169">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="ef10c-1170">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1170">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="ef10c-1171">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1171">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="ef10c-1172">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1172">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="ef10c-1173">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1173">January 17, 2018</span></span>

<span data-ttu-id="ef10c-1174">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="ef10c-1174">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="ef10c-1175">ACR</span><span class="sxs-lookup"><span data-stu-id="ef10c-1175">ACR</span></span>

* <span data-ttu-id="ef10c-1176">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1176">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="ef10c-1177">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1177">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-1178">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-1178">ACS</span></span>

* <span data-ttu-id="ef10c-1179">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1179">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="ef10c-1180">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1180">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-1181">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ef10c-1181">Appservice</span></span>

* <span data-ttu-id="ef10c-1182">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1182">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="ef10c-1183">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1183">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="ef10c-1184">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1184">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="ef10c-1185">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="ef10c-1185">Backup</span></span>

* <span data-ttu-id="ef10c-1186">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1186">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="ef10c-1187">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1187">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="ef10c-1188">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1188">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="ef10c-1189">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1189">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="ef10c-1190">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1190">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="ef10c-1191">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ef10c-1191">Batch</span></span>

* <span data-ttu-id="ef10c-1192">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1192">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="ef10c-1193">Облако</span><span class="sxs-lookup"><span data-stu-id="ef10c-1193">Cloud</span></span>

* <span data-ttu-id="ef10c-1194">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1194">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="ef10c-1195">Потребление</span><span class="sxs-lookup"><span data-stu-id="ef10c-1195">Consumption</span></span>

* <span data-ttu-id="ef10c-1196">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1196">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="ef10c-1197">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="ef10c-1197">Event Grid</span></span>

* <span data-ttu-id="ef10c-1198">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1198">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="ef10c-1199">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1199">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="ef10c-1200">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1200">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="ef10c-1201">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1201">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="ef10c-1202">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1202">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="ef10c-1203">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1203">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="ef10c-1204">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1204">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="ef10c-1205">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1205">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="ef10c-1206">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef10c-1206">Interactive</span></span>

* <span data-ttu-id="ef10c-1207">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1207">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="ef10c-1208">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1208">Fixed errors on startup</span></span>
* <span data-ttu-id="ef10c-1209">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1209">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="ef10c-1210">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ef10c-1210">IoT</span></span>

* <span data-ttu-id="ef10c-1211">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1211">Added support for device provisioning service</span></span>
* <span data-ttu-id="ef10c-1212">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1212">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="ef10c-1213">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1213">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="ef10c-1214">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ef10c-1214">Monitor</span></span>

* <span data-ttu-id="ef10c-1215">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1215">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="ef10c-1216">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1216">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="ef10c-1217">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1217">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-1218">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-1218">Network</span></span>

* <span data-ttu-id="ef10c-1219">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1219">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="ef10c-1220">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1220">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="ef10c-1221">Профиль</span><span class="sxs-lookup"><span data-stu-id="ef10c-1221">Profile</span></span>

* <span data-ttu-id="ef10c-1222">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1222">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="ef10c-1223">Роль</span><span class="sxs-lookup"><span data-stu-id="ef10c-1223">Role</span></span>

* <span data-ttu-id="ef10c-1224">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1224">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ef10c-1225">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ef10c-1225">Service Fabric</span></span>

* <span data-ttu-id="ef10c-1226">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1226">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="ef10c-1227">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1227">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-1228">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-1228">VM</span></span>

* <span data-ttu-id="ef10c-1229">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1229">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="ef10c-1230">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="ef10c-1230">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="ef10c-1231">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1231">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="ef10c-1232">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1232">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="ef10c-1233">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1233">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="ef10c-1234">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1234">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="ef10c-1235">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1235">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="ef10c-1236">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1236">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="ef10c-1237">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1237">December 19, 2017</span></span>

<span data-ttu-id="ef10c-1238">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="ef10c-1238">Version 2.0.23</span></span>

* <span data-ttu-id="ef10c-1239">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1239">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="ef10c-1240">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ef10c-1240">Container</span></span>

* <span data-ttu-id="ef10c-1241">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1241">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-1242">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-1242">Network</span></span>

* <span data-ttu-id="ef10c-1243">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1243">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="ef10c-1244">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1244">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-1245">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-1245">Storage</span></span>

* <span data-ttu-id="ef10c-1246">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1246">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-1247">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-1247">VM</span></span>

* <span data-ttu-id="ef10c-1248">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1248">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="ef10c-1249">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1249">December 5, 2017</span></span>

<span data-ttu-id="ef10c-1250">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="ef10c-1250">Version 2.0.22</span></span>

* <span data-ttu-id="ef10c-1251">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1251">Removed `az component` commands.</span></span> <span data-ttu-id="ef10c-1252">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1252">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-1253">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-1253">Core</span></span>
* <span data-ttu-id="ef10c-1254">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1254">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="ef10c-1255">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1255">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-1256">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-1256">ACS</span></span>

* <span data-ttu-id="ef10c-1257">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1257">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="ef10c-1258">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1258">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="ef10c-1259">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1259">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="ef10c-1260">Помощник</span><span class="sxs-lookup"><span data-stu-id="ef10c-1260">Advisor</span></span>

* <span data-ttu-id="ef10c-1261">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ef10c-1261">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-1262">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ef10c-1262">Appservice</span></span>

* <span data-ttu-id="ef10c-1263">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1263">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="ef10c-1264">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1264">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="ef10c-1265">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1265">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="ef10c-1266">Потребление</span><span class="sxs-lookup"><span data-stu-id="ef10c-1266">Consumption</span></span>

* <span data-ttu-id="ef10c-1267">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1267">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="ef10c-1268">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ef10c-1268">Container</span></span>

* <span data-ttu-id="ef10c-1269">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1269">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="ef10c-1270">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ef10c-1270">Monitor</span></span>

* <span data-ttu-id="ef10c-1271">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1271">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="ef10c-1272">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ef10c-1272">Resource</span></span>

* <span data-ttu-id="ef10c-1273">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1273">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="ef10c-1274">Роль</span><span class="sxs-lookup"><span data-stu-id="ef10c-1274">Role</span></span>

* <span data-ttu-id="ef10c-1275">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1275">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="ef10c-1276">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1276">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="ef10c-1277">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1277">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="ef10c-1278">SQL</span><span class="sxs-lookup"><span data-stu-id="ef10c-1278">SQL</span></span>

* <span data-ttu-id="ef10c-1279">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1279">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="ef10c-1280">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1280">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-1281">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-1281">VM</span></span>

* <span data-ttu-id="ef10c-1282">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1282">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="ef10c-1283">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1283">November 14, 2017</span></span>

<span data-ttu-id="ef10c-1284">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="ef10c-1284">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="ef10c-1285">ACR</span><span class="sxs-lookup"><span data-stu-id="ef10c-1285">ACR</span></span>

* <span data-ttu-id="ef10c-1286">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1286">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="ef10c-1287">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-1287">ACS</span></span>

* <span data-ttu-id="ef10c-1288">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1288">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="ef10c-1289">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1289">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="ef10c-1290">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1290">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="ef10c-1291">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1291">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="ef10c-1292">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1292">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-1293">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ef10c-1293">Appservice</span></span>

* <span data-ttu-id="ef10c-1294">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1294">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="ef10c-1295">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1295">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="ef10c-1296">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1296">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="ef10c-1297">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1297">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="ef10c-1298">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="ef10c-1298">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="ef10c-1299">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1299">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="ef10c-1300">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ef10c-1300">Batch</span></span>

* <span data-ttu-id="ef10c-1301">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1301">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="ef10c-1302">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ef10c-1302">Batchai</span></span>

* <span data-ttu-id="ef10c-1303">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1303">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="ef10c-1304">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1304">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="ef10c-1305">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1305">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="ef10c-1306">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1306">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="ef10c-1307">Облако</span><span class="sxs-lookup"><span data-stu-id="ef10c-1307">Cloud</span></span>

* <span data-ttu-id="ef10c-1308">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1308">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="ef10c-1309">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ef10c-1309">Container</span></span>

* <span data-ttu-id="ef10c-1310">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1310">Added support to open multiple ports</span></span>
* <span data-ttu-id="ef10c-1311">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1311">Added container group restart policy</span></span>
* <span data-ttu-id="ef10c-1312">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1312">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="ef10c-1313">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1313">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ef10c-1314">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ef10c-1314">Data Lake Analytics</span></span>

* <span data-ttu-id="ef10c-1315">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1315">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ef10c-1316">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ef10c-1316">Data Lake Store</span></span>

* <span data-ttu-id="ef10c-1317">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1317">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="ef10c-1318">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ef10c-1318">Extension</span></span>

* <span data-ttu-id="ef10c-1319">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1319">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="ef10c-1320">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1320">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="ef10c-1321">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ef10c-1321">IoT</span></span>

* <span data-ttu-id="ef10c-1322">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1322">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="ef10c-1323">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ef10c-1323">Monitor</span></span>

* <span data-ttu-id="ef10c-1324">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1324">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-1325">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-1325">Network</span></span>

* <span data-ttu-id="ef10c-1326">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1326">Added support for CAA DNS records</span></span>
* <span data-ttu-id="ef10c-1327">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1327">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="ef10c-1328">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1328">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="ef10c-1329">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1329">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="ef10c-1330">Резервирование</span><span class="sxs-lookup"><span data-stu-id="ef10c-1330">Reservations</span></span>

* <span data-ttu-id="ef10c-1331">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="ef10c-1331">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="ef10c-1332">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ef10c-1332">Resource</span></span>

* <span data-ttu-id="ef10c-1333">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1333">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="ef10c-1334">SQL</span><span class="sxs-lookup"><span data-stu-id="ef10c-1334">SQL</span></span>

* <span data-ttu-id="ef10c-1335">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1335">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-1336">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-1336">Storage</span></span>

* <span data-ttu-id="ef10c-1337">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1337">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="ef10c-1338">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1338">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="ef10c-1339">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1339">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="ef10c-1340">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1340">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="ef10c-1341">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1341">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="ef10c-1342">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1342">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="ef10c-1343">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1343">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-1344">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-1344">VM</span></span>

* <span data-ttu-id="ef10c-1345">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1345">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="ef10c-1346">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1346">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="ef10c-1347">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1347">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="ef10c-1348">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1348">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="ef10c-1349">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1349">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="ef10c-1350">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1350">October 24, 2017</span></span>

<span data-ttu-id="ef10c-1351">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="ef10c-1351">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-1352">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-1352">Core</span></span>

* <span data-ttu-id="ef10c-1353">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1353">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="ef10c-1354">ACR</span><span class="sxs-lookup"><span data-stu-id="ef10c-1354">ACR</span></span>

* <span data-ttu-id="ef10c-1355">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1355">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="ef10c-1356">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="ef10c-1356">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="ef10c-1357">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="ef10c-1357">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-1358">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-1358">ACS</span></span>

* <span data-ttu-id="ef10c-1359">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1359">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="ef10c-1360">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1360">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-1361">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ef10c-1361">Appservice</span></span>

* <span data-ttu-id="ef10c-1362">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1362">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="ef10c-1363">Компонент</span><span class="sxs-lookup"><span data-stu-id="ef10c-1363">Component</span></span>

* <span data-ttu-id="ef10c-1364">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="ef10c-1364">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="ef10c-1365">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ef10c-1365">Monitor</span></span>

* <span data-ttu-id="ef10c-1366">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1366">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="ef10c-1367">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ef10c-1367">Resource</span></span>

* <span data-ttu-id="ef10c-1368">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1368">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="ef10c-1369">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="ef10c-1369">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-1370">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-1370">VM</span></span>

* <span data-ttu-id="ef10c-1371">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1371">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="ef10c-1372">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1372">October 9, 2017</span></span>

<span data-ttu-id="ef10c-1373">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="ef10c-1373">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-1374">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-1374">Core</span></span>

* <span data-ttu-id="ef10c-1375">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1375">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-1376">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ef10c-1376">Appservice</span></span>

* <span data-ttu-id="ef10c-1377">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1377">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="ef10c-1378">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ef10c-1378">Batch</span></span>

* <span data-ttu-id="ef10c-1379">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="ef10c-1379">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="ef10c-1380">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1380">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="ef10c-1381">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1381">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="ef10c-1382">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1382">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="ef10c-1383">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ef10c-1383">Batchai</span></span>

* <span data-ttu-id="ef10c-1384">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ef10c-1384">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="ef10c-1385">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ef10c-1385">Keyvault</span></span>

* <span data-ttu-id="ef10c-1386">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1386">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="ef10c-1387">(#4448)</span><span class="sxs-lookup"><span data-stu-id="ef10c-1387">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="ef10c-1388">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-1388">Network</span></span>

* <span data-ttu-id="ef10c-1389">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1389">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="ef10c-1390">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1390">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="ef10c-1391">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ef10c-1391">Resource</span></span>

* <span data-ttu-id="ef10c-1392">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1392">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="ef10c-1393">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1393">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="ef10c-1394">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1394">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="ef10c-1395">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1395">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="ef10c-1396">SQL</span><span class="sxs-lookup"><span data-stu-id="ef10c-1396">Sql</span></span>

* <span data-ttu-id="ef10c-1397">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1397">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="ef10c-1398">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1398">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="ef10c-1399">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1399">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-1400">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-1400">Storage</span></span>

* <span data-ttu-id="ef10c-1401">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1401">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-1402">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="ef10c-1402">Vm</span></span>

* <span data-ttu-id="ef10c-1403">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1403">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="ef10c-1404">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1404">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="ef10c-1405">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1405">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="ef10c-1406">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1406">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="ef10c-1407">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1407">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="ef10c-1408">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1408">September 22, 2017</span></span>

<span data-ttu-id="ef10c-1409">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="ef10c-1409">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="ef10c-1410">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ef10c-1410">Resource</span></span>

* <span data-ttu-id="ef10c-1411">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="ef10c-1411">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="ef10c-1412">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="ef10c-1412">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="ef10c-1413">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1413">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="ef10c-1414">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1414">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-1415">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-1415">Network</span></span>

* <span data-ttu-id="ef10c-1416">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1416">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="ef10c-1417">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1417">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="ef10c-1418">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1418">Added `asg` application security group commands</span></span>
* <span data-ttu-id="ef10c-1419">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1419">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="ef10c-1420">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1420">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="ef10c-1421">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1421">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="ef10c-1422">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1422">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-1423">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-1423">Storage</span></span>

* <span data-ttu-id="ef10c-1424">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="ef10c-1424">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="ef10c-1425">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="ef10c-1425">Eventgrid</span></span>

* <span data-ttu-id="ef10c-1426">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="ef10c-1426">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="ef10c-1427">SQL</span><span class="sxs-lookup"><span data-stu-id="ef10c-1427">SQL</span></span>

* <span data-ttu-id="ef10c-1428">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1428">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="ef10c-1429">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="ef10c-1429">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="ef10c-1430">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1430">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="ef10c-1431">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ef10c-1431">Keyvault</span></span>

* <span data-ttu-id="ef10c-1432">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="ef10c-1432">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-1433">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-1433">VM</span></span>

* <span data-ttu-id="ef10c-1434">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1434">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="ef10c-1435">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="ef10c-1435">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="ef10c-1436">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1436">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="ef10c-1437">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1437">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="ef10c-1438">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1438">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="ef10c-1439">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1439">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-1440">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-1440">ACS</span></span>

* <span data-ttu-id="ef10c-1441">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="ef10c-1441">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-1442">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ef10c-1442">Appservice</span></span>

* <span data-ttu-id="ef10c-1443">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="ef10c-1443">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="ef10c-1444">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="ef10c-1444">Backup</span></span>

* <span data-ttu-id="ef10c-1445">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1445">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="ef10c-1446">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1446">September 11, 2017</span></span>

<span data-ttu-id="ef10c-1447">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="ef10c-1447">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="ef10c-1448">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-1448">Core</span></span>

* <span data-ttu-id="ef10c-1449">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1449">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="ef10c-1450">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1450">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-1451">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-1451">Acs</span></span>

* <span data-ttu-id="ef10c-1452">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1452">Added `acs list-locations` command</span></span>
* <span data-ttu-id="ef10c-1453">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1453">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-1454">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ef10c-1454">Appservice</span></span>

* <span data-ttu-id="ef10c-1455">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1455">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="ef10c-1456">CDN</span><span class="sxs-lookup"><span data-stu-id="ef10c-1456">CDN</span></span>

* <span data-ttu-id="ef10c-1457">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1457">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="ef10c-1458">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ef10c-1458">Extension</span></span>

* <span data-ttu-id="ef10c-1459">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ef10c-1459">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="ef10c-1460">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ef10c-1460">Keyvault</span></span>

* <span data-ttu-id="ef10c-1461">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1461">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-1462">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-1462">Network</span></span>

* <span data-ttu-id="ef10c-1463">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1463">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="ef10c-1464">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1464">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="ef10c-1465">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1465">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="ef10c-1466">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1466">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="ef10c-1467">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1467">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="ef10c-1468">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ef10c-1468">Resource</span></span>

* <span data-ttu-id="ef10c-1469">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1469">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="ef10c-1470">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1470">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="ef10c-1471">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1471">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="ef10c-1472">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1472">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="ef10c-1473">SQL</span><span class="sxs-lookup"><span data-stu-id="ef10c-1473">SQL</span></span>

* <span data-ttu-id="ef10c-1474">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1474">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-1475">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-1475">VM</span></span>

* <span data-ttu-id="ef10c-1476">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1476">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="ef10c-1477">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1477">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="ef10c-1478">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1478">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="ef10c-1479">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1479">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="ef10c-1480">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1480">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="ef10c-1481">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1481">August 31, 2017</span></span>

<span data-ttu-id="ef10c-1482">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="ef10c-1482">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="ef10c-1483">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ef10c-1483">Keyvault</span></span>

* <span data-ttu-id="ef10c-1484">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1484">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="ef10c-1485">Sf</span><span class="sxs-lookup"><span data-stu-id="ef10c-1485">Sf</span></span>

* <span data-ttu-id="ef10c-1486">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1486">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-1487">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-1487">Storage</span></span>

* <span data-ttu-id="ef10c-1488">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1488">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="ef10c-1489">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1489">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="ef10c-1490">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1490">August 28, 2017</span></span>

<span data-ttu-id="ef10c-1491">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="ef10c-1491">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="ef10c-1492">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="ef10c-1492">CLI</span></span>

* <span data-ttu-id="ef10c-1493">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1493">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-1494">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-1494">ACS</span></span>

* <span data-ttu-id="ef10c-1495">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1495">Corrected preview regions</span></span>
* <span data-ttu-id="ef10c-1496">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1496">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="ef10c-1497">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1497">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-1498">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ef10c-1498">Appservice</span></span>

* <span data-ttu-id="ef10c-1499">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1499">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="ef10c-1500">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1500">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="ef10c-1501">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1501">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="ef10c-1502">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1502">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="ef10c-1503">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1503">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="ef10c-1504">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ef10c-1504">IoT</span></span>

* <span data-ttu-id="ef10c-1505">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1505">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-1506">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-1506">Network</span></span>

* <span data-ttu-id="ef10c-1507">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1507">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="ef10c-1508">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1508">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="ef10c-1509">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1509">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="ef10c-1510">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1510">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="ef10c-1511">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1511">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="ef10c-1512">Профиль</span><span class="sxs-lookup"><span data-stu-id="ef10c-1512">Profile</span></span>

* <span data-ttu-id="ef10c-1513">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1513">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ef10c-1514">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ef10c-1514">Service Fabric</span></span>

* <span data-ttu-id="ef10c-1515">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1515">Preview release</span></span>
* <span data-ttu-id="ef10c-1516">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1516">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="ef10c-1517">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1517">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="ef10c-1518">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1518">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-1519">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-1519">Storage</span></span>

* <span data-ttu-id="ef10c-1520">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1520">Enabled setting blob tier</span></span>
* <span data-ttu-id="ef10c-1521">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1521">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="ef10c-1522">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1522">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="ef10c-1523">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1523">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="ef10c-1524">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1524">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="ef10c-1525">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1525">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-1526">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-1526">VM</span></span>

* <span data-ttu-id="ef10c-1527">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1527">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="ef10c-1528">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1528">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="ef10c-1529">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1529">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="ef10c-1530">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1530">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="ef10c-1531">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1531">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="ef10c-1532">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1532">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="ef10c-1533">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1533">August 15, 2017</span></span>

<span data-ttu-id="ef10c-1534">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="ef10c-1534">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-1535">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-1535">ACS</span></span>

* <span data-ttu-id="ef10c-1536">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1536">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-1537">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ef10c-1537">Appservice</span></span>

* <span data-ttu-id="ef10c-1538">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1538">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="ef10c-1539">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="ef10c-1539">Event Grid</span></span>

* <span data-ttu-id="ef10c-1540">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1540">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="ef10c-1541">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1541">August 11, 2017</span></span>

<span data-ttu-id="ef10c-1542">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="ef10c-1542">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-1543">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-1543">ACS</span></span>

* <span data-ttu-id="ef10c-1544">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1544">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="ef10c-1545">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ef10c-1545">Batch</span></span>

* <span data-ttu-id="ef10c-1546">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1546">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="ef10c-1547">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1547">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="ef10c-1548">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1548">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="ef10c-1549">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1549">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="ef10c-1550">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1550">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="ef10c-1551">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1551">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="ef10c-1552">Компонент</span><span class="sxs-lookup"><span data-stu-id="ef10c-1552">Component</span></span>

* <span data-ttu-id="ef10c-1553">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1553">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="ef10c-1554">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ef10c-1554">Container</span></span>

* <span data-ttu-id="ef10c-1555">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1555">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="ef10c-1556">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ef10c-1556">Data Lake Store</span></span>

* <span data-ttu-id="ef10c-1557">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1557">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="ef10c-1558">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="ef10c-1558">Event Grid</span></span>

* <span data-ttu-id="ef10c-1559">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ef10c-1559">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-1560">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-1560">Network</span></span>

* <span data-ttu-id="ef10c-1561">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1561">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="ef10c-1562">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1562">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="ef10c-1563">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1563">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="ef10c-1564">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1564">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="ef10c-1565">Профиль</span><span class="sxs-lookup"><span data-stu-id="ef10c-1565">Profile</span></span>

* <span data-ttu-id="ef10c-1566">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1566">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-1567">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-1567">Storage</span></span>

* <span data-ttu-id="ef10c-1568">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1568">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-1569">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-1569">VM</span></span>

* <span data-ttu-id="ef10c-1570">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1570">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="ef10c-1571">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1571">Exposed `list-skus` command</span></span>
* <span data-ttu-id="ef10c-1572">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1572">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="ef10c-1573">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1573">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="ef10c-1574">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1574">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="ef10c-1575">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1575">July 28, 2017</span></span>

<span data-ttu-id="ef10c-1576">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="ef10c-1576">Version 2.0.12</span></span>

* <span data-ttu-id="ef10c-1577">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1577">Added container commands</span></span>
* <span data-ttu-id="ef10c-1578">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1578">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="ef10c-1579">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-1579">Core</span></span>

* <span data-ttu-id="ef10c-1580">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1580">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="ef10c-1581">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1581">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="ef10c-1582">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1582">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="ef10c-1583">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1583">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="ef10c-1584">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1584">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="ef10c-1585">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1585">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="ef10c-1586">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1586">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="ef10c-1587">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1587">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="ef10c-1588">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1588">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="ef10c-1589">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1589">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="ef10c-1590">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1590">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="ef10c-1591">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1591">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="ef10c-1592">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1592">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="ef10c-1593">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1593">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="ef10c-1594">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1594">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="ef10c-1595">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1595">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="ef10c-1596">ACR</span><span class="sxs-lookup"><span data-stu-id="ef10c-1596">ACR</span></span>

* <span data-ttu-id="ef10c-1597">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1597">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="ef10c-1598">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1598">Support SKU update for managed registries</span></span>
* <span data-ttu-id="ef10c-1599">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1599">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="ef10c-1600">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1600">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="ef10c-1601">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1601">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="ef10c-1602">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1602">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-1603">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-1603">ACS</span></span>

* <span data-ttu-id="ef10c-1604">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1604">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-1605">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ef10c-1605">Appservice</span></span>

* <span data-ttu-id="ef10c-1606">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1606">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="ef10c-1607">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1607">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="ef10c-1608">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1608">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="ef10c-1609">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1609">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="ef10c-1610">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1610">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="ef10c-1611">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1611">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="ef10c-1612">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1612">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="ef10c-1613">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1613">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="ef10c-1614">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1614">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="ef10c-1615">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1615">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="ef10c-1616">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ef10c-1616">Batch</span></span>

* <span data-ttu-id="ef10c-1617">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1617">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="ef10c-1618">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1618">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="ef10c-1619">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1619">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="ef10c-1620">CDN</span><span class="sxs-lookup"><span data-stu-id="ef10c-1620">CDN</span></span>

* <span data-ttu-id="ef10c-1621">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1621">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="ef10c-1622">Облако</span><span class="sxs-lookup"><span data-stu-id="ef10c-1622">Cloud</span></span>

* <span data-ttu-id="ef10c-1623">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1623">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="ef10c-1624">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1624">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="ef10c-1625">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1625">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="ef10c-1626">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1626">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="ef10c-1627">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1627">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ef10c-1628">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ef10c-1628">CosmosDB</span></span>

* <span data-ttu-id="ef10c-1629">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1629">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="ef10c-1630">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1630">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ef10c-1631">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ef10c-1631">Data Lake Analytics</span></span>

* <span data-ttu-id="ef10c-1632">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1632">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="ef10c-1633">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1633">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="ef10c-1634">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1634">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ef10c-1635">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ef10c-1635">Data Lake Store</span></span>

* <span data-ttu-id="ef10c-1636">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1636">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="ef10c-1637">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1637">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="ef10c-1638">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1638">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="ef10c-1639">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1639">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="ef10c-1640">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="ef10c-1640">Interactive</span></span>

* <span data-ttu-id="ef10c-1641">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1641">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="ef10c-1642">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1642">Increased test coverage</span></span>
* <span data-ttu-id="ef10c-1643">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1643">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="ef10c-1644">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1644">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="ef10c-1645">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1645">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="ef10c-1646">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1646">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="ef10c-1647">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1647">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="ef10c-1648">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1648">Added `--progress` flag</span></span>
* <span data-ttu-id="ef10c-1649">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1649">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="ef10c-1650">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1650">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="ef10c-1651">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ef10c-1651">IoT</span></span>

* <span data-ttu-id="ef10c-1652">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="ef10c-1652">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="ef10c-1653">(3934).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1653">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="ef10c-1654">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ef10c-1654">Key vault</span></span>

* <span data-ttu-id="ef10c-1655">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="ef10c-1655">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="ef10c-1656">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1656">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="ef10c-1657">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="ef10c-1657">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="ef10c-1658">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="ef10c-1658">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="ef10c-1659">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1659">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="ef10c-1660">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1660">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="ef10c-1661">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="ef10c-1661">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="ef10c-1662">(3307).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1662">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="ef10c-1663">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="ef10c-1663">Lab</span></span>

* <span data-ttu-id="ef10c-1664">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1664">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="ef10c-1665">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1665">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="ef10c-1666">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ef10c-1666">Monitor</span></span>

* <span data-ttu-id="ef10c-1667">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1667">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="ef10c-1668">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1668">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="ef10c-1669">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1669">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="ef10c-1670">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1670">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="ef10c-1671">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1671">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="ef10c-1672">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="ef10c-1672">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="ef10c-1673">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="ef10c-1673">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="ef10c-1674">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="ef10c-1674">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="ef10c-1675">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="ef10c-1675">`location` no longer required</span></span>
  * <span data-ttu-id="ef10c-1676">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="ef10c-1676">Add name and ID support for target</span></span>
  * <span data-ttu-id="ef10c-1677">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="ef10c-1677">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="ef10c-1678">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="ef10c-1678">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="ef10c-1679">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="ef10c-1679">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="ef10c-1680">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1680">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="ef10c-1681">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1681">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="ef10c-1682">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1682">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-1683">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-1683">Network</span></span>

* <span data-ttu-id="ef10c-1684">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1684">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="ef10c-1685">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1685">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="ef10c-1686">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1686">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="ef10c-1687">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1687">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="ef10c-1688">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1688">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="ef10c-1689">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1689">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="ef10c-1690">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1690">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="ef10c-1691">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1691">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="ef10c-1692">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1692">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="ef10c-1693">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1693">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="ef10c-1694">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1694">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="ef10c-1695">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1695">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="ef10c-1696">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1696">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="ef10c-1697">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1697">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="ef10c-1698">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1698">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="ef10c-1699">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1699">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="ef10c-1700">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1700">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="ef10c-1701">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1701">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="ef10c-1702">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1702">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="ef10c-1703">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1703">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="ef10c-1704">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1704">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="ef10c-1705">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1705">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="ef10c-1706">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1706">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="ef10c-1707">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1707">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="ef10c-1708">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1708">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="ef10c-1709">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1709">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="ef10c-1710">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1710">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="ef10c-1711">Профиль</span><span class="sxs-lookup"><span data-stu-id="ef10c-1711">Profile</span></span>

* <span data-ttu-id="ef10c-1712">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1712">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="ef10c-1713">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1713">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="ef10c-1714">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1714">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="ef10c-1715">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1715">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="ef10c-1716">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1716">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="ef10c-1717">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ef10c-1717">RDBMS</span></span>

* <span data-ttu-id="ef10c-1718">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1718">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="ef10c-1719">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1719">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="ef10c-1720">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1720">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="ef10c-1721">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1721">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="ef10c-1722">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ef10c-1722">Resource</span></span>

* <span data-ttu-id="ef10c-1723">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1723">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="ef10c-1724">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1724">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="ef10c-1725">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1725">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="ef10c-1726">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1726">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="ef10c-1727">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1727">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="ef10c-1728">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1728">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="ef10c-1729">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1729">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="ef10c-1730">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1730">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="ef10c-1731">Роль</span><span class="sxs-lookup"><span data-stu-id="ef10c-1731">Role</span></span>

* <span data-ttu-id="ef10c-1732">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1732">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="ef10c-1733">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1733">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="ef10c-1734">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1734">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="ef10c-1735">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1735">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="ef10c-1736">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1736">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ef10c-1737">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ef10c-1737">Service Fabric</span></span>
* <span data-ttu-id="ef10c-1738">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1738">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="ef10c-1739">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1739">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="ef10c-1740">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1740">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="ef10c-1741">SQL</span><span class="sxs-lookup"><span data-stu-id="ef10c-1741">SQL</span></span>

* <span data-ttu-id="ef10c-1742">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1742">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="ef10c-1743">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1743">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="ef10c-1744">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1744">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-1745">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-1745">Storage</span></span>

* <span data-ttu-id="ef10c-1746">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1746">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="ef10c-1747">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1747">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="ef10c-1748">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1748">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="ef10c-1749">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="ef10c-1749">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="ef10c-1750">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1750">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="ef10c-1751">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1751">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-1752">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-1752">VM</span></span>

* <span data-ttu-id="ef10c-1753">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1753">Support configuring nsg</span></span>
* <span data-ttu-id="ef10c-1754">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1754">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="ef10c-1755">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1755">Support managed service identities</span></span>
* <span data-ttu-id="ef10c-1756">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1756">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="ef10c-1757">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1757">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="ef10c-1758">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1758">May 10, 2017</span></span>

<span data-ttu-id="ef10c-1759">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="ef10c-1759">Version 2.0.6</span></span>

* <span data-ttu-id="ef10c-1760">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1760">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="ef10c-1761">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1761">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="ef10c-1762">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1762">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="ef10c-1763">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1763">Include Cognitive Services module</span></span>
* <span data-ttu-id="ef10c-1764">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1764">Include Service Fabric module</span></span>
* <span data-ttu-id="ef10c-1765">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1765">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="ef10c-1766">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1766">Add support for CDN commands</span></span>
* <span data-ttu-id="ef10c-1767">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1767">Remove Container module</span></span>
* <span data-ttu-id="ef10c-1768">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1768">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="ef10c-1769">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1769">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="ef10c-1770">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-1770">Core</span></span>

* <span data-ttu-id="ef10c-1771">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1771">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="ef10c-1772">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1772">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="ef10c-1773">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1773">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="ef10c-1774">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1774">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="ef10c-1775">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1775">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="ef10c-1776">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1776">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="ef10c-1777">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1777">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="ef10c-1778">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1778">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="ef10c-1779">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1779">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="ef10c-1780">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1780">core: Improved performance</span></span>
* <span data-ttu-id="ef10c-1781">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1781">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="ef10c-1782">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1782">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-1783">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-1783">ACS</span></span>

* <span data-ttu-id="ef10c-1784">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1784">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="ef10c-1785">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1785">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="ef10c-1786">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1786">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="ef10c-1787">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1787">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-1788">AppService</span><span class="sxs-lookup"><span data-stu-id="ef10c-1788">AppService</span></span>

* <span data-ttu-id="ef10c-1789">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1789">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="ef10c-1790">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1790">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="ef10c-1791">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1791">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="ef10c-1792">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1792">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="ef10c-1793">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1793">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="ef10c-1794">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1794">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="ef10c-1795">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1795">support slot swap with preview</span></span>
* <span data-ttu-id="ef10c-1796">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1796">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="ef10c-1797">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1797">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ef10c-1798">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ef10c-1798">CosmosDB</span></span>

* <span data-ttu-id="ef10c-1799">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1799">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="ef10c-1800">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1800">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="ef10c-1801">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1801">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="ef10c-1802">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1802">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ef10c-1803">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ef10c-1803">Data Lake Analytics</span></span>

* <span data-ttu-id="ef10c-1804">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1804">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="ef10c-1805">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1805">Add support for new catalog item type: package.</span></span> <span data-ttu-id="ef10c-1806">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1806">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="ef10c-1807">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="ef10c-1807">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="ef10c-1808">Таблица</span><span class="sxs-lookup"><span data-stu-id="ef10c-1808">Table</span></span>
  * <span data-ttu-id="ef10c-1809">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="ef10c-1809">Table valued function</span></span>
  * <span data-ttu-id="ef10c-1810">Просмотр</span><span class="sxs-lookup"><span data-stu-id="ef10c-1810">View</span></span>
  * <span data-ttu-id="ef10c-1811">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1811">Table Statistics.</span></span> <span data-ttu-id="ef10c-1812">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1812">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ef10c-1813">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ef10c-1813">Data Lake Store</span></span>

* <span data-ttu-id="ef10c-1814">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1814">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="ef10c-1815">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1815">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="ef10c-1816">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1816">missed help for access show.</span></span> <span data-ttu-id="ef10c-1817">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1817">adding it.</span></span> <span data-ttu-id="ef10c-1818">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="ef10c-1818">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="ef10c-1819">Поиск</span><span class="sxs-lookup"><span data-stu-id="ef10c-1819">Find</span></span>

* <span data-ttu-id="ef10c-1820">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1820">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="ef10c-1821">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ef10c-1821">KeyVault</span></span>

* <span data-ttu-id="ef10c-1822">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1822">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="ef10c-1823">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1823">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="ef10c-1824">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1824">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="ef10c-1825">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1825">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="ef10c-1826">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1826">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="ef10c-1827">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="ef10c-1827">Lab</span></span>

* <span data-ttu-id="ef10c-1828">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1828">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="ef10c-1829">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1829">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="ef10c-1830">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1830">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="ef10c-1831">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1831">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="ef10c-1832">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1832">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="ef10c-1833">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ef10c-1833">Monitor</span></span>

* <span data-ttu-id="ef10c-1834">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1834">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="ef10c-1835">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1835">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="ef10c-1836">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-1836">Network</span></span>

* <span data-ttu-id="ef10c-1837">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1837">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="ef10c-1838">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1838">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="ef10c-1839">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1839">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="ef10c-1840">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1840">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="ef10c-1841">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1841">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="ef10c-1842">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1842">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="ef10c-1843">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1843">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="ef10c-1844">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1844">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="ef10c-1845">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1845">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="ef10c-1846">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="ef10c-1846">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="ef10c-1847">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1847">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="ef10c-1848">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1848">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="ef10c-1849">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1849">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="ef10c-1850">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1850">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="ef10c-1851">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1851">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="ef10c-1852">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1852">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="ef10c-1853">Профиль</span><span class="sxs-lookup"><span data-stu-id="ef10c-1853">Profile</span></span>

* <span data-ttu-id="ef10c-1854">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1854">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="ef10c-1855">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1855">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="ef10c-1856">Redis</span><span class="sxs-lookup"><span data-stu-id="ef10c-1856">Redis</span></span>

* <span data-ttu-id="ef10c-1857">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1857">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="ef10c-1858">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1858">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="ef10c-1859">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ef10c-1859">Resource</span></span>

* <span data-ttu-id="ef10c-1860">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1860">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="ef10c-1861">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1861">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="ef10c-1862">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1862">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="ef10c-1863">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1863">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="ef10c-1864">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="ef10c-1864">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="ef10c-1865">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1865">Add docs for az lock update.</span></span> <span data-ttu-id="ef10c-1866">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="ef10c-1866">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="ef10c-1867">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1867">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="ef10c-1868">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="ef10c-1868">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="ef10c-1869">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1869">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="ef10c-1870">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="ef10c-1870">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="ef10c-1871">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1871">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="ef10c-1872">Роль</span><span class="sxs-lookup"><span data-stu-id="ef10c-1872">Role</span></span>

* <span data-ttu-id="ef10c-1873">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1873">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="ef10c-1874">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1874">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="ef10c-1875">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1875">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="ef10c-1876">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1876">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="ef10c-1877">SQL</span><span class="sxs-lookup"><span data-stu-id="ef10c-1877">SQL</span></span>

* <span data-ttu-id="ef10c-1878">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1878">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="ef10c-1879">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1879">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="ef10c-1880">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-1880">Storage</span></span>

* <span data-ttu-id="ef10c-1881">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1881">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="ef10c-1882">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1882">Add support for incremental blob copy</span></span>
* <span data-ttu-id="ef10c-1883">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1883">Add support for large block blob upload</span></span>
* <span data-ttu-id="ef10c-1884">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1884">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-1885">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-1885">VM</span></span>

* <span data-ttu-id="ef10c-1886">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1886">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="ef10c-1887">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="ef10c-1887">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="ef10c-1888">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="ef10c-1888">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="ef10c-1889">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="ef10c-1889">az vm/vmss disk</span></span>
  3. <span data-ttu-id="ef10c-1890">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1890">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="ef10c-1891">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1891">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="ef10c-1892">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1892">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="ef10c-1893">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1893">April 3, 2017</span></span>

<span data-ttu-id="ef10c-1894">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="ef10c-1894">Version 2.0.2</span></span>

<span data-ttu-id="ef10c-1895">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1895">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="ef10c-1896">Core</span><span class="sxs-lookup"><span data-stu-id="ef10c-1896">Core</span></span>

* <span data-ttu-id="ef10c-1897">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1897">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="ef10c-1898">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1898">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="ef10c-1899">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1899">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="ef10c-1900">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1900">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ef10c-1901">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1901">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="ef10c-1902">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="ef10c-1902">Add prompting for missing template parameters.</span></span> <span data-ttu-id="ef10c-1903">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1903">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="ef10c-1904">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1904">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="ef10c-1905">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1905">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="ef10c-1906">ACS</span><span class="sxs-lookup"><span data-stu-id="ef10c-1906">ACS</span></span>

* <span data-ttu-id="ef10c-1907">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1907">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="ef10c-1908">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="ef10c-1908">Add support for ssh key password prompting.</span></span> <span data-ttu-id="ef10c-1909">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1909">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="ef10c-1910">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="ef10c-1910">Add support for windows clusters.</span></span> <span data-ttu-id="ef10c-1911">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1911">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="ef10c-1912">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="ef10c-1912">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="ef10c-1913">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1913">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="ef10c-1914">AppService</span><span class="sxs-lookup"><span data-stu-id="ef10c-1914">AppService</span></span>

* <span data-ttu-id="ef10c-1915">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1915">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="ef10c-1916">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1916">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="ef10c-1917">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1917">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="ef10c-1918">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1918">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="ef10c-1919">Data Lake</span><span class="sxs-lookup"><span data-stu-id="ef10c-1919">DataLake</span></span>

* <span data-ttu-id="ef10c-1920">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1920">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="ef10c-1921">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1921">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="ef10c-1922">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="ef10c-1922">DocuemntDB</span></span>

* <span data-ttu-id="ef10c-1923">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1923">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="ef10c-1924">ВМ</span><span class="sxs-lookup"><span data-stu-id="ef10c-1924">VM</span></span>

* <span data-ttu-id="ef10c-1925">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1925">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="ef10c-1926">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1926">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="ef10c-1927">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1927">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="ef10c-1928">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1928">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ef10c-1929">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1929">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="ef10c-1930">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1930">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="ef10c-1931">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1931">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="ef10c-1932">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1932">February 27, 2017</span></span>

<span data-ttu-id="ef10c-1933">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="ef10c-1933">Version 2.0.0</span></span>

<span data-ttu-id="ef10c-1934">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="ef10c-1934">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="ef10c-1935">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="ef10c-1935">Container Service (acs)</span></span>
- <span data-ttu-id="ef10c-1936">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="ef10c-1936">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="ef10c-1937">Сеть</span><span class="sxs-lookup"><span data-stu-id="ef10c-1937">Networking</span></span>
- <span data-ttu-id="ef10c-1938">Хранилище</span><span class="sxs-lookup"><span data-stu-id="ef10c-1938">Storage</span></span>

<span data-ttu-id="ef10c-1939">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1939">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="ef10c-1940">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1940">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="ef10c-1941">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1941">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="ef10c-1942">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1942">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="ef10c-1943">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="ef10c-1943">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="ef10c-1944">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="ef10c-1944">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="ef10c-1945">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="ef10c-1945">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="ef10c-1946">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="ef10c-1946">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="ef10c-1947">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="ef10c-1947">Provide feedback from the command line with the `az feedback` command</span></span>

