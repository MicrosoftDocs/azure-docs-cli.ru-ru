---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/06/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 51b8b8cad6d25f916006b8e68b8f300587f5d45b
ms.sourcegitcommit: 0d6b08048b5b35bf0bb3d7b91ff567adbaab2a8b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/07/2018
ms.locfileid: "51222571"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="9767d-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="9767d-103">Azure CLI release notes</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="9767d-104">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-104">November 6, 2018</span></span>

<span data-ttu-id="9767d-105">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="9767d-105">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="9767d-106">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-106">Core</span></span>
* <span data-ttu-id="9767d-107">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="9767d-107">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="9767d-108">ACR</span><span class="sxs-lookup"><span data-stu-id="9767d-108">ACR</span></span>
* <span data-ttu-id="9767d-109">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="9767d-109">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="9767d-110">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="9767d-110">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-111">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-111">ACS</span></span>
* <span data-ttu-id="9767d-112">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9767d-112">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="9767d-113">Помощник</span><span class="sxs-lookup"><span data-stu-id="9767d-113">Advisor</span></span>
* <span data-ttu-id="9767d-114">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="9767d-114">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="9767d-115">AMS</span><span class="sxs-lookup"><span data-stu-id="9767d-115">AMS</span></span>
* <span data-ttu-id="9767d-116">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="9767d-116">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="9767d-117">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="9767d-117">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="9767d-118">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-118">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="9767d-119">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="9767d-119">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="9767d-120">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="9767d-120">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="9767d-121">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="9767d-121">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="9767d-122">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="9767d-122">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="9767d-123">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="9767d-123">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="9767d-124">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="9767d-124">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="9767d-125">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="9767d-125">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="9767d-126">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="9767d-126">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="9767d-127">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="9767d-127">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="9767d-128">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="9767d-128">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="9767d-129">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="9767d-129">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="9767d-130">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="9767d-130">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="9767d-131">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="9767d-131">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="9767d-132">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="9767d-132">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-133">AppService</span><span class="sxs-lookup"><span data-stu-id="9767d-133">AppService</span></span>
* <span data-ttu-id="9767d-134">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="9767d-134">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="9767d-135">Настройка</span><span class="sxs-lookup"><span data-stu-id="9767d-135">Configure</span></span>
* <span data-ttu-id="9767d-136">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="9767d-136">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="9767d-137">Контейнер</span><span class="sxs-lookup"><span data-stu-id="9767d-137">Container</span></span>
* <span data-ttu-id="9767d-138">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="9767d-138">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="9767d-139">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="9767d-139">EventHub</span></span>
* <span data-ttu-id="9767d-140">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-140">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="9767d-141">Interactive</span><span class="sxs-lookup"><span data-stu-id="9767d-141">Interactive</span></span>
* <span data-ttu-id="9767d-142">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="9767d-142">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="9767d-143">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="9767d-143">Monitor</span></span>
* <span data-ttu-id="9767d-144">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-144">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="9767d-145">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-145">Network</span></span>
* <span data-ttu-id="9767d-146">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="9767d-146">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="9767d-147">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="9767d-147">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="9767d-148">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-148">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="9767d-149">Профиль</span><span class="sxs-lookup"><span data-stu-id="9767d-149">Profile</span></span>
* <span data-ttu-id="9767d-150">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="9767d-150">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="9767d-151">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="9767d-151">RDBMS</span></span>
* <span data-ttu-id="9767d-152">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="9767d-152">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="9767d-153">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9767d-153">Resource</span></span>
* <span data-ttu-id="9767d-154">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="9767d-154">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="9767d-155">Роль</span><span class="sxs-lookup"><span data-stu-id="9767d-155">Role</span></span>
* <span data-ttu-id="9767d-156">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="9767d-156">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="9767d-157">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="9767d-157">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="9767d-158">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="9767d-158">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-159">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-159">Storage</span></span>
* <span data-ttu-id="9767d-160">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="9767d-160">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-161">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-161">VM</span></span>
* <span data-ttu-id="9767d-162">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="9767d-162">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="9767d-163">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="9767d-163">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="9767d-164">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="9767d-164">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="9767d-165">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="9767d-165">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="9767d-166">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="9767d-166">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="9767d-167">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="9767d-167">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="9767d-168">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-168">October 23, 2018</span></span>

<span data-ttu-id="9767d-169">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="9767d-169">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="9767d-170">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-170">Core</span></span>
* <span data-ttu-id="9767d-171">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="9767d-171">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="9767d-172">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="9767d-172">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="9767d-173">ACR</span><span class="sxs-lookup"><span data-stu-id="9767d-173">ACR</span></span>
* <span data-ttu-id="9767d-174">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="9767d-174">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="9767d-175">CDN</span><span class="sxs-lookup"><span data-stu-id="9767d-175">CDN</span></span>
* <span data-ttu-id="9767d-176">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9767d-176">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="9767d-177">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="9767d-177">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="9767d-178">Контейнер</span><span class="sxs-lookup"><span data-stu-id="9767d-178">Container</span></span>
* <span data-ttu-id="9767d-179">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="9767d-179">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="9767d-180">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="9767d-180">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="9767d-181">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="9767d-181">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="9767d-182">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="9767d-182">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="9767d-183">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="9767d-183">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="9767d-184">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="9767d-184">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="9767d-185">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="9767d-185">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9767d-186">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9767d-186">CosmosDB</span></span>
* <span data-ttu-id="9767d-187">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="9767d-187">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="9767d-188">Interactive</span><span class="sxs-lookup"><span data-stu-id="9767d-188">Interactive</span></span>
* <span data-ttu-id="9767d-189">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="9767d-189">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="9767d-190">IoT Central</span><span class="sxs-lookup"><span data-stu-id="9767d-190">IoT Central</span></span>
* <span data-ttu-id="9767d-191">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="9767d-191">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="9767d-192">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="9767d-192">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="9767d-193">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="9767d-193">Monitor</span></span>
* <span data-ttu-id="9767d-194">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="9767d-194">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="9767d-195">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="9767d-195">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="9767d-196">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="9767d-196">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="9767d-197">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="9767d-197">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="9767d-198">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="9767d-198">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="9767d-199">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="9767d-199">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="9767d-200">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="9767d-200">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="9767d-201">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="9767d-201">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="9767d-202">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="9767d-202">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="9767d-203">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-203">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="9767d-204">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-204">Network</span></span>
* <span data-ttu-id="9767d-205">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="9767d-205">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="9767d-206">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="9767d-206">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="9767d-207">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="9767d-207">ServiceBus</span></span>
* <span data-ttu-id="9767d-208">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="9767d-208">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="9767d-209">SQL</span><span class="sxs-lookup"><span data-stu-id="9767d-209">SQL</span></span>
* <span data-ttu-id="9767d-210">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="9767d-210">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-211">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-211">Storage</span></span>
* <span data-ttu-id="9767d-212">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="9767d-212">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="9767d-213">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="9767d-213">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-214">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-214">VM</span></span>
* <span data-ttu-id="9767d-215">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="9767d-215">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="9767d-216">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="9767d-216">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="9767d-217">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="9767d-217">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="9767d-218">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-218">October 16, 2018</span></span>

<span data-ttu-id="9767d-219">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="9767d-219">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-220">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-220">VM</span></span>
* <span data-ttu-id="9767d-221">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="9767d-221">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="9767d-222">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-222">October 9, 2018</span></span>

<span data-ttu-id="9767d-223">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="9767d-223">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="9767d-224">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-224">Core</span></span>
* <span data-ttu-id="9767d-225">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="9767d-225">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="9767d-226">ACR</span><span class="sxs-lookup"><span data-stu-id="9767d-226">ACR</span></span>
* <span data-ttu-id="9767d-227">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="9767d-227">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-228">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-228">ACS</span></span>
* <span data-ttu-id="9767d-229">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="9767d-229">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="9767d-230">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="9767d-230">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="9767d-231">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="9767d-231">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="9767d-232">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="9767d-232">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="9767d-233">Контейнер</span><span class="sxs-lookup"><span data-stu-id="9767d-233">Container</span></span>
* <span data-ttu-id="9767d-234">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="9767d-234">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="9767d-235">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="9767d-235">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="9767d-236">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="9767d-236">Event Hub</span></span>
* <span data-ttu-id="9767d-237">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-237">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="9767d-238">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="9767d-238">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="9767d-239">расширения.</span><span class="sxs-lookup"><span data-stu-id="9767d-239">Extensions</span></span>
* <span data-ttu-id="9767d-240">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="9767d-240">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9767d-241">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9767d-241">HDInsight</span></span>
* <span data-ttu-id="9767d-242">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="9767d-242">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="9767d-243">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="9767d-243">IoT</span></span>
* <span data-ttu-id="9767d-244">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="9767d-244">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="9767d-245">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="9767d-245">KeyVault</span></span>
* <span data-ttu-id="9767d-246">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="9767d-246">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="9767d-247">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-247">Network</span></span>
* <span data-ttu-id="9767d-248">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9767d-248">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="9767d-249">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="9767d-249">See #6052</span></span>
* <span data-ttu-id="9767d-250">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-250">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="9767d-251">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="9767d-251">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="9767d-252">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="9767d-252">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="9767d-253">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="9767d-253">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="9767d-254">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="9767d-254">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="9767d-255">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-255">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="9767d-256">Роль</span><span class="sxs-lookup"><span data-stu-id="9767d-256">Role</span></span>
* <span data-ttu-id="9767d-257">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="9767d-257">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="9767d-258">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="9767d-258">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="9767d-259">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="9767d-259">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="9767d-260">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="9767d-260">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="9767d-261">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="9767d-261">Service Bus</span></span>
* <span data-ttu-id="9767d-262">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="9767d-262">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-263">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-263">VM</span></span>
* <span data-ttu-id="9767d-264">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="9767d-264">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="9767d-265">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="9767d-265">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="9767d-266">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="9767d-266">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="9767d-267">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="9767d-267">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="9767d-268">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="9767d-268">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="9767d-269">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="9767d-269">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="9767d-270">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-270">September 21, 2018</span></span>

<span data-ttu-id="9767d-271">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="9767d-271">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="9767d-272">ACR</span><span class="sxs-lookup"><span data-stu-id="9767d-272">ACR</span></span>
* <span data-ttu-id="9767d-273">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="9767d-273">Added ACR Task commands</span></span>
* <span data-ttu-id="9767d-274">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="9767d-274">Added quick run command</span></span>
* <span data-ttu-id="9767d-275">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="9767d-275">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="9767d-276">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="9767d-276">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="9767d-277">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="9767d-277">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="9767d-278">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="9767d-278">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-279">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-279">ACS</span></span>
* <span data-ttu-id="9767d-280">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="9767d-280">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="9767d-281">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="9767d-281">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-282">AppService</span><span class="sxs-lookup"><span data-stu-id="9767d-282">AppService</span></span>

