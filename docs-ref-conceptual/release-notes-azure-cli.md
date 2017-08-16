---
title: "Заметки о выпуске Azure CLI 2.0"
description: "Узнайте о последних обновлениях в Azure CLI 2.0"
keywords: "Azure CLI 2.0, заметки о выпуске"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: 3bd4b9c059da3b841fc0757a11bc7ce78ec64b08
ms.sourcegitcommit: 66d997a5afcf32143a4d4817ec1608cbdf58a59f
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="a700b-104">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="a700b-104">Azure CLI 2.0 release notes</span></span>

## <a name="may-10-2017"></a><span data-ttu-id="a700b-105">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a700b-105">May 10, 2017</span></span>

<span data-ttu-id="a700b-106">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="a700b-106">Version 2.0.6</span></span>

* <span data-ttu-id="a700b-107">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="a700b-107">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="a700b-108">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="a700b-108">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="a700b-109">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="a700b-109">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="a700b-110">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="a700b-110">Include Cognitive Services module.</span></span>
* <span data-ttu-id="a700b-111">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="a700b-111">Include Service Fabric module.</span></span>
* <span data-ttu-id="a700b-112">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="a700b-112">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="a700b-113">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="a700b-113">Add support for CDN commands.</span></span>
* <span data-ttu-id="a700b-114">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="a700b-114">Remove Container module.</span></span>
* <span data-ttu-id="a700b-115">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="a700b-115">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="a700b-116">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="a700b-116">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="a700b-117">Core</span><span class="sxs-lookup"><span data-stu-id="a700b-117">Core</span></span>

* <span data-ttu-id="a700b-118">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="a700b-118">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="a700b-119">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="a700b-119">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="a700b-120">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="a700b-120">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="a700b-121">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="a700b-121">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="a700b-122">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="a700b-122">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="a700b-123">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="a700b-123">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="a700b-124">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="a700b-124">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="a700b-125">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="a700b-125">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="a700b-126">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="a700b-126">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="a700b-127">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="a700b-127">core: Improved performance</span></span>
* <span data-ttu-id="a700b-128">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="a700b-128">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="a700b-129">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="a700b-129">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="a700b-130">ACS</span><span class="sxs-lookup"><span data-stu-id="a700b-130">ACS</span></span>

* <span data-ttu-id="a700b-131">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="a700b-131">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="a700b-132">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="a700b-132">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="a700b-133">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="a700b-133">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="a700b-134">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="a700b-134">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="a700b-135">AppService</span><span class="sxs-lookup"><span data-stu-id="a700b-135">AppService</span></span>

* <span data-ttu-id="a700b-136">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="a700b-136">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="a700b-137">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="a700b-137">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="a700b-138">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="a700b-138">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="a700b-139">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="a700b-139">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="a700b-140">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="a700b-140">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="a700b-141">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="a700b-141">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="a700b-142">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="a700b-142">support slot swap with preview</span></span>
* <span data-ttu-id="a700b-143">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="a700b-143">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="a700b-144">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="a700b-144">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a700b-145">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a700b-145">CosmosDB</span></span>

* <span data-ttu-id="a700b-146">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="a700b-146">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="a700b-147">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="a700b-147">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="a700b-148">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="a700b-148">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="a700b-149">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="a700b-149">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a700b-150">Аналитика озера данных</span><span class="sxs-lookup"><span data-stu-id="a700b-150">Data Lake Analytics</span></span>

* <span data-ttu-id="a700b-151">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="a700b-151">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="a700b-152">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="a700b-152">Add support for new catalog item type: package.</span></span> <span data-ttu-id="a700b-153">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="a700b-153">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="a700b-154">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="a700b-154">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="a700b-155">Таблица</span><span class="sxs-lookup"><span data-stu-id="a700b-155">Table</span></span>
  * <span data-ttu-id="a700b-156">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="a700b-156">Table valued function</span></span>
  * <span data-ttu-id="a700b-157">Просмотр</span><span class="sxs-lookup"><span data-stu-id="a700b-157">View</span></span>
  * <span data-ttu-id="a700b-158">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="a700b-158">Table Statistics.</span></span> <span data-ttu-id="a700b-159">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="a700b-159">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a700b-160">Хранилище озера данных</span><span class="sxs-lookup"><span data-stu-id="a700b-160">Data Lake Store</span></span>

