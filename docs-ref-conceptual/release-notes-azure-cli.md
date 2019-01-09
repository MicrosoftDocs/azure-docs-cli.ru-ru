---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 12/18/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 10663ad8e85a15b8fedb5ac12c5d17256d07e523
ms.sourcegitcommit: 614811ea63ceb0e71bd99323846dc1b754e15255
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/28/2018
ms.locfileid: "53805964"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="bd590-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="bd590-103">Azure CLI release notes</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="bd590-104">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-104">December 20, 2018</span></span>

<span data-ttu-id="bd590-105">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="bd590-105">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="bd590-106">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-106">Appservice</span></span>
* <span data-ttu-id="bd590-107">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="bd590-107">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="bd590-108">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="bd590-108">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="bd590-109">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="bd590-109">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="bd590-110">IoT Central</span><span class="sxs-lookup"><span data-stu-id="bd590-110">IoTCentral</span></span>
* <span data-ttu-id="bd590-111">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="bd590-111">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="bd590-112">Роль</span><span class="sxs-lookup"><span data-stu-id="bd590-112">Role</span></span>
* <span data-ttu-id="bd590-113">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="bd590-113">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="bd590-114">SQL</span><span class="sxs-lookup"><span data-stu-id="bd590-114">SQL</span></span>
* <span data-ttu-id="bd590-115">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="bd590-115">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-116">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-116">VM</span></span>
* <span data-ttu-id="bd590-117">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-117">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="bd590-118">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-118">December 18, 2018</span></span>

<span data-ttu-id="bd590-119">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="bd590-119">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="bd590-120">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-120">ACR</span></span>
* <span data-ttu-id="bd590-121">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bd590-121">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="bd590-122">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="bd590-122">Condensed the table layout for task list</span></span>
* <span data-ttu-id="bd590-123">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="bd590-123">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-124">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-124">ACS</span></span>
* <span data-ttu-id="bd590-125">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="bd590-125">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="bd590-126">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="bd590-126">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="bd590-127">[УСТАРЕЛО] Команды `az acs` объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="bd590-127">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="bd590-128">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-128">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="bd590-129">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="bd590-129">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="bd590-130">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="bd590-130">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-131">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-131">Appservice</span></span>
* <span data-ttu-id="bd590-132">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="bd590-132">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="bd590-133">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="bd590-133">Botservice</span></span>
* <span data-ttu-id="bd590-134">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="bd590-134">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="bd590-135">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="bd590-135">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="bd590-136">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="bd590-136">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="bd590-137">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="bd590-137">Reduced Kudu network calls</span></span>
* <span data-ttu-id="bd590-138">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="bd590-138">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="bd590-139">Потребление</span><span class="sxs-lookup"><span data-stu-id="bd590-139">Consumption</span></span>
* <span data-ttu-id="bd590-140">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="bd590-140">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bd590-141">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="bd590-141">CosmosDB</span></span>
* <span data-ttu-id="bd590-142">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="bd590-142">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="bd590-143">Карты</span><span class="sxs-lookup"><span data-stu-id="bd590-143">Maps</span></span>
* <span data-ttu-id="bd590-144">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="bd590-144">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="bd590-145">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-145">Network</span></span>
* <span data-ttu-id="bd590-146">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="bd590-146">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="bd590-147">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="bd590-147">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="bd590-148">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bd590-148">Resource</span></span>
* <span data-ttu-id="bd590-149">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-149">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="bd590-150">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="bd590-150">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-151">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-151">Storage</span></span>
*  <span data-ttu-id="bd590-152">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="bd590-152">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-153">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-153">VM</span></span>
* <span data-ttu-id="bd590-154">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="bd590-154">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="bd590-155">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-155">December 4, 2018</span></span>