* <span data-ttu-id="9767d-283">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="9767d-283">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="9767d-284">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="9767d-284">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="9767d-285">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="9767d-285">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="9767d-286">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="9767d-286">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="9767d-287">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="9767d-287">Batch</span></span>
* <span data-ttu-id="9767d-288">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="9767d-288">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="9767d-289">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="9767d-289">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="9767d-290">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-290">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="9767d-291">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="9767d-291">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9767d-292">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="9767d-292">Batch AI</span></span> 
* <span data-ttu-id="9767d-293">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-293">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9767d-294">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9767d-294">Cognitive Services</span></span>
* <span data-ttu-id="9767d-295">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="9767d-295">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="9767d-296">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="9767d-296">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="9767d-297">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="9767d-297">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="9767d-298">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="9767d-298">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="9767d-299">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="9767d-299">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="9767d-300">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="9767d-300">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="9767d-301">Контейнер</span><span class="sxs-lookup"><span data-stu-id="9767d-301">Container</span></span>
* <span data-ttu-id="9767d-302">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="9767d-302">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="9767d-303">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="9767d-303">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="9767d-304">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="9767d-304">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="9767d-305">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="9767d-305">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="9767d-306">Data Lake</span><span class="sxs-lookup"><span data-stu-id="9767d-306">Datalake</span></span>
* <span data-ttu-id="9767d-307">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="9767d-307">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="9767d-308">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="9767d-308">Interactive Shell</span></span>
* <span data-ttu-id="9767d-309">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="9767d-309">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="9767d-310">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="9767d-310">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="9767d-311">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="9767d-311">IoT</span></span>
* <span data-ttu-id="9767d-312">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="9767d-312">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="9767d-313">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9767d-313">Key Vault</span></span>
* <span data-ttu-id="9767d-314">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="9767d-314">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="9767d-315">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-315">Network</span></span>
* <span data-ttu-id="9767d-316">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="9767d-316">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="9767d-317">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="9767d-317">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="9767d-318">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="9767d-318">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="9767d-319">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="9767d-319">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="9767d-320">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-320">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="9767d-321">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-321">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="9767d-322">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="9767d-322">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="9767d-323">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="9767d-323">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="9767d-324">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="9767d-324">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="9767d-325">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="9767d-325">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="9767d-326">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="9767d-326">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="9767d-327">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="9767d-327">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="9767d-328">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры`--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="9767d-328">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="9767d-329">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="9767d-329">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="9767d-330">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="9767d-330">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="9767d-331">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="9767d-331">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="9767d-332">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="9767d-332">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="9767d-333">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="9767d-333">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="9767d-334">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="9767d-334">RDBMS</span></span>
* <span data-ttu-id="9767d-335">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="9767d-335">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="9767d-336">резервирование.</span><span class="sxs-lookup"><span data-stu-id="9767d-336">Reservation</span></span>
* <span data-ttu-id="9767d-337">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="9767d-337">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="9767d-338">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="9767d-338">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="9767d-339">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="9767d-339">Manage App</span></span>
* <span data-ttu-id="9767d-340">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="9767d-340">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="9767d-341">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="9767d-341">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="9767d-342">Роль</span><span class="sxs-lookup"><span data-stu-id="9767d-342">Role</span></span>
* <span data-ttu-id="9767d-343">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="9767d-343">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="9767d-344">SignalR</span><span class="sxs-lookup"><span data-stu-id="9767d-344">SignalR</span></span>
* <span data-ttu-id="9767d-345">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="9767d-345">First release</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-346">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-346">Storage</span></span>
* <span data-ttu-id="9767d-347">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="9767d-347">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="9767d-348">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="9767d-348">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-349">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-349">VM</span></span>
* <span data-ttu-id="9767d-350">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="9767d-350">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="9767d-351">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="9767d-351">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="9767d-352">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-352">August 28, 2018</span></span>

<span data-ttu-id="9767d-353">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="9767d-353">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="9767d-354">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-354">Core</span></span>

* <span data-ttu-id="9767d-355">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="9767d-355">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="9767d-356">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="9767d-356">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="9767d-357">ACR</span><span class="sxs-lookup"><span data-stu-id="9767d-357">ACR</span></span>

* <span data-ttu-id="9767d-358">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="9767d-358">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="9767d-359">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="9767d-359">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-360">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-360">ACS</span></span>

* <span data-ttu-id="9767d-361">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="9767d-361">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="9767d-362">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="9767d-362">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-363">AppService</span><span class="sxs-lookup"><span data-stu-id="9767d-363">AppService</span></span>

* <span data-ttu-id="9767d-364">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="9767d-364">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="9767d-365">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="9767d-365">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="9767d-366">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="9767d-366">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="9767d-367">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="9767d-367">Backup</span></span>

* <span data-ttu-id="9767d-368">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="9767d-368">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="9767d-369">Служба Bot Service</span><span class="sxs-lookup"><span data-stu-id="9767d-369">Bot Service</span></span>

* <span data-ttu-id="9767d-370">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="9767d-370">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9767d-371">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9767d-371">Cognitive Services</span></span>

* <span data-ttu-id="9767d-372">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="9767d-372">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="9767d-373">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="9767d-373">IoT</span></span>

* <span data-ttu-id="9767d-374">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="9767d-374">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="9767d-375">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="9767d-375">Monitor</span></span>

* <span data-ttu-id="9767d-376">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="9767d-376">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="9767d-377">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="9767d-377">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="9767d-378">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-378">Network</span></span>

* <span data-ttu-id="9767d-379">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="9767d-379">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="9767d-380">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9767d-380">Resource</span></span>

* <span data-ttu-id="9767d-381">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="9767d-381">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-382">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-382">Storage</span></span>

* <span data-ttu-id="9767d-383">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="9767d-383">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-384">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-384">VM</span></span>

* <span data-ttu-id="9767d-385">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="9767d-385">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="9767d-386">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-386">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="9767d-387">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-387">Auguest 14, 2018</span></span>

<span data-ttu-id="9767d-388">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="9767d-388">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="9767d-389">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-389">Core</span></span>

* <span data-ttu-id="9767d-390">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="9767d-390">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="9767d-391">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="9767d-391">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="9767d-392">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="9767d-392">Telemetry</span></span>

* <span data-ttu-id="9767d-393">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="9767d-393">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="9767d-394">ACR</span><span class="sxs-lookup"><span data-stu-id="9767d-394">ACR</span></span>

* <span data-ttu-id="9767d-395">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="9767d-395">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="9767d-396">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="9767d-396">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-397">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-397">ACS</span></span>

* <span data-ttu-id="9767d-398">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="9767d-398">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="9767d-399">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="9767d-399">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="9767d-400">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="9767d-400">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="9767d-401">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="9767d-401">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="9767d-402">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="9767d-402">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="9767d-403">AppService</span><span class="sxs-lookup"><span data-stu-id="9767d-403">AppService</span></span>

* <span data-ttu-id="9767d-404">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="9767d-404">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="9767d-405">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="9767d-405">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="9767d-406">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9767d-406">BatchAI</span></span>

* <span data-ttu-id="9767d-407">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="9767d-407">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="9767d-408">Контейнер</span><span class="sxs-lookup"><span data-stu-id="9767d-408">Container</span></span>

* <span data-ttu-id="9767d-409">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="9767d-409">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="9767d-410">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="9767d-410">IoT</span></span>

* <span data-ttu-id="9767d-411">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="9767d-411">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="9767d-412">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="9767d-412">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="9767d-413">IoT Central</span><span class="sxs-lookup"><span data-stu-id="9767d-413">Iot Central</span></span>

* <span data-ttu-id="9767d-414">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="9767d-414">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="9767d-415">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="9767d-415">KeyVault</span></span>


* <span data-ttu-id="9767d-416">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="9767d-416">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="9767d-417">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="9767d-417">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="9767d-418">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="9767d-418">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="9767d-419">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="9767d-419">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="9767d-420">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="9767d-420">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="9767d-421">Передача</span><span class="sxs-lookup"><span data-stu-id="9767d-421">Relay</span></span>

* <span data-ttu-id="9767d-422">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="9767d-422">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="9767d-423">SQL</span><span class="sxs-lookup"><span data-stu-id="9767d-423">Sql</span></span>

* <span data-ttu-id="9767d-424">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="9767d-424">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-425">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-425">Storage</span></span>

* <span data-ttu-id="9767d-426">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="9767d-426">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="9767d-427">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="9767d-427">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="9767d-428">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="9767d-428">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="9767d-429">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="9767d-429">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="9767d-430">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="9767d-430">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-431">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-431">VM</span></span>

* <span data-ttu-id="9767d-432">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="9767d-432">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="9767d-433">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-433">July 31, 2018</span></span>

<span data-ttu-id="9767d-434">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="9767d-434">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="9767d-435">ACR</span><span class="sxs-lookup"><span data-stu-id="9767d-435">ACR</span></span>

* <span data-ttu-id="9767d-436">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="9767d-436">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="9767d-437">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="9767d-437">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-438">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-438">ACS</span></span>

* <span data-ttu-id="9767d-439">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="9767d-439">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="9767d-440">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="9767d-440">Batch</span></span>

* <span data-ttu-id="9767d-441">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="9767d-441">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="9767d-442">Контейнер</span><span class="sxs-lookup"><span data-stu-id="9767d-442">Container</span></span>

* <span data-ttu-id="9767d-443">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="9767d-443">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="9767d-444">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-444">Network</span></span>

* <span data-ttu-id="9767d-445">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="9767d-445">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="9767d-446">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9767d-446">Resource</span></span>

* <span data-ttu-id="9767d-447">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="9767d-447">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="9767d-448">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="9767d-448">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="9767d-449">Роль</span><span class="sxs-lookup"><span data-stu-id="9767d-449">Role</span></span>

* <span data-ttu-id="9767d-450">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="9767d-450">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="9767d-451">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="9767d-451">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="9767d-452">поиска</span><span class="sxs-lookup"><span data-stu-id="9767d-452">Search</span></span>

* <span data-ttu-id="9767d-453">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="9767d-453">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="9767d-454">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="9767d-454">Service Bus</span></span>

* <span data-ttu-id="9767d-455">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="9767d-455">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="9767d-456">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="9767d-456">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="9767d-457">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="9767d-457">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="9767d-458">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="9767d-458">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-459">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-459">Storage</span></span>

* <span data-ttu-id="9767d-460">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="9767d-460">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="9767d-461">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="9767d-461">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-462">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-462">VM</span></span>

* <span data-ttu-id="9767d-463">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="9767d-463">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="9767d-464">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="9767d-464">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="9767d-465">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="9767d-465">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="9767d-466">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="9767d-466">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="9767d-467">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-467">July 18, 2018</span></span>

<span data-ttu-id="9767d-468">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="9767d-468">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="9767d-469">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-469">Core</span></span>

* <span data-ttu-id="9767d-470">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="9767d-470">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="9767d-471">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="9767d-471">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="9767d-472">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="9767d-472">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="9767d-473">ACR</span><span class="sxs-lookup"><span data-stu-id="9767d-473">ACR</span></span>

* <span data-ttu-id="9767d-474">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="9767d-474">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="9767d-475">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-475">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="9767d-476">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="9767d-476">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="9767d-477">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="9767d-477">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-478">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-478">ACS</span></span>

* <span data-ttu-id="9767d-479">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="9767d-479">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-480">AppService</span><span class="sxs-lookup"><span data-stu-id="9767d-480">AppService</span></span>

* <span data-ttu-id="9767d-481">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="9767d-481">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="9767d-482">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="9767d-482">Batch</span></span>

* <span data-ttu-id="9767d-483">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="9767d-483">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="9767d-484">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="9767d-484">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9767d-485">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="9767d-485">Batch AI</span></span>

* <span data-ttu-id="9767d-486">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="9767d-486">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="9767d-487">Контейнер</span><span class="sxs-lookup"><span data-stu-id="9767d-487">Container</span></span>

* <span data-ttu-id="9767d-488">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="9767d-488">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="9767d-489">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="9767d-489">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="9767d-490">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-490">Network</span></span>

* <span data-ttu-id="9767d-491">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="9767d-491">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="9767d-492">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="9767d-492">Added `network nic wait`</span></span>
* <span data-ttu-id="9767d-493">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="9767d-493">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="9767d-494">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="9767d-494">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="9767d-495">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9767d-495">Resource</span></span>

* <span data-ttu-id="9767d-496">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="9767d-496">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="9767d-497">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="9767d-497">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="9767d-498">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="9767d-498">Added `deployment wait` command</span></span>
* <span data-ttu-id="9767d-499">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="9767d-499">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="9767d-500">SQL</span><span class="sxs-lookup"><span data-stu-id="9767d-500">SQL</span></span>

* <span data-ttu-id="9767d-501">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-501">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="9767d-502">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="9767d-502">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="9767d-503">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="9767d-503">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-504">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-504">Storage</span></span>

* <span data-ttu-id="9767d-505">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="9767d-505">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-506">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-506">VM</span></span>

* <span data-ttu-id="9767d-507">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9767d-507">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="9767d-508">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-508">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="9767d-509">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="9767d-509">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="9767d-510">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-510">July 3, 2018</span></span>

<span data-ttu-id="9767d-511">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="9767d-511">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="9767d-512">AKS</span><span class="sxs-lookup"><span data-stu-id="9767d-512">AKS</span></span>

* <span data-ttu-id="9767d-513">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="9767d-513">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="9767d-514">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-514">July 3, 2018</span></span>

<span data-ttu-id="9767d-515">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="9767d-515">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="9767d-516">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-516">Core</span></span>

* <span data-ttu-id="9767d-517">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="9767d-517">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="9767d-518">ACR</span><span class="sxs-lookup"><span data-stu-id="9767d-518">ACR</span></span>

* <span data-ttu-id="9767d-519">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="9767d-519">Added polling build status</span></span>
* <span data-ttu-id="9767d-520">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="9767d-520">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="9767d-521">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="9767d-521">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-522">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-522">ACS</span></span>

* <span data-ttu-id="9767d-523">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9767d-523">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="9767d-524">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9767d-524">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="9767d-525">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="9767d-525">Updated options for `aks browse` command.</span></span> <span data-ttu-id="9767d-526">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="9767d-526">Added `--listen-port` support</span></span>
* <span data-ttu-id="9767d-527">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="9767d-527">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="9767d-528">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="9767d-528">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="9767d-529">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="9767d-529">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-530">AppService</span><span class="sxs-lookup"><span data-stu-id="9767d-530">AppService</span></span>

* <span data-ttu-id="9767d-531">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="9767d-531">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="9767d-532">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="9767d-532">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="9767d-533">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="9767d-533">Backup</span></span>

* <span data-ttu-id="9767d-534">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="9767d-534">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="9767d-535">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9767d-535">BatchAI</span></span>

* <span data-ttu-id="9767d-536">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="9767d-536">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="9767d-537">Облако</span><span class="sxs-lookup"><span data-stu-id="9767d-537">Cloud</span></span>

* <span data-ttu-id="9767d-538">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="9767d-538">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="9767d-539">Контейнер</span><span class="sxs-lookup"><span data-stu-id="9767d-539">Container</span></span>

* <span data-ttu-id="9767d-540">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="9767d-540">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="9767d-541">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="9767d-541">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="9767d-542">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="9767d-542">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="9767d-543">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="9767d-543">Extension</span></span>

* <span data-ttu-id="9767d-544">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="9767d-544">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="9767d-545">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-545">Network</span></span>

* <span data-ttu-id="9767d-546">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="9767d-546">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="9767d-547">Rdbms</span><span class="sxs-lookup"><span data-stu-id="9767d-547">Rdbms</span></span>

* <span data-ttu-id="9767d-548">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="9767d-548">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="9767d-549">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9767d-549">Resource</span></span>

* <span data-ttu-id="9767d-550">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="9767d-550">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-551">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-551">VM</span></span>

* <span data-ttu-id="9767d-552">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="9767d-552">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="9767d-553">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-553">June 25, 2018</span></span>

<span data-ttu-id="9767d-554">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="9767d-554">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="9767d-555">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="9767d-555">CLI</span></span>

* <span data-ttu-id="9767d-556">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="9767d-556">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="9767d-557">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-557">June 19, 2018</span></span>

<span data-ttu-id="9767d-558">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="9767d-558">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="9767d-559">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-559">Core</span></span>

* <span data-ttu-id="9767d-560">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="9767d-560">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="9767d-561">ACR</span><span class="sxs-lookup"><span data-stu-id="9767d-561">ACR</span></span>

* <span data-ttu-id="9767d-562">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="9767d-562">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="9767d-563">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="9767d-563">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-564">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-564">ACS</span></span>

* <span data-ttu-id="9767d-565">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="9767d-565">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="9767d-566">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-566">Added `--update` support</span></span>
* <span data-ttu-id="9767d-567">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="9767d-567">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="9767d-568">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="9767d-568">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="9767d-569">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="9767d-569">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="9767d-570">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="9767d-570">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="9767d-571">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="9767d-571">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="9767d-572">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="9767d-572">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-573">AppService</span><span class="sxs-lookup"><span data-stu-id="9767d-573">AppService</span></span>

* <span data-ttu-id="9767d-574">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="9767d-574">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="9767d-575">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="9767d-575">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="9767d-576">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="9767d-576">Batch</span></span>

* <span data-ttu-id="9767d-577">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="9767d-577">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9767d-578">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="9767d-578">Batch AI</span></span>

* <span data-ttu-id="9767d-579">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="9767d-579">Added support for workspaces.</span></span> <span data-ttu-id="9767d-580">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="9767d-580">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="9767d-581">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="9767d-581">Added support for experiments.</span></span> <span data-ttu-id="9767d-582">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="9767d-582">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="9767d-583">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="9767d-583">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="9767d-584">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="9767d-584">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="9767d-585">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="9767d-585">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="9767d-586">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="9767d-586">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="9767d-587">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="9767d-587">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="9767d-588">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="9767d-588">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="9767d-589">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-589">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="9767d-590">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="9767d-590">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="9767d-591">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-591">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="9767d-592">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="9767d-592">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="9767d-593">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="9767d-593">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="9767d-594">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="9767d-594">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="9767d-595">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-595">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="9767d-596">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="9767d-596">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="9767d-597">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="9767d-597">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="9767d-598">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="9767d-598">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="9767d-599">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="9767d-599">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="9767d-600">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="9767d-600">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="9767d-601">Карты</span><span class="sxs-lookup"><span data-stu-id="9767d-601">Maps</span></span>

* <span data-ttu-id="9767d-602">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="9767d-602">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="9767d-603">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-603">Network</span></span>

* <span data-ttu-id="9767d-604">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="9767d-604">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="9767d-605">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="9767d-605">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="9767d-606">#6502</span><span class="sxs-lookup"><span data-stu-id="9767d-606">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="9767d-607">Резервирование</span><span class="sxs-lookup"><span data-stu-id="9767d-607">Reservations</span></span>

* <span data-ttu-id="9767d-608">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="9767d-608">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="9767d-609">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="9767d-609">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="9767d-610">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="9767d-610">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="9767d-611">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="9767d-611">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="9767d-612">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="9767d-612">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="9767d-613">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-613">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="9767d-614">Роль</span><span class="sxs-lookup"><span data-stu-id="9767d-614">Role</span></span>

* <span data-ttu-id="9767d-615">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="9767d-615">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="9767d-616">SQL</span><span class="sxs-lookup"><span data-stu-id="9767d-616">SQL</span></span>

* <span data-ttu-id="9767d-617">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="9767d-617">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-618">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-618">Storage</span></span>

* <span data-ttu-id="9767d-619">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="9767d-619">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-620">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-620">VM</span></span>

* <span data-ttu-id="9767d-621">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-621">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="9767d-622">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="9767d-622">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="9767d-623">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="9767d-623">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="9767d-624">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-624">June 13, 2018</span></span>

<span data-ttu-id="9767d-625">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="9767d-625">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="9767d-626">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-626">Core</span></span>

* <span data-ttu-id="9767d-627">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="9767d-627">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="9767d-628">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-628">June 13, 2018</span></span>

<span data-ttu-id="9767d-629">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="9767d-629">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="9767d-630">AKS</span><span class="sxs-lookup"><span data-stu-id="9767d-630">AKS</span></span>

* <span data-ttu-id="9767d-631">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="9767d-631">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="9767d-632">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="9767d-632">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="9767d-633">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="9767d-633">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="9767d-634">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="9767d-634">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="9767d-635">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9767d-635">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-636">AppService</span><span class="sxs-lookup"><span data-stu-id="9767d-636">AppService</span></span>

* <span data-ttu-id="9767d-637">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="9767d-637">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="9767d-638">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-638">June 5, 2018</span></span>

<span data-ttu-id="9767d-639">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="9767d-639">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="9767d-640">Interactive</span><span class="sxs-lookup"><span data-stu-id="9767d-640">Interactive</span></span>

* <span data-ttu-id="9767d-641">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="9767d-641">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="9767d-642">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-642">June 5, 2018</span></span>

<span data-ttu-id="9767d-643">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="9767d-643">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="9767d-644">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-644">Core</span></span>

* <span data-ttu-id="9767d-645">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="9767d-645">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="9767d-646">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="9767d-646">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="9767d-647">ACR</span><span class="sxs-lookup"><span data-stu-id="9767d-647">ACR</span></span>

* <span data-ttu-id="9767d-648">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="9767d-648">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="9767d-649">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="9767d-649">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="9767d-650">AKS</span><span class="sxs-lookup"><span data-stu-id="9767d-650">AKS</span></span>

* <span data-ttu-id="9767d-651">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="9767d-651">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="9767d-652">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="9767d-652">Batch</span></span>

* <span data-ttu-id="9767d-653">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="9767d-653">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="9767d-654">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="9767d-654">IOT</span></span>

* <span data-ttu-id="9767d-655">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="9767d-655">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="9767d-656">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-656">Network</span></span>

* <span data-ttu-id="9767d-657">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="9767d-657">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="9767d-658">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="9767d-658">Policy Insights</span></span>

* <span data-ttu-id="9767d-659">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="9767d-659">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="9767d-660">ARM</span><span class="sxs-lookup"><span data-stu-id="9767d-660">ARM</span></span>

* <span data-ttu-id="9767d-661">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="9767d-661">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="9767d-662">SQL</span><span class="sxs-lookup"><span data-stu-id="9767d-662">SQL</span></span>

* <span data-ttu-id="9767d-663">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="9767d-663">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="9767d-664">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="9767d-664">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="9767d-665">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-665">Storage</span></span>

* <span data-ttu-id="9767d-666">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="9767d-666">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-667">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-667">VM</span></span>

* <span data-ttu-id="9767d-668">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="9767d-668">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="9767d-669">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-669">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="9767d-670">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-670">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="9767d-671">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-671">May 22, 2018</span></span>

<span data-ttu-id="9767d-672">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="9767d-672">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="9767d-673">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-673">Core</span></span>

* <span data-ttu-id="9767d-674">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="9767d-674">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-675">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-675">ACS</span></span>

* <span data-ttu-id="9767d-676">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="9767d-676">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="9767d-677">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="9767d-677">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-678">AppService</span><span class="sxs-lookup"><span data-stu-id="9767d-678">AppService</span></span>

* <span data-ttu-id="9767d-679">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="9767d-679">Improved generic update commands</span></span>
* <span data-ttu-id="9767d-680">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="9767d-680">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="9767d-681">Контейнер</span><span class="sxs-lookup"><span data-stu-id="9767d-681">Container</span></span>

* <span data-ttu-id="9767d-682">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="9767d-682">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="9767d-683">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="9767d-683">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="9767d-684">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="9767d-684">Extension</span></span>

* <span data-ttu-id="9767d-685">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="9767d-685">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="9767d-686">Interactive</span><span class="sxs-lookup"><span data-stu-id="9767d-686">Interactive</span></span>

* <span data-ttu-id="9767d-687">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="9767d-687">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="9767d-688">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="9767d-688">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="9767d-689">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="9767d-689">KeyVault</span></span>

* <span data-ttu-id="9767d-690">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="9767d-690">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="9767d-691">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-691">Network</span></span>

* <span data-ttu-id="9767d-692">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="9767d-692">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="9767d-693">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="9767d-693">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="9767d-694">SQL</span><span class="sxs-lookup"><span data-stu-id="9767d-694">SQL</span></span>

* <span data-ttu-id="9767d-695">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="9767d-695">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="9767d-696">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="9767d-696">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="9767d-697">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="9767d-697">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="9767d-698">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="9767d-698">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="9767d-699">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="9767d-699">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="9767d-700">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="9767d-700">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="9767d-701">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="9767d-701">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="9767d-702">`edition`.</span><span class="sxs-lookup"><span data-stu-id="9767d-702">`edition`.</span></span> <span data-ttu-id="9767d-703">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="9767d-703">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="9767d-704">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="9767d-704">`elasticPoolName`.</span></span> <span data-ttu-id="9767d-705">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="9767d-705">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="9767d-706">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="9767d-706">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="9767d-707">`edition`.</span><span class="sxs-lookup"><span data-stu-id="9767d-707">`edition`.</span></span> <span data-ttu-id="9767d-708">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="9767d-708">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="9767d-709">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="9767d-709">`dtu`.</span></span> <span data-ttu-id="9767d-710">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="9767d-710">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="9767d-711">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="9767d-711">`databaseDtuMin`.</span></span> <span data-ttu-id="9767d-712">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="9767d-712">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="9767d-713">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="9767d-713">`databaseDtuMax`.</span></span> <span data-ttu-id="9767d-714">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="9767d-714">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="9767d-715">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="9767d-715">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="9767d-716">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="9767d-716">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-717">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-717">Storage</span></span>

* <span data-ttu-id="9767d-718">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="9767d-718">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="9767d-719">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="9767d-719">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-720">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-720">VM</span></span>

* <span data-ttu-id="9767d-721">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-721">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="9767d-722">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="9767d-722">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="9767d-723">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="9767d-723">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="9767d-724">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="9767d-724">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="9767d-725">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-725">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="9767d-726">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-726">May 7, 2018</span></span>

<span data-ttu-id="9767d-727">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="9767d-727">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="9767d-728">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-728">Core</span></span>

* <span data-ttu-id="9767d-729">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="9767d-729">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="9767d-730">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="9767d-730">Added limited support for positional arguments</span></span>
* <span data-ttu-id="9767d-731">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="9767d-731">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="9767d-732">#5591</span><span class="sxs-lookup"><span data-stu-id="9767d-732">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="9767d-733">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="9767d-733">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="9767d-734">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="9767d-734">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="9767d-735">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="9767d-735">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="9767d-736">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="9767d-736">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="9767d-737">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="9767d-737">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="9767d-738">ACR</span><span class="sxs-lookup"><span data-stu-id="9767d-738">ACR</span></span>

* <span data-ttu-id="9767d-739">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="9767d-739">Added ACR Build commands</span></span>
* <span data-ttu-id="9767d-740">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="9767d-740">Improved resource not found error messages</span></span>
* <span data-ttu-id="9767d-741">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="9767d-741">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="9767d-742">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="9767d-742">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="9767d-743">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="9767d-743">Improved repository commands error messages</span></span>
* <span data-ttu-id="9767d-744">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="9767d-744">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-745">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-745">ACS</span></span>

* <span data-ttu-id="9767d-746">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="9767d-746">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="9767d-747">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="9767d-747">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="9767d-748">AMS</span><span class="sxs-lookup"><span data-stu-id="9767d-748">AMS</span></span>

* <span data-ttu-id="9767d-749">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="9767d-749">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-750">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="9767d-750">Appservice</span></span>

* <span data-ttu-id="9767d-751">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="9767d-751">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="9767d-752">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-752">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="9767d-753">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="9767d-753">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="9767d-754">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="9767d-754">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9767d-755">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="9767d-755">Batch AI</span></span>

* <span data-ttu-id="9767d-756">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="9767d-756">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9767d-757">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9767d-757">Cognitive Services</span></span>

* <span data-ttu-id="9767d-758">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="9767d-758">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="9767d-759">Потребление</span><span class="sxs-lookup"><span data-stu-id="9767d-759">Consumption</span></span>

* <span data-ttu-id="9767d-760">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="9767d-760">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="9767d-761">Контейнер</span><span class="sxs-lookup"><span data-stu-id="9767d-761">Container</span></span>

* <span data-ttu-id="9767d-762">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="9767d-762">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="9767d-763">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="9767d-763">Cosmos DB</span></span>

* <span data-ttu-id="9767d-764">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9767d-764">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="9767d-765">DMS</span><span class="sxs-lookup"><span data-stu-id="9767d-765">DMS</span></span>

* <span data-ttu-id="9767d-766">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="9767d-766">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="9767d-767">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="9767d-767">Extension</span></span>

* <span data-ttu-id="9767d-768">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="9767d-768">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="9767d-769">Interactive</span><span class="sxs-lookup"><span data-stu-id="9767d-769">Interactive</span></span>

* <span data-ttu-id="9767d-770">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="9767d-770">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="9767d-771">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="9767d-771">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="9767d-772">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="9767d-772">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="9767d-773">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="9767d-773">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="9767d-774">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="9767d-774">Lab</span></span>

* <span data-ttu-id="9767d-775">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="9767d-775">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="9767d-776">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-776">Network</span></span>

* <span data-ttu-id="9767d-777">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="9767d-777">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="9767d-778">Профиль</span><span class="sxs-lookup"><span data-stu-id="9767d-778">Profile</span></span>

* <span data-ttu-id="9767d-779">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-779">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="9767d-780">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="9767d-780">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="9767d-781">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="9767d-781">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="9767d-782">Redis</span><span class="sxs-lookup"><span data-stu-id="9767d-782">Redis</span></span>

* <span data-ttu-id="9767d-783">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="9767d-783">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="9767d-784">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="9767d-784">Deprecated `redis list-all`.</span></span> <span data-ttu-id="9767d-785">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="9767d-785">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="9767d-786">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="9767d-786">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="9767d-787">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="9767d-787">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="9767d-788">Роль</span><span class="sxs-lookup"><span data-stu-id="9767d-788">Role</span></span>

* <span data-ttu-id="9767d-789">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="9767d-789">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-790">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-790">Storage</span></span>

* <span data-ttu-id="9767d-791">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="9767d-791">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="9767d-792">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="9767d-792">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="9767d-793">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="9767d-793">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="9767d-794">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="9767d-794">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="9767d-795">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="9767d-795">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-796">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-796">VM</span></span>

* <span data-ttu-id="9767d-797">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="9767d-797">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="9767d-798">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="9767d-798">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="9767d-799">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="9767d-799">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="9767d-800">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="9767d-800">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="9767d-801">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="9767d-801">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="9767d-802">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="9767d-802">Added write accelerator support</span></span>
* <span data-ttu-id="9767d-803">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="9767d-803">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="9767d-804">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="9767d-804">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="9767d-805">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="9767d-805">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="9767d-806">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-806">April 10, 2018</span></span>

<span data-ttu-id="9767d-807">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="9767d-807">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="9767d-808">ACR</span><span class="sxs-lookup"><span data-stu-id="9767d-808">ACR</span></span>

* <span data-ttu-id="9767d-809">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="9767d-809">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-810">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-810">ACS</span></span>

* <span data-ttu-id="9767d-811">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="9767d-811">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-812">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="9767d-812">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="9767d-814">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="9767d-814">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="9767d-815">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9767d-815">BatchAI</span></span>

* <span data-ttu-id="9767d-816">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="9767d-816">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="9767d-817">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="9767d-817">Job level mounting</span></span>
  - <span data-ttu-id="9767d-818">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="9767d-818">Environment variables with secret values</span></span>
  - <span data-ttu-id="9767d-819">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="9767d-819">Performance counters settings</span></span>
  - <span data-ttu-id="9767d-820">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="9767d-820">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="9767d-821">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="9767d-821">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="9767d-822">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="9767d-822">Usage and limits reporting</span></span>
  - <span data-ttu-id="9767d-823">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="9767d-823">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="9767d-824">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="9767d-824">Support for custom images</span></span>
  - <span data-ttu-id="9767d-825">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="9767d-825">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="9767d-826">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="9767d-826">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="9767d-827">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="9767d-827">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="9767d-828">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="9767d-828">National clouds are supported</span></span>
* <span data-ttu-id="9767d-829">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="9767d-829">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="9767d-830">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="9767d-830">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="9767d-831">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="9767d-831">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="9767d-832">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="9767d-832">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="9767d-833">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="9767d-833">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="9767d-834">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="9767d-834">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="9767d-835">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="9767d-835">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="9767d-836">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="9767d-836">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="9767d-837">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="9767d-837">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="9767d-838">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-838">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="9767d-839">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="9767d-839">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="9767d-840">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="9767d-840">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="9767d-841">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-841">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="9767d-842">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="9767d-842">Billing</span></span>

* <span data-ttu-id="9767d-843">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="9767d-843">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="9767d-844">Потребление</span><span class="sxs-lookup"><span data-stu-id="9767d-844">Consumption</span></span>

* <span data-ttu-id="9767d-845">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="9767d-845">Added `marketplace` commands</span></span>
* <span data-ttu-id="9767d-846">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="9767d-846">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="9767d-847">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="9767d-847">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="9767d-848">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="9767d-848">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="9767d-849">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="9767d-849">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="9767d-850">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="9767d-850">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="9767d-851">Контейнер</span><span class="sxs-lookup"><span data-stu-id="9767d-851">Container</span></span>

* <span data-ttu-id="9767d-852">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="9767d-852">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="9767d-853">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="9767d-853">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="9767d-854">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="9767d-854">Extension</span></span>

* <span data-ttu-id="9767d-855">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="9767d-855">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="9767d-856">Interactive</span><span class="sxs-lookup"><span data-stu-id="9767d-856">Interactive</span></span>

* <span data-ttu-id="9767d-857">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="9767d-857">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="9767d-858">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="9767d-858">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="9767d-859">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="9767d-859">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="9767d-860">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-860">Network</span></span>

* <span data-ttu-id="9767d-861">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-861">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="9767d-862">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-862">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="9767d-863">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="9767d-863">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="9767d-864">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="9767d-864">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="9767d-865">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="9767d-865">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="9767d-866">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-866">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="9767d-867">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-867">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="9767d-868">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="9767d-868">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="9767d-869">Профиль</span><span class="sxs-lookup"><span data-stu-id="9767d-869">Profile</span></span>

* <span data-ttu-id="9767d-870">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="9767d-870">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="9767d-871">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="9767d-871">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="9767d-872">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="9767d-872">RDBMS</span></span>

* <span data-ttu-id="9767d-873">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="9767d-873">Added `georestore` command</span></span>
* <span data-ttu-id="9767d-874">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="9767d-874">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="9767d-875">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9767d-875">Resource</span></span>

* <span data-ttu-id="9767d-876">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-876">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="9767d-877">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-877">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="9767d-878">SQL</span><span class="sxs-lookup"><span data-stu-id="9767d-878">SQL</span></span>

* <span data-ttu-id="9767d-879">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="9767d-879">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-880">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-880">Storage</span></span>

* <span data-ttu-id="9767d-881">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="9767d-881">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-882">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-882">VM</span></span>

* <span data-ttu-id="9767d-883">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="9767d-883">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="9767d-884">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="9767d-884">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="9767d-886">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-886">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="9767d-887">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="9767d-887">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="9767d-888">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="9767d-888">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="9767d-889">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="9767d-889">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="9767d-890">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-890">March 27, 2018</span></span>

<span data-ttu-id="9767d-891">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="9767d-891">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="9767d-892">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-892">Core</span></span>

* <span data-ttu-id="9767d-893">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="9767d-893">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-894">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-894">ACS</span></span>

* <span data-ttu-id="9767d-895">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="9767d-895">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-896">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="9767d-896">Appservice</span></span>

* <span data-ttu-id="9767d-897">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-897">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="9767d-898">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-898">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="9767d-899">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="9767d-899">Backup</span></span>

* <span data-ttu-id="9767d-900">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="9767d-900">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="9767d-901">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="9767d-901">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="9767d-902">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="9767d-902">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="9767d-903">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="9767d-903">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="9767d-904">Контейнер</span><span class="sxs-lookup"><span data-stu-id="9767d-904">Container</span></span>

* <span data-ttu-id="9767d-905">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="9767d-905">Added `container exec` command.</span></span> <span data-ttu-id="9767d-906">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="9767d-906">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="9767d-907">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="9767d-907">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="9767d-908">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="9767d-908">Extension</span></span>

* <span data-ttu-id="9767d-909">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="9767d-909">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="9767d-910">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="9767d-910">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="9767d-911">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9767d-911">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="9767d-912">Interactive</span><span class="sxs-lookup"><span data-stu-id="9767d-912">Interactive</span></span>

* <span data-ttu-id="9767d-913">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="9767d-913">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="9767d-914">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="9767d-914">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="9767d-915">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="9767d-915">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="9767d-916">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="9767d-916">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="9767d-917">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="9767d-917">Lab</span></span>

* <span data-ttu-id="9767d-918">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="9767d-918">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="9767d-919">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="9767d-919">Monitor</span></span>

* <span data-ttu-id="9767d-920">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="9767d-920">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="9767d-921">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="9767d-921">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="9767d-922">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="9767d-922">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="9767d-923">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-923">Network</span></span>

* <span data-ttu-id="9767d-924">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="9767d-924">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="9767d-925">Профиль</span><span class="sxs-lookup"><span data-stu-id="9767d-925">Profile</span></span>

* <span data-ttu-id="9767d-926">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="9767d-926">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="9767d-927">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="9767d-927">RDBMS</span></span>

* <span data-ttu-id="9767d-928">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="9767d-928">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="9767d-929">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9767d-929">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="9767d-931">Роль</span><span class="sxs-lookup"><span data-stu-id="9767d-931">Role</span></span>

* <span data-ttu-id="9767d-932">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-932">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="9767d-933">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="9767d-933">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="9767d-934">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="9767d-934">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="9767d-935">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-935">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="9767d-936">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="9767d-936">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-937">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-937">Storage</span></span>

* <span data-ttu-id="9767d-938">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="9767d-938">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="9767d-939">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049): проблемы, когда при отправке добавочного большого двоичного объекта игнорируются параметры условия.</span><span class="sxs-lookup"><span data-stu-id="9767d-939">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-940">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-940">VM</span></span>

* <span data-ttu-id="9767d-941">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="9767d-941">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="9767d-942">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-942">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="9767d-943">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="9767d-943">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="9767d-944">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="9767d-944">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="9767d-945">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-945">March 13, 2018</span></span>

<span data-ttu-id="9767d-946">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="9767d-946">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="9767d-947">ACR</span><span class="sxs-lookup"><span data-stu-id="9767d-947">ACR</span></span>

* <span data-ttu-id="9767d-948">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="9767d-948">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="9767d-949">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="9767d-949">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="9767d-950">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="9767d-950">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-951">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-951">ACS</span></span>

* <span data-ttu-id="9767d-952">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="9767d-952">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="9767d-953">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="9767d-953">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="9767d-954">Помощник</span><span class="sxs-lookup"><span data-stu-id="9767d-954">Advisor</span></span>

* <span data-ttu-id="9767d-955">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="9767d-955">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="9767d-956">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-956">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="9767d-957">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="9767d-957">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="9767d-958">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="9767d-958">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="9767d-959">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="9767d-959">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-960">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="9767d-960">Appservice</span></span>

* <span data-ttu-id="9767d-961">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="9767d-961">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="9767d-962">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-962">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="9767d-963">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="9767d-963">Eventhubs</span></span>

* <span data-ttu-id="9767d-964">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="9767d-964">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="9767d-965">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="9767d-965">Extension</span></span>

* <span data-ttu-id="9767d-966">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="9767d-966">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="9767d-967">Interactive</span><span class="sxs-lookup"><span data-stu-id="9767d-967">Interactive</span></span>

* <span data-ttu-id="9767d-968">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625): теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="9767d-968">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="9767d-969">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016): при использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="9767d-969">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="9767d-970">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688): если при загрузке таблицы команд возникало исключение, опережающий ввод не выполнялся.</span><span class="sxs-lookup"><span data-stu-id="9767d-970">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="9767d-971">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="9767d-971">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="9767d-972">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="9767d-972">Monitor</span></span>

* <span data-ttu-id="9767d-973">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="9767d-973">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="9767d-974">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="9767d-974">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="9767d-975">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="9767d-975">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="9767d-976">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="9767d-976">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="9767d-977">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-977">Network</span></span>

* <span data-ttu-id="9767d-978">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-978">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="9767d-979">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="9767d-979">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="9767d-980">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="9767d-980">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="9767d-981">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="9767d-981">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="9767d-982">Профиль</span><span class="sxs-lookup"><span data-stu-id="9767d-982">Profile</span></span>

* <span data-ttu-id="9767d-983">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="9767d-983">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="9767d-984">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="9767d-984">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="9767d-985">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="9767d-985">RDBMS</span></span>

* <span data-ttu-id="9767d-986">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="9767d-986">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="9767d-987">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="9767d-987">Service Bus</span></span>

* <span data-ttu-id="9767d-988">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="9767d-988">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-989">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-989">Storage</span></span>

* <span data-ttu-id="9767d-990">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="9767d-990">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="9767d-991">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286): при пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="9767d-991">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-992">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-992">VM</span></span>

* <span data-ttu-id="9767d-993">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="9767d-993">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="9767d-994">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="9767d-994">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="9767d-995">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-995">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="9767d-996">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="9767d-996">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="9767d-997">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="9767d-997">February 27, 2018</span></span>

<span data-ttu-id="9767d-998">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="9767d-998">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="9767d-999">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-999">Core</span></span>

* <span data-ttu-id="9767d-1000">Исправлена ошибка с установкой Homebrew [#5184](https://github.com/Azure/azure-cli/issues/5184).</span><span class="sxs-lookup"><span data-stu-id="9767d-1000">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="9767d-1001">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="9767d-1001">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="9767d-1002">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1002">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-1003">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-1003">ACS</span></span>

* <span data-ttu-id="9767d-1004">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9767d-1004">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="9767d-1005">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="9767d-1005">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="9767d-1006">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1006">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="9767d-1007">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1007">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-1008">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="9767d-1008">Appservice</span></span>

* <span data-ttu-id="9767d-1009">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="9767d-1009">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="9767d-1010">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="9767d-1010">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9767d-1011">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9767d-1011">Cognitive Services</span></span>

* <span data-ttu-id="9767d-1012">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="9767d-1012">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="9767d-1013">Потребление</span><span class="sxs-lookup"><span data-stu-id="9767d-1013">Consumption</span></span>

* <span data-ttu-id="9767d-1014">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="9767d-1014">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="9767d-1015">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="9767d-1015">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="9767d-1016">Контейнер</span><span class="sxs-lookup"><span data-stu-id="9767d-1016">Container</span></span>

* <span data-ttu-id="9767d-1017">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="9767d-1017">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="9767d-1018">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-1018">Network</span></span>

* <span data-ttu-id="9767d-1019">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559): отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1019">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="9767d-1020">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9767d-1020">Resource</span></span>

* <span data-ttu-id="9767d-1021">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="9767d-1021">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="9767d-1022">Роль</span><span class="sxs-lookup"><span data-stu-id="9767d-1022">Role</span></span>

* <span data-ttu-id="9767d-1023">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="9767d-1023">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="9767d-1024">SQL</span><span class="sxs-lookup"><span data-stu-id="9767d-1024">SQL</span></span>

* <span data-ttu-id="9767d-1025">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="9767d-1025">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-1026">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-1026">Storage</span></span>

* <span data-ttu-id="9767d-1027">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1027">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-1028">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-1028">VM</span></span>

* <span data-ttu-id="9767d-1029">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="9767d-1029">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="9767d-1030">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-1030">February 13, 2018</span></span>

<span data-ttu-id="9767d-1031">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="9767d-1031">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="9767d-1032">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-1032">Core</span></span>

* <span data-ttu-id="9767d-1033">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="9767d-1033">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-1034">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-1034">ACS</span></span>

* <span data-ttu-id="9767d-1035">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="9767d-1035">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="9767d-1036">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1036">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="9767d-1037">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="9767d-1037">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="9767d-1038">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="9767d-1038">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="9767d-1039">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="9767d-1039">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="9767d-1040">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1040">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="9767d-1041">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="9767d-1041">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="9767d-1042">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1042">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-1043">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="9767d-1043">Appservice</span></span>

* <span data-ttu-id="9767d-1044">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="9767d-1044">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="9767d-1045">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1045">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="9767d-1046">CDN</span><span class="sxs-lookup"><span data-stu-id="9767d-1046">CDN</span></span>

* <span data-ttu-id="9767d-1047">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1047">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="9767d-1048">Контейнер</span><span class="sxs-lookup"><span data-stu-id="9767d-1048">Container</span></span>

* <span data-ttu-id="9767d-1049">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="9767d-1049">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="9767d-1050">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="9767d-1050">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9767d-1051">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9767d-1051">CosmosDB</span></span>

* <span data-ttu-id="9767d-1052">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="9767d-1052">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="9767d-1053">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="9767d-1053">Extension</span></span>

* <span data-ttu-id="9767d-1054">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1054">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="9767d-1055">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1055">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="9767d-1056">Отзыв</span><span class="sxs-lookup"><span data-stu-id="9767d-1056">Feedback</span></span>

* <span data-ttu-id="9767d-1057">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="9767d-1057">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="9767d-1058">Interactive</span><span class="sxs-lookup"><span data-stu-id="9767d-1058">Interactive</span></span>

* <span data-ttu-id="9767d-1059">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="9767d-1059">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="9767d-1060">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="9767d-1060">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="9767d-1061">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="9767d-1061">IoT</span></span>

* <span data-ttu-id="9767d-1062">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="9767d-1062">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="9767d-1063">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="9767d-1063">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="9767d-1064">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1064">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="9767d-1065">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="9767d-1065">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="9767d-1066">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="9767d-1066">Monitor</span></span>

* <span data-ttu-id="9767d-1067">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1067">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="9767d-1068">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-1068">Network</span></span>

* <span data-ttu-id="9767d-1069">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="9767d-1069">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="9767d-1070">Профиль</span><span class="sxs-lookup"><span data-stu-id="9767d-1070">Profile</span></span>

* <span data-ttu-id="9767d-1071">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="9767d-1071">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="9767d-1072">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9767d-1072">Resource</span></span>

* <span data-ttu-id="9767d-1073">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1073">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="9767d-1074">Роль</span><span class="sxs-lookup"><span data-stu-id="9767d-1074">Role</span></span>

* <span data-ttu-id="9767d-1075">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="9767d-1075">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="9767d-1076">SQL</span><span class="sxs-lookup"><span data-stu-id="9767d-1076">SQL</span></span>

* <span data-ttu-id="9767d-1077">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1077">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="9767d-1078">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1078">Added `sql db rename`</span></span>
* <span data-ttu-id="9767d-1079">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="9767d-1079">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-1080">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-1080">Storage</span></span>

* <span data-ttu-id="9767d-1081">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="9767d-1081">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-1082">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-1082">VM</span></span>

* <span data-ttu-id="9767d-1083">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="9767d-1083">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="9767d-1084">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="9767d-1084">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="9767d-1085">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="9767d-1085">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="9767d-1086">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-1086">January 31, 2018</span></span>

<span data-ttu-id="9767d-1087">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="9767d-1087">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="9767d-1088">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-1088">Core</span></span>

* <span data-ttu-id="9767d-1089">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="9767d-1089">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="9767d-1090">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="9767d-1090">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="9767d-1091">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="9767d-1091">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="9767d-1092">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="9767d-1092">Use `--verbose` to see</span></span>
* <span data-ttu-id="9767d-1093">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="9767d-1093">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-1094">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-1094">ACS</span></span>

* <span data-ttu-id="9767d-1095">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1095">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="9767d-1096">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1096">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-1097">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="9767d-1097">Appservice</span></span>

* <span data-ttu-id="9767d-1098">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="9767d-1098">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="9767d-1099">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="9767d-1099">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="9767d-1100">CDN</span><span class="sxs-lookup"><span data-stu-id="9767d-1100">CDN</span></span>

* <span data-ttu-id="9767d-1101">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1101">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9767d-1102">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9767d-1102">CosmosDB</span></span>

* <span data-ttu-id="9767d-1103">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="9767d-1103">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="9767d-1104">Interactive</span><span class="sxs-lookup"><span data-stu-id="9767d-1104">Interactive</span></span>

* <span data-ttu-id="9767d-1105">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="9767d-1105">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="9767d-1106">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-1106">Network</span></span>

* <span data-ttu-id="9767d-1107">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1107">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="9767d-1108">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9767d-1108">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="9767d-1109">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1109">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="9767d-1110">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1110">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="9767d-1111">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1111">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="9767d-1112">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="9767d-1112">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="9767d-1113">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="9767d-1113">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="9767d-1114">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="9767d-1114">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="9767d-1115">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1115">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="9767d-1116">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1116">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="9767d-1117">Профиль</span><span class="sxs-lookup"><span data-stu-id="9767d-1117">Profile</span></span>

* <span data-ttu-id="9767d-1118">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="9767d-1118">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="9767d-1119">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9767d-1119">Resource</span></span>

* <span data-ttu-id="9767d-1120">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="9767d-1120">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-1121">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-1121">Storage</span></span>

* <span data-ttu-id="9767d-1122">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="9767d-1122">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="9767d-1123">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="9767d-1123">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="9767d-1124">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1124">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="9767d-1125">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1125">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="9767d-1126">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="9767d-1126">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-1127">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-1127">VM</span></span>

* <span data-ttu-id="9767d-1128">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="9767d-1128">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="9767d-1129">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="9767d-1129">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="9767d-1130">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="9767d-1130">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="9767d-1131">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1131">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="9767d-1132">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-1132">January 17, 2018</span></span>

<span data-ttu-id="9767d-1133">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="9767d-1133">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="9767d-1134">ACR</span><span class="sxs-lookup"><span data-stu-id="9767d-1134">ACR</span></span>

* <span data-ttu-id="9767d-1135">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="9767d-1135">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="9767d-1136">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="9767d-1136">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-1137">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-1137">ACS</span></span>

* <span data-ttu-id="9767d-1138">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1138">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="9767d-1139">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="9767d-1139">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-1140">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="9767d-1140">Appservice</span></span>

* <span data-ttu-id="9767d-1141">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="9767d-1141">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="9767d-1142">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="9767d-1142">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="9767d-1143">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1143">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="9767d-1144">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="9767d-1144">Backup</span></span>

* <span data-ttu-id="9767d-1145">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="9767d-1145">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="9767d-1146">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="9767d-1146">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="9767d-1147">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="9767d-1147">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="9767d-1148">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="9767d-1148">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="9767d-1149">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="9767d-1149">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="9767d-1150">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="9767d-1150">Batch</span></span>

* <span data-ttu-id="9767d-1151">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="9767d-1151">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="9767d-1152">Облако</span><span class="sxs-lookup"><span data-stu-id="9767d-1152">Cloud</span></span>

* <span data-ttu-id="9767d-1153">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="9767d-1153">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="9767d-1154">Потребление</span><span class="sxs-lookup"><span data-stu-id="9767d-1154">Consumption</span></span>

* <span data-ttu-id="9767d-1155">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1155">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="9767d-1156">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="9767d-1156">Event Grid</span></span>

* <span data-ttu-id="9767d-1157">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1157">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="9767d-1158">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1158">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="9767d-1159">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1159">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="9767d-1160">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1160">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="9767d-1161">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1161">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="9767d-1162">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1162">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="9767d-1163">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1163">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="9767d-1164">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="9767d-1164">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="9767d-1165">Interactive</span><span class="sxs-lookup"><span data-stu-id="9767d-1165">Interactive</span></span>

* <span data-ttu-id="9767d-1166">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="9767d-1166">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="9767d-1167">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="9767d-1167">Fixed errors on startup</span></span>
* <span data-ttu-id="9767d-1168">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="9767d-1168">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="9767d-1169">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="9767d-1169">IoT</span></span>

* <span data-ttu-id="9767d-1170">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="9767d-1170">Added support for device provisioning service</span></span>
* <span data-ttu-id="9767d-1171">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="9767d-1171">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="9767d-1172">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="9767d-1172">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="9767d-1173">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="9767d-1173">Monitor</span></span>

* <span data-ttu-id="9767d-1174">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="9767d-1174">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="9767d-1175">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1175">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="9767d-1176">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="9767d-1176">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="9767d-1177">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-1177">Network</span></span>

* <span data-ttu-id="9767d-1178">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="9767d-1178">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="9767d-1179">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="9767d-1179">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="9767d-1180">Профиль</span><span class="sxs-lookup"><span data-stu-id="9767d-1180">Profile</span></span>

* <span data-ttu-id="9767d-1181">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="9767d-1181">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="9767d-1182">Роль</span><span class="sxs-lookup"><span data-stu-id="9767d-1182">Role</span></span>

* <span data-ttu-id="9767d-1183">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="9767d-1183">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="9767d-1184">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9767d-1184">Service Fabric</span></span>

* <span data-ttu-id="9767d-1185">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="9767d-1185">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="9767d-1186">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="9767d-1186">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-1187">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-1187">VM</span></span>

* <span data-ttu-id="9767d-1188">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1188">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="9767d-1189">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="9767d-1189">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="9767d-1190">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1190">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="9767d-1191">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="9767d-1191">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="9767d-1192">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="9767d-1192">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="9767d-1193">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1193">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="9767d-1194">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1194">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="9767d-1195">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1195">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="9767d-1196">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-1196">December 19, 2017</span></span>

<span data-ttu-id="9767d-1197">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="9767d-1197">Version 2.0.23</span></span>

* <span data-ttu-id="9767d-1198">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="9767d-1198">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="9767d-1199">Контейнер</span><span class="sxs-lookup"><span data-stu-id="9767d-1199">Container</span></span>

* <span data-ttu-id="9767d-1200">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="9767d-1200">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="9767d-1201">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-1201">Network</span></span>

* <span data-ttu-id="9767d-1202">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9767d-1202">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="9767d-1203">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9767d-1203">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-1204">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-1204">Storage</span></span>

* <span data-ttu-id="9767d-1205">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="9767d-1205">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-1206">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-1206">VM</span></span>

* <span data-ttu-id="9767d-1207">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="9767d-1207">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="9767d-1208">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-1208">December 5, 2017</span></span>

<span data-ttu-id="9767d-1209">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="9767d-1209">Version 2.0.22</span></span>

* <span data-ttu-id="9767d-1210">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1210">Removed `az component` commands.</span></span> <span data-ttu-id="9767d-1211">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1211">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="9767d-1212">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-1212">Core</span></span>
* <span data-ttu-id="9767d-1213">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="9767d-1213">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="9767d-1214">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="9767d-1214">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-1215">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-1215">ACS</span></span>

* <span data-ttu-id="9767d-1216">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1216">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="9767d-1217">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1217">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="9767d-1218">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="9767d-1218">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="9767d-1219">Помощник</span><span class="sxs-lookup"><span data-stu-id="9767d-1219">Advisor</span></span>

* <span data-ttu-id="9767d-1220">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="9767d-1220">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-1221">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="9767d-1221">Appservice</span></span>

* <span data-ttu-id="9767d-1222">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1222">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="9767d-1223">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="9767d-1223">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="9767d-1224">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1224">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="9767d-1225">Потребление</span><span class="sxs-lookup"><span data-stu-id="9767d-1225">Consumption</span></span>

* <span data-ttu-id="9767d-1226">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="9767d-1226">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="9767d-1227">Контейнер</span><span class="sxs-lookup"><span data-stu-id="9767d-1227">Container</span></span>

* <span data-ttu-id="9767d-1228">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="9767d-1228">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="9767d-1229">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="9767d-1229">Monitor</span></span>

* <span data-ttu-id="9767d-1230">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="9767d-1230">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="9767d-1231">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9767d-1231">Resource</span></span>

* <span data-ttu-id="9767d-1232">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="9767d-1232">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="9767d-1233">Роль</span><span class="sxs-lookup"><span data-stu-id="9767d-1233">Role</span></span>

* <span data-ttu-id="9767d-1234">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1234">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="9767d-1235">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="9767d-1235">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="9767d-1236">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1236">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="9767d-1237">SQL</span><span class="sxs-lookup"><span data-stu-id="9767d-1237">SQL</span></span>

* <span data-ttu-id="9767d-1238">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1238">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="9767d-1239">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1239">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-1240">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-1240">VM</span></span>

* <span data-ttu-id="9767d-1241">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1241">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="9767d-1242">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-1242">November 14, 2017</span></span>

<span data-ttu-id="9767d-1243">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="9767d-1243">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="9767d-1244">ACR</span><span class="sxs-lookup"><span data-stu-id="9767d-1244">ACR</span></span>

* <span data-ttu-id="9767d-1245">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="9767d-1245">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="9767d-1246">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-1246">ACS</span></span>

* <span data-ttu-id="9767d-1247">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="9767d-1247">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="9767d-1248">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="9767d-1248">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="9767d-1249">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1249">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="9767d-1250">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="9767d-1250">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="9767d-1251">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="9767d-1251">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-1252">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="9767d-1252">Appservice</span></span>

* <span data-ttu-id="9767d-1253">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="9767d-1253">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="9767d-1254">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1254">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="9767d-1255">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1255">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="9767d-1256">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1256">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="9767d-1257">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="9767d-1257">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="9767d-1258">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="9767d-1258">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="9767d-1259">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="9767d-1259">Batch</span></span>

* <span data-ttu-id="9767d-1260">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1260">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="9767d-1261">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="9767d-1261">Batchai</span></span>

* <span data-ttu-id="9767d-1262">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1262">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="9767d-1263">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1263">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="9767d-1264">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1264">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="9767d-1265">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1265">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="9767d-1266">Облако</span><span class="sxs-lookup"><span data-stu-id="9767d-1266">Cloud</span></span>

* <span data-ttu-id="9767d-1267">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="9767d-1267">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="9767d-1268">Контейнер</span><span class="sxs-lookup"><span data-stu-id="9767d-1268">Container</span></span>

* <span data-ttu-id="9767d-1269">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="9767d-1269">Added support to open multiple ports</span></span>
* <span data-ttu-id="9767d-1270">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="9767d-1270">Added container group restart policy</span></span>
* <span data-ttu-id="9767d-1271">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="9767d-1271">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="9767d-1272">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="9767d-1272">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="9767d-1273">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="9767d-1273">Data Lake Analytics</span></span>

* <span data-ttu-id="9767d-1274">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="9767d-1274">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="9767d-1275">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9767d-1275">Data Lake Store</span></span>

* <span data-ttu-id="9767d-1276">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="9767d-1276">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="9767d-1277">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="9767d-1277">Extension</span></span>

* <span data-ttu-id="9767d-1278">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="9767d-1278">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="9767d-1279">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="9767d-1279">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="9767d-1280">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="9767d-1280">IoT</span></span>

* <span data-ttu-id="9767d-1281">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="9767d-1281">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="9767d-1282">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="9767d-1282">Monitor</span></span>

* <span data-ttu-id="9767d-1283">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1283">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="9767d-1284">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-1284">Network</span></span>

* <span data-ttu-id="9767d-1285">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="9767d-1285">Added support for CAA DNS records</span></span>
* <span data-ttu-id="9767d-1286">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1286">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="9767d-1287">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="9767d-1287">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="9767d-1288">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1288">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="9767d-1289">Резервирование</span><span class="sxs-lookup"><span data-stu-id="9767d-1289">Reservations</span></span>

* <span data-ttu-id="9767d-1290">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="9767d-1290">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="9767d-1291">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9767d-1291">Resource</span></span>

* <span data-ttu-id="9767d-1292">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1292">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="9767d-1293">SQL</span><span class="sxs-lookup"><span data-stu-id="9767d-1293">SQL</span></span>

* <span data-ttu-id="9767d-1294">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1294">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-1295">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-1295">Storage</span></span>

* <span data-ttu-id="9767d-1296">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9767d-1296">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="9767d-1297">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="9767d-1297">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="9767d-1298">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1298">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="9767d-1299">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1299">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="9767d-1300">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1300">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="9767d-1301">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1301">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="9767d-1302">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1302">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-1303">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-1303">VM</span></span>

* <span data-ttu-id="9767d-1304">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1304">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="9767d-1305">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="9767d-1305">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="9767d-1306">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1306">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="9767d-1307">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1307">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="9767d-1308">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="9767d-1308">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="9767d-1309">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-1309">October 24, 2017</span></span>

<span data-ttu-id="9767d-1310">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="9767d-1310">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="9767d-1311">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-1311">Core</span></span>

* <span data-ttu-id="9767d-1312">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="9767d-1312">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="9767d-1313">ACR</span><span class="sxs-lookup"><span data-stu-id="9767d-1313">ACR</span></span>

* <span data-ttu-id="9767d-1314">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="9767d-1314">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="9767d-1315">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="9767d-1315">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="9767d-1316">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="9767d-1316">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-1317">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-1317">ACS</span></span>

* <span data-ttu-id="9767d-1318">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="9767d-1318">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="9767d-1319">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="9767d-1319">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-1320">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="9767d-1320">Appservice</span></span>

* <span data-ttu-id="9767d-1321">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="9767d-1321">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="9767d-1322">Компонент</span><span class="sxs-lookup"><span data-stu-id="9767d-1322">Component</span></span>

* <span data-ttu-id="9767d-1323">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="9767d-1323">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="9767d-1324">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="9767d-1324">Monitor</span></span>

* <span data-ttu-id="9767d-1325">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1325">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="9767d-1326">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9767d-1326">Resource</span></span>

* <span data-ttu-id="9767d-1327">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="9767d-1327">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="9767d-1328">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="9767d-1328">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-1329">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-1329">VM</span></span>

* <span data-ttu-id="9767d-1330">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="9767d-1330">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="9767d-1331">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-1331">October 9, 2017</span></span>

<span data-ttu-id="9767d-1332">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="9767d-1332">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="9767d-1333">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-1333">Core</span></span>

* <span data-ttu-id="9767d-1334">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="9767d-1334">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-1335">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="9767d-1335">Appservice</span></span>

* <span data-ttu-id="9767d-1336">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1336">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="9767d-1337">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="9767d-1337">Batch</span></span>

* <span data-ttu-id="9767d-1338">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="9767d-1338">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="9767d-1339">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="9767d-1339">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="9767d-1340">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="9767d-1340">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="9767d-1341">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="9767d-1341">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="9767d-1342">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="9767d-1342">Batchai</span></span>

* <span data-ttu-id="9767d-1343">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="9767d-1343">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="9767d-1344">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="9767d-1344">Keyvault</span></span>

* <span data-ttu-id="9767d-1345">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="9767d-1345">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="9767d-1346">(#4448)</span><span class="sxs-lookup"><span data-stu-id="9767d-1346">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="9767d-1347">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-1347">Network</span></span>

* <span data-ttu-id="9767d-1348">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="9767d-1348">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="9767d-1349">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="9767d-1349">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="9767d-1350">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9767d-1350">Resource</span></span>

* <span data-ttu-id="9767d-1351">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1351">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="9767d-1352">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="9767d-1352">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="9767d-1353">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="9767d-1353">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="9767d-1354">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="9767d-1354">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="9767d-1355">SQL</span><span class="sxs-lookup"><span data-stu-id="9767d-1355">Sql</span></span>

* <span data-ttu-id="9767d-1356">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="9767d-1356">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="9767d-1357">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="9767d-1357">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="9767d-1358">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="9767d-1358">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-1359">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-1359">Storage</span></span>

* <span data-ttu-id="9767d-1360">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="9767d-1360">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-1361">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="9767d-1361">Vm</span></span>

* <span data-ttu-id="9767d-1362">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="9767d-1362">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="9767d-1363">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1363">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="9767d-1364">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1364">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="9767d-1365">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1365">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="9767d-1366">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="9767d-1366">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="9767d-1367">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-1367">September 22, 2017</span></span>

<span data-ttu-id="9767d-1368">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="9767d-1368">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="9767d-1369">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9767d-1369">Resource</span></span>

* <span data-ttu-id="9767d-1370">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="9767d-1370">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="9767d-1371">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="9767d-1371">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="9767d-1372">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="9767d-1372">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="9767d-1373">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1373">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="9767d-1374">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-1374">Network</span></span>

* <span data-ttu-id="9767d-1375">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="9767d-1375">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="9767d-1376">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="9767d-1376">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="9767d-1377">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="9767d-1377">Added `asg` application security group commands</span></span>
* <span data-ttu-id="9767d-1378">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="9767d-1378">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="9767d-1379">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9767d-1379">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="9767d-1380">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9767d-1380">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="9767d-1381">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1381">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-1382">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-1382">Storage</span></span>

* <span data-ttu-id="9767d-1383">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="9767d-1383">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="9767d-1384">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="9767d-1384">Eventgrid</span></span>

* <span data-ttu-id="9767d-1385">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="9767d-1385">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="9767d-1386">SQL</span><span class="sxs-lookup"><span data-stu-id="9767d-1386">SQL</span></span>

* <span data-ttu-id="9767d-1387">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="9767d-1387">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="9767d-1388">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="9767d-1388">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="9767d-1389">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9767d-1389">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="9767d-1390">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="9767d-1390">Keyvault</span></span>

* <span data-ttu-id="9767d-1391">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="9767d-1391">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-1392">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-1392">VM</span></span>

* <span data-ttu-id="9767d-1393">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="9767d-1393">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="9767d-1394">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="9767d-1394">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="9767d-1395">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="9767d-1395">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="9767d-1396">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="9767d-1396">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="9767d-1397">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="9767d-1397">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="9767d-1398">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="9767d-1398">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-1399">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-1399">ACS</span></span>

* <span data-ttu-id="9767d-1400">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="9767d-1400">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-1401">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="9767d-1401">Appservice</span></span>

* <span data-ttu-id="9767d-1402">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="9767d-1402">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="9767d-1403">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="9767d-1403">Backup</span></span>

* <span data-ttu-id="9767d-1404">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="9767d-1404">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="9767d-1405">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-1405">September 11, 2017</span></span>

<span data-ttu-id="9767d-1406">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="9767d-1406">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="9767d-1407">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-1407">Core</span></span>

* <span data-ttu-id="9767d-1408">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="9767d-1408">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="9767d-1409">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="9767d-1409">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-1410">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-1410">Acs</span></span>

* <span data-ttu-id="9767d-1411">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1411">Added `acs list-locations` command</span></span>
* <span data-ttu-id="9767d-1412">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9767d-1412">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-1413">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="9767d-1413">Appservice</span></span>

* <span data-ttu-id="9767d-1414">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="9767d-1414">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="9767d-1415">CDN</span><span class="sxs-lookup"><span data-stu-id="9767d-1415">CDN</span></span>

* <span data-ttu-id="9767d-1416">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1416">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="9767d-1417">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="9767d-1417">Extension</span></span>

* <span data-ttu-id="9767d-1418">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="9767d-1418">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="9767d-1419">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="9767d-1419">Keyvault</span></span>

* <span data-ttu-id="9767d-1420">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1420">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="9767d-1421">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-1421">Network</span></span>

* <span data-ttu-id="9767d-1422">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1422">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="9767d-1423">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1423">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="9767d-1424">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1424">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="9767d-1425">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1425">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="9767d-1426">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1426">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="9767d-1427">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9767d-1427">Resource</span></span>

* <span data-ttu-id="9767d-1428">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1428">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="9767d-1429">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1429">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="9767d-1430">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="9767d-1430">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="9767d-1431">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="9767d-1431">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="9767d-1432">SQL</span><span class="sxs-lookup"><span data-stu-id="9767d-1432">SQL</span></span>

* <span data-ttu-id="9767d-1433">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1433">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-1434">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-1434">VM</span></span>

* <span data-ttu-id="9767d-1435">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="9767d-1435">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="9767d-1436">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="9767d-1436">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="9767d-1437">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1437">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="9767d-1438">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="9767d-1438">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="9767d-1439">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="9767d-1439">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="9767d-1440">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-1440">August 31, 2017</span></span>

<span data-ttu-id="9767d-1441">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="9767d-1441">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="9767d-1442">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="9767d-1442">Keyvault</span></span>

* <span data-ttu-id="9767d-1443">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1443">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="9767d-1444">Sf</span><span class="sxs-lookup"><span data-stu-id="9767d-1444">Sf</span></span>

* <span data-ttu-id="9767d-1445">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="9767d-1445">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-1446">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-1446">Storage</span></span>

* <span data-ttu-id="9767d-1447">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="9767d-1447">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="9767d-1448">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="9767d-1448">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="9767d-1449">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-1449">August 28, 2017</span></span>

<span data-ttu-id="9767d-1450">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="9767d-1450">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="9767d-1451">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="9767d-1451">CLI</span></span>

* <span data-ttu-id="9767d-1452">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="9767d-1452">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-1453">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-1453">ACS</span></span>

* <span data-ttu-id="9767d-1454">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="9767d-1454">Corrected preview regions</span></span>
* <span data-ttu-id="9767d-1455">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1455">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="9767d-1456">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="9767d-1456">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-1457">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="9767d-1457">Appservice</span></span>

* <span data-ttu-id="9767d-1458">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1458">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="9767d-1459">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1459">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="9767d-1460">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1460">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="9767d-1461">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="9767d-1461">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="9767d-1462">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="9767d-1462">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="9767d-1463">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="9767d-1463">IoT</span></span>

* <span data-ttu-id="9767d-1464">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="9767d-1464">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="9767d-1465">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-1465">Network</span></span>

* <span data-ttu-id="9767d-1466">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1466">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="9767d-1467">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1467">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="9767d-1468">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1468">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="9767d-1469">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1469">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="9767d-1470">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1470">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="9767d-1471">Профиль</span><span class="sxs-lookup"><span data-stu-id="9767d-1471">Profile</span></span>

* <span data-ttu-id="9767d-1472">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="9767d-1472">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="9767d-1473">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9767d-1473">Service Fabric</span></span>

* <span data-ttu-id="9767d-1474">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="9767d-1474">Preview release</span></span>
* <span data-ttu-id="9767d-1475">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="9767d-1475">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="9767d-1476">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="9767d-1476">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="9767d-1477">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1477">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-1478">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-1478">Storage</span></span>

* <span data-ttu-id="9767d-1479">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="9767d-1479">Enabled setting blob tier</span></span>
* <span data-ttu-id="9767d-1480">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="9767d-1480">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="9767d-1481">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1481">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="9767d-1482">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="9767d-1482">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="9767d-1483">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1483">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="9767d-1484">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1484">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-1485">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-1485">VM</span></span>

* <span data-ttu-id="9767d-1486">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1486">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="9767d-1487">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1487">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="9767d-1488">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="9767d-1488">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="9767d-1489">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="9767d-1489">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="9767d-1490">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="9767d-1490">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="9767d-1491">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1491">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="9767d-1492">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-1492">August 15, 2017</span></span>

<span data-ttu-id="9767d-1493">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="9767d-1493">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-1494">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-1494">ACS</span></span>

* <span data-ttu-id="9767d-1495">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="9767d-1495">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-1496">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="9767d-1496">Appservice</span></span>

* <span data-ttu-id="9767d-1497">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="9767d-1497">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="9767d-1498">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="9767d-1498">Event Grid</span></span>

* <span data-ttu-id="9767d-1499">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="9767d-1499">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="9767d-1500">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-1500">August 11, 2017</span></span>

<span data-ttu-id="9767d-1501">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="9767d-1501">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-1502">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-1502">ACS</span></span>

* <span data-ttu-id="9767d-1503">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="9767d-1503">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="9767d-1504">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="9767d-1504">Batch</span></span>

* <span data-ttu-id="9767d-1505">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="9767d-1505">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="9767d-1506">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="9767d-1506">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="9767d-1507">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="9767d-1507">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="9767d-1508">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="9767d-1508">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="9767d-1509">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="9767d-1509">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="9767d-1510">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="9767d-1510">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="9767d-1511">Компонент</span><span class="sxs-lookup"><span data-stu-id="9767d-1511">Component</span></span>

* <span data-ttu-id="9767d-1512">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="9767d-1512">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="9767d-1513">Контейнер</span><span class="sxs-lookup"><span data-stu-id="9767d-1513">Container</span></span>

* <span data-ttu-id="9767d-1514">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="9767d-1514">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="9767d-1515">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9767d-1515">Data Lake Store</span></span>

* <span data-ttu-id="9767d-1516">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="9767d-1516">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="9767d-1517">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="9767d-1517">Event Grid</span></span>

* <span data-ttu-id="9767d-1518">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="9767d-1518">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="9767d-1519">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-1519">Network</span></span>

* <span data-ttu-id="9767d-1520">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="9767d-1520">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="9767d-1521">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1521">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="9767d-1522">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1522">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="9767d-1523">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1523">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="9767d-1524">Профиль</span><span class="sxs-lookup"><span data-stu-id="9767d-1524">Profile</span></span>

* <span data-ttu-id="9767d-1525">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="9767d-1525">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-1526">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-1526">Storage</span></span>

* <span data-ttu-id="9767d-1527">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="9767d-1527">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-1528">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-1528">VM</span></span>

* <span data-ttu-id="9767d-1529">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="9767d-1529">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="9767d-1530">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1530">Exposed `list-skus` command</span></span>
* <span data-ttu-id="9767d-1531">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="9767d-1531">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="9767d-1532">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="9767d-1532">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="9767d-1533">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="9767d-1533">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="9767d-1534">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-1534">July 28, 2017</span></span>

<span data-ttu-id="9767d-1535">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="9767d-1535">Version 2.0.12</span></span>

* <span data-ttu-id="9767d-1536">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="9767d-1536">Added container commands</span></span>
* <span data-ttu-id="9767d-1537">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="9767d-1537">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="9767d-1538">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-1538">Core</span></span>

* <span data-ttu-id="9767d-1539">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="9767d-1539">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="9767d-1540">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="9767d-1540">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="9767d-1541">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="9767d-1541">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="9767d-1542">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="9767d-1542">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="9767d-1543">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="9767d-1543">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="9767d-1544">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="9767d-1544">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="9767d-1545">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="9767d-1545">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="9767d-1546">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="9767d-1546">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="9767d-1547">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="9767d-1547">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="9767d-1548">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="9767d-1548">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="9767d-1549">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="9767d-1549">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="9767d-1550">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="9767d-1550">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="9767d-1551">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="9767d-1551">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="9767d-1552">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="9767d-1552">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="9767d-1553">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="9767d-1553">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="9767d-1554">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="9767d-1554">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="9767d-1555">ACR</span><span class="sxs-lookup"><span data-stu-id="9767d-1555">ACR</span></span>

* <span data-ttu-id="9767d-1556">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="9767d-1556">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="9767d-1557">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="9767d-1557">Support SKU update for managed registries</span></span>
* <span data-ttu-id="9767d-1558">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="9767d-1558">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="9767d-1559">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="9767d-1559">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="9767d-1560">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="9767d-1560">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="9767d-1561">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="9767d-1561">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-1562">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-1562">ACS</span></span>

* <span data-ttu-id="9767d-1563">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="9767d-1563">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-1564">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="9767d-1564">Appservice</span></span>

* <span data-ttu-id="9767d-1565">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="9767d-1565">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="9767d-1566">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="9767d-1566">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="9767d-1567">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1567">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="9767d-1568">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="9767d-1568">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="9767d-1569">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="9767d-1569">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="9767d-1570">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="9767d-1570">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="9767d-1571">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="9767d-1571">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="9767d-1572">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="9767d-1572">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="9767d-1573">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="9767d-1573">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="9767d-1574">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1574">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="9767d-1575">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="9767d-1575">Batch</span></span>

* <span data-ttu-id="9767d-1576">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="9767d-1576">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="9767d-1577">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1577">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="9767d-1578">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1578">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="9767d-1579">CDN</span><span class="sxs-lookup"><span data-stu-id="9767d-1579">CDN</span></span>

* <span data-ttu-id="9767d-1580">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="9767d-1580">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="9767d-1581">Облако</span><span class="sxs-lookup"><span data-stu-id="9767d-1581">Cloud</span></span>

* <span data-ttu-id="9767d-1582">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="9767d-1582">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="9767d-1583">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="9767d-1583">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="9767d-1584">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="9767d-1584">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="9767d-1585">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="9767d-1585">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="9767d-1586">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1586">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9767d-1587">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9767d-1587">CosmosDB</span></span>

* <span data-ttu-id="9767d-1588">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="9767d-1588">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="9767d-1589">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="9767d-1589">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="9767d-1590">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="9767d-1590">Data Lake Analytics</span></span>

* <span data-ttu-id="9767d-1591">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1591">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="9767d-1592">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1592">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="9767d-1593">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1593">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="9767d-1594">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9767d-1594">Data Lake Store</span></span>

* <span data-ttu-id="9767d-1595">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1595">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="9767d-1596">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="9767d-1596">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="9767d-1597">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1597">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="9767d-1598">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="9767d-1598">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="9767d-1599">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="9767d-1599">Interactive</span></span>

* <span data-ttu-id="9767d-1600">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="9767d-1600">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="9767d-1601">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="9767d-1601">Increased test coverage</span></span>
* <span data-ttu-id="9767d-1602">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="9767d-1602">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="9767d-1603">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="9767d-1603">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="9767d-1604">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="9767d-1604">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="9767d-1605">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="9767d-1605">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="9767d-1606">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="9767d-1606">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="9767d-1607">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1607">Added `--progress` flag</span></span>
* <span data-ttu-id="9767d-1608">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1608">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="9767d-1609">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="9767d-1609">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="9767d-1610">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="9767d-1610">IoT</span></span>

* <span data-ttu-id="9767d-1611">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="9767d-1611">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="9767d-1612">(3934).</span><span class="sxs-lookup"><span data-stu-id="9767d-1612">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="9767d-1613">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="9767d-1613">Key vault</span></span>

* <span data-ttu-id="9767d-1614">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="9767d-1614">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="9767d-1615">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1615">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="9767d-1616">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="9767d-1616">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="9767d-1617">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="9767d-1617">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="9767d-1618">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1618">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="9767d-1619">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="9767d-1619">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="9767d-1620">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="9767d-1620">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="9767d-1621">(3307).</span><span class="sxs-lookup"><span data-stu-id="9767d-1621">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="9767d-1622">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="9767d-1622">Lab</span></span>

* <span data-ttu-id="9767d-1623">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1623">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="9767d-1624">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1624">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="9767d-1625">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="9767d-1625">Monitor</span></span>

* <span data-ttu-id="9767d-1626">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="9767d-1626">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="9767d-1627">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1627">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="9767d-1628">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1628">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="9767d-1629">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1629">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="9767d-1630">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1630">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="9767d-1631">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="9767d-1631">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="9767d-1632">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="9767d-1632">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="9767d-1633">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="9767d-1633">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="9767d-1634">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="9767d-1634">`location` no longer required</span></span>
  * <span data-ttu-id="9767d-1635">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="9767d-1635">Add name and ID support for target</span></span>
  * <span data-ttu-id="9767d-1636">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="9767d-1636">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="9767d-1637">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="9767d-1637">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="9767d-1638">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="9767d-1638">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="9767d-1639">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="9767d-1639">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="9767d-1640">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1640">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="9767d-1641">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1641">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="9767d-1642">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-1642">Network</span></span>

* <span data-ttu-id="9767d-1643">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1643">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="9767d-1644">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1644">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="9767d-1645">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="9767d-1645">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="9767d-1646">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1646">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="9767d-1647">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1647">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="9767d-1648">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1648">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="9767d-1649">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1649">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="9767d-1650">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1650">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="9767d-1651">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1651">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="9767d-1652">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1652">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="9767d-1653">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1653">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="9767d-1654">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1654">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="9767d-1655">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1655">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="9767d-1656">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1656">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="9767d-1657">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1657">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="9767d-1658">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1658">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="9767d-1659">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="9767d-1659">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="9767d-1660">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1660">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="9767d-1661">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1661">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="9767d-1662">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1662">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="9767d-1663">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1663">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="9767d-1664">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1664">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="9767d-1665">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1665">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="9767d-1666">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="9767d-1666">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="9767d-1667">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="9767d-1667">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="9767d-1668">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="9767d-1668">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="9767d-1669">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="9767d-1669">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="9767d-1670">Профиль</span><span class="sxs-lookup"><span data-stu-id="9767d-1670">Profile</span></span>

* <span data-ttu-id="9767d-1671">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="9767d-1671">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="9767d-1672">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="9767d-1672">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="9767d-1673">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="9767d-1673">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="9767d-1674">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="9767d-1674">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="9767d-1675">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="9767d-1675">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="9767d-1676">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="9767d-1676">RDBMS</span></span>

* <span data-ttu-id="9767d-1677">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="9767d-1677">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="9767d-1678">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="9767d-1678">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="9767d-1679">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="9767d-1679">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="9767d-1680">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="9767d-1680">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="9767d-1681">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9767d-1681">Resource</span></span>

* <span data-ttu-id="9767d-1682">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1682">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="9767d-1683">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1683">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="9767d-1684">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1684">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="9767d-1685">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1685">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="9767d-1686">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="9767d-1686">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="9767d-1687">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1687">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="9767d-1688">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="9767d-1688">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="9767d-1689">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1689">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="9767d-1690">Роль</span><span class="sxs-lookup"><span data-stu-id="9767d-1690">Role</span></span>

* <span data-ttu-id="9767d-1691">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="9767d-1691">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="9767d-1692">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="9767d-1692">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="9767d-1693">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="9767d-1693">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="9767d-1694">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="9767d-1694">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="9767d-1695">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1695">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="9767d-1696">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9767d-1696">Service Fabric</span></span>
* <span data-ttu-id="9767d-1697">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="9767d-1697">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="9767d-1698">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="9767d-1698">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="9767d-1699">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="9767d-1699">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="9767d-1700">SQL</span><span class="sxs-lookup"><span data-stu-id="9767d-1700">SQL</span></span>

* <span data-ttu-id="9767d-1701">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1701">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="9767d-1702">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1702">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="9767d-1703">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1703">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-1704">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-1704">Storage</span></span>

* <span data-ttu-id="9767d-1705">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="9767d-1705">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="9767d-1706">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="9767d-1706">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="9767d-1707">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="9767d-1707">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="9767d-1708">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="9767d-1708">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="9767d-1709">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="9767d-1709">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="9767d-1710">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="9767d-1710">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-1711">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-1711">VM</span></span>

* <span data-ttu-id="9767d-1712">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="9767d-1712">Support configuring nsg</span></span>
* <span data-ttu-id="9767d-1713">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="9767d-1713">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="9767d-1714">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="9767d-1714">Support managed service identities</span></span>
* <span data-ttu-id="9767d-1715">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1715">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="9767d-1716">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="9767d-1716">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="9767d-1717">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-1717">May 10, 2017</span></span>

<span data-ttu-id="9767d-1718">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="9767d-1718">Version 2.0.6</span></span>

* <span data-ttu-id="9767d-1719">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="9767d-1719">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="9767d-1720">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="9767d-1720">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="9767d-1721">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="9767d-1721">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="9767d-1722">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="9767d-1722">Include Cognitive Services module</span></span>
* <span data-ttu-id="9767d-1723">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="9767d-1723">Include Service Fabric module</span></span>
* <span data-ttu-id="9767d-1724">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="9767d-1724">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="9767d-1725">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="9767d-1725">Add support for CDN commands</span></span>
* <span data-ttu-id="9767d-1726">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="9767d-1726">Remove Container module</span></span>
* <span data-ttu-id="9767d-1727">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1727">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="9767d-1728">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1728">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="9767d-1729">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-1729">Core</span></span>

* <span data-ttu-id="9767d-1730">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="9767d-1730">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="9767d-1731">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1731">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="9767d-1732">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1732">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="9767d-1733">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1733">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="9767d-1734">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1734">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="9767d-1735">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1735">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="9767d-1736">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1736">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="9767d-1737">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1737">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="9767d-1738">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1738">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="9767d-1739">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="9767d-1739">core: Improved performance</span></span>
* <span data-ttu-id="9767d-1740">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="9767d-1740">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="9767d-1741">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="9767d-1741">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-1742">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-1742">ACS</span></span>

* <span data-ttu-id="9767d-1743">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="9767d-1743">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="9767d-1744">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="9767d-1744">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="9767d-1745">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="9767d-1745">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="9767d-1746">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1746">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-1747">AppService</span><span class="sxs-lookup"><span data-stu-id="9767d-1747">AppService</span></span>

* <span data-ttu-id="9767d-1748">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="9767d-1748">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="9767d-1749">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="9767d-1749">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="9767d-1750">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="9767d-1750">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="9767d-1751">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="9767d-1751">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="9767d-1752">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="9767d-1752">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="9767d-1753">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1753">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="9767d-1754">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="9767d-1754">support slot swap with preview</span></span>
* <span data-ttu-id="9767d-1755">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1755">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="9767d-1756">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1756">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9767d-1757">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9767d-1757">CosmosDB</span></span>

* <span data-ttu-id="9767d-1758">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="9767d-1758">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="9767d-1759">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="9767d-1759">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="9767d-1760">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="9767d-1760">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="9767d-1761">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="9767d-1761">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="9767d-1762">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="9767d-1762">Data Lake Analytics</span></span>

* <span data-ttu-id="9767d-1763">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="9767d-1763">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="9767d-1764">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="9767d-1764">Add support for new catalog item type: package.</span></span> <span data-ttu-id="9767d-1765">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1765">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="9767d-1766">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="9767d-1766">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="9767d-1767">Таблица</span><span class="sxs-lookup"><span data-stu-id="9767d-1767">Table</span></span>
  * <span data-ttu-id="9767d-1768">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="9767d-1768">Table valued function</span></span>
  * <span data-ttu-id="9767d-1769">Просмотр</span><span class="sxs-lookup"><span data-stu-id="9767d-1769">View</span></span>
  * <span data-ttu-id="9767d-1770">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="9767d-1770">Table Statistics.</span></span> <span data-ttu-id="9767d-1771">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="9767d-1771">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="9767d-1772">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9767d-1772">Data Lake Store</span></span>

* <span data-ttu-id="9767d-1773">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="9767d-1773">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="9767d-1774">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1774">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="9767d-1775">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="9767d-1775">missed help for access show.</span></span> <span data-ttu-id="9767d-1776">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="9767d-1776">adding it.</span></span> <span data-ttu-id="9767d-1777">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="9767d-1777">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="9767d-1778">Поиск</span><span class="sxs-lookup"><span data-stu-id="9767d-1778">Find</span></span>

* <span data-ttu-id="9767d-1779">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="9767d-1779">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="9767d-1780">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="9767d-1780">KeyVault</span></span>

* <span data-ttu-id="9767d-1781">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="9767d-1781">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="9767d-1782">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="9767d-1782">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="9767d-1783">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="9767d-1783">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="9767d-1784">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="9767d-1784">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="9767d-1785">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1785">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="9767d-1786">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="9767d-1786">Lab</span></span>

* <span data-ttu-id="9767d-1787">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="9767d-1787">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="9767d-1788">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="9767d-1788">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="9767d-1789">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="9767d-1789">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="9767d-1790">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="9767d-1790">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="9767d-1791">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="9767d-1791">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="9767d-1792">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="9767d-1792">Monitor</span></span>

* <span data-ttu-id="9767d-1793">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1793">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="9767d-1794">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1794">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="9767d-1795">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-1795">Network</span></span>

* <span data-ttu-id="9767d-1796">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1796">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="9767d-1797">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1797">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="9767d-1798">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="9767d-1798">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="9767d-1799">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="9767d-1799">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="9767d-1800">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="9767d-1800">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="9767d-1801">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="9767d-1801">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="9767d-1802">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="9767d-1802">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="9767d-1803">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="9767d-1803">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="9767d-1804">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1804">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="9767d-1805">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="9767d-1805">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="9767d-1806">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1806">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="9767d-1807">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1807">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="9767d-1808">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="9767d-1808">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="9767d-1809">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="9767d-1809">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="9767d-1810">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="9767d-1810">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="9767d-1811">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="9767d-1811">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="9767d-1812">Профиль</span><span class="sxs-lookup"><span data-stu-id="9767d-1812">Profile</span></span>

* <span data-ttu-id="9767d-1813">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1813">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="9767d-1814">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1814">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="9767d-1815">Redis</span><span class="sxs-lookup"><span data-stu-id="9767d-1815">Redis</span></span>

* <span data-ttu-id="9767d-1816">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="9767d-1816">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="9767d-1817">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="9767d-1817">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="9767d-1818">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9767d-1818">Resource</span></span>

* <span data-ttu-id="9767d-1819">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1819">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="9767d-1820">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1820">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="9767d-1821">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1821">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="9767d-1822">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="9767d-1822">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="9767d-1823">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="9767d-1823">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="9767d-1824">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="9767d-1824">Add docs for az lock update.</span></span> <span data-ttu-id="9767d-1825">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="9767d-1825">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="9767d-1826">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="9767d-1826">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="9767d-1827">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="9767d-1827">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="9767d-1828">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="9767d-1828">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="9767d-1829">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="9767d-1829">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="9767d-1830">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1830">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="9767d-1831">Роль</span><span class="sxs-lookup"><span data-stu-id="9767d-1831">Role</span></span>

* <span data-ttu-id="9767d-1832">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1832">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="9767d-1833">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1833">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="9767d-1834">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1834">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="9767d-1835">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="9767d-1835">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="9767d-1836">SQL</span><span class="sxs-lookup"><span data-stu-id="9767d-1836">SQL</span></span>

* <span data-ttu-id="9767d-1837">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="9767d-1837">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="9767d-1838">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1838">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="9767d-1839">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-1839">Storage</span></span>

* <span data-ttu-id="9767d-1840">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1840">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="9767d-1841">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="9767d-1841">Add support for incremental blob copy</span></span>
* <span data-ttu-id="9767d-1842">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="9767d-1842">Add support for large block blob upload</span></span>
* <span data-ttu-id="9767d-1843">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="9767d-1843">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-1844">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-1844">VM</span></span>

* <span data-ttu-id="9767d-1845">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="9767d-1845">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="9767d-1846">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="9767d-1846">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="9767d-1847">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="9767d-1847">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="9767d-1848">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="9767d-1848">az vm/vmss disk</span></span>
  3. <span data-ttu-id="9767d-1849">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="9767d-1849">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="9767d-1850">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="9767d-1850">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="9767d-1851">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1851">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="9767d-1852">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-1852">April 3, 2017</span></span>

<span data-ttu-id="9767d-1853">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="9767d-1853">Version 2.0.2</span></span>

<span data-ttu-id="9767d-1854">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="9767d-1854">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="9767d-1855">Core</span><span class="sxs-lookup"><span data-stu-id="9767d-1855">Core</span></span>

* <span data-ttu-id="9767d-1856">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9767d-1856">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="9767d-1857">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1857">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="9767d-1858">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1858">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="9767d-1859">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1859">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="9767d-1860">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1860">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="9767d-1861">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="9767d-1861">Add prompting for missing template parameters.</span></span> <span data-ttu-id="9767d-1862">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1862">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="9767d-1863">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9767d-1863">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="9767d-1864">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="9767d-1864">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="9767d-1865">ACS</span><span class="sxs-lookup"><span data-stu-id="9767d-1865">ACS</span></span>

* <span data-ttu-id="9767d-1866">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1866">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="9767d-1867">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="9767d-1867">Add support for ssh key password prompting.</span></span> <span data-ttu-id="9767d-1868">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1868">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="9767d-1869">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="9767d-1869">Add support for windows clusters.</span></span> <span data-ttu-id="9767d-1870">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1870">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="9767d-1871">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="9767d-1871">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="9767d-1872">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1872">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="9767d-1873">AppService</span><span class="sxs-lookup"><span data-stu-id="9767d-1873">AppService</span></span>

* <span data-ttu-id="9767d-1874">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1874">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="9767d-1875">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1875">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="9767d-1876">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1876">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="9767d-1877">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1877">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="9767d-1878">Data Lake</span><span class="sxs-lookup"><span data-stu-id="9767d-1878">DataLake</span></span>

* <span data-ttu-id="9767d-1879">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="9767d-1879">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="9767d-1880">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="9767d-1880">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="9767d-1881">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="9767d-1881">DocuemntDB</span></span>

* <span data-ttu-id="9767d-1882">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1882">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="9767d-1883">ВМ</span><span class="sxs-lookup"><span data-stu-id="9767d-1883">VM</span></span>

* <span data-ttu-id="9767d-1884">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1884">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="9767d-1885">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1885">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="9767d-1886">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1886">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="9767d-1887">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1887">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="9767d-1888">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1888">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="9767d-1889">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1889">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="9767d-1890">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="9767d-1890">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="9767d-1891">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="9767d-1891">February 27, 2017</span></span>

<span data-ttu-id="9767d-1892">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="9767d-1892">Version 2.0.0</span></span>

<span data-ttu-id="9767d-1893">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="9767d-1893">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="9767d-1894">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="9767d-1894">Container Service (acs)</span></span>
- <span data-ttu-id="9767d-1895">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="9767d-1895">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="9767d-1896">Сеть</span><span class="sxs-lookup"><span data-stu-id="9767d-1896">Networking</span></span>
- <span data-ttu-id="9767d-1897">Хранилище</span><span class="sxs-lookup"><span data-stu-id="9767d-1897">Storage</span></span>

<span data-ttu-id="9767d-1898">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1898">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="9767d-1899">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="9767d-1899">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="9767d-1900">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="9767d-1900">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="9767d-1901">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="9767d-1901">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="9767d-1902">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="9767d-1902">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="9767d-1903">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="9767d-1903">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="9767d-1904">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="9767d-1904">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="9767d-1905">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="9767d-1905">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="9767d-1906">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="9767d-1906">Provide feedback from the command line with the `az feedback` command</span></span>