* <span data-ttu-id="a700b-161">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="a700b-161">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="a700b-162">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="a700b-162">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="a700b-163">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="a700b-163">missed help for access show.</span></span> <span data-ttu-id="a700b-164">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="a700b-164">adding it.</span></span> <span data-ttu-id="a700b-165">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="a700b-165">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="a700b-166">Поиск</span><span class="sxs-lookup"><span data-stu-id="a700b-166">Find</span></span>

* <span data-ttu-id="a700b-167">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="a700b-167">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="a700b-168">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a700b-168">KeyVault</span></span>

* <span data-ttu-id="a700b-169">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="a700b-169">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="a700b-170">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="a700b-170">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="a700b-171">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="a700b-171">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="a700b-172">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="a700b-172">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="a700b-173">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="a700b-173">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="a700b-174">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="a700b-174">Lab</span></span>

* <span data-ttu-id="a700b-175">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a700b-175">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="a700b-176">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a700b-176">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="a700b-177">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a700b-177">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="a700b-178">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a700b-178">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="a700b-179">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a700b-179">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="a700b-180">Монитор</span><span class="sxs-lookup"><span data-stu-id="a700b-180">Monitor</span></span>

* <span data-ttu-id="a700b-181">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="a700b-181">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="a700b-182">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="a700b-182">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="a700b-183">Сеть</span><span class="sxs-lookup"><span data-stu-id="a700b-183">Network</span></span>

* <span data-ttu-id="a700b-184">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="a700b-184">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="a700b-185">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="a700b-185">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="a700b-186">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="a700b-186">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="a700b-187">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="a700b-187">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="a700b-188">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="a700b-188">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="a700b-189">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="a700b-189">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="a700b-190">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="a700b-190">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="a700b-191">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="a700b-191">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="a700b-192">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="a700b-192">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="a700b-193">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="a700b-193">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="a700b-194">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="a700b-194">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="a700b-195">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="a700b-195">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="a700b-196">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="a700b-196">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="a700b-197">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="a700b-197">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="a700b-198">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="a700b-198">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="a700b-199">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="a700b-199">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="a700b-200">Профиль</span><span class="sxs-lookup"><span data-stu-id="a700b-200">Profile</span></span>

* <span data-ttu-id="a700b-201">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="a700b-201">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="a700b-202">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="a700b-202">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="a700b-203">Redis</span><span class="sxs-lookup"><span data-stu-id="a700b-203">Redis</span></span>

* <span data-ttu-id="a700b-204">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="a700b-204">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="a700b-205">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="a700b-205">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="a700b-206">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a700b-206">Resource</span></span>

* <span data-ttu-id="a700b-207">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="a700b-207">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="a700b-208">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="a700b-208">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="a700b-209">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="a700b-209">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="a700b-210">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="a700b-210">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="a700b-211">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="a700b-211">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="a700b-212">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="a700b-212">Add docs for az lock update.</span></span> <span data-ttu-id="a700b-213">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="a700b-213">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="a700b-214">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="a700b-214">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="a700b-215">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="a700b-215">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="a700b-216">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="a700b-216">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="a700b-217">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="a700b-217">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="a700b-218">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="a700b-218">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="a700b-219">Роль</span><span class="sxs-lookup"><span data-stu-id="a700b-219">Role</span></span>

* <span data-ttu-id="a700b-220">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="a700b-220">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="a700b-221">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="a700b-221">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="a700b-222">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="a700b-222">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="a700b-223">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="a700b-223">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="a700b-224">SQL</span><span class="sxs-lookup"><span data-stu-id="a700b-224">SQL</span></span>

* <span data-ttu-id="a700b-225">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="a700b-225">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="a700b-226">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="a700b-226">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="a700b-227">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a700b-227">Storage</span></span>

* <span data-ttu-id="a700b-228">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="a700b-228">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="a700b-229">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="a700b-229">Add support for incremental blob copy</span></span>
* <span data-ttu-id="a700b-230">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="a700b-230">Add support for large block blob upload</span></span>
* <span data-ttu-id="a700b-231">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="a700b-231">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="a700b-232">ВМ</span><span class="sxs-lookup"><span data-stu-id="a700b-232">VM</span></span>

* <span data-ttu-id="a700b-233">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="a700b-233">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="a700b-234">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="a700b-234">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="a700b-235">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="a700b-235">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="a700b-236">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="a700b-236">az vm/vmss disk</span></span>
  3. <span data-ttu-id="a700b-237">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="a700b-237">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="a700b-238">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="a700b-238">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="a700b-239">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="a700b-239">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="a700b-240">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a700b-240">April 3, 2017</span></span>

<span data-ttu-id="a700b-241">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="a700b-241">Version 2.0.2</span></span>