<span data-ttu-id="bd590-156">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="bd590-156">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="bd590-157">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-157">Core</span></span>
* <span data-ttu-id="bd590-158">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="bd590-158">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="bd590-159">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="bd590-159">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-160">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-160">Appservice</span></span>
* <span data-ttu-id="bd590-161">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="bd590-161">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="bd590-162">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="bd590-162">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="bd590-163">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-163">Network</span></span>
* <span data-ttu-id="bd590-164">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="bd590-164">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="bd590-165">Роль</span><span class="sxs-lookup"><span data-stu-id="bd590-165">Role</span></span>
* <span data-ttu-id="bd590-166">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="bd590-166">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="bd590-167">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-167">VM</span></span>
* <span data-ttu-id="bd590-168">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` устарел.</span><span class="sxs-lookup"><span data-stu-id="bd590-168">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="bd590-169">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="bd590-169">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="bd590-170">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="bd590-170">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="bd590-171">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="bd590-171">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="bd590-172">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-172">November 20, 2018</span></span>

<span data-ttu-id="bd590-173">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="bd590-173">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="bd590-174">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-174">Core</span></span>
* <span data-ttu-id="bd590-175">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="bd590-175">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="bd590-176">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-176">ACR</span></span>
* <span data-ttu-id="bd590-177">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="bd590-177">Added context token to task step</span></span>
* <span data-ttu-id="bd590-178">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="bd590-178">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="bd590-179">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="bd590-179">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-180">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-180">Appservice</span></span>
* <span data-ttu-id="bd590-181">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="bd590-181">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="bd590-182">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bd590-182">Updated the default `node_version`.</span></span> <span data-ttu-id="bd590-183">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="bd590-183">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="bd590-184">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="bd590-184">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="bd590-185">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="bd590-185">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="bd590-186">IotCentral</span><span class="sxs-lookup"><span data-stu-id="bd590-186">IotCentral</span></span>
* <span data-ttu-id="bd590-187">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="bd590-187">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="bd590-188">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bd590-188">KeyVault</span></span>
* <span data-ttu-id="bd590-189">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="bd590-189">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="bd590-190">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-190">Network</span></span>
* <span data-ttu-id="bd590-191">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="bd590-191">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="bd590-192">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="bd590-192">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="bd590-193">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="bd590-193">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="bd590-194">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="bd590-194">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="bd590-195">Rdbms</span><span class="sxs-lookup"><span data-stu-id="bd590-195">Rdbms</span></span>
* <span data-ttu-id="bd590-196">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="bd590-196">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="bd590-197">RBAC:</span><span class="sxs-lookup"><span data-stu-id="bd590-197">Rbac</span></span>
* <span data-ttu-id="bd590-198">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-198">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="bd590-199">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="bd590-199">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="bd590-200">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-200">Storage</span></span>
* <span data-ttu-id="bd590-201">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="bd590-201">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="bd590-202">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="bd590-202">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="bd590-203">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="bd590-203">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="bd590-204">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="bd590-204">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-205">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-205">VM</span></span>
* <span data-ttu-id="bd590-206">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="bd590-206">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="bd590-207">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="bd590-207">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="bd590-208">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="bd590-208">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="bd590-209">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="bd590-209">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="bd590-210">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-210">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="bd590-211">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="bd590-211">Added `snapshot wait` command</span></span>
* <span data-ttu-id="bd590-212">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="bd590-212">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="bd590-213">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-213">November 6, 2018</span></span>

<span data-ttu-id="bd590-214">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="bd590-214">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="bd590-215">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-215">Core</span></span>
* <span data-ttu-id="bd590-216">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="bd590-216">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="bd590-217">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-217">ACR</span></span>
* <span data-ttu-id="bd590-218">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="bd590-218">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="bd590-219">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="bd590-219">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-220">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-220">ACS</span></span>
* <span data-ttu-id="bd590-221">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bd590-221">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="bd590-222">Помощник</span><span class="sxs-lookup"><span data-stu-id="bd590-222">Advisor</span></span>
* <span data-ttu-id="bd590-223">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="bd590-223">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="bd590-224">AMS</span><span class="sxs-lookup"><span data-stu-id="bd590-224">AMS</span></span>
* <span data-ttu-id="bd590-225">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="bd590-225">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="bd590-226">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="bd590-226">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="bd590-227">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-227">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="bd590-228">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="bd590-228">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="bd590-229">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="bd590-229">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="bd590-230">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="bd590-230">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="bd590-231">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="bd590-231">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="bd590-232">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="bd590-232">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="bd590-233">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="bd590-233">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="bd590-234">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="bd590-234">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="bd590-235">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="bd590-235">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="bd590-236">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="bd590-236">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="bd590-237">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="bd590-237">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="bd590-238">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="bd590-238">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="bd590-239">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="bd590-239">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="bd590-240">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="bd590-240">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="bd590-241">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="bd590-241">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-242">AppService</span><span class="sxs-lookup"><span data-stu-id="bd590-242">AppService</span></span>
* <span data-ttu-id="bd590-243">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="bd590-243">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="bd590-244">Настройка</span><span class="sxs-lookup"><span data-stu-id="bd590-244">Configure</span></span>
* <span data-ttu-id="bd590-245">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="bd590-245">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="bd590-246">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bd590-246">Container</span></span>
* <span data-ttu-id="bd590-247">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="bd590-247">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="bd590-248">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="bd590-248">EventHub</span></span>
* <span data-ttu-id="bd590-249">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-249">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="bd590-250">Interactive</span><span class="sxs-lookup"><span data-stu-id="bd590-250">Interactive</span></span>
* <span data-ttu-id="bd590-251">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="bd590-251">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="bd590-252">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bd590-252">Monitor</span></span>
* <span data-ttu-id="bd590-253">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-253">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="bd590-254">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-254">Network</span></span>
* <span data-ttu-id="bd590-255">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="bd590-255">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="bd590-256">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="bd590-256">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="bd590-257">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-257">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="bd590-258">Профиль</span><span class="sxs-lookup"><span data-stu-id="bd590-258">Profile</span></span>
* <span data-ttu-id="bd590-259">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="bd590-259">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="bd590-260">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="bd590-260">RDBMS</span></span>
* <span data-ttu-id="bd590-261">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="bd590-261">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="bd590-262">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bd590-262">Resource</span></span>
* <span data-ttu-id="bd590-263">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="bd590-263">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="bd590-264">Роль</span><span class="sxs-lookup"><span data-stu-id="bd590-264">Role</span></span>
* <span data-ttu-id="bd590-265">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="bd590-265">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="bd590-266">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="bd590-266">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="bd590-267">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="bd590-267">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-268">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-268">Storage</span></span>
* <span data-ttu-id="bd590-269">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="bd590-269">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-270">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-270">VM</span></span>
* <span data-ttu-id="bd590-271">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="bd590-271">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="bd590-272">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="bd590-272">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="bd590-273">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="bd590-273">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="bd590-274">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="bd590-274">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="bd590-275">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="bd590-275">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="bd590-276">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="bd590-276">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="bd590-277">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-277">October 23, 2018</span></span>

<span data-ttu-id="bd590-278">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="bd590-278">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="bd590-279">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-279">Core</span></span>
* <span data-ttu-id="bd590-280">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="bd590-280">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="bd590-281">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="bd590-281">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="bd590-282">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-282">ACR</span></span>
* <span data-ttu-id="bd590-283">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="bd590-283">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="bd590-284">CDN</span><span class="sxs-lookup"><span data-stu-id="bd590-284">CDN</span></span>
* <span data-ttu-id="bd590-285">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bd590-285">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="bd590-286">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="bd590-286">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="bd590-287">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bd590-287">Container</span></span>
* <span data-ttu-id="bd590-288">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="bd590-288">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="bd590-289">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="bd590-289">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="bd590-290">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bd590-290">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="bd590-291">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bd590-291">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="bd590-292">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="bd590-292">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="bd590-293">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="bd590-293">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="bd590-294">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="bd590-294">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bd590-295">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="bd590-295">CosmosDB</span></span>
* <span data-ttu-id="bd590-296">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="bd590-296">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="bd590-297">Interactive</span><span class="sxs-lookup"><span data-stu-id="bd590-297">Interactive</span></span>
* <span data-ttu-id="bd590-298">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="bd590-298">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="bd590-299">IoT Central</span><span class="sxs-lookup"><span data-stu-id="bd590-299">IoT Central</span></span>
* <span data-ttu-id="bd590-300">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="bd590-300">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="bd590-301">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="bd590-301">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="bd590-302">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bd590-302">Monitor</span></span>
* <span data-ttu-id="bd590-303">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="bd590-303">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="bd590-304">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="bd590-304">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="bd590-305">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="bd590-305">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="bd590-306">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="bd590-306">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="bd590-307">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="bd590-307">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="bd590-308">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="bd590-308">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="bd590-309">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="bd590-309">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="bd590-310">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="bd590-310">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="bd590-311">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="bd590-311">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="bd590-312">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-312">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="bd590-313">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-313">Network</span></span>
* <span data-ttu-id="bd590-314">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="bd590-314">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="bd590-315">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="bd590-315">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="bd590-316">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="bd590-316">ServiceBus</span></span>
* <span data-ttu-id="bd590-317">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="bd590-317">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="bd590-318">SQL</span><span class="sxs-lookup"><span data-stu-id="bd590-318">SQL</span></span>
* <span data-ttu-id="bd590-319">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="bd590-319">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-320">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-320">Storage</span></span>
* <span data-ttu-id="bd590-321">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="bd590-321">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="bd590-322">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="bd590-322">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-323">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-323">VM</span></span>
* <span data-ttu-id="bd590-324">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="bd590-324">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="bd590-325">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="bd590-325">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="bd590-326">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="bd590-326">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="bd590-327">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-327">October 16, 2018</span></span>

<span data-ttu-id="bd590-328">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="bd590-328">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-329">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-329">VM</span></span>
* <span data-ttu-id="bd590-330">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="bd590-330">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="bd590-331">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-331">October 9, 2018</span></span>

<span data-ttu-id="bd590-332">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="bd590-332">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="bd590-333">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-333">Core</span></span>
* <span data-ttu-id="bd590-334">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="bd590-334">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="bd590-335">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-335">ACR</span></span>
* <span data-ttu-id="bd590-336">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="bd590-336">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-337">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-337">ACS</span></span>
* <span data-ttu-id="bd590-338">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="bd590-338">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="bd590-339">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="bd590-339">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="bd590-340">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="bd590-340">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="bd590-341">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="bd590-341">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="bd590-342">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bd590-342">Container</span></span>
* <span data-ttu-id="bd590-343">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="bd590-343">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="bd590-344">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="bd590-344">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="bd590-345">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="bd590-345">Event Hub</span></span>
* <span data-ttu-id="bd590-346">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-346">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="bd590-347">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="bd590-347">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="bd590-348">расширения.</span><span class="sxs-lookup"><span data-stu-id="bd590-348">Extensions</span></span>
* <span data-ttu-id="bd590-349">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="bd590-349">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="bd590-350">HDInsight</span><span class="sxs-lookup"><span data-stu-id="bd590-350">HDInsight</span></span>
* <span data-ttu-id="bd590-351">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="bd590-351">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="bd590-352">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bd590-352">IoT</span></span>
* <span data-ttu-id="bd590-353">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="bd590-353">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="bd590-354">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bd590-354">KeyVault</span></span>
* <span data-ttu-id="bd590-355">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="bd590-355">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="bd590-356">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-356">Network</span></span>
* <span data-ttu-id="bd590-357">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bd590-357">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="bd590-358">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="bd590-358">See #6052</span></span>
* <span data-ttu-id="bd590-359">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-359">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="bd590-360">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="bd590-360">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="bd590-361">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="bd590-361">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="bd590-362">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="bd590-362">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="bd590-363">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="bd590-363">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="bd590-364">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-364">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="bd590-365">Роль</span><span class="sxs-lookup"><span data-stu-id="bd590-365">Role</span></span>
* <span data-ttu-id="bd590-366">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="bd590-366">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="bd590-367">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="bd590-367">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="bd590-368">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="bd590-368">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="bd590-369">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="bd590-369">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="bd590-370">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="bd590-370">Service Bus</span></span>
* <span data-ttu-id="bd590-371">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="bd590-371">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-372">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-372">VM</span></span>
* <span data-ttu-id="bd590-373">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="bd590-373">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="bd590-374">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="bd590-374">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="bd590-375">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="bd590-375">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="bd590-376">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="bd590-376">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="bd590-377">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="bd590-377">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="bd590-378">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="bd590-378">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="bd590-379">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-379">September 21, 2018</span></span>

<span data-ttu-id="bd590-380">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="bd590-380">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="bd590-381">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-381">ACR</span></span>
* <span data-ttu-id="bd590-382">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="bd590-382">Added ACR Task commands</span></span>
* <span data-ttu-id="bd590-383">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="bd590-383">Added quick run command</span></span>
* <span data-ttu-id="bd590-384">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="bd590-384">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="bd590-385">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="bd590-385">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="bd590-386">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="bd590-386">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="bd590-387">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="bd590-387">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-388">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-388">ACS</span></span>
* <span data-ttu-id="bd590-389">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="bd590-389">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="bd590-390">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="bd590-390">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-391">AppService</span><span class="sxs-lookup"><span data-stu-id="bd590-391">AppService</span></span>

* <span data-ttu-id="bd590-392">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="bd590-392">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="bd590-393">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="bd590-393">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="bd590-394">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="bd590-394">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="bd590-395">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="bd590-395">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="bd590-396">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bd590-396">Batch</span></span>
* <span data-ttu-id="bd590-397">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="bd590-397">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="bd590-398">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="bd590-398">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="bd590-399">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-399">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="bd590-400">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="bd590-400">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="bd590-401">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="bd590-401">Batch AI</span></span> 
* <span data-ttu-id="bd590-402">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-402">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="bd590-403">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="bd590-403">Cognitive Services</span></span>
* <span data-ttu-id="bd590-404">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="bd590-404">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="bd590-405">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="bd590-405">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="bd590-406">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="bd590-406">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="bd590-407">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="bd590-407">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="bd590-408">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="bd590-408">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="bd590-409">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="bd590-409">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="bd590-410">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bd590-410">Container</span></span>
* <span data-ttu-id="bd590-411">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bd590-411">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="bd590-412">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="bd590-412">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="bd590-413">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="bd590-413">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="bd590-414">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bd590-414">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="bd590-415">Data Lake</span><span class="sxs-lookup"><span data-stu-id="bd590-415">Datalake</span></span>
* <span data-ttu-id="bd590-416">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="bd590-416">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="bd590-417">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="bd590-417">Interactive Shell</span></span>
* <span data-ttu-id="bd590-418">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="bd590-418">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="bd590-419">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="bd590-419">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="bd590-420">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bd590-420">IoT</span></span>
* <span data-ttu-id="bd590-421">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="bd590-421">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="bd590-422">Key Vault</span><span class="sxs-lookup"><span data-stu-id="bd590-422">Key Vault</span></span>
* <span data-ttu-id="bd590-423">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="bd590-423">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="bd590-424">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-424">Network</span></span>
* <span data-ttu-id="bd590-425">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="bd590-425">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="bd590-426">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="bd590-426">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="bd590-427">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="bd590-427">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="bd590-428">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="bd590-428">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="bd590-429">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-429">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="bd590-430">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-430">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="bd590-431">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="bd590-431">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="bd590-432">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="bd590-432">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="bd590-433">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="bd590-433">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="bd590-434">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="bd590-434">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="bd590-435">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="bd590-435">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="bd590-436">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="bd590-436">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="bd590-437">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="bd590-437">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="bd590-438">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="bd590-438">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="bd590-439">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="bd590-439">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="bd590-440">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="bd590-440">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="bd590-441">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="bd590-441">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="bd590-442">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="bd590-442">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="bd590-443">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="bd590-443">RDBMS</span></span>
* <span data-ttu-id="bd590-444">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="bd590-444">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="bd590-445">резервирование.</span><span class="sxs-lookup"><span data-stu-id="bd590-445">Reservation</span></span>
* <span data-ttu-id="bd590-446">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bd590-446">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="bd590-447">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="bd590-447">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="bd590-448">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="bd590-448">Manage App</span></span>
* <span data-ttu-id="bd590-449">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="bd590-449">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="bd590-450">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="bd590-450">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="bd590-451">Роль</span><span class="sxs-lookup"><span data-stu-id="bd590-451">Role</span></span>
* <span data-ttu-id="bd590-452">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="bd590-452">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="bd590-453">SignalR</span><span class="sxs-lookup"><span data-stu-id="bd590-453">SignalR</span></span>
* <span data-ttu-id="bd590-454">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="bd590-454">First release</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-455">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-455">Storage</span></span>
* <span data-ttu-id="bd590-456">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="bd590-456">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="bd590-457">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="bd590-457">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-458">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-458">VM</span></span>
* <span data-ttu-id="bd590-459">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="bd590-459">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="bd590-460">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="bd590-460">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="bd590-461">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-461">August 28, 2018</span></span>

<span data-ttu-id="bd590-462">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="bd590-462">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="bd590-463">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-463">Core</span></span>

* <span data-ttu-id="bd590-464">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="bd590-464">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="bd590-465">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="bd590-465">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="bd590-466">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-466">ACR</span></span>

* <span data-ttu-id="bd590-467">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="bd590-467">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="bd590-468">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="bd590-468">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-469">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-469">ACS</span></span>

* <span data-ttu-id="bd590-470">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="bd590-470">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="bd590-471">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="bd590-471">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-472">AppService</span><span class="sxs-lookup"><span data-stu-id="bd590-472">AppService</span></span>

* <span data-ttu-id="bd590-473">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="bd590-473">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="bd590-474">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="bd590-474">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="bd590-475">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="bd590-475">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="bd590-476">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="bd590-476">Backup</span></span>

* <span data-ttu-id="bd590-477">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="bd590-477">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="bd590-478">Служба Bot Service</span><span class="sxs-lookup"><span data-stu-id="bd590-478">Bot Service</span></span>

* <span data-ttu-id="bd590-479">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="bd590-479">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="bd590-480">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="bd590-480">Cognitive Services</span></span>

* <span data-ttu-id="bd590-481">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="bd590-481">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="bd590-482">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bd590-482">IoT</span></span>

* <span data-ttu-id="bd590-483">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="bd590-483">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="bd590-484">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bd590-484">Monitor</span></span>

* <span data-ttu-id="bd590-485">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="bd590-485">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="bd590-486">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="bd590-486">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="bd590-487">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-487">Network</span></span>

* <span data-ttu-id="bd590-488">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="bd590-488">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="bd590-489">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bd590-489">Resource</span></span>

* <span data-ttu-id="bd590-490">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="bd590-490">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-491">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-491">Storage</span></span>

* <span data-ttu-id="bd590-492">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="bd590-492">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-493">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-493">VM</span></span>

* <span data-ttu-id="bd590-494">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="bd590-494">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="bd590-495">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-495">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="bd590-496">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-496">Auguest 14, 2018</span></span>

<span data-ttu-id="bd590-497">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="bd590-497">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="bd590-498">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-498">Core</span></span>

* <span data-ttu-id="bd590-499">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="bd590-499">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="bd590-500">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="bd590-500">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="bd590-501">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="bd590-501">Telemetry</span></span>

* <span data-ttu-id="bd590-502">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="bd590-502">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="bd590-503">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-503">ACR</span></span>

* <span data-ttu-id="bd590-504">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="bd590-504">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="bd590-505">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="bd590-505">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-506">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-506">ACS</span></span>

* <span data-ttu-id="bd590-507">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="bd590-507">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="bd590-508">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="bd590-508">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="bd590-509">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="bd590-509">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="bd590-510">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="bd590-510">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="bd590-511">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="bd590-511">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="bd590-512">AppService</span><span class="sxs-lookup"><span data-stu-id="bd590-512">AppService</span></span>

* <span data-ttu-id="bd590-513">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bd590-513">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="bd590-514">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="bd590-514">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="bd590-515">Batch AI</span><span class="sxs-lookup"><span data-stu-id="bd590-515">BatchAI</span></span>

* <span data-ttu-id="bd590-516">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="bd590-516">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="bd590-517">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bd590-517">Container</span></span>

* <span data-ttu-id="bd590-518">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="bd590-518">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="bd590-519">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bd590-519">IoT</span></span>

* <span data-ttu-id="bd590-520">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="bd590-520">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="bd590-521">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="bd590-521">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="bd590-522">IoT Central</span><span class="sxs-lookup"><span data-stu-id="bd590-522">Iot Central</span></span>

* <span data-ttu-id="bd590-523">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="bd590-523">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="bd590-524">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bd590-524">KeyVault</span></span>


* <span data-ttu-id="bd590-525">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="bd590-525">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="bd590-526">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="bd590-526">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="bd590-527">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="bd590-527">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="bd590-528">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="bd590-528">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="bd590-529">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="bd590-529">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="bd590-530">Передача</span><span class="sxs-lookup"><span data-stu-id="bd590-530">Relay</span></span>

* <span data-ttu-id="bd590-531">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="bd590-531">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="bd590-532">SQL</span><span class="sxs-lookup"><span data-stu-id="bd590-532">Sql</span></span>

* <span data-ttu-id="bd590-533">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="bd590-533">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-534">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-534">Storage</span></span>

* <span data-ttu-id="bd590-535">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="bd590-535">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="bd590-536">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="bd590-536">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="bd590-537">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="bd590-537">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="bd590-538">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="bd590-538">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="bd590-539">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="bd590-539">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-540">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-540">VM</span></span>

* <span data-ttu-id="bd590-541">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="bd590-541">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="bd590-542">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-542">July 31, 2018</span></span>

<span data-ttu-id="bd590-543">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="bd590-543">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="bd590-544">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-544">ACR</span></span>

* <span data-ttu-id="bd590-545">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="bd590-545">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="bd590-546">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="bd590-546">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-547">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-547">ACS</span></span>

* <span data-ttu-id="bd590-548">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="bd590-548">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="bd590-549">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bd590-549">Batch</span></span>

* <span data-ttu-id="bd590-550">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="bd590-550">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="bd590-551">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bd590-551">Container</span></span>

* <span data-ttu-id="bd590-552">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="bd590-552">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="bd590-553">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-553">Network</span></span>

* <span data-ttu-id="bd590-554">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="bd590-554">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="bd590-555">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bd590-555">Resource</span></span>

* <span data-ttu-id="bd590-556">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="bd590-556">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="bd590-557">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="bd590-557">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="bd590-558">Роль</span><span class="sxs-lookup"><span data-stu-id="bd590-558">Role</span></span>

* <span data-ttu-id="bd590-559">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="bd590-559">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="bd590-560">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="bd590-560">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="bd590-561">поиска</span><span class="sxs-lookup"><span data-stu-id="bd590-561">Search</span></span>

* <span data-ttu-id="bd590-562">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="bd590-562">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="bd590-563">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="bd590-563">Service Bus</span></span>

* <span data-ttu-id="bd590-564">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="bd590-564">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="bd590-565">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="bd590-565">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="bd590-566">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="bd590-566">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="bd590-567">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="bd590-567">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-568">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-568">Storage</span></span>

* <span data-ttu-id="bd590-569">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="bd590-569">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="bd590-570">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="bd590-570">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-571">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-571">VM</span></span>

* <span data-ttu-id="bd590-572">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="bd590-572">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="bd590-573">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="bd590-573">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="bd590-574">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="bd590-574">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="bd590-575">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="bd590-575">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="bd590-576">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-576">July 18, 2018</span></span>

<span data-ttu-id="bd590-577">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="bd590-577">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="bd590-578">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-578">Core</span></span>

* <span data-ttu-id="bd590-579">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="bd590-579">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="bd590-580">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="bd590-580">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="bd590-581">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="bd590-581">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="bd590-582">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-582">ACR</span></span>

* <span data-ttu-id="bd590-583">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="bd590-583">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="bd590-584">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-584">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="bd590-585">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="bd590-585">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="bd590-586">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="bd590-586">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-587">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-587">ACS</span></span>

* <span data-ttu-id="bd590-588">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="bd590-588">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-589">AppService</span><span class="sxs-lookup"><span data-stu-id="bd590-589">AppService</span></span>

* <span data-ttu-id="bd590-590">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="bd590-590">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="bd590-591">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bd590-591">Batch</span></span>

* <span data-ttu-id="bd590-592">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="bd590-592">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="bd590-593">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="bd590-593">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="bd590-594">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="bd590-594">Batch AI</span></span>

* <span data-ttu-id="bd590-595">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="bd590-595">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="bd590-596">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bd590-596">Container</span></span>

* <span data-ttu-id="bd590-597">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="bd590-597">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="bd590-598">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="bd590-598">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="bd590-599">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-599">Network</span></span>

* <span data-ttu-id="bd590-600">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="bd590-600">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="bd590-601">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="bd590-601">Added `network nic wait`</span></span>
* <span data-ttu-id="bd590-602">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="bd590-602">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="bd590-603">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="bd590-603">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="bd590-604">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bd590-604">Resource</span></span>

* <span data-ttu-id="bd590-605">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="bd590-605">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="bd590-606">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="bd590-606">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="bd590-607">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="bd590-607">Added `deployment wait` command</span></span>
* <span data-ttu-id="bd590-608">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="bd590-608">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="bd590-609">SQL</span><span class="sxs-lookup"><span data-stu-id="bd590-609">SQL</span></span>

* <span data-ttu-id="bd590-610">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-610">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="bd590-611">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="bd590-611">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="bd590-612">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="bd590-612">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-613">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-613">Storage</span></span>

* <span data-ttu-id="bd590-614">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="bd590-614">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-615">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-615">VM</span></span>

* <span data-ttu-id="bd590-616">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bd590-616">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="bd590-617">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-617">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="bd590-618">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="bd590-618">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="bd590-619">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-619">July 3, 2018</span></span>

<span data-ttu-id="bd590-620">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="bd590-620">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="bd590-621">AKS</span><span class="sxs-lookup"><span data-stu-id="bd590-621">AKS</span></span>

* <span data-ttu-id="bd590-622">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="bd590-622">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="bd590-623">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-623">July 3, 2018</span></span>

<span data-ttu-id="bd590-624">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="bd590-624">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="bd590-625">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-625">Core</span></span>

* <span data-ttu-id="bd590-626">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="bd590-626">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="bd590-627">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-627">ACR</span></span>

* <span data-ttu-id="bd590-628">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="bd590-628">Added polling build status</span></span>
* <span data-ttu-id="bd590-629">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="bd590-629">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="bd590-630">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="bd590-630">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-631">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-631">ACS</span></span>

* <span data-ttu-id="bd590-632">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bd590-632">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="bd590-633">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bd590-633">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="bd590-634">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="bd590-634">Updated options for `aks browse` command.</span></span> <span data-ttu-id="bd590-635">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="bd590-635">Added `--listen-port` support</span></span>
* <span data-ttu-id="bd590-636">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="bd590-636">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="bd590-637">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="bd590-637">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="bd590-638">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="bd590-638">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-639">AppService</span><span class="sxs-lookup"><span data-stu-id="bd590-639">AppService</span></span>

* <span data-ttu-id="bd590-640">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="bd590-640">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="bd590-641">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="bd590-641">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="bd590-642">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="bd590-642">Backup</span></span>

* <span data-ttu-id="bd590-643">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="bd590-643">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="bd590-644">Batch AI</span><span class="sxs-lookup"><span data-stu-id="bd590-644">BatchAI</span></span>

* <span data-ttu-id="bd590-645">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="bd590-645">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="bd590-646">Облако</span><span class="sxs-lookup"><span data-stu-id="bd590-646">Cloud</span></span>

* <span data-ttu-id="bd590-647">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="bd590-647">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="bd590-648">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bd590-648">Container</span></span>

* <span data-ttu-id="bd590-649">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="bd590-649">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="bd590-650">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="bd590-650">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="bd590-651">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="bd590-651">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="bd590-652">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="bd590-652">Extension</span></span>

* <span data-ttu-id="bd590-653">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="bd590-653">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="bd590-654">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-654">Network</span></span>

* <span data-ttu-id="bd590-655">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="bd590-655">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="bd590-656">Rdbms</span><span class="sxs-lookup"><span data-stu-id="bd590-656">Rdbms</span></span>

* <span data-ttu-id="bd590-657">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="bd590-657">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="bd590-658">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bd590-658">Resource</span></span>

* <span data-ttu-id="bd590-659">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="bd590-659">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-660">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-660">VM</span></span>

* <span data-ttu-id="bd590-661">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="bd590-661">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="bd590-662">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-662">June 25, 2018</span></span>

<span data-ttu-id="bd590-663">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="bd590-663">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="bd590-664">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="bd590-664">CLI</span></span>

* <span data-ttu-id="bd590-665">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="bd590-665">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="bd590-666">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-666">June 19, 2018</span></span>

<span data-ttu-id="bd590-667">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="bd590-667">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="bd590-668">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-668">Core</span></span>

* <span data-ttu-id="bd590-669">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="bd590-669">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="bd590-670">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-670">ACR</span></span>

* <span data-ttu-id="bd590-671">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="bd590-671">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="bd590-672">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="bd590-672">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-673">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-673">ACS</span></span>

* <span data-ttu-id="bd590-674">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="bd590-674">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="bd590-675">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-675">Added `--update` support</span></span>
* <span data-ttu-id="bd590-676">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="bd590-676">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="bd590-677">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="bd590-677">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="bd590-678">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="bd590-678">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="bd590-679">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="bd590-679">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="bd590-680">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="bd590-680">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="bd590-681">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="bd590-681">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-682">AppService</span><span class="sxs-lookup"><span data-stu-id="bd590-682">AppService</span></span>

* <span data-ttu-id="bd590-683">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="bd590-683">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="bd590-684">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bd590-684">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="bd590-685">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bd590-685">Batch</span></span>

* <span data-ttu-id="bd590-686">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="bd590-686">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="bd590-687">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="bd590-687">Batch AI</span></span>

* <span data-ttu-id="bd590-688">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="bd590-688">Added support for workspaces.</span></span> <span data-ttu-id="bd590-689">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bd590-689">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="bd590-690">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="bd590-690">Added support for experiments.</span></span> <span data-ttu-id="bd590-691">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="bd590-691">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="bd590-692">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="bd590-692">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="bd590-693">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="bd590-693">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="bd590-694">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="bd590-694">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="bd590-695">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="bd590-695">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="bd590-696">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="bd590-696">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="bd590-697">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="bd590-697">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="bd590-698">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-698">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="bd590-699">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="bd590-699">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="bd590-700">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-700">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="bd590-701">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="bd590-701">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="bd590-702">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="bd590-702">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="bd590-703">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="bd590-703">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="bd590-704">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-704">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="bd590-705">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="bd590-705">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="bd590-706">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="bd590-706">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="bd590-707">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="bd590-707">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="bd590-708">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="bd590-708">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="bd590-709">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="bd590-709">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="bd590-710">Карты</span><span class="sxs-lookup"><span data-stu-id="bd590-710">Maps</span></span>

* <span data-ttu-id="bd590-711">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="bd590-711">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="bd590-712">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-712">Network</span></span>

* <span data-ttu-id="bd590-713">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="bd590-713">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="bd590-714">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="bd590-714">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="bd590-715">#6502</span><span class="sxs-lookup"><span data-stu-id="bd590-715">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="bd590-716">Резервирование</span><span class="sxs-lookup"><span data-stu-id="bd590-716">Reservations</span></span>

* <span data-ttu-id="bd590-717">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="bd590-717">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="bd590-718">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="bd590-718">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="bd590-719">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="bd590-719">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="bd590-720">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="bd590-720">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="bd590-721">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="bd590-721">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="bd590-722">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-722">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="bd590-723">Роль</span><span class="sxs-lookup"><span data-stu-id="bd590-723">Role</span></span>

* <span data-ttu-id="bd590-724">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="bd590-724">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="bd590-725">SQL</span><span class="sxs-lookup"><span data-stu-id="bd590-725">SQL</span></span>

* <span data-ttu-id="bd590-726">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="bd590-726">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-727">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-727">Storage</span></span>

* <span data-ttu-id="bd590-728">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="bd590-728">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-729">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-729">VM</span></span>

* <span data-ttu-id="bd590-730">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-730">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="bd590-731">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="bd590-731">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="bd590-732">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="bd590-732">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="bd590-733">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-733">June 13, 2018</span></span>

<span data-ttu-id="bd590-734">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="bd590-734">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="bd590-735">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-735">Core</span></span>

* <span data-ttu-id="bd590-736">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="bd590-736">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="bd590-737">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-737">June 13, 2018</span></span>

<span data-ttu-id="bd590-738">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="bd590-738">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="bd590-739">AKS</span><span class="sxs-lookup"><span data-stu-id="bd590-739">AKS</span></span>

* <span data-ttu-id="bd590-740">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="bd590-740">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="bd590-741">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="bd590-741">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="bd590-742">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="bd590-742">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="bd590-743">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="bd590-743">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="bd590-744">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bd590-744">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-745">AppService</span><span class="sxs-lookup"><span data-stu-id="bd590-745">AppService</span></span>

* <span data-ttu-id="bd590-746">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="bd590-746">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="bd590-747">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-747">June 5, 2018</span></span>

<span data-ttu-id="bd590-748">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="bd590-748">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="bd590-749">Interactive</span><span class="sxs-lookup"><span data-stu-id="bd590-749">Interactive</span></span>

* <span data-ttu-id="bd590-750">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="bd590-750">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="bd590-751">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-751">June 5, 2018</span></span>

<span data-ttu-id="bd590-752">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="bd590-752">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="bd590-753">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-753">Core</span></span>

* <span data-ttu-id="bd590-754">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="bd590-754">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="bd590-755">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="bd590-755">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="bd590-756">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-756">ACR</span></span>

* <span data-ttu-id="bd590-757">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="bd590-757">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="bd590-758">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="bd590-758">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="bd590-759">AKS</span><span class="sxs-lookup"><span data-stu-id="bd590-759">AKS</span></span>

* <span data-ttu-id="bd590-760">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="bd590-760">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="bd590-761">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bd590-761">Batch</span></span>

* <span data-ttu-id="bd590-762">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="bd590-762">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="bd590-763">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bd590-763">IOT</span></span>

* <span data-ttu-id="bd590-764">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="bd590-764">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="bd590-765">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-765">Network</span></span>

* <span data-ttu-id="bd590-766">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="bd590-766">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="bd590-767">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="bd590-767">Policy Insights</span></span>

* <span data-ttu-id="bd590-768">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="bd590-768">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="bd590-769">ARM</span><span class="sxs-lookup"><span data-stu-id="bd590-769">ARM</span></span>

* <span data-ttu-id="bd590-770">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="bd590-770">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="bd590-771">SQL</span><span class="sxs-lookup"><span data-stu-id="bd590-771">SQL</span></span>

* <span data-ttu-id="bd590-772">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="bd590-772">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="bd590-773">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="bd590-773">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="bd590-774">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-774">Storage</span></span>

* <span data-ttu-id="bd590-775">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="bd590-775">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-776">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-776">VM</span></span>

* <span data-ttu-id="bd590-777">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="bd590-777">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="bd590-778">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-778">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="bd590-779">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-779">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="bd590-780">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-780">May 22, 2018</span></span>

<span data-ttu-id="bd590-781">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="bd590-781">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="bd590-782">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-782">Core</span></span>

* <span data-ttu-id="bd590-783">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="bd590-783">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-784">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-784">ACS</span></span>

* <span data-ttu-id="bd590-785">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="bd590-785">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="bd590-786">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="bd590-786">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-787">AppService</span><span class="sxs-lookup"><span data-stu-id="bd590-787">AppService</span></span>

* <span data-ttu-id="bd590-788">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="bd590-788">Improved generic update commands</span></span>
* <span data-ttu-id="bd590-789">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="bd590-789">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="bd590-790">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bd590-790">Container</span></span>

* <span data-ttu-id="bd590-791">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="bd590-791">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="bd590-792">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bd590-792">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="bd590-793">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="bd590-793">Extension</span></span>

* <span data-ttu-id="bd590-794">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="bd590-794">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="bd590-795">Interactive</span><span class="sxs-lookup"><span data-stu-id="bd590-795">Interactive</span></span>

* <span data-ttu-id="bd590-796">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="bd590-796">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="bd590-797">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="bd590-797">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="bd590-798">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bd590-798">KeyVault</span></span>

* <span data-ttu-id="bd590-799">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="bd590-799">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="bd590-800">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-800">Network</span></span>

* <span data-ttu-id="bd590-801">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="bd590-801">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="bd590-802">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="bd590-802">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="bd590-803">SQL</span><span class="sxs-lookup"><span data-stu-id="bd590-803">SQL</span></span>

* <span data-ttu-id="bd590-804">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="bd590-804">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="bd590-805">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="bd590-805">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="bd590-806">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="bd590-806">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="bd590-807">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="bd590-807">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="bd590-808">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="bd590-808">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="bd590-809">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="bd590-809">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="bd590-810">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="bd590-810">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="bd590-811">`edition`.</span><span class="sxs-lookup"><span data-stu-id="bd590-811">`edition`.</span></span> <span data-ttu-id="bd590-812">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="bd590-812">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="bd590-813">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="bd590-813">`elasticPoolName`.</span></span> <span data-ttu-id="bd590-814">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="bd590-814">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="bd590-815">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="bd590-815">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="bd590-816">`edition`.</span><span class="sxs-lookup"><span data-stu-id="bd590-816">`edition`.</span></span> <span data-ttu-id="bd590-817">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="bd590-817">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="bd590-818">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="bd590-818">`dtu`.</span></span> <span data-ttu-id="bd590-819">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="bd590-819">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="bd590-820">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="bd590-820">`databaseDtuMin`.</span></span> <span data-ttu-id="bd590-821">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="bd590-821">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="bd590-822">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="bd590-822">`databaseDtuMax`.</span></span> <span data-ttu-id="bd590-823">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="bd590-823">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="bd590-824">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="bd590-824">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="bd590-825">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="bd590-825">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-826">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-826">Storage</span></span>

* <span data-ttu-id="bd590-827">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="bd590-827">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="bd590-828">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="bd590-828">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-829">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-829">VM</span></span>

* <span data-ttu-id="bd590-830">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-830">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="bd590-831">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="bd590-831">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="bd590-832">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="bd590-832">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="bd590-833">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="bd590-833">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="bd590-834">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-834">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="bd590-835">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-835">May 7, 2018</span></span>

<span data-ttu-id="bd590-836">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="bd590-836">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="bd590-837">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-837">Core</span></span>

* <span data-ttu-id="bd590-838">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="bd590-838">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="bd590-839">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="bd590-839">Added limited support for positional arguments</span></span>
* <span data-ttu-id="bd590-840">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="bd590-840">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="bd590-841">#5591</span><span class="sxs-lookup"><span data-stu-id="bd590-841">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="bd590-842">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="bd590-842">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="bd590-843">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="bd590-843">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="bd590-844">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="bd590-844">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="bd590-845">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="bd590-845">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="bd590-846">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="bd590-846">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="bd590-847">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-847">ACR</span></span>

* <span data-ttu-id="bd590-848">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="bd590-848">Added ACR Build commands</span></span>
* <span data-ttu-id="bd590-849">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="bd590-849">Improved resource not found error messages</span></span>
* <span data-ttu-id="bd590-850">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="bd590-850">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="bd590-851">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="bd590-851">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="bd590-852">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="bd590-852">Improved repository commands error messages</span></span>
* <span data-ttu-id="bd590-853">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="bd590-853">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-854">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-854">ACS</span></span>

* <span data-ttu-id="bd590-855">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="bd590-855">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="bd590-856">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="bd590-856">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="bd590-857">AMS</span><span class="sxs-lookup"><span data-stu-id="bd590-857">AMS</span></span>

* <span data-ttu-id="bd590-858">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="bd590-858">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-859">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-859">Appservice</span></span>

* <span data-ttu-id="bd590-860">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="bd590-860">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="bd590-861">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-861">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="bd590-862">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="bd590-862">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="bd590-863">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bd590-863">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="bd590-864">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="bd590-864">Batch AI</span></span>

* <span data-ttu-id="bd590-865">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="bd590-865">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="bd590-866">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="bd590-866">Cognitive Services</span></span>

* <span data-ttu-id="bd590-867">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="bd590-867">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="bd590-868">Потребление</span><span class="sxs-lookup"><span data-stu-id="bd590-868">Consumption</span></span>

* <span data-ttu-id="bd590-869">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="bd590-869">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="bd590-870">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bd590-870">Container</span></span>

* <span data-ttu-id="bd590-871">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="bd590-871">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="bd590-872">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="bd590-872">Cosmos DB</span></span>

* <span data-ttu-id="bd590-873">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="bd590-873">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="bd590-874">DMS</span><span class="sxs-lookup"><span data-stu-id="bd590-874">DMS</span></span>

* <span data-ttu-id="bd590-875">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="bd590-875">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="bd590-876">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="bd590-876">Extension</span></span>

* <span data-ttu-id="bd590-877">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="bd590-877">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="bd590-878">Interactive</span><span class="sxs-lookup"><span data-stu-id="bd590-878">Interactive</span></span>

* <span data-ttu-id="bd590-879">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="bd590-879">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="bd590-880">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="bd590-880">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="bd590-881">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="bd590-881">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="bd590-882">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="bd590-882">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="bd590-883">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="bd590-883">Lab</span></span>

* <span data-ttu-id="bd590-884">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="bd590-884">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="bd590-885">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-885">Network</span></span>

* <span data-ttu-id="bd590-886">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="bd590-886">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="bd590-887">Профиль</span><span class="sxs-lookup"><span data-stu-id="bd590-887">Profile</span></span>

* <span data-ttu-id="bd590-888">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-888">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="bd590-889">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="bd590-889">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="bd590-890">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="bd590-890">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="bd590-891">Redis</span><span class="sxs-lookup"><span data-stu-id="bd590-891">Redis</span></span>

* <span data-ttu-id="bd590-892">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="bd590-892">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="bd590-893">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="bd590-893">Deprecated `redis list-all`.</span></span> <span data-ttu-id="bd590-894">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="bd590-894">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="bd590-895">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="bd590-895">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="bd590-896">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="bd590-896">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="bd590-897">Роль</span><span class="sxs-lookup"><span data-stu-id="bd590-897">Role</span></span>

* <span data-ttu-id="bd590-898">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="bd590-898">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-899">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-899">Storage</span></span>

* <span data-ttu-id="bd590-900">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="bd590-900">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="bd590-901">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="bd590-901">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="bd590-902">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="bd590-902">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="bd590-903">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="bd590-903">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="bd590-904">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="bd590-904">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-905">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-905">VM</span></span>

* <span data-ttu-id="bd590-906">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="bd590-906">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="bd590-907">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="bd590-907">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="bd590-908">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="bd590-908">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="bd590-909">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="bd590-909">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="bd590-910">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="bd590-910">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="bd590-911">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="bd590-911">Added write accelerator support</span></span>
* <span data-ttu-id="bd590-912">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="bd590-912">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="bd590-913">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="bd590-913">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="bd590-914">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="bd590-914">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="bd590-915">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-915">April 10, 2018</span></span>

<span data-ttu-id="bd590-916">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="bd590-916">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="bd590-917">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-917">ACR</span></span>

* <span data-ttu-id="bd590-918">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="bd590-918">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-919">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-919">ACS</span></span>

* <span data-ttu-id="bd590-920">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="bd590-920">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-921">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-921">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="bd590-923">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="bd590-923">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="bd590-924">Batch AI</span><span class="sxs-lookup"><span data-stu-id="bd590-924">BatchAI</span></span>

* <span data-ttu-id="bd590-925">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="bd590-925">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="bd590-926">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="bd590-926">Job level mounting</span></span>
  - <span data-ttu-id="bd590-927">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="bd590-927">Environment variables with secret values</span></span>
  - <span data-ttu-id="bd590-928">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="bd590-928">Performance counters settings</span></span>
  - <span data-ttu-id="bd590-929">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="bd590-929">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="bd590-930">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="bd590-930">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="bd590-931">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="bd590-931">Usage and limits reporting</span></span>
  - <span data-ttu-id="bd590-932">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="bd590-932">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="bd590-933">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="bd590-933">Support for custom images</span></span>
  - <span data-ttu-id="bd590-934">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="bd590-934">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="bd590-935">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="bd590-935">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="bd590-936">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="bd590-936">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="bd590-937">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="bd590-937">National clouds are supported</span></span>
* <span data-ttu-id="bd590-938">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="bd590-938">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="bd590-939">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="bd590-939">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="bd590-940">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="bd590-940">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="bd590-941">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="bd590-941">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="bd590-942">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="bd590-942">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="bd590-943">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="bd590-943">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="bd590-944">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="bd590-944">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="bd590-945">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="bd590-945">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="bd590-946">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="bd590-946">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="bd590-947">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-947">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="bd590-948">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="bd590-948">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="bd590-949">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="bd590-949">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="bd590-950">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-950">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="bd590-951">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="bd590-951">Billing</span></span>

* <span data-ttu-id="bd590-952">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="bd590-952">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="bd590-953">Потребление</span><span class="sxs-lookup"><span data-stu-id="bd590-953">Consumption</span></span>

* <span data-ttu-id="bd590-954">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="bd590-954">Added `marketplace` commands</span></span>
* <span data-ttu-id="bd590-955">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="bd590-955">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="bd590-956">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="bd590-956">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="bd590-957">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="bd590-957">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="bd590-958">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="bd590-958">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="bd590-959">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="bd590-959">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="bd590-960">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bd590-960">Container</span></span>

* <span data-ttu-id="bd590-961">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="bd590-961">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="bd590-962">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="bd590-962">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="bd590-963">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="bd590-963">Extension</span></span>

* <span data-ttu-id="bd590-964">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="bd590-964">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="bd590-965">Interactive</span><span class="sxs-lookup"><span data-stu-id="bd590-965">Interactive</span></span>

* <span data-ttu-id="bd590-966">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="bd590-966">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="bd590-967">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="bd590-967">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="bd590-968">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="bd590-968">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="bd590-969">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-969">Network</span></span>

* <span data-ttu-id="bd590-970">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-970">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="bd590-971">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-971">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="bd590-972">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="bd590-972">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="bd590-973">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="bd590-973">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="bd590-974">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="bd590-974">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="bd590-975">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-975">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="bd590-976">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-976">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="bd590-977">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="bd590-977">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="bd590-978">Профиль</span><span class="sxs-lookup"><span data-stu-id="bd590-978">Profile</span></span>

* <span data-ttu-id="bd590-979">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="bd590-979">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="bd590-980">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="bd590-980">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="bd590-981">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="bd590-981">RDBMS</span></span>

* <span data-ttu-id="bd590-982">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="bd590-982">Added `georestore` command</span></span>
* <span data-ttu-id="bd590-983">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="bd590-983">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="bd590-984">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bd590-984">Resource</span></span>

* <span data-ttu-id="bd590-985">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-985">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="bd590-986">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-986">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="bd590-987">SQL</span><span class="sxs-lookup"><span data-stu-id="bd590-987">SQL</span></span>

* <span data-ttu-id="bd590-988">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="bd590-988">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-989">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-989">Storage</span></span>

* <span data-ttu-id="bd590-990">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="bd590-990">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-991">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-991">VM</span></span>

* <span data-ttu-id="bd590-992">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="bd590-992">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="bd590-993">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="bd590-993">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="bd590-995">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-995">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="bd590-996">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="bd590-996">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="bd590-997">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="bd590-997">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="bd590-998">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="bd590-998">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="bd590-999">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-999">March 27, 2018</span></span>

<span data-ttu-id="bd590-1000">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="bd590-1000">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="bd590-1001">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-1001">Core</span></span>

* <span data-ttu-id="bd590-1002">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="bd590-1002">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-1003">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-1003">ACS</span></span>

* <span data-ttu-id="bd590-1004">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="bd590-1004">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-1005">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-1005">Appservice</span></span>

* <span data-ttu-id="bd590-1006">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1006">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="bd590-1007">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1007">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="bd590-1008">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="bd590-1008">Backup</span></span>

* <span data-ttu-id="bd590-1009">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1009">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="bd590-1010">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="bd590-1010">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="bd590-1011">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="bd590-1011">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="bd590-1012">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1012">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="bd590-1013">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bd590-1013">Container</span></span>

* <span data-ttu-id="bd590-1014">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1014">Added `container exec` command.</span></span> <span data-ttu-id="bd590-1015">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bd590-1015">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="bd590-1016">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bd590-1016">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="bd590-1017">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="bd590-1017">Extension</span></span>

* <span data-ttu-id="bd590-1018">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="bd590-1018">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="bd590-1019">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1019">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="bd590-1020">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bd590-1020">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="bd590-1021">Interactive</span><span class="sxs-lookup"><span data-stu-id="bd590-1021">Interactive</span></span>

* <span data-ttu-id="bd590-1022">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="bd590-1022">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="bd590-1023">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1023">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="bd590-1024">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="bd590-1024">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="bd590-1025">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="bd590-1025">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="bd590-1026">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="bd590-1026">Lab</span></span>

* <span data-ttu-id="bd590-1027">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1027">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="bd590-1028">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bd590-1028">Monitor</span></span>

* <span data-ttu-id="bd590-1029">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="bd590-1029">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="bd590-1030">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="bd590-1030">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="bd590-1031">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="bd590-1031">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="bd590-1032">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-1032">Network</span></span>

* <span data-ttu-id="bd590-1033">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="bd590-1033">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="bd590-1034">Профиль</span><span class="sxs-lookup"><span data-stu-id="bd590-1034">Profile</span></span>

* <span data-ttu-id="bd590-1035">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1035">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="bd590-1036">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="bd590-1036">RDBMS</span></span>

* <span data-ttu-id="bd590-1037">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="bd590-1037">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="bd590-1038">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bd590-1038">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="bd590-1040">Роль</span><span class="sxs-lookup"><span data-stu-id="bd590-1040">Role</span></span>

* <span data-ttu-id="bd590-1041">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1041">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="bd590-1042">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="bd590-1042">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="bd590-1043">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="bd590-1043">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="bd590-1044">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1044">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="bd590-1045">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1045">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-1046">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-1046">Storage</span></span>

* <span data-ttu-id="bd590-1047">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="bd590-1047">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="bd590-1048">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="bd590-1048">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-1049">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-1049">VM</span></span>

* <span data-ttu-id="bd590-1050">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="bd590-1050">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="bd590-1051">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1051">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="bd590-1052">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="bd590-1052">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="bd590-1053">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="bd590-1053">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="bd590-1054">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-1054">March 13, 2018</span></span>

<span data-ttu-id="bd590-1055">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="bd590-1055">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="bd590-1056">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-1056">ACR</span></span>

* <span data-ttu-id="bd590-1057">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1057">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="bd590-1058">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="bd590-1058">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="bd590-1059">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="bd590-1059">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-1060">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-1060">ACS</span></span>

* <span data-ttu-id="bd590-1061">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="bd590-1061">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="bd590-1062">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="bd590-1062">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="bd590-1063">Помощник</span><span class="sxs-lookup"><span data-stu-id="bd590-1063">Advisor</span></span>

* <span data-ttu-id="bd590-1064">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1064">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="bd590-1065">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1065">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="bd590-1066">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1066">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="bd590-1067">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1067">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="bd590-1068">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1068">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-1069">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-1069">Appservice</span></span>

* <span data-ttu-id="bd590-1070">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="bd590-1070">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="bd590-1071">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1071">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="bd590-1072">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="bd590-1072">Eventhubs</span></span>

* <span data-ttu-id="bd590-1073">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="bd590-1073">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="bd590-1074">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="bd590-1074">Extension</span></span>

* <span data-ttu-id="bd590-1075">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="bd590-1075">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="bd590-1076">Interactive</span><span class="sxs-lookup"><span data-stu-id="bd590-1076">Interactive</span></span>

* <span data-ttu-id="bd590-1077">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="bd590-1077">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="bd590-1078">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="bd590-1078">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="bd590-1079">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="bd590-1079">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="bd590-1080">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="bd590-1080">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="bd590-1081">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bd590-1081">Monitor</span></span>

* <span data-ttu-id="bd590-1082">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="bd590-1082">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="bd590-1083">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1083">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="bd590-1084">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1084">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="bd590-1085">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1085">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="bd590-1086">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-1086">Network</span></span>

* <span data-ttu-id="bd590-1087">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1087">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="bd590-1088">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="bd590-1088">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="bd590-1089">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1089">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="bd590-1090">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1090">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="bd590-1091">Профиль</span><span class="sxs-lookup"><span data-stu-id="bd590-1091">Profile</span></span>

* <span data-ttu-id="bd590-1092">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="bd590-1092">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="bd590-1093">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1093">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="bd590-1094">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="bd590-1094">RDBMS</span></span>

* <span data-ttu-id="bd590-1095">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="bd590-1095">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="bd590-1096">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="bd590-1096">Service Bus</span></span>

* <span data-ttu-id="bd590-1097">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="bd590-1097">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-1098">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-1098">Storage</span></span>

* <span data-ttu-id="bd590-1099">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="bd590-1099">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="bd590-1100">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="bd590-1100">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-1101">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-1101">VM</span></span>

* <span data-ttu-id="bd590-1102">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="bd590-1102">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="bd590-1103">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="bd590-1103">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="bd590-1104">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1104">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="bd590-1105">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="bd590-1105">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="bd590-1106">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="bd590-1106">February 27, 2018</span></span>

<span data-ttu-id="bd590-1107">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="bd590-1107">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="bd590-1108">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-1108">Core</span></span>

* <span data-ttu-id="bd590-1109">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="bd590-1109">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="bd590-1110">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="bd590-1110">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="bd590-1111">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1111">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-1112">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-1112">ACS</span></span>

* <span data-ttu-id="bd590-1113">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bd590-1113">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="bd590-1114">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="bd590-1114">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="bd590-1115">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1115">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="bd590-1116">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1116">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-1117">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-1117">Appservice</span></span>

* <span data-ttu-id="bd590-1118">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="bd590-1118">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="bd590-1119">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="bd590-1119">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="bd590-1120">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="bd590-1120">Cognitive Services</span></span>

* <span data-ttu-id="bd590-1121">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="bd590-1121">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="bd590-1122">Потребление</span><span class="sxs-lookup"><span data-stu-id="bd590-1122">Consumption</span></span>

* <span data-ttu-id="bd590-1123">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="bd590-1123">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="bd590-1124">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="bd590-1124">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="bd590-1125">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bd590-1125">Container</span></span>

* <span data-ttu-id="bd590-1126">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="bd590-1126">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="bd590-1127">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-1127">Network</span></span>

* <span data-ttu-id="bd590-1128">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1128">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="bd590-1129">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bd590-1129">Resource</span></span>

* <span data-ttu-id="bd590-1130">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="bd590-1130">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="bd590-1131">Роль</span><span class="sxs-lookup"><span data-stu-id="bd590-1131">Role</span></span>

* <span data-ttu-id="bd590-1132">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="bd590-1132">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="bd590-1133">SQL</span><span class="sxs-lookup"><span data-stu-id="bd590-1133">SQL</span></span>

* <span data-ttu-id="bd590-1134">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="bd590-1134">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-1135">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-1135">Storage</span></span>

* <span data-ttu-id="bd590-1136">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1136">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-1137">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-1137">VM</span></span>

* <span data-ttu-id="bd590-1138">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="bd590-1138">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="bd590-1139">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-1139">February 13, 2018</span></span>

<span data-ttu-id="bd590-1140">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="bd590-1140">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="bd590-1141">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-1141">Core</span></span>

* <span data-ttu-id="bd590-1142">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="bd590-1142">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-1143">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-1143">ACS</span></span>

* <span data-ttu-id="bd590-1144">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="bd590-1144">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="bd590-1145">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1145">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="bd590-1146">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="bd590-1146">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="bd590-1147">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="bd590-1147">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="bd590-1148">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="bd590-1148">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="bd590-1149">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1149">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="bd590-1150">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="bd590-1150">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="bd590-1151">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1151">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-1152">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-1152">Appservice</span></span>

* <span data-ttu-id="bd590-1153">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="bd590-1153">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="bd590-1154">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1154">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="bd590-1155">CDN</span><span class="sxs-lookup"><span data-stu-id="bd590-1155">CDN</span></span>

* <span data-ttu-id="bd590-1156">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1156">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="bd590-1157">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bd590-1157">Container</span></span>

* <span data-ttu-id="bd590-1158">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="bd590-1158">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="bd590-1159">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bd590-1159">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bd590-1160">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="bd590-1160">CosmosDB</span></span>

* <span data-ttu-id="bd590-1161">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="bd590-1161">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="bd590-1162">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="bd590-1162">Extension</span></span>

* <span data-ttu-id="bd590-1163">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1163">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="bd590-1164">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1164">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="bd590-1165">Отзыв</span><span class="sxs-lookup"><span data-stu-id="bd590-1165">Feedback</span></span>

* <span data-ttu-id="bd590-1166">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="bd590-1166">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="bd590-1167">Interactive</span><span class="sxs-lookup"><span data-stu-id="bd590-1167">Interactive</span></span>

* <span data-ttu-id="bd590-1168">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="bd590-1168">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="bd590-1169">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="bd590-1169">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="bd590-1170">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bd590-1170">IoT</span></span>

* <span data-ttu-id="bd590-1171">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="bd590-1171">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="bd590-1172">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="bd590-1172">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="bd590-1173">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1173">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="bd590-1174">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="bd590-1174">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="bd590-1175">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bd590-1175">Monitor</span></span>

* <span data-ttu-id="bd590-1176">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1176">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="bd590-1177">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-1177">Network</span></span>

* <span data-ttu-id="bd590-1178">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="bd590-1178">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="bd590-1179">Профиль</span><span class="sxs-lookup"><span data-stu-id="bd590-1179">Profile</span></span>

* <span data-ttu-id="bd590-1180">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="bd590-1180">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="bd590-1181">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bd590-1181">Resource</span></span>

* <span data-ttu-id="bd590-1182">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1182">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="bd590-1183">Роль</span><span class="sxs-lookup"><span data-stu-id="bd590-1183">Role</span></span>

* <span data-ttu-id="bd590-1184">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="bd590-1184">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="bd590-1185">SQL</span><span class="sxs-lookup"><span data-stu-id="bd590-1185">SQL</span></span>

* <span data-ttu-id="bd590-1186">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1186">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="bd590-1187">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1187">Added `sql db rename`</span></span>
* <span data-ttu-id="bd590-1188">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="bd590-1188">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-1189">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-1189">Storage</span></span>

* <span data-ttu-id="bd590-1190">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="bd590-1190">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-1191">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-1191">VM</span></span>

* <span data-ttu-id="bd590-1192">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="bd590-1192">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="bd590-1193">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="bd590-1193">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="bd590-1194">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="bd590-1194">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="bd590-1195">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-1195">January 31, 2018</span></span>

<span data-ttu-id="bd590-1196">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="bd590-1196">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="bd590-1197">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-1197">Core</span></span>

* <span data-ttu-id="bd590-1198">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="bd590-1198">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="bd590-1199">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="bd590-1199">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="bd590-1200">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="bd590-1200">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="bd590-1201">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="bd590-1201">Use `--verbose` to see</span></span>
* <span data-ttu-id="bd590-1202">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="bd590-1202">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-1203">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-1203">ACS</span></span>

* <span data-ttu-id="bd590-1204">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1204">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="bd590-1205">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1205">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-1206">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-1206">Appservice</span></span>

* <span data-ttu-id="bd590-1207">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="bd590-1207">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="bd590-1208">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="bd590-1208">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="bd590-1209">CDN</span><span class="sxs-lookup"><span data-stu-id="bd590-1209">CDN</span></span>

* <span data-ttu-id="bd590-1210">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1210">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bd590-1211">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="bd590-1211">CosmosDB</span></span>

* <span data-ttu-id="bd590-1212">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="bd590-1212">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="bd590-1213">Interactive</span><span class="sxs-lookup"><span data-stu-id="bd590-1213">Interactive</span></span>

* <span data-ttu-id="bd590-1214">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="bd590-1214">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="bd590-1215">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-1215">Network</span></span>

* <span data-ttu-id="bd590-1216">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1216">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="bd590-1217">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bd590-1217">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="bd590-1218">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1218">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="bd590-1219">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1219">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="bd590-1220">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1220">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="bd590-1221">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="bd590-1221">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="bd590-1222">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="bd590-1222">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="bd590-1223">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="bd590-1223">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="bd590-1224">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1224">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="bd590-1225">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1225">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="bd590-1226">Профиль</span><span class="sxs-lookup"><span data-stu-id="bd590-1226">Profile</span></span>

* <span data-ttu-id="bd590-1227">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="bd590-1227">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="bd590-1228">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bd590-1228">Resource</span></span>

* <span data-ttu-id="bd590-1229">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="bd590-1229">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-1230">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-1230">Storage</span></span>

* <span data-ttu-id="bd590-1231">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="bd590-1231">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="bd590-1232">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="bd590-1232">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="bd590-1233">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1233">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="bd590-1234">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1234">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="bd590-1235">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="bd590-1235">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-1236">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-1236">VM</span></span>

* <span data-ttu-id="bd590-1237">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="bd590-1237">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="bd590-1238">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="bd590-1238">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="bd590-1239">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="bd590-1239">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="bd590-1240">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1240">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="bd590-1241">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-1241">January 17, 2018</span></span>

<span data-ttu-id="bd590-1242">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="bd590-1242">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="bd590-1243">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-1243">ACR</span></span>

* <span data-ttu-id="bd590-1244">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="bd590-1244">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="bd590-1245">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="bd590-1245">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-1246">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-1246">ACS</span></span>

* <span data-ttu-id="bd590-1247">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1247">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="bd590-1248">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="bd590-1248">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-1249">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-1249">Appservice</span></span>

* <span data-ttu-id="bd590-1250">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="bd590-1250">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="bd590-1251">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="bd590-1251">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="bd590-1252">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1252">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="bd590-1253">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="bd590-1253">Backup</span></span>

* <span data-ttu-id="bd590-1254">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="bd590-1254">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="bd590-1255">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="bd590-1255">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="bd590-1256">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="bd590-1256">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="bd590-1257">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="bd590-1257">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="bd590-1258">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="bd590-1258">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="bd590-1259">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bd590-1259">Batch</span></span>

* <span data-ttu-id="bd590-1260">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="bd590-1260">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="bd590-1261">Облако</span><span class="sxs-lookup"><span data-stu-id="bd590-1261">Cloud</span></span>

* <span data-ttu-id="bd590-1262">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="bd590-1262">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="bd590-1263">Потребление</span><span class="sxs-lookup"><span data-stu-id="bd590-1263">Consumption</span></span>

* <span data-ttu-id="bd590-1264">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1264">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="bd590-1265">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="bd590-1265">Event Grid</span></span>

* <span data-ttu-id="bd590-1266">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1266">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="bd590-1267">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1267">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="bd590-1268">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1268">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="bd590-1269">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1269">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="bd590-1270">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1270">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="bd590-1271">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1271">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="bd590-1272">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1272">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="bd590-1273">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="bd590-1273">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="bd590-1274">Interactive</span><span class="sxs-lookup"><span data-stu-id="bd590-1274">Interactive</span></span>

* <span data-ttu-id="bd590-1275">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="bd590-1275">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="bd590-1276">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="bd590-1276">Fixed errors on startup</span></span>
* <span data-ttu-id="bd590-1277">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="bd590-1277">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="bd590-1278">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bd590-1278">IoT</span></span>

* <span data-ttu-id="bd590-1279">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="bd590-1279">Added support for device provisioning service</span></span>
* <span data-ttu-id="bd590-1280">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="bd590-1280">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="bd590-1281">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="bd590-1281">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="bd590-1282">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bd590-1282">Monitor</span></span>

* <span data-ttu-id="bd590-1283">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="bd590-1283">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="bd590-1284">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1284">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="bd590-1285">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="bd590-1285">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="bd590-1286">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-1286">Network</span></span>

* <span data-ttu-id="bd590-1287">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="bd590-1287">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="bd590-1288">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="bd590-1288">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="bd590-1289">Профиль</span><span class="sxs-lookup"><span data-stu-id="bd590-1289">Profile</span></span>

* <span data-ttu-id="bd590-1290">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="bd590-1290">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="bd590-1291">Роль</span><span class="sxs-lookup"><span data-stu-id="bd590-1291">Role</span></span>

* <span data-ttu-id="bd590-1292">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="bd590-1292">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="bd590-1293">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="bd590-1293">Service Fabric</span></span>

* <span data-ttu-id="bd590-1294">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="bd590-1294">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="bd590-1295">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="bd590-1295">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-1296">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-1296">VM</span></span>

* <span data-ttu-id="bd590-1297">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1297">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="bd590-1298">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="bd590-1298">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="bd590-1299">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1299">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="bd590-1300">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="bd590-1300">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="bd590-1301">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="bd590-1301">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="bd590-1302">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1302">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="bd590-1303">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1303">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="bd590-1304">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1304">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="bd590-1305">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-1305">December 19, 2017</span></span>

<span data-ttu-id="bd590-1306">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="bd590-1306">Version 2.0.23</span></span>

* <span data-ttu-id="bd590-1307">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="bd590-1307">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="bd590-1308">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bd590-1308">Container</span></span>

* <span data-ttu-id="bd590-1309">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bd590-1309">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="bd590-1310">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-1310">Network</span></span>

* <span data-ttu-id="bd590-1311">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bd590-1311">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="bd590-1312">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bd590-1312">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-1313">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-1313">Storage</span></span>

* <span data-ttu-id="bd590-1314">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="bd590-1314">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-1315">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-1315">VM</span></span>

* <span data-ttu-id="bd590-1316">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="bd590-1316">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="bd590-1317">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-1317">December 5, 2017</span></span>

<span data-ttu-id="bd590-1318">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="bd590-1318">Version 2.0.22</span></span>

* <span data-ttu-id="bd590-1319">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1319">Removed `az component` commands.</span></span> <span data-ttu-id="bd590-1320">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1320">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="bd590-1321">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-1321">Core</span></span>
* <span data-ttu-id="bd590-1322">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="bd590-1322">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="bd590-1323">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="bd590-1323">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-1324">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-1324">ACS</span></span>

* <span data-ttu-id="bd590-1325">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1325">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="bd590-1326">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1326">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="bd590-1327">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="bd590-1327">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="bd590-1328">Помощник</span><span class="sxs-lookup"><span data-stu-id="bd590-1328">Advisor</span></span>

* <span data-ttu-id="bd590-1329">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="bd590-1329">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-1330">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-1330">Appservice</span></span>

* <span data-ttu-id="bd590-1331">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1331">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="bd590-1332">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="bd590-1332">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="bd590-1333">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1333">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="bd590-1334">Потребление</span><span class="sxs-lookup"><span data-stu-id="bd590-1334">Consumption</span></span>

* <span data-ttu-id="bd590-1335">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="bd590-1335">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="bd590-1336">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bd590-1336">Container</span></span>

* <span data-ttu-id="bd590-1337">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="bd590-1337">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="bd590-1338">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bd590-1338">Monitor</span></span>

* <span data-ttu-id="bd590-1339">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="bd590-1339">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="bd590-1340">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bd590-1340">Resource</span></span>

* <span data-ttu-id="bd590-1341">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="bd590-1341">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="bd590-1342">Роль</span><span class="sxs-lookup"><span data-stu-id="bd590-1342">Role</span></span>

* <span data-ttu-id="bd590-1343">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1343">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="bd590-1344">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="bd590-1344">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="bd590-1345">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1345">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="bd590-1346">SQL</span><span class="sxs-lookup"><span data-stu-id="bd590-1346">SQL</span></span>

* <span data-ttu-id="bd590-1347">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1347">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="bd590-1348">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1348">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-1349">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-1349">VM</span></span>

* <span data-ttu-id="bd590-1350">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1350">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="bd590-1351">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-1351">November 14, 2017</span></span>

<span data-ttu-id="bd590-1352">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="bd590-1352">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="bd590-1353">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-1353">ACR</span></span>

* <span data-ttu-id="bd590-1354">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="bd590-1354">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="bd590-1355">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-1355">ACS</span></span>

* <span data-ttu-id="bd590-1356">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="bd590-1356">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="bd590-1357">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="bd590-1357">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="bd590-1358">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1358">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="bd590-1359">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="bd590-1359">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="bd590-1360">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="bd590-1360">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-1361">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-1361">Appservice</span></span>

* <span data-ttu-id="bd590-1362">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="bd590-1362">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="bd590-1363">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1363">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="bd590-1364">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1364">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="bd590-1365">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1365">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="bd590-1366">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="bd590-1366">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="bd590-1367">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="bd590-1367">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="bd590-1368">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bd590-1368">Batch</span></span>

* <span data-ttu-id="bd590-1369">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1369">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="bd590-1370">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="bd590-1370">Batchai</span></span>

* <span data-ttu-id="bd590-1371">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1371">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="bd590-1372">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1372">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="bd590-1373">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1373">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="bd590-1374">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1374">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="bd590-1375">Облако</span><span class="sxs-lookup"><span data-stu-id="bd590-1375">Cloud</span></span>

* <span data-ttu-id="bd590-1376">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="bd590-1376">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="bd590-1377">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bd590-1377">Container</span></span>

* <span data-ttu-id="bd590-1378">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="bd590-1378">Added support to open multiple ports</span></span>
* <span data-ttu-id="bd590-1379">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bd590-1379">Added container group restart policy</span></span>
* <span data-ttu-id="bd590-1380">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="bd590-1380">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="bd590-1381">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="bd590-1381">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="bd590-1382">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="bd590-1382">Data Lake Analytics</span></span>

* <span data-ttu-id="bd590-1383">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="bd590-1383">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="bd590-1384">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="bd590-1384">Data Lake Store</span></span>

* <span data-ttu-id="bd590-1385">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="bd590-1385">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="bd590-1386">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="bd590-1386">Extension</span></span>

* <span data-ttu-id="bd590-1387">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="bd590-1387">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="bd590-1388">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="bd590-1388">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="bd590-1389">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bd590-1389">IoT</span></span>

* <span data-ttu-id="bd590-1390">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="bd590-1390">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="bd590-1391">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bd590-1391">Monitor</span></span>

* <span data-ttu-id="bd590-1392">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1392">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="bd590-1393">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-1393">Network</span></span>

* <span data-ttu-id="bd590-1394">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="bd590-1394">Added support for CAA DNS records</span></span>
* <span data-ttu-id="bd590-1395">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1395">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="bd590-1396">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="bd590-1396">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="bd590-1397">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1397">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="bd590-1398">Резервирование</span><span class="sxs-lookup"><span data-stu-id="bd590-1398">Reservations</span></span>

* <span data-ttu-id="bd590-1399">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="bd590-1399">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="bd590-1400">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bd590-1400">Resource</span></span>

* <span data-ttu-id="bd590-1401">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1401">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="bd590-1402">SQL</span><span class="sxs-lookup"><span data-stu-id="bd590-1402">SQL</span></span>

* <span data-ttu-id="bd590-1403">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1403">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-1404">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-1404">Storage</span></span>

* <span data-ttu-id="bd590-1405">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bd590-1405">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="bd590-1406">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="bd590-1406">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="bd590-1407">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1407">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="bd590-1408">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1408">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="bd590-1409">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1409">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="bd590-1410">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1410">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="bd590-1411">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1411">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-1412">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-1412">VM</span></span>

* <span data-ttu-id="bd590-1413">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1413">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="bd590-1414">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="bd590-1414">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="bd590-1415">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1415">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="bd590-1416">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1416">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="bd590-1417">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="bd590-1417">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="bd590-1418">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-1418">October 24, 2017</span></span>

<span data-ttu-id="bd590-1419">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="bd590-1419">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="bd590-1420">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-1420">Core</span></span>

* <span data-ttu-id="bd590-1421">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="bd590-1421">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="bd590-1422">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-1422">ACR</span></span>

* <span data-ttu-id="bd590-1423">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="bd590-1423">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="bd590-1424">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="bd590-1424">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="bd590-1425">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="bd590-1425">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-1426">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-1426">ACS</span></span>

* <span data-ttu-id="bd590-1427">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="bd590-1427">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="bd590-1428">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="bd590-1428">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-1429">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-1429">Appservice</span></span>

* <span data-ttu-id="bd590-1430">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="bd590-1430">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="bd590-1431">Компонент</span><span class="sxs-lookup"><span data-stu-id="bd590-1431">Component</span></span>

* <span data-ttu-id="bd590-1432">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="bd590-1432">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="bd590-1433">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bd590-1433">Monitor</span></span>

* <span data-ttu-id="bd590-1434">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1434">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="bd590-1435">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bd590-1435">Resource</span></span>

* <span data-ttu-id="bd590-1436">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="bd590-1436">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="bd590-1437">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="bd590-1437">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-1438">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-1438">VM</span></span>

* <span data-ttu-id="bd590-1439">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="bd590-1439">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="bd590-1440">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-1440">October 9, 2017</span></span>

<span data-ttu-id="bd590-1441">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="bd590-1441">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="bd590-1442">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-1442">Core</span></span>

* <span data-ttu-id="bd590-1443">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="bd590-1443">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-1444">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-1444">Appservice</span></span>

* <span data-ttu-id="bd590-1445">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1445">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="bd590-1446">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bd590-1446">Batch</span></span>

* <span data-ttu-id="bd590-1447">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="bd590-1447">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="bd590-1448">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="bd590-1448">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="bd590-1449">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="bd590-1449">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="bd590-1450">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="bd590-1450">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="bd590-1451">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="bd590-1451">Batchai</span></span>

* <span data-ttu-id="bd590-1452">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="bd590-1452">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="bd590-1453">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bd590-1453">Keyvault</span></span>

* <span data-ttu-id="bd590-1454">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="bd590-1454">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="bd590-1455">(#4448)</span><span class="sxs-lookup"><span data-stu-id="bd590-1455">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="bd590-1456">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-1456">Network</span></span>

* <span data-ttu-id="bd590-1457">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="bd590-1457">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="bd590-1458">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="bd590-1458">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="bd590-1459">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bd590-1459">Resource</span></span>

* <span data-ttu-id="bd590-1460">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1460">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="bd590-1461">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="bd590-1461">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="bd590-1462">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="bd590-1462">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="bd590-1463">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="bd590-1463">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="bd590-1464">SQL</span><span class="sxs-lookup"><span data-stu-id="bd590-1464">Sql</span></span>

* <span data-ttu-id="bd590-1465">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="bd590-1465">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="bd590-1466">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="bd590-1466">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="bd590-1467">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="bd590-1467">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-1468">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-1468">Storage</span></span>

* <span data-ttu-id="bd590-1469">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bd590-1469">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-1470">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="bd590-1470">Vm</span></span>

* <span data-ttu-id="bd590-1471">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="bd590-1471">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="bd590-1472">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1472">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="bd590-1473">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1473">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="bd590-1474">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1474">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="bd590-1475">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="bd590-1475">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="bd590-1476">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-1476">September 22, 2017</span></span>

<span data-ttu-id="bd590-1477">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="bd590-1477">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="bd590-1478">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bd590-1478">Resource</span></span>

* <span data-ttu-id="bd590-1479">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="bd590-1479">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="bd590-1480">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="bd590-1480">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="bd590-1481">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="bd590-1481">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="bd590-1482">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1482">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="bd590-1483">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-1483">Network</span></span>

* <span data-ttu-id="bd590-1484">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="bd590-1484">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="bd590-1485">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="bd590-1485">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="bd590-1486">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="bd590-1486">Added `asg` application security group commands</span></span>
* <span data-ttu-id="bd590-1487">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="bd590-1487">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="bd590-1488">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bd590-1488">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="bd590-1489">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bd590-1489">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="bd590-1490">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1490">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-1491">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-1491">Storage</span></span>

* <span data-ttu-id="bd590-1492">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="bd590-1492">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="bd590-1493">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="bd590-1493">Eventgrid</span></span>

* <span data-ttu-id="bd590-1494">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="bd590-1494">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="bd590-1495">SQL</span><span class="sxs-lookup"><span data-stu-id="bd590-1495">SQL</span></span>

* <span data-ttu-id="bd590-1496">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="bd590-1496">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="bd590-1497">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="bd590-1497">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="bd590-1498">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bd590-1498">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="bd590-1499">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bd590-1499">Keyvault</span></span>

* <span data-ttu-id="bd590-1500">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="bd590-1500">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-1501">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-1501">VM</span></span>

* <span data-ttu-id="bd590-1502">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="bd590-1502">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="bd590-1503">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="bd590-1503">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="bd590-1504">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="bd590-1504">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="bd590-1505">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="bd590-1505">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="bd590-1506">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="bd590-1506">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="bd590-1507">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="bd590-1507">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-1508">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-1508">ACS</span></span>

* <span data-ttu-id="bd590-1509">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="bd590-1509">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-1510">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-1510">Appservice</span></span>

* <span data-ttu-id="bd590-1511">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="bd590-1511">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="bd590-1512">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="bd590-1512">Backup</span></span>

* <span data-ttu-id="bd590-1513">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="bd590-1513">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="bd590-1514">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-1514">September 11, 2017</span></span>

<span data-ttu-id="bd590-1515">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="bd590-1515">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="bd590-1516">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-1516">Core</span></span>

* <span data-ttu-id="bd590-1517">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="bd590-1517">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="bd590-1518">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="bd590-1518">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-1519">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-1519">Acs</span></span>

* <span data-ttu-id="bd590-1520">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1520">Added `acs list-locations` command</span></span>
* <span data-ttu-id="bd590-1521">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bd590-1521">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-1522">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-1522">Appservice</span></span>

* <span data-ttu-id="bd590-1523">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="bd590-1523">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="bd590-1524">CDN</span><span class="sxs-lookup"><span data-stu-id="bd590-1524">CDN</span></span>

* <span data-ttu-id="bd590-1525">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1525">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="bd590-1526">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="bd590-1526">Extension</span></span>

* <span data-ttu-id="bd590-1527">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="bd590-1527">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="bd590-1528">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bd590-1528">Keyvault</span></span>

* <span data-ttu-id="bd590-1529">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1529">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="bd590-1530">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-1530">Network</span></span>

* <span data-ttu-id="bd590-1531">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1531">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="bd590-1532">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1532">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="bd590-1533">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1533">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="bd590-1534">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1534">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="bd590-1535">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1535">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="bd590-1536">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bd590-1536">Resource</span></span>

* <span data-ttu-id="bd590-1537">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1537">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="bd590-1538">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1538">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="bd590-1539">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="bd590-1539">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="bd590-1540">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="bd590-1540">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="bd590-1541">SQL</span><span class="sxs-lookup"><span data-stu-id="bd590-1541">SQL</span></span>

* <span data-ttu-id="bd590-1542">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1542">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-1543">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-1543">VM</span></span>

* <span data-ttu-id="bd590-1544">Исправлено. Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="bd590-1544">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="bd590-1545">Исправлено. Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="bd590-1545">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="bd590-1546">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1546">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="bd590-1547">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="bd590-1547">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="bd590-1548">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="bd590-1548">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="bd590-1549">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-1549">August 31, 2017</span></span>

<span data-ttu-id="bd590-1550">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="bd590-1550">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="bd590-1551">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bd590-1551">Keyvault</span></span>

* <span data-ttu-id="bd590-1552">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1552">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="bd590-1553">Sf</span><span class="sxs-lookup"><span data-stu-id="bd590-1553">Sf</span></span>

* <span data-ttu-id="bd590-1554">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="bd590-1554">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-1555">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-1555">Storage</span></span>

* <span data-ttu-id="bd590-1556">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="bd590-1556">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="bd590-1557">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="bd590-1557">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="bd590-1558">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-1558">August 28, 2017</span></span>

<span data-ttu-id="bd590-1559">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="bd590-1559">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="bd590-1560">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="bd590-1560">CLI</span></span>

* <span data-ttu-id="bd590-1561">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="bd590-1561">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-1562">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-1562">ACS</span></span>

* <span data-ttu-id="bd590-1563">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="bd590-1563">Corrected preview regions</span></span>
* <span data-ttu-id="bd590-1564">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1564">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="bd590-1565">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="bd590-1565">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-1566">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-1566">Appservice</span></span>

* <span data-ttu-id="bd590-1567">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1567">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="bd590-1568">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1568">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="bd590-1569">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1569">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="bd590-1570">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="bd590-1570">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="bd590-1571">Исправлено. Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="bd590-1571">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="bd590-1572">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bd590-1572">IoT</span></span>

* <span data-ttu-id="bd590-1573">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="bd590-1573">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="bd590-1574">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-1574">Network</span></span>

* <span data-ttu-id="bd590-1575">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1575">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="bd590-1576">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1576">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="bd590-1577">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1577">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="bd590-1578">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1578">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="bd590-1579">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1579">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="bd590-1580">Профиль</span><span class="sxs-lookup"><span data-stu-id="bd590-1580">Profile</span></span>

* <span data-ttu-id="bd590-1581">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="bd590-1581">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="bd590-1582">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="bd590-1582">Service Fabric</span></span>

* <span data-ttu-id="bd590-1583">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="bd590-1583">Preview release</span></span>
* <span data-ttu-id="bd590-1584">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="bd590-1584">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="bd590-1585">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="bd590-1585">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="bd590-1586">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1586">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-1587">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-1587">Storage</span></span>

* <span data-ttu-id="bd590-1588">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="bd590-1588">Enabled setting blob tier</span></span>
* <span data-ttu-id="bd590-1589">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="bd590-1589">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="bd590-1590">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1590">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="bd590-1591">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="bd590-1591">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="bd590-1592">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1592">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="bd590-1593">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1593">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-1594">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-1594">VM</span></span>

* <span data-ttu-id="bd590-1595">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1595">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="bd590-1596">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1596">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="bd590-1597">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="bd590-1597">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="bd590-1598">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="bd590-1598">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="bd590-1599">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="bd590-1599">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="bd590-1600">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1600">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="bd590-1601">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-1601">August 15, 2017</span></span>

<span data-ttu-id="bd590-1602">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="bd590-1602">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-1603">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-1603">ACS</span></span>

* <span data-ttu-id="bd590-1604">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="bd590-1604">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-1605">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-1605">Appservice</span></span>

* <span data-ttu-id="bd590-1606">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="bd590-1606">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="bd590-1607">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="bd590-1607">Event Grid</span></span>

* <span data-ttu-id="bd590-1608">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="bd590-1608">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="bd590-1609">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-1609">August 11, 2017</span></span>

<span data-ttu-id="bd590-1610">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="bd590-1610">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-1611">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-1611">ACS</span></span>

* <span data-ttu-id="bd590-1612">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="bd590-1612">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="bd590-1613">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bd590-1613">Batch</span></span>

* <span data-ttu-id="bd590-1614">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="bd590-1614">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="bd590-1615">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="bd590-1615">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="bd590-1616">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bd590-1616">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="bd590-1617">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="bd590-1617">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="bd590-1618">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="bd590-1618">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="bd590-1619">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="bd590-1619">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="bd590-1620">Компонент</span><span class="sxs-lookup"><span data-stu-id="bd590-1620">Component</span></span>

* <span data-ttu-id="bd590-1621">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="bd590-1621">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="bd590-1622">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bd590-1622">Container</span></span>

* <span data-ttu-id="bd590-1623">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="bd590-1623">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="bd590-1624">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="bd590-1624">Data Lake Store</span></span>

* <span data-ttu-id="bd590-1625">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="bd590-1625">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="bd590-1626">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="bd590-1626">Event Grid</span></span>

* <span data-ttu-id="bd590-1627">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="bd590-1627">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="bd590-1628">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-1628">Network</span></span>

* <span data-ttu-id="bd590-1629">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="bd590-1629">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="bd590-1630">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1630">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="bd590-1631">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1631">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="bd590-1632">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1632">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="bd590-1633">Профиль</span><span class="sxs-lookup"><span data-stu-id="bd590-1633">Profile</span></span>

* <span data-ttu-id="bd590-1634">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="bd590-1634">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-1635">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-1635">Storage</span></span>

* <span data-ttu-id="bd590-1636">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="bd590-1636">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-1637">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-1637">VM</span></span>

* <span data-ttu-id="bd590-1638">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="bd590-1638">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="bd590-1639">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1639">Exposed `list-skus` command</span></span>
* <span data-ttu-id="bd590-1640">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="bd590-1640">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="bd590-1641">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="bd590-1641">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="bd590-1642">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="bd590-1642">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="bd590-1643">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-1643">July 28, 2017</span></span>

<span data-ttu-id="bd590-1644">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="bd590-1644">Version 2.0.12</span></span>

* <span data-ttu-id="bd590-1645">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bd590-1645">Added container commands</span></span>
* <span data-ttu-id="bd590-1646">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bd590-1646">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="bd590-1647">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-1647">Core</span></span>

* <span data-ttu-id="bd590-1648">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="bd590-1648">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="bd590-1649">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="bd590-1649">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="bd590-1650">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="bd590-1650">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="bd590-1651">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="bd590-1651">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="bd590-1652">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="bd590-1652">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="bd590-1653">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="bd590-1653">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="bd590-1654">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="bd590-1654">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="bd590-1655">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="bd590-1655">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="bd590-1656">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="bd590-1656">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="bd590-1657">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="bd590-1657">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="bd590-1658">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="bd590-1658">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="bd590-1659">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="bd590-1659">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="bd590-1660">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="bd590-1660">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="bd590-1661">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="bd590-1661">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="bd590-1662">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="bd590-1662">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="bd590-1663">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="bd590-1663">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="bd590-1664">ACR</span><span class="sxs-lookup"><span data-stu-id="bd590-1664">ACR</span></span>

* <span data-ttu-id="bd590-1665">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="bd590-1665">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="bd590-1666">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="bd590-1666">Support SKU update for managed registries</span></span>
* <span data-ttu-id="bd590-1667">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="bd590-1667">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="bd590-1668">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="bd590-1668">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="bd590-1669">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="bd590-1669">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="bd590-1670">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="bd590-1670">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-1671">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-1671">ACS</span></span>

* <span data-ttu-id="bd590-1672">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="bd590-1672">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-1673">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bd590-1673">Appservice</span></span>

* <span data-ttu-id="bd590-1674">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="bd590-1674">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="bd590-1675">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="bd590-1675">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="bd590-1676">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1676">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="bd590-1677">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="bd590-1677">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="bd590-1678">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="bd590-1678">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="bd590-1679">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="bd590-1679">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="bd590-1680">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="bd590-1680">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="bd590-1681">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="bd590-1681">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="bd590-1682">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="bd590-1682">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="bd590-1683">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1683">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="bd590-1684">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bd590-1684">Batch</span></span>

* <span data-ttu-id="bd590-1685">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="bd590-1685">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="bd590-1686">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1686">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="bd590-1687">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1687">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="bd590-1688">CDN</span><span class="sxs-lookup"><span data-stu-id="bd590-1688">CDN</span></span>

* <span data-ttu-id="bd590-1689">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="bd590-1689">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="bd590-1690">Облако</span><span class="sxs-lookup"><span data-stu-id="bd590-1690">Cloud</span></span>

* <span data-ttu-id="bd590-1691">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="bd590-1691">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="bd590-1692">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="bd590-1692">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="bd590-1693">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="bd590-1693">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="bd590-1694">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="bd590-1694">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="bd590-1695">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1695">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bd590-1696">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="bd590-1696">CosmosDB</span></span>

* <span data-ttu-id="bd590-1697">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="bd590-1697">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="bd590-1698">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="bd590-1698">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="bd590-1699">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="bd590-1699">Data Lake Analytics</span></span>

* <span data-ttu-id="bd590-1700">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1700">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="bd590-1701">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1701">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="bd590-1702">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1702">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="bd590-1703">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="bd590-1703">Data Lake Store</span></span>

* <span data-ttu-id="bd590-1704">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1704">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="bd590-1705">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="bd590-1705">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="bd590-1706">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1706">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="bd590-1707">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="bd590-1707">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="bd590-1708">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="bd590-1708">Interactive</span></span>

* <span data-ttu-id="bd590-1709">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="bd590-1709">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="bd590-1710">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="bd590-1710">Increased test coverage</span></span>
* <span data-ttu-id="bd590-1711">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="bd590-1711">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="bd590-1712">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="bd590-1712">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="bd590-1713">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="bd590-1713">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="bd590-1714">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="bd590-1714">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="bd590-1715">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="bd590-1715">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="bd590-1716">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1716">Added `--progress` flag</span></span>
* <span data-ttu-id="bd590-1717">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1717">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="bd590-1718">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="bd590-1718">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="bd590-1719">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bd590-1719">IoT</span></span>

* <span data-ttu-id="bd590-1720">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="bd590-1720">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="bd590-1721">(3934).</span><span class="sxs-lookup"><span data-stu-id="bd590-1721">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="bd590-1722">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bd590-1722">Key vault</span></span>

* <span data-ttu-id="bd590-1723">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="bd590-1723">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="bd590-1724">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1724">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="bd590-1725">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="bd590-1725">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="bd590-1726">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="bd590-1726">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="bd590-1727">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1727">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="bd590-1728">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="bd590-1728">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="bd590-1729">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="bd590-1729">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="bd590-1730">(3307).</span><span class="sxs-lookup"><span data-stu-id="bd590-1730">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="bd590-1731">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="bd590-1731">Lab</span></span>

* <span data-ttu-id="bd590-1732">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1732">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="bd590-1733">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1733">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="bd590-1734">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bd590-1734">Monitor</span></span>

* <span data-ttu-id="bd590-1735">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="bd590-1735">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="bd590-1736">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1736">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="bd590-1737">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1737">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="bd590-1738">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1738">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="bd590-1739">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1739">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="bd590-1740">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="bd590-1740">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="bd590-1741">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="bd590-1741">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="bd590-1742">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="bd590-1742">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="bd590-1743">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="bd590-1743">`location` no longer required</span></span>
  * <span data-ttu-id="bd590-1744">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="bd590-1744">Add name and ID support for target</span></span>
  * <span data-ttu-id="bd590-1745">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="bd590-1745">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="bd590-1746">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="bd590-1746">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="bd590-1747">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="bd590-1747">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="bd590-1748">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="bd590-1748">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="bd590-1749">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1749">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="bd590-1750">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1750">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="bd590-1751">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-1751">Network</span></span>

* <span data-ttu-id="bd590-1752">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1752">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="bd590-1753">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1753">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="bd590-1754">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="bd590-1754">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="bd590-1755">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1755">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="bd590-1756">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1756">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="bd590-1757">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1757">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="bd590-1758">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1758">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="bd590-1759">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1759">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="bd590-1760">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1760">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="bd590-1761">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1761">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="bd590-1762">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1762">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="bd590-1763">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1763">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="bd590-1764">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1764">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="bd590-1765">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1765">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="bd590-1766">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1766">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="bd590-1767">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1767">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="bd590-1768">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="bd590-1768">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="bd590-1769">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1769">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="bd590-1770">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1770">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="bd590-1771">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1771">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="bd590-1772">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1772">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="bd590-1773">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1773">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="bd590-1774">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1774">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="bd590-1775">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="bd590-1775">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="bd590-1776">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="bd590-1776">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="bd590-1777">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="bd590-1777">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="bd590-1778">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="bd590-1778">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="bd590-1779">Профиль</span><span class="sxs-lookup"><span data-stu-id="bd590-1779">Profile</span></span>

* <span data-ttu-id="bd590-1780">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="bd590-1780">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="bd590-1781">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="bd590-1781">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="bd590-1782">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="bd590-1782">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="bd590-1783">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="bd590-1783">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="bd590-1784">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="bd590-1784">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="bd590-1785">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="bd590-1785">RDBMS</span></span>

* <span data-ttu-id="bd590-1786">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="bd590-1786">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="bd590-1787">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="bd590-1787">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="bd590-1788">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="bd590-1788">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="bd590-1789">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="bd590-1789">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="bd590-1790">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bd590-1790">Resource</span></span>

* <span data-ttu-id="bd590-1791">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1791">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="bd590-1792">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1792">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="bd590-1793">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1793">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="bd590-1794">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1794">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="bd590-1795">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="bd590-1795">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="bd590-1796">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1796">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="bd590-1797">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="bd590-1797">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="bd590-1798">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1798">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="bd590-1799">Роль</span><span class="sxs-lookup"><span data-stu-id="bd590-1799">Role</span></span>

* <span data-ttu-id="bd590-1800">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="bd590-1800">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="bd590-1801">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="bd590-1801">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="bd590-1802">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="bd590-1802">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="bd590-1803">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="bd590-1803">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="bd590-1804">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1804">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="bd590-1805">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="bd590-1805">Service Fabric</span></span>
* <span data-ttu-id="bd590-1806">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="bd590-1806">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="bd590-1807">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="bd590-1807">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="bd590-1808">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="bd590-1808">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="bd590-1809">SQL</span><span class="sxs-lookup"><span data-stu-id="bd590-1809">SQL</span></span>

* <span data-ttu-id="bd590-1810">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1810">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="bd590-1811">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1811">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="bd590-1812">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1812">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-1813">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-1813">Storage</span></span>

* <span data-ttu-id="bd590-1814">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="bd590-1814">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="bd590-1815">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="bd590-1815">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="bd590-1816">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="bd590-1816">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="bd590-1817">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="bd590-1817">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="bd590-1818">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="bd590-1818">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="bd590-1819">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="bd590-1819">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-1820">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-1820">VM</span></span>

* <span data-ttu-id="bd590-1821">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="bd590-1821">Support configuring nsg</span></span>
* <span data-ttu-id="bd590-1822">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="bd590-1822">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="bd590-1823">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="bd590-1823">Support managed service identities</span></span>
* <span data-ttu-id="bd590-1824">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1824">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="bd590-1825">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="bd590-1825">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="bd590-1826">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-1826">May 10, 2017</span></span>

<span data-ttu-id="bd590-1827">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="bd590-1827">Version 2.0.6</span></span>

* <span data-ttu-id="bd590-1828">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="bd590-1828">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="bd590-1829">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="bd590-1829">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="bd590-1830">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="bd590-1830">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="bd590-1831">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="bd590-1831">Include Cognitive Services module</span></span>
* <span data-ttu-id="bd590-1832">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="bd590-1832">Include Service Fabric module</span></span>
* <span data-ttu-id="bd590-1833">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="bd590-1833">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="bd590-1834">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="bd590-1834">Add support for CDN commands</span></span>
* <span data-ttu-id="bd590-1835">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="bd590-1835">Remove Container module</span></span>
* <span data-ttu-id="bd590-1836">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1836">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="bd590-1837">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1837">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="bd590-1838">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-1838">Core</span></span>

* <span data-ttu-id="bd590-1839">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="bd590-1839">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="bd590-1840">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1840">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="bd590-1841">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1841">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="bd590-1842">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1842">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="bd590-1843">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1843">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="bd590-1844">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1844">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="bd590-1845">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1845">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="bd590-1846">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1846">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="bd590-1847">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1847">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="bd590-1848">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="bd590-1848">core: Improved performance</span></span>
* <span data-ttu-id="bd590-1849">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="bd590-1849">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="bd590-1850">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="bd590-1850">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-1851">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-1851">ACS</span></span>

* <span data-ttu-id="bd590-1852">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="bd590-1852">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="bd590-1853">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="bd590-1853">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="bd590-1854">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="bd590-1854">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="bd590-1855">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1855">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-1856">AppService</span><span class="sxs-lookup"><span data-stu-id="bd590-1856">AppService</span></span>

* <span data-ttu-id="bd590-1857">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="bd590-1857">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="bd590-1858">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="bd590-1858">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="bd590-1859">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="bd590-1859">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="bd590-1860">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="bd590-1860">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="bd590-1861">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="bd590-1861">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="bd590-1862">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1862">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="bd590-1863">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="bd590-1863">support slot swap with preview</span></span>
* <span data-ttu-id="bd590-1864">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1864">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="bd590-1865">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1865">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bd590-1866">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="bd590-1866">CosmosDB</span></span>

* <span data-ttu-id="bd590-1867">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="bd590-1867">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="bd590-1868">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="bd590-1868">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="bd590-1869">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="bd590-1869">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="bd590-1870">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="bd590-1870">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="bd590-1871">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="bd590-1871">Data Lake Analytics</span></span>

* <span data-ttu-id="bd590-1872">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="bd590-1872">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="bd590-1873">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="bd590-1873">Add support for new catalog item type: package.</span></span> <span data-ttu-id="bd590-1874">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1874">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="bd590-1875">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="bd590-1875">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="bd590-1876">Таблица</span><span class="sxs-lookup"><span data-stu-id="bd590-1876">Table</span></span>
  * <span data-ttu-id="bd590-1877">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="bd590-1877">Table valued function</span></span>
  * <span data-ttu-id="bd590-1878">Просмотр</span><span class="sxs-lookup"><span data-stu-id="bd590-1878">View</span></span>
  * <span data-ttu-id="bd590-1879">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="bd590-1879">Table Statistics.</span></span> <span data-ttu-id="bd590-1880">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="bd590-1880">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="bd590-1881">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="bd590-1881">Data Lake Store</span></span>

* <span data-ttu-id="bd590-1882">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="bd590-1882">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="bd590-1883">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1883">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="bd590-1884">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="bd590-1884">missed help for access show.</span></span> <span data-ttu-id="bd590-1885">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="bd590-1885">adding it.</span></span> <span data-ttu-id="bd590-1886">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="bd590-1886">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="bd590-1887">Поиск</span><span class="sxs-lookup"><span data-stu-id="bd590-1887">Find</span></span>

* <span data-ttu-id="bd590-1888">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="bd590-1888">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="bd590-1889">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bd590-1889">KeyVault</span></span>

* <span data-ttu-id="bd590-1890">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="bd590-1890">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="bd590-1891">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="bd590-1891">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="bd590-1892">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="bd590-1892">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="bd590-1893">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="bd590-1893">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="bd590-1894">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1894">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="bd590-1895">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="bd590-1895">Lab</span></span>

* <span data-ttu-id="bd590-1896">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="bd590-1896">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="bd590-1897">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="bd590-1897">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="bd590-1898">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="bd590-1898">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="bd590-1899">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="bd590-1899">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="bd590-1900">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="bd590-1900">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="bd590-1901">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bd590-1901">Monitor</span></span>

* <span data-ttu-id="bd590-1902">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1902">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="bd590-1903">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1903">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="bd590-1904">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-1904">Network</span></span>

* <span data-ttu-id="bd590-1905">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1905">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="bd590-1906">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1906">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="bd590-1907">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="bd590-1907">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="bd590-1908">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="bd590-1908">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="bd590-1909">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="bd590-1909">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="bd590-1910">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="bd590-1910">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="bd590-1911">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="bd590-1911">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="bd590-1912">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="bd590-1912">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="bd590-1913">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1913">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="bd590-1914">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="bd590-1914">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="bd590-1915">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1915">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="bd590-1916">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1916">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="bd590-1917">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="bd590-1917">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="bd590-1918">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="bd590-1918">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="bd590-1919">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="bd590-1919">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="bd590-1920">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="bd590-1920">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="bd590-1921">Профиль</span><span class="sxs-lookup"><span data-stu-id="bd590-1921">Profile</span></span>

* <span data-ttu-id="bd590-1922">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1922">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="bd590-1923">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1923">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="bd590-1924">Redis</span><span class="sxs-lookup"><span data-stu-id="bd590-1924">Redis</span></span>

* <span data-ttu-id="bd590-1925">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="bd590-1925">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="bd590-1926">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="bd590-1926">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="bd590-1927">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bd590-1927">Resource</span></span>

* <span data-ttu-id="bd590-1928">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1928">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="bd590-1929">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1929">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="bd590-1930">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1930">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="bd590-1931">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="bd590-1931">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="bd590-1932">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="bd590-1932">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="bd590-1933">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="bd590-1933">Add docs for az lock update.</span></span> <span data-ttu-id="bd590-1934">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="bd590-1934">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="bd590-1935">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="bd590-1935">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="bd590-1936">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="bd590-1936">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="bd590-1937">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="bd590-1937">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="bd590-1938">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="bd590-1938">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="bd590-1939">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1939">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="bd590-1940">Роль</span><span class="sxs-lookup"><span data-stu-id="bd590-1940">Role</span></span>

* <span data-ttu-id="bd590-1941">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1941">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="bd590-1942">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1942">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="bd590-1943">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1943">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="bd590-1944">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="bd590-1944">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="bd590-1945">SQL</span><span class="sxs-lookup"><span data-stu-id="bd590-1945">SQL</span></span>

* <span data-ttu-id="bd590-1946">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="bd590-1946">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="bd590-1947">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1947">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="bd590-1948">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-1948">Storage</span></span>

* <span data-ttu-id="bd590-1949">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="bd590-1949">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="bd590-1950">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="bd590-1950">Add support for incremental blob copy</span></span>
* <span data-ttu-id="bd590-1951">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="bd590-1951">Add support for large block blob upload</span></span>
* <span data-ttu-id="bd590-1952">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="bd590-1952">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-1953">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-1953">VM</span></span>

* <span data-ttu-id="bd590-1954">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="bd590-1954">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="bd590-1955">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="bd590-1955">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="bd590-1956">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="bd590-1956">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="bd590-1957">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="bd590-1957">az vm/vmss disk</span></span>
  3. <span data-ttu-id="bd590-1958">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="bd590-1958">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="bd590-1959">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="bd590-1959">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="bd590-1960">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1960">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="bd590-1961">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-1961">April 3, 2017</span></span>

<span data-ttu-id="bd590-1962">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="bd590-1962">Version 2.0.2</span></span>

<span data-ttu-id="bd590-1963">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="bd590-1963">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="bd590-1964">Core</span><span class="sxs-lookup"><span data-stu-id="bd590-1964">Core</span></span>

* <span data-ttu-id="bd590-1965">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bd590-1965">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="bd590-1966">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1966">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="bd590-1967">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1967">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="bd590-1968">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1968">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="bd590-1969">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1969">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="bd590-1970">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="bd590-1970">Add prompting for missing template parameters.</span></span> <span data-ttu-id="bd590-1971">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1971">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="bd590-1972">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bd590-1972">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="bd590-1973">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="bd590-1973">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="bd590-1974">ACS</span><span class="sxs-lookup"><span data-stu-id="bd590-1974">ACS</span></span>

* <span data-ttu-id="bd590-1975">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1975">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="bd590-1976">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="bd590-1976">Add support for ssh key password prompting.</span></span> <span data-ttu-id="bd590-1977">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1977">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="bd590-1978">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="bd590-1978">Add support for windows clusters.</span></span> <span data-ttu-id="bd590-1979">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1979">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="bd590-1980">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="bd590-1980">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="bd590-1981">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1981">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="bd590-1982">AppService</span><span class="sxs-lookup"><span data-stu-id="bd590-1982">AppService</span></span>

* <span data-ttu-id="bd590-1983">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1983">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="bd590-1984">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1984">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="bd590-1985">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1985">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="bd590-1986">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1986">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="bd590-1987">Data Lake</span><span class="sxs-lookup"><span data-stu-id="bd590-1987">DataLake</span></span>

* <span data-ttu-id="bd590-1988">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="bd590-1988">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="bd590-1989">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="bd590-1989">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="bd590-1990">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="bd590-1990">DocuemntDB</span></span>

* <span data-ttu-id="bd590-1991">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1991">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="bd590-1992">ВМ</span><span class="sxs-lookup"><span data-stu-id="bd590-1992">VM</span></span>

* <span data-ttu-id="bd590-1993">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1993">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="bd590-1994">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1994">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="bd590-1995">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1995">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="bd590-1996">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1996">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="bd590-1997">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1997">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="bd590-1998">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1998">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="bd590-1999">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="bd590-1999">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="bd590-2000">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bd590-2000">February 27, 2017</span></span>

<span data-ttu-id="bd590-2001">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="bd590-2001">Version 2.0.0</span></span>

<span data-ttu-id="bd590-2002">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="bd590-2002">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="bd590-2003">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="bd590-2003">Container Service (acs)</span></span>
- <span data-ttu-id="bd590-2004">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="bd590-2004">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="bd590-2005">Сеть</span><span class="sxs-lookup"><span data-stu-id="bd590-2005">Networking</span></span>
- <span data-ttu-id="bd590-2006">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bd590-2006">Storage</span></span>

<span data-ttu-id="bd590-2007">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="bd590-2007">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="bd590-2008">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="bd590-2008">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="bd590-2009">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="bd590-2009">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="bd590-2010">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="bd590-2010">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="bd590-2011">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="bd590-2011">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="bd590-2012">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="bd590-2012">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="bd590-2013">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="bd590-2013">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="bd590-2014">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="bd590-2014">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="bd590-2015">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="bd590-2015">Provide feedback from the command line with the `az feedback` command</span></span>