<span data-ttu-id="a700b-242">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="a700b-242">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="a700b-243">Core</span><span class="sxs-lookup"><span data-stu-id="a700b-243">Core</span></span>

* <span data-ttu-id="a700b-244">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a700b-244">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="a700b-245">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="a700b-245">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="a700b-246">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="a700b-246">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="a700b-247">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="a700b-247">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a700b-248">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="a700b-248">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="a700b-249">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="a700b-249">Add prompting for missing template parameters.</span></span> <span data-ttu-id="a700b-250">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="a700b-250">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="a700b-251">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a700b-251">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="a700b-252">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="a700b-252">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="a700b-253">ACS</span><span class="sxs-lookup"><span data-stu-id="a700b-253">ACS</span></span>

* <span data-ttu-id="a700b-254">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="a700b-254">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="a700b-255">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="a700b-255">Add support for ssh key password prompting.</span></span> <span data-ttu-id="a700b-256">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="a700b-256">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="a700b-257">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="a700b-257">Add support for windows clusters.</span></span> <span data-ttu-id="a700b-258">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="a700b-258">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="a700b-259">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="a700b-259">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="a700b-260">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="a700b-260">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="a700b-261">AppService</span><span class="sxs-lookup"><span data-stu-id="a700b-261">AppService</span></span>

* <span data-ttu-id="a700b-262">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="a700b-262">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="a700b-263">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="a700b-263">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="a700b-264">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="a700b-264">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="a700b-265">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="a700b-265">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="a700b-266">DataLake</span><span class="sxs-lookup"><span data-stu-id="a700b-266">DataLake</span></span>

* <span data-ttu-id="a700b-267">Первоначальный выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="a700b-267">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="a700b-268">Первоначальный выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="a700b-268">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="a700b-269">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="a700b-269">DocuemntDB</span></span>

* <span data-ttu-id="a700b-270">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="a700b-270">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="a700b-271">ВМ</span><span class="sxs-lookup"><span data-stu-id="a700b-271">VM</span></span>

* <span data-ttu-id="a700b-272">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="a700b-272">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="a700b-273">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="a700b-273">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="a700b-274">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="a700b-274">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="a700b-275">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="a700b-275">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a700b-276">Масштабируемый набор виртуальных машин: добавлена поддержка * для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="a700b-276">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="a700b-277">Добавлена команда --secrets для виртуальных машин и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="a700b-277">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="a700b-278">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="a700b-278">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="a700b-279">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a700b-279">February 27, 2017</span></span>

<span data-ttu-id="a700b-280">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="a700b-280">Version 2.0.0</span></span>

<span data-ttu-id="a700b-281">Этот первый общедоступный выпуск Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="a700b-281">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="a700b-282">Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="a700b-282">General availability applies to these command modules:</span></span>
- <span data-ttu-id="a700b-283">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="a700b-283">Container Service (acs)</span></span>
- <span data-ttu-id="a700b-284">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="a700b-284">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="a700b-285">Сеть</span><span class="sxs-lookup"><span data-stu-id="a700b-285">Networking</span></span>
- <span data-ttu-id="a700b-286">Хранилище</span><span class="sxs-lookup"><span data-stu-id="a700b-286">Storage</span></span>

<span data-ttu-id="a700b-287">Эти командные модули могут использоваться в рабочих средах и поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания.</span><span class="sxs-lookup"><span data-stu-id="a700b-287">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="a700b-288">Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="a700b-288">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="a700b-289">Вы можете задавать вопросы на сайте [StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="a700b-289">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
<span data-ttu-id="a700b-290">Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="a700b-290">You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="a700b-291">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="a700b-291">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="a700b-292">Чтобы проверить версию интерфейса командной строки, используйте `az --version`.</span><span class="sxs-lookup"><span data-stu-id="a700b-292">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="a700b-293">В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="a700b-293">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="a700b-294">Некоторые командные модули имеют постфикс b*n* или rc*n*.</span><span class="sxs-lookup"><span data-stu-id="a700b-294">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="a700b-295">Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="a700b-295">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="a700b-296">У нас также есть предварительные ежедневные сборки интерфейса командной строки.</span><span class="sxs-lookup"><span data-stu-id="a700b-296">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="a700b-297">Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="a700b-297">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="a700b-298">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="a700b-298">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="a700b-299">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="a700b-299">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="a700b-300">обратившись к специалистам группы разработчиков продукта по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com);</span><span class="sxs-lookup"><span data-stu-id="a700b-300">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="a700b-301">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="a700b-301">Provide feedback from the command line with the `az feedback` command.</span></span>

