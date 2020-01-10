---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/07/2020
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 9fc54add3bfb2a75d1912c47f0a2571d9d065ec0
ms.sourcegitcommit: 5646008e7a521dd9a8a627418f57bd92ee180352
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "75694280"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="dc563-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="dc563-103">Azure CLI release notes</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="dc563-104">7 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-104">January 07, 2020</span></span>

<span data-ttu-id="dc563-105">Версия 2.0.79</span><span class="sxs-lookup"><span data-stu-id="dc563-105">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-106">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-106">ACR</span></span>

* <span data-ttu-id="dc563-107">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --os для команд acr build, acr task create/update, acr run и acr pack.</span><span class="sxs-lookup"><span data-stu-id="dc563-107">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="dc563-108">Вместо этого используется параметр --platform.</span><span class="sxs-lookup"><span data-stu-id="dc563-108">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="dc563-109">AppConfig</span><span class="sxs-lookup"><span data-stu-id="dc563-109">AppConfig</span></span>

* <span data-ttu-id="dc563-110">Добавлена поддержка импорта и экспорта флагов функций.</span><span class="sxs-lookup"><span data-stu-id="dc563-110">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="dc563-111">Добавлена новая команда az appconfig kv set-keyvault для создания ссылки на хранилище ключей.</span><span class="sxs-lookup"><span data-stu-id="dc563-111">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="dc563-112">Добавлена поддержка различных соглашений об именовании при экспорте флагов функций в файл.</span><span class="sxs-lookup"><span data-stu-id="dc563-112">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-113">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-113">AppService</span></span>

* <span data-ttu-id="dc563-114">Устранена проблема № 7154: обновлена документация по команде <> — теперь в ней используются обратные, а не одинарные кавычки.</span><span class="sxs-lookup"><span data-stu-id="dc563-114">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="dc563-115">Устранена проблема № 11287 (webapp up): по умолчанию для приложения, созданного с использованием этого флага, должен быть включен SSL.</span><span class="sxs-lookup"><span data-stu-id="dc563-115">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="dc563-116">Устранена проблема № 11592: добавлен флаг az webapp up для статических сайтов HTML.</span><span class="sxs-lookup"><span data-stu-id="dc563-116">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="dc563-117">ARM</span><span class="sxs-lookup"><span data-stu-id="dc563-117">ARM</span></span>

* <span data-ttu-id="dc563-118">Исправлена ошибка с командой `az resource tag`: невозможно было обновить теги хранилища Служб восстановления.</span><span class="sxs-lookup"><span data-stu-id="dc563-118">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="dc563-119">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="dc563-119">Backup</span></span>

* <span data-ttu-id="dc563-120">Добавлена новая команда backup protection undelete для включения функции обратимого удаления рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="dc563-120">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="dc563-121">Добавлен новый параметр --soft-delete-feature-state для команды set backup-properties.</span><span class="sxs-lookup"><span data-stu-id="dc563-121">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="dc563-122">Добавлена поддержка исключения диска для рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="dc563-122">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="dc563-123">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="dc563-123">Compute</span></span>

* <span data-ttu-id="dc563-124">Исправлен сбой `vm create` в профиле Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="dc563-124">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="dc563-125">Добавлена поддержка определений списков и метрик запросов для виртуальной машины (vm monitor metrics tail/list-definitions).</span><span class="sxs-lookup"><span data-stu-id="dc563-125">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="dc563-126">Добавлено новое действия повторного применения команды az vm</span><span class="sxs-lookup"><span data-stu-id="dc563-126">Add new reapply command action for az vm</span></span>

### <a name="misc"></a><span data-ttu-id="dc563-127">Прочее</span><span class="sxs-lookup"><span data-stu-id="dc563-127">Misc.</span></span>

* <span data-ttu-id="dc563-128">Добавлена команда `az version show` предварительного просмотра для отображения версий модулей и расширений Azure CLI в формате JSON по умолчанию или в формате, настроенном с помощью параметра --output</span><span class="sxs-lookup"><span data-stu-id="dc563-128">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="dc563-129">Центры событий</span><span class="sxs-lookup"><span data-stu-id="dc563-129">Event Hubs</span></span>

* <span data-ttu-id="dc563-130">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az eventhubs eventhub update и az eventhubs eventhub create.</span><span class="sxs-lookup"><span data-stu-id="dc563-130">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="dc563-131">Данный параметр недопустим для сущностей концентратора событий.</span><span class="sxs-lookup"><span data-stu-id="dc563-131">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="dc563-132">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="dc563-132">Service Bus</span></span>

* <span data-ttu-id="dc563-133">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az servicebus topic create, az servicebus topic update, az servicebus queue create и az servicebus queue update.</span><span class="sxs-lookup"><span data-stu-id="dc563-133">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="dc563-134">Этот параметр является недопустимым для разделов и очередей служебной шины.</span><span class="sxs-lookup"><span data-stu-id="dc563-134">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="dc563-135">RBAC</span><span class="sxs-lookup"><span data-stu-id="dc563-135">RBAC</span></span>

* <span data-ttu-id="dc563-136">Устранена проблема № 11712: команда `az ad app/sp show` не возвращала код выхода 3, если приложение или субъект-служба не существует.</span><span class="sxs-lookup"><span data-stu-id="dc563-136">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-137">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-137">Storage</span></span>

* <span data-ttu-id="dc563-138">`az storage account create`: удален флаг предварительного просмотра для параметра --enable-hierarchical-namespace.</span><span class="sxs-lookup"><span data-stu-id="dc563-138">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="dc563-139">Хранилище azure-mgmt-storage обновлено до версии 7.0.0 для использования API версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="dc563-139">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="dc563-140">Добавлены новые параметры (`--enable-delete-retention` и `--delete-retention-days`) для поддержки управления политикой хранения удаленных свойств службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="dc563-140">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="dc563-141">17 декабря 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-141">December 17, 2019</span></span>

<span data-ttu-id="dc563-142">2.0.78</span><span class="sxs-lookup"><span data-stu-id="dc563-142">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-143">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-143">ACR</span></span>

* <span data-ttu-id="dc563-144">Добавлена поддержка локального контекста во время выполнения задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="dc563-144">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-145">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-145">ACS</span></span>

* <span data-ttu-id="dc563-146">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде az openshift create параметр `--workspace-resource-id` переименован на `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="dc563-146">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="dc563-147">AMS</span><span class="sxs-lookup"><span data-stu-id="dc563-147">AMS</span></span>

* <span data-ttu-id="dc563-148">Команды show обновлены для возвращения ответа 3, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="dc563-148">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="dc563-149">AppConfig</span><span class="sxs-lookup"><span data-stu-id="dc563-149">AppConfig</span></span>

* <span data-ttu-id="dc563-150">Исправлена ошибка, возникающая при добавлении api-version в URL-адрес запроса.</span><span class="sxs-lookup"><span data-stu-id="dc563-150">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="dc563-151">Имеющееся решение не работает с разбивкой на страницы.</span><span class="sxs-lookup"><span data-stu-id="dc563-151">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="dc563-152">Добавлена поддержка отображения языков, кроме английского, так как наша внутренняя служба поддерживает Юникод для глобализации.</span><span class="sxs-lookup"><span data-stu-id="dc563-152">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-153">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-153">AppService</span></span>

* <span data-ttu-id="dc563-154">Устранена проблема № 11217 (webapp): теперь команда az webapp config ssl upload поддерживает параметр слота.</span><span class="sxs-lookup"><span data-stu-id="dc563-154">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="dc563-155">Устранена проблема № 10965. Ошибка: Имя не может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="dc563-155">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="dc563-156">Разрешено удаление по IP-адресу и подсети.</span><span class="sxs-lookup"><span data-stu-id="dc563-156">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="dc563-157">Добавлена поддержка импорта сертификатов из хранилища ключей: `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="dc563-157">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="dc563-158">ARM</span><span class="sxs-lookup"><span data-stu-id="dc563-158">ARM</span></span>

* <span data-ttu-id="dc563-159">Обновлен пакет ресурсов azure-mgmt-resource для использования версии 6.0.0</span><span class="sxs-lookup"><span data-stu-id="dc563-159">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="dc563-160">Добавлена межклиентская поддержка команды `az group deployment create` путем добавления нового параметра `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="dc563-160">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="dc563-161">Добавлен новый параметр `--metadata` для поддержки добавления метаданных определений наборов политик.</span><span class="sxs-lookup"><span data-stu-id="dc563-161">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="dc563-162">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="dc563-162">Backup</span></span>

* <span data-ttu-id="dc563-163">Добавлена поддержка резервного копирования для рабочей нагрузки SQL и SAP HANA.</span><span class="sxs-lookup"><span data-stu-id="dc563-163">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="dc563-164">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="dc563-164">BotService</span></span>

* <span data-ttu-id="dc563-165">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг --version из предварительной версии команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="dc563-165">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="dc563-166">Поддерживаются только боты пакетов SDK версии 4.</span><span class="sxs-lookup"><span data-stu-id="dc563-166">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="dc563-167">Добавлена проверка доступности имени для команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="dc563-167">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="dc563-168">Добавлена поддержка обновления URL-адреса значка для бота с помощью команды az bot update.</span><span class="sxs-lookup"><span data-stu-id="dc563-168">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="dc563-169">Добавлена поддержка обновления канала Direct Line с помощью команды az bot directline update.</span><span class="sxs-lookup"><span data-stu-id="dc563-169">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="dc563-170">Добавлена поддержка флага --enable-enhanced-auth в команде az bot directline create.</span><span class="sxs-lookup"><span data-stu-id="dc563-170">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="dc563-171">Следующие группы команд предоставляются в общедоступной, а не в предварительной версии: az bot authsetting.</span><span class="sxs-lookup"><span data-stu-id="dc563-171">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="dc563-172">Следующие команды в az bot предоставляются в общедоступной, а не в предварительной версии: create, prepare-deploy, show, delete и update.</span><span class="sxs-lookup"><span data-stu-id="dc563-172">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="dc563-173">Устранена проблема с командой az bot prepare-deploy, которая изменяла значение параметра --proj-file-path на нижний регистр (например, с Test.csproj на test.csproj).</span><span class="sxs-lookup"><span data-stu-id="dc563-173">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="dc563-174">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="dc563-174">Compute</span></span>

* <span data-ttu-id="dc563-175">vmss create/update: добавлен параметр --scale-on-policy, который определяет, какие виртуальные машины выбираются для удаления при масштабировании VMSS.</span><span class="sxs-lookup"><span data-stu-id="dc563-175">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="dc563-176">vm/vmss update: добавлен параметр --priority.</span><span class="sxs-lookup"><span data-stu-id="dc563-176">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="dc563-177">vm/vmss update: добавлен параметр --max-price.</span><span class="sxs-lookup"><span data-stu-id="dc563-177">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="dc563-178">Добавлена группа команд для шифрования дисков (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="dc563-178">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="dc563-179">disk create: добавлены параметры --encryption-type и --disk-encryption-set.</span><span class="sxs-lookup"><span data-stu-id="dc563-179">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="dc563-180">vm/vmss create. Добавлены параметры --os-disk-encryption-set и --data-disk-encryption-sets.</span><span class="sxs-lookup"><span data-stu-id="dc563-180">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="dc563-181">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-181">Core</span></span>

* <span data-ttu-id="dc563-182">Удалена поддержка Python версии 3.4.</span><span class="sxs-lookup"><span data-stu-id="dc563-182">Removed support for Python 3.4</span></span>
* <span data-ttu-id="dc563-183">Подключение к опросу HaTS в нескольких командах.</span><span class="sxs-lookup"><span data-stu-id="dc563-183">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="dc563-184">DLS</span><span class="sxs-lookup"><span data-stu-id="dc563-184">DLS</span></span>

* <span data-ttu-id="dc563-185">Обновлена версия пакета SDK для ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="dc563-185">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="dc563-186">Установка</span><span class="sxs-lookup"><span data-stu-id="dc563-186">Install</span></span>

* <span data-ttu-id="dc563-187">Добавлена поддержка установки скриптов Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="dc563-187">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="dc563-188">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="dc563-188">IOT</span></span>

* <span data-ttu-id="dc563-189">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --failover-region из команды manual-failover.</span><span class="sxs-lookup"><span data-stu-id="dc563-189">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="dc563-190">Теперь она будет выполнять отработку отказа в назначенный геопарный дополнительный регион.</span><span class="sxs-lookup"><span data-stu-id="dc563-190">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="dc563-191">Key Vault</span><span class="sxs-lookup"><span data-stu-id="dc563-191">Key Vault</span></span>

* <span data-ttu-id="dc563-192">Устранена проблема № 8095: (`az keyvault storage remove`): улучшено справочное сообщение.</span><span class="sxs-lookup"><span data-stu-id="dc563-192">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="dc563-193">Устранена проблема № 8921 (`az keyvault key/secret/certificate list/list-deleted/list-versions`): исправлена ошибка проверки в параметре `--maxresults`.</span><span class="sxs-lookup"><span data-stu-id="dc563-193">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="dc563-194">Устранена проблема № 10512 (`az keyvault set-policy`): улучшено сообщение об ошибке, возвращаемое, если не указан ни один из параметров `--object-id`, `--spn` или `--upn`.</span><span class="sxs-lookup"><span data-stu-id="dc563-194">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="dc563-195">Устранена проблема № 10846 (`az keyvault secret show-deleted`): при указании значения `--id` значение `--name/-n` не требовалось.</span><span class="sxs-lookup"><span data-stu-id="dc563-195">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="dc563-196">Устранена проблема № 11084: (`az keyvault secret download`): улучшено справочное сообщение параметра `--encoding`.</span><span class="sxs-lookup"><span data-stu-id="dc563-196">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="dc563-197">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-197">Network</span></span>

* <span data-ttu-id="dc563-198">az network application-gateway probe: добавлена поддержка параметра --port, позволяющего указать порт, который используется для проверки внутренних серверов при создании и обновлении.</span><span class="sxs-lookup"><span data-stu-id="dc563-198">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="dc563-199">az network application-gateway url-path-map create/update: исправлена ошибка с `--waf-policy`.</span><span class="sxs-lookup"><span data-stu-id="dc563-199">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="dc563-200">az network application-gateway: добавлена поддержка параметра `--rewrite-rule-set`.</span><span class="sxs-lookup"><span data-stu-id="dc563-200">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="dc563-201">az network list-service-aliases: добавлена поддержка перечисления псевдонимов служб, которые можно использовать для политик конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="dc563-201">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="dc563-202">az network dns zone import: добавлена поддержка символа .@ в имени записи.</span><span class="sxs-lookup"><span data-stu-id="dc563-202">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="dc563-203">Упаковка</span><span class="sxs-lookup"><span data-stu-id="dc563-203">Packaging</span></span>

* <span data-ttu-id="dc563-204">Снова добавлены сборки Edge для установки PIP.</span><span class="sxs-lookup"><span data-stu-id="dc563-204">Added back edge builds for pip install</span></span>
* <span data-ttu-id="dc563-205">Добавлен пакет Ubuntu eoan.</span><span class="sxs-lookup"><span data-stu-id="dc563-205">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="dc563-206">Политика</span><span class="sxs-lookup"><span data-stu-id="dc563-206">Policy</span></span>

* <span data-ttu-id="dc563-207">Добавлена поддержка API Политики версии 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="dc563-207">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="dc563-208">az policy set-definition: добавлена поддержка группирования в определениях наборов политик с помощью параметра `--definition-groups`.</span><span class="sxs-lookup"><span data-stu-id="dc563-208">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="dc563-209">Redis</span><span class="sxs-lookup"><span data-stu-id="dc563-209">Redis</span></span>

* <span data-ttu-id="dc563-210">В команду `az redis create` добавлена предварительная версия параметра `--replicas-per-master`.</span><span class="sxs-lookup"><span data-stu-id="dc563-210">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="dc563-211">Обновлена версия azure-mgmt-redis с 6.0.0 на 7.0.0 RC1.</span><span class="sxs-lookup"><span data-stu-id="dc563-211">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="dc563-212">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="dc563-212">ServiceFabric</span></span>

* <span data-ttu-id="dc563-213">Исправлена логика добавления типа узла, а также устранена проблема № 10963: при добавлении нового типа узла с уровнем устойчивости Gold возникала ошибка CLI.</span><span class="sxs-lookup"><span data-stu-id="dc563-213">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="dc563-214">Обновлена версия параметра ServiceFabricNodeVmExt до 1.1 в шаблоне создания.</span><span class="sxs-lookup"><span data-stu-id="dc563-214">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-215">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-215">SQL</span></span>

* <span data-ttu-id="dc563-216">В команды create и update базы данных SQL добавлены параметры --read-scale и --read-replicas для поддержки управления масштабированием операций чтения.</span><span class="sxs-lookup"><span data-stu-id="dc563-216">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-217">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-217">Storage</span></span>

* <span data-ttu-id="dc563-218">Выпущена общедоступная версия больших файловых ресурсов для команды создания и обновления учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="dc563-218">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="dc563-219">Выпущена общедоступная версия поддержки маркера SAS для делегирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="dc563-219">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="dc563-220">Добавлены новые команды (`az storage account blob-service-properties show` и `az storage account blob-service-properties update --enable-change-feed`) для управления свойствами службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="dc563-220">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="dc563-221">[ОЖИДАЕТСЯ КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] `az storage copy`: символ `*` больше не поддерживается в качестве подстановочного знака в URL-адресе. Тем не менее новые параметры--include-pattern и--exclude-pattern будут добавлены с поддержкой подстановочных знаков `*`.</span><span class="sxs-lookup"><span data-stu-id="dc563-221">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="dc563-222">Устранена проблема № 11043: добавлена поддержка удаления всего контейнера или общего ресурса в команде `az storage remove`.</span><span class="sxs-lookup"><span data-stu-id="dc563-222">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="dc563-223">26 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-223">November 26, 2019</span></span>

<span data-ttu-id="dc563-224">Версия 2.0.77</span><span class="sxs-lookup"><span data-stu-id="dc563-224">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-225">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-225">ACR</span></span>

* <span data-ttu-id="dc563-226">Параметр `--branch`, используемый при обновлении или создании задачи ACR, объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="dc563-226">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="dc563-227">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="dc563-227">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="dc563-228">Добавлен флаг `--workspace-resource-id` для создания кластера Azure Red Hat Openshift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="dc563-228">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="dc563-229">Добавлен флаг `monitor_profile` для создания кластера Azure Red Hat OpenShift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="dc563-229">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="dc563-230">AKS</span><span class="sxs-lookup"><span data-stu-id="dc563-230">AKS</span></span>

* <span data-ttu-id="dc563-231">Включена поддержка операции смены сертификата кластера с использованием команды az aks rotate-certs.</span><span class="sxs-lookup"><span data-stu-id="dc563-231">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="dc563-232">AppConfig</span><span class="sxs-lookup"><span data-stu-id="dc563-232">AppConfig</span></span>

* <span data-ttu-id="dc563-233">Включена поддержка использования символа ":" для разделителя `as az appconfig kv import`.</span><span class="sxs-lookup"><span data-stu-id="dc563-233">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="dc563-234">Исправлена проблема с перечислением значений ключей с несколькими метками, включая метку NULL.</span><span class="sxs-lookup"><span data-stu-id="dc563-234">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="dc563-235">Обновлен пакет SDK для плоскости управления, azure-mgmt-appconfiguration, до версии 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="dc563-235">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="dc563-236">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-236">AppService</span></span>

* <span data-ttu-id="dc563-237">Исправлена ошибка № 11100. Использование AttributeError для az webapp up при создании плана службы.</span><span class="sxs-lookup"><span data-stu-id="dc563-237">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="dc563-238">az webapp up. При принудительном создании или развертывании сайта для поддерживаемых языков значения по умолчанию не используются.</span><span class="sxs-lookup"><span data-stu-id="dc563-238">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="dc563-239">Включена поддержка Среды службы приложений: az appservice ase show | list | list-addresses | list-plans | create | update | delete.</span><span class="sxs-lookup"><span data-stu-id="dc563-239">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="dc563-240">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="dc563-240">Backup</span></span>

* <span data-ttu-id="dc563-241">Исправлена проблема в команде az backup policy list-associated-items.</span><span class="sxs-lookup"><span data-stu-id="dc563-241">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="dc563-242">Добавлен необязательный параметр BackupManagementType.</span><span class="sxs-lookup"><span data-stu-id="dc563-242">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="dc563-243">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="dc563-243">Compute</span></span>

* <span data-ttu-id="dc563-244">Обновлена версия API вычислений, дисков, моментальных снимков до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="dc563-244">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="dc563-245">vmss create. Улучшение для --orchestration-mode.</span><span class="sxs-lookup"><span data-stu-id="dc563-245">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="dc563-246">sig image-definition create. Добавлен параметр --os-state для указания того, являются ли виртуальные машины, созданные в этом образе, универсальными или специализированными.</span><span class="sxs-lookup"><span data-stu-id="dc563-246">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="dc563-247">sig image-definition create. Добавлен параметр --hyper-v-generation для указания создания гипервизора.</span><span class="sxs-lookup"><span data-stu-id="dc563-247">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="dc563-248">sig image-version create. Включена поддержка параметров --os-snapshot и --data-snapshots.</span><span class="sxs-lookup"><span data-stu-id="dc563-248">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="dc563-249">image create. Включена поддержка параметра --data-disk-caching для указания параметра кэширования для дисков данных.</span><span class="sxs-lookup"><span data-stu-id="dc563-249">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="dc563-250">Обновлена версия пакета SDK для вычислений Python до 10.0.0.</span><span class="sxs-lookup"><span data-stu-id="dc563-250">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="dc563-251">vm/vmss create. Добавлен фрагмент Spot в свойство перечисления Priority.</span><span class="sxs-lookup"><span data-stu-id="dc563-251">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="dc563-252">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименование параметра --max-billing в --max-price для виртуальных машин и Масштабируемых наборов виртуальных машин в соответствии с командлетами Swagger и PowerShell.</span><span class="sxs-lookup"><span data-stu-id="dc563-252">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="dc563-253">vm monitor log show. Включена поддержка запроса журналов в связанной рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="dc563-253">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="dc563-254">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="dc563-254">IOT</span></span>

* <span data-ttu-id="dc563-255">Исправление № 2531. Добавлены вспомогательные аргументы для обновления концентратора.</span><span class="sxs-lookup"><span data-stu-id="dc563-255">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="dc563-256">Исправление № 8323. Добавлены недостающие параметры для создания пользовательской конечной точки хранилища.</span><span class="sxs-lookup"><span data-stu-id="dc563-256">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="dc563-257">Исправлена ошибка регрессии. Отменены изменения, переопределяющие конечную точку хранилища по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-257">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="dc563-258">Key Vault</span><span class="sxs-lookup"><span data-stu-id="dc563-258">Key Vault</span></span>

* <span data-ttu-id="dc563-259">Исправление № 11121. При использовании `az keyvault certificate list` для передачи `--include-pending` теперь не требуется значение `true` или `false`.</span><span class="sxs-lookup"><span data-stu-id="dc563-259">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="dc563-260">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="dc563-260">NetAppFiles</span></span>

* <span data-ttu-id="dc563-261">Обновлена версия azure-mgmt-netapp до 0.7.0, которая включает некоторые дополнительные свойства тома, связанные с предстоящими операциями репликации.</span><span class="sxs-lookup"><span data-stu-id="dc563-261">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="dc563-262">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-262">Network</span></span>

* <span data-ttu-id="dc563-263">application-gateway waf-config. Не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="dc563-263">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="dc563-264">application-gateway waf-policy. Добавлены управляемые правила подгрупп для контроля управляемых наборов правил и правил исключения.</span><span class="sxs-lookup"><span data-stu-id="dc563-264">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="dc563-265">application-gateway waf-policy. Добавлен параметр политики подгруппы для управления глобальной конфигурацией политики WAF.</span><span class="sxs-lookup"><span data-stu-id="dc563-265">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="dc563-266">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] application-gateway waf-policy. Переименовано правило подгруппы в пользовательское правило.</span><span class="sxs-lookup"><span data-stu-id="dc563-266">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="dc563-267">application-gateway http-listener. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="dc563-267">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="dc563-268">application-gateway url-path-map rule. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="dc563-268">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="dc563-269">Упаковка</span><span class="sxs-lookup"><span data-stu-id="dc563-269">Packaging</span></span>

* <span data-ttu-id="dc563-270">Удалена команда az wrapper в Python.</span><span class="sxs-lookup"><span data-stu-id="dc563-270">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="dc563-271">Включена поддержка Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="dc563-271">Added support for Python 3.8</span></span>
* <span data-ttu-id="dc563-272">Изменена версия на Python 3 для пакета RPM.</span><span class="sxs-lookup"><span data-stu-id="dc563-272">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="dc563-273">Профиль</span><span class="sxs-lookup"><span data-stu-id="dc563-273">Profile</span></span>

* <span data-ttu-id="dc563-274">Исправлена ошибка при выполнении `az login -u {} -p {}` с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="dc563-274">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="dc563-275">Исправлена ошибка с `SSLError` при выполнении `az login` за прокси-сервером с самозаверяющим корневым сертификатом.</span><span class="sxs-lookup"><span data-stu-id="dc563-275">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="dc563-276">Исправлена ошибка № 10578. `az login` зависает при одновременном запуске нескольких экземпляров в Windows или WSL.</span><span class="sxs-lookup"><span data-stu-id="dc563-276">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="dc563-277">Исправлена ошибка № 11059. Сбой выполнения `az login --allow-no-subscriptions`, если в клиенте есть подписки.</span><span class="sxs-lookup"><span data-stu-id="dc563-277">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="dc563-278">Исправлена ошибка № 11238. После переименования подписки вход с помощью MSI приведет к тому, что одна и та же подписка появится дважды.</span><span class="sxs-lookup"><span data-stu-id="dc563-278">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="dc563-279">RBAC</span><span class="sxs-lookup"><span data-stu-id="dc563-279">RBAC</span></span>

* <span data-ttu-id="dc563-280">Исправлена ошибка № 10996. Исправлена ошибка с `--force-change-password-next-login` в `az ad user update`, если `--password` не указывается.</span><span class="sxs-lookup"><span data-stu-id="dc563-280">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="dc563-281">Redis</span><span class="sxs-lookup"><span data-stu-id="dc563-281">Redis</span></span>

* <span data-ttu-id="dc563-282">Исправлена ошибка № 2902. Предотвращена настройка конфигураций памяти при обновлении кэша с номером SKU "Базовый".</span><span class="sxs-lookup"><span data-stu-id="dc563-282">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="dc563-283">Резервирование</span><span class="sxs-lookup"><span data-stu-id="dc563-283">Reservations</span></span>

* <span data-ttu-id="dc563-284">Обновлена версия пакета SDK до 0.6.0</span><span class="sxs-lookup"><span data-stu-id="dc563-284">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="dc563-285">Добавлены сведения о плане выставления счетов после вызова Get-Catalogs.</span><span class="sxs-lookup"><span data-stu-id="dc563-285">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="dc563-286">Добавлена новая команда `az reservations reservation-order calculate` для вычисления стоимости резервирования.</span><span class="sxs-lookup"><span data-stu-id="dc563-286">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="dc563-287">Добавлена новая команда `az reservations reservation-order purchase` для приобретения нового резервирования.</span><span class="sxs-lookup"><span data-stu-id="dc563-287">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="dc563-288">Rest</span><span class="sxs-lookup"><span data-stu-id="dc563-288">Rest</span></span>
* <span data-ttu-id="dc563-289">Изменена версия `az rest` на общедоступную.</span><span class="sxs-lookup"><span data-stu-id="dc563-289">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-290">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-290">SQL</span></span>

* <span data-ttu-id="dc563-291">Обновлена версия azure-mgmt-sql до 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="dc563-291">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-292">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-292">Storage</span></span>

* <span data-ttu-id="dc563-293">storage account create. Добавлен параметр --enable-hierarchical-namespace для включения поддержки семантики файловой системы в службе больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="dc563-293">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="dc563-294">Удалено несвязанное исключение из сообщения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="dc563-294">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="dc563-295">Исправлены проблемы, из-за которых появлялось неверное сообщение об отсутствии нужных разрешений на выполнение требуемой операции</span><span class="sxs-lookup"><span data-stu-id="dc563-295">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="dc563-296">при блокировке правилами сети (AuthenticationFailed).</span><span class="sxs-lookup"><span data-stu-id="dc563-296">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="dc563-297">4 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-297">November 4, 2019</span></span>

<span data-ttu-id="dc563-298">Версия 2.0.76</span><span class="sxs-lookup"><span data-stu-id="dc563-298">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-299">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-299">ACR</span></span>

* <span data-ttu-id="dc563-300">В команду `az acr pack build` добавлен параметр предварительной версии `--pack-image-tag`.</span><span class="sxs-lookup"><span data-stu-id="dc563-300">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="dc563-301">Добавлена поддержка включения аудита при создании реестра.</span><span class="sxs-lookup"><span data-stu-id="dc563-301">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="dc563-302">Включена поддержка функции RBAC, распространяющаяся на репозиторий.</span><span class="sxs-lookup"><span data-stu-id="dc563-302">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="dc563-303">AKS</span><span class="sxs-lookup"><span data-stu-id="dc563-303">AKS</span></span>

* <span data-ttu-id="dc563-304">В команду `az aks create` добавлены `--enable-cluster-autoscaler`, `--min-count` и `--max-count`, что позволяет автоматически масштабировать кластер для пула узлов.</span><span class="sxs-lookup"><span data-stu-id="dc563-304">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="dc563-305">Добавлены указанные выше флаги, а также `--update-cluster-autoscaler` и `--disable-cluster-autoscaler` в команду `az aks update`, что позволяет обновлять средство автоматического масштабирования кластера.</span><span class="sxs-lookup"><span data-stu-id="dc563-305">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="dc563-306">AppConfig</span><span class="sxs-lookup"><span data-stu-id="dc563-306">AppConfig</span></span>

* <span data-ttu-id="dc563-307">Добавлена группа команд функции appconfig для управления флагами функций, хранимыми в Конфигурации приложений.</span><span class="sxs-lookup"><span data-stu-id="dc563-307">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="dc563-308">Исправлена незначительная ошибка команды экспорта в файл appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="dc563-308">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="dc563-309">Прерывание чтения содержимого конечного файла во время экспорта.</span><span class="sxs-lookup"><span data-stu-id="dc563-309">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-310">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-310">AppService</span></span>

* <span data-ttu-id="dc563-311">`az appservice plan create`: Добавлена поддержка определения persitescaling при создании плана appservice.</span><span class="sxs-lookup"><span data-stu-id="dc563-311">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="dc563-312">Исправлена проблема, из-за которой операция webapp config ssl bind удаляла существующие теги из ресурса.</span><span class="sxs-lookup"><span data-stu-id="dc563-312">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="dc563-313">Добавлен флаг `--build-remote` для `az functionapp deployment source config-zip` для включения поддержки действия удаленной сборки во время развертывания приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="dc563-313">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="dc563-314">Изменена версия узла по умолчанию для приложений-функций на ~10 для Windows</span><span class="sxs-lookup"><span data-stu-id="dc563-314">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="dc563-315">В `az functionapp create` добавлено свойство `--runtime-version`.</span><span class="sxs-lookup"><span data-stu-id="dc563-315">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="dc563-316">ARM</span><span class="sxs-lookup"><span data-stu-id="dc563-316">ARM</span></span>

* <span data-ttu-id="dc563-317">`az deployment/group deployment validate`: В `--handle-extended-json-format` добавлен параметр для включения поддержки многострочности и комментариев в шаблоне JSON при развертывании.</span><span class="sxs-lookup"><span data-stu-id="dc563-317">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="dc563-318">Версия azure-mgmt-resource обновлена до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="dc563-318">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="dc563-319">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="dc563-319">Backup</span></span>

* <span data-ttu-id="dc563-320">Добавлена поддержка резервного копирования AzureFiles.</span><span class="sxs-lookup"><span data-stu-id="dc563-320">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="dc563-321">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="dc563-321">Compute</span></span>

* <span data-ttu-id="dc563-322">`az vm create`: Добавлено предупреждение при одновременном определении ускоренной сети и существующей сетевой карты.</span><span class="sxs-lookup"><span data-stu-id="dc563-322">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="dc563-323">`az vm create`: Добавлен параметр `--vmss` для определения существующего масштабируемого набора виртуальных машин, которому должна быть назначена виртуальная машина.</span><span class="sxs-lookup"><span data-stu-id="dc563-323">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="dc563-324">`az vm/vmss create`: Добавлена локальная копия файла псевдонима изображения, к которой можно получить доступ в ограниченной сетевой среде.</span><span class="sxs-lookup"><span data-stu-id="dc563-324">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="dc563-325">`az vmss create`: Добавлен параметр `--orchestration-mode` для определения того, как виртуальные машины управляются масштабируемым набором.</span><span class="sxs-lookup"><span data-stu-id="dc563-325">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="dc563-326">`az vm/vmss update`: Добавлен параметр `--ultra-ssd-enabled`, чтобы разрешить обновление параметра Ultra SSD.</span><span class="sxs-lookup"><span data-stu-id="dc563-326">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="dc563-327">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az vm extension set`: Исправлена ошибка, из-за которой пользователям не удавалось определять расширение на виртуальной машине с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="dc563-327">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="dc563-328">Добавлены новые команды `az vm image terms accept/cancel/show` для управления условиями использования образов Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="dc563-328">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="dc563-329">Расширение VMAccessForLinux обновлено до версии 1.5.</span><span class="sxs-lookup"><span data-stu-id="dc563-329">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="dc563-330">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="dc563-330">CosmosDB</span></span>

* <span data-ttu-id="dc563-331">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql container create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="dc563-331">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="dc563-332">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az gremlin graph create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="dc563-332">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="dc563-333">`az sql container create`: Добавлены команды `--unique-key-policy` и `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="dc563-333">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="dc563-334">`az sql container create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-334">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="dc563-335">`gremlin graph create`: Добавлена команда `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="dc563-335">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="dc563-336">`gremlin graph create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-336">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="dc563-337">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="dc563-337">Fixed typo in help message</span></span>
* <span data-ttu-id="dc563-338">База данных: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="dc563-338">database: Added deprecation infomation</span></span>
* <span data-ttu-id="dc563-339">Коллекция: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="dc563-339">collection: Added deprecation infomation</span></span>

### <a name="iot"></a><span data-ttu-id="dc563-340">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="dc563-340">IoT</span></span>

* <span data-ttu-id="dc563-341">Добавлен новый тип источника маршрутизации: DigitalTwinChangeEvents.</span><span class="sxs-lookup"><span data-stu-id="dc563-341">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="dc563-342">Добавлены отсутствующие компоненты в `az iot hub create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-342">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="dc563-343">Key Vault</span><span class="sxs-lookup"><span data-stu-id="dc563-343">Key Vault</span></span>

* <span data-ttu-id="dc563-344">Исправлена непредвиденная ошибка с отсутствием файла сертификата.</span><span class="sxs-lookup"><span data-stu-id="dc563-344">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="dc563-345">Исправлена ошибка с неработающей командой `az keyvault recover/purge`.</span><span class="sxs-lookup"><span data-stu-id="dc563-345">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="dc563-346">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="dc563-346">NetAppFiles</span></span>

* <span data-ttu-id="dc563-347">Пакет azure-mgmt-netapp обновлен до версии 0.6.0 для включения поддержки API версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="dc563-347">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="dc563-348">Эта новая версия API включает:</span><span class="sxs-lookup"><span data-stu-id="dc563-348">This new API version includes:</span></span>

    - <span data-ttu-id="dc563-349">При создании тома с использованием `--protocol-types` допускается NFSv4.1 вместо NFSv4.</span><span class="sxs-lookup"><span data-stu-id="dc563-349">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="dc563-350">Свойство политики экспорта томов теперь называется nfsv41, а не nfsv4.</span><span class="sxs-lookup"><span data-stu-id="dc563-350">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="dc563-351">Параметр `--creation-token` для тома переименован в `--file-path`.</span><span class="sxs-lookup"><span data-stu-id="dc563-351">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="dc563-352">Дата создания моментального снимка теперь имеет значение Created.</span><span class="sxs-lookup"><span data-stu-id="dc563-352">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="dc563-353">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-353">Network</span></span>

* <span data-ttu-id="dc563-354">`az network private-dns link vnet create/update`: Добавлена поддержка связывания виртуальных сетей между клиентами.</span><span class="sxs-lookup"><span data-stu-id="dc563-354">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="dc563-355">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az network vnet subnet list`: Параметры `--resource-group` и `--vnet-name` теперь являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="dc563-355">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="dc563-356">`az network public-ip prefix create`: Включена поддержка определения версии IP-адреса (IPv4, IPv6) при создании.</span><span class="sxs-lookup"><span data-stu-id="dc563-356">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="dc563-357">Версия azure-mgmt-network обновлена до 7.0.0 и версия api-version до 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="dc563-357">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="dc563-358">`az network vrouter`: Включена поддержка нового виртуального маршрутизатора службы и пиринга виртуальных маршрутизаторов.</span><span class="sxs-lookup"><span data-stu-id="dc563-358">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="dc563-359">`az network express-route gateway connection`: Добавлена поддержка параметра `--internet-security`.</span><span class="sxs-lookup"><span data-stu-id="dc563-359">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="dc563-360">Профиль</span><span class="sxs-lookup"><span data-stu-id="dc563-360">Profile</span></span>

* <span data-ttu-id="dc563-361">Исправлена ошибка с неработающей командой `az account get-access-token --resource-type ms-graph`.</span><span class="sxs-lookup"><span data-stu-id="dc563-361">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="dc563-362">Удалено предупреждение из `az login`.</span><span class="sxs-lookup"><span data-stu-id="dc563-362">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="dc563-363">RBAC</span><span class="sxs-lookup"><span data-stu-id="dc563-363">RBAC</span></span>

* <span data-ttu-id="dc563-364">Исправление `az ad app update --id {} --display-name {}` не работает.</span><span class="sxs-lookup"><span data-stu-id="dc563-364">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="dc563-365">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="dc563-365">ServiceFabric</span></span>

* <span data-ttu-id="dc563-366">`az sf cluster create`: Исправлена проблема путем изменения VMSS для вычислений с использованием файла template.json для Service Fabric Linux и Windows со стандартных дисков на управляемые.</span><span class="sxs-lookup"><span data-stu-id="dc563-366">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-367">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-367">SQL</span></span>

* <span data-ttu-id="dc563-368">Добавлены параметры `--compute-model`, `--auto-pause-delay` и `--min-capacity` для включения поддержки операций CRUD для нового предложения Базы данных SQL: Модель бессерверных вычислений.</span><span class="sxs-lookup"><span data-stu-id="dc563-368">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-369">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-369">Storage</span></span>

* <span data-ttu-id="dc563-370">`az storage account create/update`: Добавлен параметр --enable-files-adds и группа аргументов свойств Azure Active Directory для включения поддержки аутентификации доменных служб Azure Active Directory для Файлов Azure.</span><span class="sxs-lookup"><span data-stu-id="dc563-370">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="dc563-371">Расширена команда `az storage account keys list/renew` для включения поддержки перечисления или повторного создания ключей Kerberos для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="dc563-371">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="dc563-372">15 октября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-372">October 15, 2019</span></span>

<span data-ttu-id="dc563-373">Версия 2.0.75</span><span class="sxs-lookup"><span data-stu-id="dc563-373">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="dc563-374">AKS</span><span class="sxs-lookup"><span data-stu-id="dc563-374">AKS</span></span>

* <span data-ttu-id="dc563-375">Для параметра `--load-balancer-sku` изменено значение по умолчанию на `standard`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="dc563-375">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="dc563-376">Для параметра `--vm-set-type` изменено значение по умолчанию на `virtualmachinescalesets`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="dc563-376">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="dc563-377">AMS</span><span class="sxs-lookup"><span data-stu-id="dc563-377">AMS</span></span>

* <span data-ttu-id="dc563-378">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя `job start` изменено на `job create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-378">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="dc563-379">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В параметре `--ask` команды `content-key-policy create` вместо кодировки UTF8 теперь используется шестнадцатеричная строка из 32 символов.</span><span class="sxs-lookup"><span data-stu-id="dc563-379">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-380">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-380">AppService</span></span>

* <span data-ttu-id="dc563-381">Добавлены команды `webapp config access-restriction show|set|add|remove`.</span><span class="sxs-lookup"><span data-stu-id="dc563-381">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="dc563-382">Улучшена обработка ошибок в `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="dc563-382">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="dc563-383">Для `appservice plan update` добавлена поддержка номера SKU `Isolated`.</span><span class="sxs-lookup"><span data-stu-id="dc563-383">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="dc563-384">ARM</span><span class="sxs-lookup"><span data-stu-id="dc563-384">ARM</span></span>

* <span data-ttu-id="dc563-385">В `deployment create` добавлен параметр `--handle-extended-json-format` для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="dc563-385">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="dc563-386">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="dc563-386">Compute</span></span>

* <span data-ttu-id="dc563-387">Добавлен параметр `--enable-agent` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-387">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="dc563-388">Внесены изменения в `vm create`, позволяющие автоматически использовать номер SKU "Стандартный" для общедоступных IP-адресов при использовании зон.</span><span class="sxs-lookup"><span data-stu-id="dc563-388">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="dc563-389">Внесены изменения в `vm create`, позволяющие автоматически создавать допустимое имя для виртуальной машины, если оно не задано.</span><span class="sxs-lookup"><span data-stu-id="dc563-389">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="dc563-390">В `vmss create` добавлен параметр `--computer-name-prefix` для поддержки пользовательского префикса имени для виртуальных машин в VMSS.</span><span class="sxs-lookup"><span data-stu-id="dc563-390">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="dc563-391">В `vm create` добавлен параметр `--workspace` для автоматического включения рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="dc563-391">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="dc563-392">API коллекций обновлен до версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="dc563-392">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="dc563-393">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-393">Core</span></span>

* <span data-ttu-id="dc563-394">Добавлена проверка синтаксиса для параметра `--set` в универсальной команде обновления.</span><span class="sxs-lookup"><span data-stu-id="dc563-394">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="dc563-395">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="dc563-395">IoT</span></span>

* <span data-ttu-id="dc563-396">Исправлена проблема, при которой `iot hub show` неправильно выдавал ошибку "Ресурс не найден".</span><span class="sxs-lookup"><span data-stu-id="dc563-396">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="dc563-397">Монитор</span><span class="sxs-lookup"><span data-stu-id="dc563-397">Monitor</span></span>

* <span data-ttu-id="dc563-398">В `monitor log-analytics workspace` добавлена поддержка CRUD.</span><span class="sxs-lookup"><span data-stu-id="dc563-398">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="dc563-399">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-399">Network</span></span>

* <span data-ttu-id="dc563-400">В `network private-dns link vnet [create|update]` добавлена поддержка виртуального канала для клиентов.</span><span class="sxs-lookup"><span data-stu-id="dc563-400">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="dc563-401">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для `network vnet subnet list` теперь требуются параметры `--resource-group` и `--vnet-name`.</span><span class="sxs-lookup"><span data-stu-id="dc563-401">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-402">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-402">SQL</span></span>

* <span data-ttu-id="dc563-403">В `sql mi ad-admin` добавлены команды, которые поддерживают назначение администратора AAD в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="dc563-403">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-404">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-404">Storage</span></span>

* <span data-ttu-id="dc563-405">В `storage copy` добавлен параметр `--preserve-s2s-access-tier`, позволяющий сохранить уровень доступа во время копирования между службами.</span><span class="sxs-lookup"><span data-stu-id="dc563-405">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="dc563-406">В `storage account [create|update]` добавлен параметр `--enable-large-file-share` для поддержки общих папок большого размера в учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="dc563-406">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="dc563-407">24 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-407">September 24, 2019</span></span>

<span data-ttu-id="dc563-408">Версия 2.0.74</span><span class="sxs-lookup"><span data-stu-id="dc563-408">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-409">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-409">ACR</span></span>

* <span data-ttu-id="dc563-410">В `acr config retention update` добавлен обязательный параметр `--type`.</span><span class="sxs-lookup"><span data-stu-id="dc563-410">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="dc563-411">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Переименованный параметр `--name -n` изменен на `--registry -r ` для группы команд `acr config`.</span><span class="sxs-lookup"><span data-stu-id="dc563-411">[BREAKING CHNAGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="dc563-412">AKS</span><span class="sxs-lookup"><span data-stu-id="dc563-412">AKS</span></span>

* <span data-ttu-id="dc563-413">В команду `aks create` добавлен параметр `--load-balancer-sku`, позволяющий создать кластер AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="dc563-413">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="dc563-414">В команды `aks [create|update]` добавлены параметры `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` и `--load-balancer-outbound-ip-prefixes`, позволяющие обновлять профиль подсистемы балансировки нагрузки у кластера AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="dc563-414">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="dc563-415">В команду `aks create` добавлен параметр `--vm-set-type`, позволяющий указывать типы виртуальных машин в кластере AKS.</span><span class="sxs-lookup"><span data-stu-id="dc563-415">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="dc563-416">ARM</span><span class="sxs-lookup"><span data-stu-id="dc563-416">ARM</span></span>

* <span data-ttu-id="dc563-417">В команду `group deployment create` добавлен параметр `--handle-extended-json-format`, для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="dc563-417">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="dc563-418">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="dc563-418">Compute</span></span>

* <span data-ttu-id="dc563-419">В команды `vmss [create|update]` добавлен параметр `--terminate-notification-time`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="dc563-419">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="dc563-420">В команду `vmss update` добавлен параметр `--enable-terminate-notification`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="dc563-420">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="dc563-421">В команды `[vm|vmss] create` добавлены параметры `--priority,`, `--eviction-policy,` и `--max-billing`.</span><span class="sxs-lookup"><span data-stu-id="dc563-421">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="dc563-422">Изменена команда `disk create`, которая теперь позволяет указать точный размер отправки на диск.</span><span class="sxs-lookup"><span data-stu-id="dc563-422">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="dc563-423">В `snapshot create` добавлена поддержка добавочных моментальных снимков для управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="dc563-423">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="dc563-424">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="dc563-424">Cosmos DB</span></span>

* <span data-ttu-id="dc563-425">В команду `cosmosdb keys list` добавлен параметр `--type <key-type>` для отображения ключей, ключей только для чтения или строк подключения.</span><span class="sxs-lookup"><span data-stu-id="dc563-425">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="dc563-426">Добавлена команда `cosmosdb keys regenerate`.</span><span class="sxs-lookup"><span data-stu-id="dc563-426">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="dc563-427">[УСТАРЕЛО] Команды `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` и `cosmosdb list-read-only-keys` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="dc563-427">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="dc563-428">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="dc563-428">EventGrid</span></span>

* <span data-ttu-id="dc563-429">Исправлен текст справки по конечной точке — дана ссылка на правильный параметр.</span><span class="sxs-lookup"><span data-stu-id="dc563-429">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="dc563-430">Key Vault</span><span class="sxs-lookup"><span data-stu-id="dc563-430">Key Vault</span></span>

* <span data-ttu-id="dc563-431">Исправлена проблема, из-за которой вход с помощью клиента (`login -t`) мог приводить к сбою `keyvault create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-431">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="dc563-432">Монитор</span><span class="sxs-lookup"><span data-stu-id="dc563-432">Monitor</span></span>

* <span data-ttu-id="dc563-433">Исправлена проблема с тем, что символ `:` являлся недопустимым в аргументе `--condition` для `monitor metrics alert create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-433">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="dc563-434">Политика</span><span class="sxs-lookup"><span data-stu-id="dc563-434">Policy</span></span>

* <span data-ttu-id="dc563-435">Добавлена поддержка API Политики версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="dc563-435">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="dc563-436">В команду `policy assignment create` добавлен параметр `--enforcement-mode`.</span><span class="sxs-lookup"><span data-stu-id="dc563-436">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-437">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-437">Storage</span></span>

* <span data-ttu-id="dc563-438">В команду `az storage copy` добавлен параметр `--blob-type`.</span><span class="sxs-lookup"><span data-stu-id="dc563-438">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="dc563-439">10 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-439">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-440">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-440">ACR</span></span>

* <span data-ttu-id="dc563-441">Добавлена группа команд `acr config retention` для настройки политики хранения.</span><span class="sxs-lookup"><span data-stu-id="dc563-441">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="dc563-442">AKS</span><span class="sxs-lookup"><span data-stu-id="dc563-442">AKS</span></span>

* <span data-ttu-id="dc563-443">Добавлена возможность интеграции ACR с помощью следующих команд:</span><span class="sxs-lookup"><span data-stu-id="dc563-443">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="dc563-444">В `aks [create|update]` добавлен параметр `--attach-acr` для подключения ACR к кластеру AKS.</span><span class="sxs-lookup"><span data-stu-id="dc563-444">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="dc563-445">В `aks update` добавлен параметр `--detach-acr` для отключения ACR от кластера AKS.</span><span class="sxs-lookup"><span data-stu-id="dc563-445">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="dc563-446">ARM</span><span class="sxs-lookup"><span data-stu-id="dc563-446">ARM</span></span>

* <span data-ttu-id="dc563-447">Добавлена возможность использования API версии 2019-05-10.</span><span class="sxs-lookup"><span data-stu-id="dc563-447">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="dc563-448">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="dc563-448">Batch</span></span>

* <span data-ttu-id="dc563-449">Добавлены новые параметры конфигурации JSON в `--json-file` для `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="dc563-449">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="dc563-450">Добавлен параметр `MountConfigurations` для подключений файловой системы (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="dc563-450">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="dc563-451">Добавлено необязательное свойство `publicIPs` в `NetworkConfiguration` для общедоступных IP-адресов в пулах (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="dc563-451">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="dc563-452">В `--image` добавлена поддержка коллекций общих образов.</span><span class="sxs-lookup"><span data-stu-id="dc563-452">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="dc563-453">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `--start-task-wait-for-success` в `batch pool create` изменено на `true`.</span><span class="sxs-lookup"><span data-stu-id="dc563-453">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="dc563-454">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `Scope` в `AutoUserSpecification` задано как Pool (ранее `Task` на узлах Windows и `Pool` на узлах Linux).</span><span class="sxs-lookup"><span data-stu-id="dc563-454">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="dc563-455">Этот аргумент можно задать только в конфигурации JSON с помощью `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="dc563-455">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="dc563-456">HDInsight</span><span class="sxs-lookup"><span data-stu-id="dc563-456">HDInsight</span></span>

* <span data-ttu-id="dc563-457">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="dc563-457">GA release</span></span>
* <span data-ttu-id="dc563-458">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--workernode-count/-c` в `az hdinsight resize` теперь является обязательным.</span><span class="sxs-lookup"><span data-stu-id="dc563-458">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="dc563-459">Key Vault</span><span class="sxs-lookup"><span data-stu-id="dc563-459">Key Vault</span></span>

* <span data-ttu-id="dc563-460">Исправлена проблема, когда подсети не удавалось удалить из сетевых правил.</span><span class="sxs-lookup"><span data-stu-id="dc563-460">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="dc563-461">Исправлена проблема, когда дублированные подсети и IP-адреса могли быть добавлены к сетевым правилам.</span><span class="sxs-lookup"><span data-stu-id="dc563-461">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="dc563-462">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-462">Network</span></span>

* <span data-ttu-id="dc563-463">Добавлен параметр `--interval` в `network watcher flow-log` для выбора значения интервала анализа трафика.</span><span class="sxs-lookup"><span data-stu-id="dc563-463">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="dc563-464">Добавлена команда `network application-gateway identity` для управления удостоверением шлюза.</span><span class="sxs-lookup"><span data-stu-id="dc563-464">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="dc563-465">Добавлена возможность указать идентификатор Key Vault в команде `network application-gateway ssl-cert`.</span><span class="sxs-lookup"><span data-stu-id="dc563-465">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="dc563-466">Добавлена команда `network express-route peering peer-connection [show|list]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-466">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="dc563-467">Политика</span><span class="sxs-lookup"><span data-stu-id="dc563-467">Policy</span></span>

* <span data-ttu-id="dc563-468">Добавлена возможность использования API версии 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="dc563-468">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="dc563-469">27 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-469">August 27, 2019</span></span>

<span data-ttu-id="dc563-470">Версия 2.0.72</span><span class="sxs-lookup"><span data-stu-id="dc563-470">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-471">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-471">ACR</span></span>

* <span data-ttu-id="dc563-472">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка SKU `classic`.</span><span class="sxs-lookup"><span data-stu-id="dc563-472">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="dc563-473">Управление API</span><span class="sxs-lookup"><span data-stu-id="dc563-473">API Management</span></span>

* <span data-ttu-id="dc563-474">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена группа команд `apim`.</span><span class="sxs-lookup"><span data-stu-id="dc563-474">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-475">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-475">AppService</span></span>

* <span data-ttu-id="dc563-476">Исправлена проблема с командой `webapp webjob continuous start` при указании слота.</span><span class="sxs-lookup"><span data-stu-id="dc563-476">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="dc563-477">Изменена команда `webapp up` для обнаружения и удаления папки `env` из файла, используемого для развертывания.</span><span class="sxs-lookup"><span data-stu-id="dc563-477">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="dc563-478">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="dc563-478">Keyvault</span></span>

* <span data-ttu-id="dc563-479">Исправлена ошибка в команде `keyvault secret set`, которая игнорировала аргумент `--expires`.</span><span class="sxs-lookup"><span data-stu-id="dc563-479">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="dc563-480">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-480">Network</span></span>

* <span data-ttu-id="dc563-481">Добавлена поддержка IPv6-адресов для аргументов `--private-ip-address-version`.</span><span class="sxs-lookup"><span data-stu-id="dc563-481">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="dc563-482">Добавлены новые команды `network private-endpoint [create|update|list-types]` для управления закрытыми конечными точками.</span><span class="sxs-lookup"><span data-stu-id="dc563-482">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="dc563-483">Добавлена группа команд для `network private-link-service`.</span><span class="sxs-lookup"><span data-stu-id="dc563-483">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="dc563-484">Добавлены аргументы `--private-endpoint-network-policies` и `--private-link-service-network-policies` для команды `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="dc563-484">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="dc563-485">RBAC</span><span class="sxs-lookup"><span data-stu-id="dc563-485">RBAC</span></span>

* <span data-ttu-id="dc563-486">Исправлена проблема с `ad app update --homepage`, когда домашнюю страницу нельзя было обновить.</span><span class="sxs-lookup"><span data-stu-id="dc563-486">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="dc563-487">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="dc563-487">ServiceFabric</span></span>

* <span data-ttu-id="dc563-488">Добавлена поддержка имен Key Vault в смешанном регистре.</span><span class="sxs-lookup"><span data-stu-id="dc563-488">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="dc563-489">Исправлена проблема с использованием сертификатов в Key Vault.</span><span class="sxs-lookup"><span data-stu-id="dc563-489">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="dc563-490">Исправлена проблема с использованием файлов сертификатов PFX.</span><span class="sxs-lookup"><span data-stu-id="dc563-490">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="dc563-491">Исправлена проблема с `sf cluster certificate add`, когда группа ресурсов Key Vault не была указана.</span><span class="sxs-lookup"><span data-stu-id="dc563-491">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="dc563-492">Исправлена проблема с неработающей командой `sf cluster set`.</span><span class="sxs-lookup"><span data-stu-id="dc563-492">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="dc563-493">SignalR</span><span class="sxs-lookup"><span data-stu-id="dc563-493">SignalR</span></span>

* <span data-ttu-id="dc563-494">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="dc563-494">Added new commands:</span></span>
  * <span data-ttu-id="dc563-495">`signalr cors`: Управление CORS SignalR</span><span class="sxs-lookup"><span data-stu-id="dc563-495">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="dc563-496">`signalr restart`: Перезапуск службы SignalR</span><span class="sxs-lookup"><span data-stu-id="dc563-496">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="dc563-497">`signalr update`: Обновление службы SignalR</span><span class="sxs-lookup"><span data-stu-id="dc563-497">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="dc563-498">Добавлен аргумент `--service-mode` для команды `signalr create`</span><span class="sxs-lookup"><span data-stu-id="dc563-498">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-499">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-499">Storage</span></span>

* <span data-ttu-id="dc563-500">Добавлена команда `storage account revoke-delegation-keys`.</span><span class="sxs-lookup"><span data-stu-id="dc563-500">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="dc563-501">13 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-501">August 13, 2019</span></span>

<span data-ttu-id="dc563-502">Версия 2.0.71</span><span class="sxs-lookup"><span data-stu-id="dc563-502">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-503">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-503">AppService</span></span>

* <span data-ttu-id="dc563-504">Исправлена проблема, из-за которой выполнение команд `webapp webjob continuous` для слотов завершалось сбоем.</span><span class="sxs-lookup"><span data-stu-id="dc563-504">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="dc563-505">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="dc563-505">BotService</span></span>

* <span data-ttu-id="dc563-506">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка создания ботов на основе пакета SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="dc563-506">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="dc563-507">Cognitive Services:</span><span class="sxs-lookup"><span data-stu-id="dc563-507">CognitiveServices</span></span>

* <span data-ttu-id="dc563-508">Добавлены команды `cognitiveservices account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="dc563-508">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="dc563-509">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="dc563-509">Cosmos DB</span></span>

* <span data-ttu-id="dc563-510">Удалено предупреждение при обновлении нескольких расположений для записи.</span><span class="sxs-lookup"><span data-stu-id="dc563-510">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="dc563-511">Добавлены команды CRUD для ресурсов CosmosDB SQL, MongoDB, Cassandra, Gremlin и ресурсов таблиц, а также пропускной способности ресурсов.</span><span class="sxs-lookup"><span data-stu-id="dc563-511">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="dc563-512">HDInsight</span><span class="sxs-lookup"><span data-stu-id="dc563-512">HDInsight</span></span>

<span data-ttu-id="dc563-513">Этот выпуск содержит большое число критических изменений.</span><span class="sxs-lookup"><span data-stu-id="dc563-513">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="dc563-514">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="dc563-514">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="dc563-515">Переименование `--storage-default-container` в `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="dc563-515">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="dc563-516">Переименование `--storage-default-filesystem` в `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="dc563-516">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="dc563-517">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--name` для `application create`, чтобы представлять имя приложения вместо имени кластера.</span><span class="sxs-lookup"><span data-stu-id="dc563-517">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="dc563-518">Добавлен аргумент `--cluster-name` для `application create`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="dc563-518">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="dc563-519">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="dc563-519">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="dc563-520">Переименование `--application-type` в `--type`</span><span class="sxs-lookup"><span data-stu-id="dc563-520">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="dc563-521">Переименование `--marketplace-identifier` в `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="dc563-521">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="dc563-522">Переименование `--https-endpoint-access-mode` в `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="dc563-522">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="dc563-523">Переименован аргумент `--https-endpoint-destination-port` на `--destination-port`.</span><span class="sxs-lookup"><span data-stu-id="dc563-523">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="dc563-524">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="dc563-524">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="dc563-525">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Переименован аргумент `--target-instance-count` на `--workernode-count` для `hdinsight resize`.</span><span class="sxs-lookup"><span data-stu-id="dc563-525">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="dc563-526">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены все команды в группе `hdinsight script-action`, чтобы использовать параметр `--name` в качестве имени действия скрипта.</span><span class="sxs-lookup"><span data-stu-id="dc563-526">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="dc563-527">Добавлен аргумент `--cluster-name` для всех команд `hdinsight script-action`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="dc563-527">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="dc563-528">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименован аргумент `--script-execution-id` на `--execution-id`для всех команд `hdinsight script-action`.</span><span class="sxs-lookup"><span data-stu-id="dc563-528">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="dc563-529">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `hdinsight script-action show` переименована в `hdinsight script-action show-execution-details`.</span><span class="sxs-lookup"><span data-stu-id="dc563-529">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="dc563-530">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Изменены параметры для `hdinsight script-action execute --roles`, чтобы они разделялись пробелами, а не запятыми.</span><span class="sxs-lookup"><span data-stu-id="dc563-530">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="dc563-531">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--persisted` для `hdinsight script-action list`.</span><span class="sxs-lookup"><span data-stu-id="dc563-531">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="dc563-532">Изменен параметр `hdinsight create --cluster-configurations`, чтобы принимать путь к локальному файлу JSON или строке JSON.</span><span class="sxs-lookup"><span data-stu-id="dc563-532">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="dc563-533">Добавлена команда `hdinsight script-action list-execution-history`.</span><span class="sxs-lookup"><span data-stu-id="dc563-533">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="dc563-534">Изменен параметр `hdinsight monitor enable --workspace`, чтобы принимать идентификатор или имя рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="dc563-534">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="dc563-535">Добавлен аргумент `hdinsight monitor enable --primary-key`, который требуется, если в качестве параметра указан идентификатор рабочей области.</span><span class="sxs-lookup"><span data-stu-id="dc563-535">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="dc563-536">Добавлены дополнительные примеры и обновленные описания для справочных сообщений.</span><span class="sxs-lookup"><span data-stu-id="dc563-536">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="dc563-537">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="dc563-537">Interactive</span></span>

* <span data-ttu-id="dc563-538">Исправлена ошибка загрузки.</span><span class="sxs-lookup"><span data-stu-id="dc563-538">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="dc563-539">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="dc563-539">Kubernetes</span></span>

* <span data-ttu-id="dc563-540">Теперь используется `https`, если порт контейнера панели мониторинга использует `https`.</span><span class="sxs-lookup"><span data-stu-id="dc563-540">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="dc563-541">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-541">Network</span></span>

* <span data-ttu-id="dc563-542">Добавлен аргумент `--yes` для `network dns record-set cname delete`.</span><span class="sxs-lookup"><span data-stu-id="dc563-542">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="dc563-543">Профиль</span><span class="sxs-lookup"><span data-stu-id="dc563-543">Profile</span></span>

* <span data-ttu-id="dc563-544">Добавлен аргумент `--resource-type` для `account get-access-token`, чтобы получать маркеры доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="dc563-544">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="dc563-545">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="dc563-545">ServiceFabric</span></span>

* <span data-ttu-id="dc563-546">Добавлены все поддерживаемые версии ОС для команды sf cluster create.</span><span class="sxs-lookup"><span data-stu-id="dc563-546">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="dc563-547">Исправлена ошибка проверки основного сертификата.</span><span class="sxs-lookup"><span data-stu-id="dc563-547">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-548">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-548">Storage</span></span>

* <span data-ttu-id="dc563-549">Добавлена команда `storage copy`.</span><span class="sxs-lookup"><span data-stu-id="dc563-549">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="dc563-550">30 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-550">July 30, 2019</span></span>

<span data-ttu-id="dc563-551">Версия 2.0.70</span><span class="sxs-lookup"><span data-stu-id="dc563-551">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-552">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-552">ACR</span></span>

* <span data-ttu-id="dc563-553">Исправлена проблема № 9952 (регрессия в команде `acr pack build`).</span><span class="sxs-lookup"><span data-stu-id="dc563-553">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="dc563-554">Удалено имя образа построителя по умолчанию в `acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="dc563-554">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-555">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-555">Appservice</span></span>

* <span data-ttu-id="dc563-556">Команда `webapp config ssl` изменена для отображения сообщения, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="dc563-556">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="dc563-557">Исправлена проблема, когда команда `functionapp create` не принимала тип учетной записи хранения `Standard_RAGRS`.</span><span class="sxs-lookup"><span data-stu-id="dc563-557">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="dc563-558">Исправлена проблема, когда команда `webapp up` завершала работу со сбоем в случае выполнения со старой версией Python.</span><span class="sxs-lookup"><span data-stu-id="dc563-558">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="dc563-559">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-559">Network</span></span>

* <span data-ttu-id="dc563-560">Удален недопустимый параметр `--ids` из `network nic ip-config add` (исправление проблемы № 9861).</span><span class="sxs-lookup"><span data-stu-id="dc563-560">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="dc563-561">Исправлена проблема № 9604.</span><span class="sxs-lookup"><span data-stu-id="dc563-561">Fixes #9604.</span></span> <span data-ttu-id="dc563-562">Добавлен параметр `--root-certs` в `network application-gateway http-settings [create|update]` для поддержки связанных с пользователем доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="dc563-562">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="dc563-563">Исправлен аргумент `--subscription` для `network dns record-set ns create` (проблема № 9965).</span><span class="sxs-lookup"><span data-stu-id="dc563-563">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="dc563-564">RBAC</span><span class="sxs-lookup"><span data-stu-id="dc563-564">RBAC</span></span>

* <span data-ttu-id="dc563-565">Добавлена команда `user update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-565">Added `user update` command</span></span>
* <span data-ttu-id="dc563-566">[УСТАРЕЛО]`--upn-or-object-id` не рекомендуется использовать в связанных с пользователями командах.</span><span class="sxs-lookup"><span data-stu-id="dc563-566">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="dc563-567">Вместо этого применяйте аргумент `--id`.</span><span class="sxs-lookup"><span data-stu-id="dc563-567">Use replacement argument `--id`</span></span>
* <span data-ttu-id="dc563-568">Добавлен аргумент `--id` в связанные с пользователями команды.</span><span class="sxs-lookup"><span data-stu-id="dc563-568">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-569">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-569">SQL</span></span>

* <span data-ttu-id="dc563-570">Добавлены команды управления для ключей и предохранителя TDE управляемого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="dc563-570">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-571">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-571">Storage</span></span>

* <span data-ttu-id="dc563-572">Добавлена команда `storage remove`.</span><span class="sxs-lookup"><span data-stu-id="dc563-572">Added `storage remove` command</span></span>
* <span data-ttu-id="dc563-573">Исправлена проблема с `storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-573">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-574">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-574">VM</span></span>

* <span data-ttu-id="dc563-575">Изменена команда `list-skus` для использования новой версии API для вывода сведений о зонах.</span><span class="sxs-lookup"><span data-stu-id="dc563-575">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="dc563-576">Изменено значение по умолчанию параметра `--single-placement-group` на `false` для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-576">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="dc563-577">Добавлена возможность выбирать номера SKU хранилища ZRS для `[snapshot|disk] create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-577">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="dc563-578">Добавлена новая группа команд `vm host` для поддержки выделенных узлов.</span><span class="sxs-lookup"><span data-stu-id="dc563-578">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="dc563-579">Добавлены параметры `--host` и `--host-group` в команде `vm create` для указания выделенного узла виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="dc563-579">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="dc563-580">16 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-580">July 16, 2019</span></span>

<span data-ttu-id="dc563-581">Версия 2.0.69</span><span class="sxs-lookup"><span data-stu-id="dc563-581">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-582">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-582">Appservice</span></span>

* <span data-ttu-id="dc563-583">Изменены команды `webapp identity`. Теперь они возвращают правильное сообщение об ошибке, если параметр ResourceGroupName или имя приложения недопустимы.</span><span class="sxs-lookup"><span data-stu-id="dc563-583">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="dc563-584">Исправлена команда `webapp list`. Теперь она возвращает правильное значение для параметра numberOfSites, если не указан параметр ResourceGroup.</span><span class="sxs-lookup"><span data-stu-id="dc563-584">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="dc563-585">Исправлены побочные эффекты для команд `appservice plan create` и `webapp create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-585">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="dc563-586">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-586">Core</span></span>

* <span data-ttu-id="dc563-587">Исправлена ошибка, при которой отображался параметр `--subscription`, хотя он был неприменим.</span><span class="sxs-lookup"><span data-stu-id="dc563-587">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="dc563-588">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="dc563-588">Batch</span></span>

* <span data-ttu-id="dc563-589">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `batch pool node-agent-skus list` заменена на `batch pool supported-images list`.</span><span class="sxs-lookup"><span data-stu-id="dc563-589">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="dc563-590">Добавлена поддержка правил безопасности, которые блокируют сетевой доступ к пулу на основе исходного порта трафика при использовании параметра `--json-file` команды `batch pool create network`.</span><span class="sxs-lookup"><span data-stu-id="dc563-590">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="dc563-591">Добавлена поддержка выполнения задачи в рабочей папке контейнера или рабочей папке задачи пакета при использовании параметра `--json-file` команды `batch task create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-591">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="dc563-592">Исправлена ошибка в параметре `--application-package-references` команды `batch pool create`, которая позволяла работать только со значениями по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-592">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="dc563-593">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="dc563-593">Eventhubs</span></span>

* <span data-ttu-id="dc563-594">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="dc563-594">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="dc563-595">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="dc563-595">RDBMS</span></span>

* <span data-ttu-id="dc563-596">Добавлен необязательный параметр для указания номера SKU реплики в команде создания реплики.</span><span class="sxs-lookup"><span data-stu-id="dc563-596">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="dc563-597">Исправлена ошибка теста CI при создании реплики MySQL.</span><span class="sxs-lookup"><span data-stu-id="dc563-597">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="dc563-598">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="dc563-598">Relay</span></span>

* <span data-ttu-id="dc563-599">Исправлена проблема с гибридным подключением при выключенной авторизации клиента ([8775](https://github.com/azure/azure-cli/issues/8775)).</span><span class="sxs-lookup"><span data-stu-id="dc563-599">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="dc563-600">Добавлен параметр `--requires-transport-security` для команды `relay wcfrelay create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-600">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="dc563-601">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="dc563-601">Servicebus</span></span>

* <span data-ttu-id="dc563-602">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="dc563-602">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-603">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-603">Storage</span></span>

* <span data-ttu-id="dc563-604">Добавлена возможность обновления учетной записи хранения для AADDS в службе "Файлы".</span><span class="sxs-lookup"><span data-stu-id="dc563-604">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="dc563-605">Устранена проблема, описанная здесь: `storage blob service-properties update --set`.</span><span class="sxs-lookup"><span data-stu-id="dc563-605">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="dc563-606">2 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-606">July 2, 2019</span></span>

<span data-ttu-id="dc563-607">Версия 2.0.68</span><span class="sxs-lookup"><span data-stu-id="dc563-607">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="dc563-608">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-608">Core</span></span>

* <span data-ttu-id="dc563-609">Командные модули теперь объединены в один распространяемый пакет Python.</span><span class="sxs-lookup"><span data-stu-id="dc563-609">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="dc563-610">В результате этого прекращается непосредственное использование множества пакетов `azure-cli-` в PyPI.</span><span class="sxs-lookup"><span data-stu-id="dc563-610">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="dc563-611">Это также должно уменьшить размер установки и повлияет только на пользователей, которые выполняли установку непосредственно через `pip`.</span><span class="sxs-lookup"><span data-stu-id="dc563-611">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-612">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-612">ACR</span></span>

* <span data-ttu-id="dc563-613">В заданиях добавлена поддержка триггеров таймера.</span><span class="sxs-lookup"><span data-stu-id="dc563-613">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-614">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-614">Appservice</span></span>

* <span data-ttu-id="dc563-615">Внесены изменения в `functionapp create` для включения Application Insights по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-615">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="dc563-616">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена устаревшая команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="dc563-616">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="dc563-617">Вместо нее используйте новую команду `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="dc563-617">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="dc563-618">В `functionapp deployment config-zip` добавлена поддержка плана потребления приложения-функции Linux.</span><span class="sxs-lookup"><span data-stu-id="dc563-618">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="dc563-619">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="dc563-619">Cosmos DB</span></span>

* <span data-ttu-id="dc563-620">Добавлена возможность отключения TTL.</span><span class="sxs-lookup"><span data-stu-id="dc563-620">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="dc563-621">DLS</span><span class="sxs-lookup"><span data-stu-id="dc563-621">DLS</span></span>

* <span data-ttu-id="dc563-622">Обновленная версия ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="dc563-622">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="dc563-623">Отзывы</span><span class="sxs-lookup"><span data-stu-id="dc563-623">Feedback</span></span>

* <span data-ttu-id="dc563-624">При сообщении о сбое при выполнении команды расширения `az feedback` теперь пытается открыть браузер по URL-адресу репозитория или проекта расширения из индекса.</span><span class="sxs-lookup"><span data-stu-id="dc563-624">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="dc563-625">HDInsight</span><span class="sxs-lookup"><span data-stu-id="dc563-625">HDInsight</span></span>

* <span data-ttu-id="dc563-626">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя группы команд `oms` изменилось на `monitor`.</span><span class="sxs-lookup"><span data-stu-id="dc563-626">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="dc563-627">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--http-password/-p` стал обязательным.</span><span class="sxs-lookup"><span data-stu-id="dc563-627">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="dc563-628">Добавлены средства заполнения для `--cluster-admin-account` и средство заполнения для параметров `cluster-users-group-dns`.</span><span class="sxs-lookup"><span data-stu-id="dc563-628">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="dc563-629">Параметр `cluster-users-group-dns` стал обязательным, если присутствует `—esp`.</span><span class="sxs-lookup"><span data-stu-id="dc563-629">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="dc563-630">Добавлено время ожидания для всех существующих средств автоматического заполнения аргументов.</span><span class="sxs-lookup"><span data-stu-id="dc563-630">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="dc563-631">Добавлено время ожидания для преобразования имени ресурса в идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="dc563-631">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="dc563-632">Внесены изменения в средства автоматического заполнения для выбора ресурсов из любой группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="dc563-632">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="dc563-633">Это может быть группа ресурсов, отличная от той, которая указана с помощью `-g`.</span><span class="sxs-lookup"><span data-stu-id="dc563-633">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="dc563-634">Добавлена поддержка параметров `--sub-domain-suffix` и `--disable_gateway_auth` в команде `hdinsight application create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-634">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="dc563-635">Управляемые службы</span><span class="sxs-lookup"><span data-stu-id="dc563-635">Managed Services</span></span>

* <span data-ttu-id="dc563-636">Командный модуль управляемых служб выпущен в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="dc563-636">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="dc563-637">Профиль</span><span class="sxs-lookup"><span data-stu-id="dc563-637">Profile</span></span>
* <span data-ttu-id="dc563-638">Аргумент `--subscription` подавляется для команды выхода.</span><span class="sxs-lookup"><span data-stu-id="dc563-638">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="dc563-639">RBAC</span><span class="sxs-lookup"><span data-stu-id="dc563-639">RBAC</span></span>

* <span data-ttu-id="dc563-640">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален аргумент `--password` для `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="dc563-640">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="dc563-641">В команду `create` добавлен параметр `--assignee-principal-type` для устранения периодических сбоев из-за задержки репликации сервера AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="dc563-641">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="dc563-642">Исправлен сбой в `ad signed-in-user` при перечислении собственных объектов.</span><span class="sxs-lookup"><span data-stu-id="dc563-642">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="dc563-643">Исправлена проблема, при которой `ad sp` не удавалось найти нужное приложение в субъекте-службе.</span><span class="sxs-lookup"><span data-stu-id="dc563-643">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="dc563-644">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="dc563-644">RDBMS</span></span>

* <span data-ttu-id="dc563-645">Добавлена поддержка репликации MariaDB.</span><span class="sxs-lookup"><span data-stu-id="dc563-645">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-646">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-646">SQL</span></span>

* <span data-ttu-id="dc563-647">Описаны допустимые значения для `sql db create --sample-name`.</span><span class="sxs-lookup"><span data-stu-id="dc563-647">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-648">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-648">Storage</span></span>

* <span data-ttu-id="dc563-649">В `storage blob generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="dc563-649">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="dc563-650">В `storage container generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="dc563-650">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="dc563-651">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-651">VM</span></span>

* <span data-ttu-id="dc563-652">Исправлена ошибка, при которой команда `vmss create` возвращала сообщение об ошибке при выполнении с `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="dc563-652">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="dc563-653">Прекращена проверка `vmss create --single-placement-group` на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="dc563-653">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="dc563-654">Команда не завершается сбоем, если для `--single-placement-group` задано значение `true`, а значение `--instance-count` больше 100 или указаны зоны доступности. Сама проверка теперь выполняется службой вычислений.</span><span class="sxs-lookup"><span data-stu-id="dc563-654">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="dc563-655">Исправлена ошибка, при которой команда `[vm|vmss] extension image list` завершалась сбоем при указании `--latest`.</span><span class="sxs-lookup"><span data-stu-id="dc563-655">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="dc563-656">18 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-656">June 18, 2019</span></span>

<span data-ttu-id="dc563-657">Версия 2.0.67</span><span class="sxs-lookup"><span data-stu-id="dc563-657">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="dc563-658">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-658">Core</span></span>

<span data-ttu-id="dc563-659">В этом выпуске добавлен новый тег [Предварительная версия], который яснее дает понять, что группа команд, команда или аргумент находятся в состоянии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="dc563-659">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="dc563-660">Ранее это указывалось в тексте справки или подразумевалось в номере версии командного модуля.</span><span class="sxs-lookup"><span data-stu-id="dc563-660">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="dc563-661">В будущем в интерфейсе командной строки номера версий отдельных пакетов не будут указываться.</span><span class="sxs-lookup"><span data-stu-id="dc563-661">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="dc563-662">Если команда доступна в предварительной версии, это также касается и всех ее аргументов.</span><span class="sxs-lookup"><span data-stu-id="dc563-662">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="dc563-663">Если группа команд помечается как находящаяся в предварительной версии, значит все команды и аргументы также считаются доступными в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="dc563-663">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="dc563-664">В результате этого изменения несколько групп команд могут "внезапно" оказаться в состоянии предварительной версии в этом выпуске.</span><span class="sxs-lookup"><span data-stu-id="dc563-664">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="dc563-665">В действительности большинство пакетов, которые находились в состоянии предварительной версии, в этом выпуске будут считаться общедоступными.</span><span class="sxs-lookup"><span data-stu-id="dc563-665">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-666">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-666">ACR</span></span>
* <span data-ttu-id="dc563-667">Добавлена команда acr check-health.</span><span class="sxs-lookup"><span data-stu-id="dc563-667">Added 'acr check-health' command</span></span>
* <span data-ttu-id="dc563-668">Улучшена обработка ошибок с маркерами безопасности AAD и ошибок при получении внешних команд.</span><span class="sxs-lookup"><span data-stu-id="dc563-668">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-669">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-669">ACS</span></span>
* <span data-ttu-id="dc563-670">Устаревшие команды ACS теперь скрыты в тексте справки.</span><span class="sxs-lookup"><span data-stu-id="dc563-670">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="dc563-671">AMS</span><span class="sxs-lookup"><span data-stu-id="dc563-671">AMS</span></span>
* <span data-ttu-id="dc563-672">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в возврате строк времени ISO 8601 для archive-window-length и key-frame-interval-duration.</span><span class="sxs-lookup"><span data-stu-id="dc563-672">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-673">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-673">AppService</span></span>
* <span data-ttu-id="dc563-674">Добавлена маршрутизация на основе расположение для `webapp deleted list` и `webapp deleted restore`.</span><span class="sxs-lookup"><span data-stu-id="dc563-674">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="dc563-675">Исправлена проблема, при которой целевой URL-адрес веб-приложения ("Вы можете запустить приложение в...") не был активным в Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="dc563-675">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="dc563-676">Устранена проблема, при которой создание приложений в некоторых SKU завершалось сбоем с ошибкой AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="dc563-676">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="dc563-677">Добавлена предварительная проверка в `[appservice|webapp] create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-677">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="dc563-678">Исправлено `[webapp|functionapp] traffic-routing` для использования правильного actionHostName.</span><span class="sxs-lookup"><span data-stu-id="dc563-678">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="dc563-679">Добавлена поддержка слотов для команд `functionapp`.</span><span class="sxs-lookup"><span data-stu-id="dc563-679">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="dc563-680">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="dc563-680">Batch</span></span>
* <span data-ttu-id="dc563-681">Исправлена регрессия проверки подлинности AAD, которую вызывал чрезмерный поток уведомлений об авторизации с помощью общего ключа.</span><span class="sxs-lookup"><span data-stu-id="dc563-681">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="dc563-682">Batch AI</span><span class="sxs-lookup"><span data-stu-id="dc563-682">BatchAI</span></span>
* <span data-ttu-id="dc563-683">Команды BatchAI теперь признаны устаревшими и скрыты.</span><span class="sxs-lookup"><span data-stu-id="dc563-683">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="dc563-684">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="dc563-684">BotService</span></span>
* <span data-ttu-id="dc563-685">Добавлены предупреждающие сообщения о прекращении поддержки и режиме обслуживания для команд, которые поддерживают пакет SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="dc563-685">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="dc563-686">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="dc563-686">CosmosDB</span></span>
* <span data-ttu-id="dc563-687">[УСТАРЕЛО] использовать команду `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="dc563-687">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="dc563-688">Добавлена команда `cosmosdb keys list`, заменяющая `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="dc563-688">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="dc563-689">`cosmsodb create/update`: Добавлен новый формат для --location, который позволяет задавать свойство isZoneRedundant.</span><span class="sxs-lookup"><span data-stu-id="dc563-689">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="dc563-690">Нерекомендуемый старый формат.</span><span class="sxs-lookup"><span data-stu-id="dc563-690">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="dc563-691">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="dc563-691">EventGrid</span></span>
* <span data-ttu-id="dc563-692">Добавлены команды `eventgrid domain` для операций CRUD домена.</span><span class="sxs-lookup"><span data-stu-id="dc563-692">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="dc563-693">Добавлены команды `eventgrid domain topic` для операций CRUD разделов домена.</span><span class="sxs-lookup"><span data-stu-id="dc563-693">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="dc563-694">В `eventgrid [topic|event-subscription] list` добавлен аргумент `--odata-query` для фильтрации результатов с использованием синтаксиса OData.</span><span class="sxs-lookup"><span data-stu-id="dc563-694">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="dc563-695">`event-subscription create/update`: Добавлена ServiceBusQueue в качестве новых значений для параметра `--endpoint-type`.</span><span class="sxs-lookup"><span data-stu-id="dc563-695">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="dc563-696">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в прекращении поддержки `--included-event-types All` с `eventgrid event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-696">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="dc563-697">HDInsight</span><span class="sxs-lookup"><span data-stu-id="dc563-697">HDInsight</span></span>
* <span data-ttu-id="dc563-698">Добавлена поддержка параметра `--ssh-public-key` в команде `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-698">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="dc563-699">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="dc563-699">IoT</span></span>
* <span data-ttu-id="dc563-700">Добавлена поддержка для повторного создания ключей политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="dc563-700">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="dc563-701">Добавлен пакет SDK и поддержка для службы подготовки репозитория DigitalTwin.</span><span class="sxs-lookup"><span data-stu-id="dc563-701">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="dc563-702">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-702">Network</span></span>
* <span data-ttu-id="dc563-703">Добавлена поддержка зон для Шлюза NAT.</span><span class="sxs-lookup"><span data-stu-id="dc563-703">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="dc563-704">Добавлена команда `network list-service-tags`.</span><span class="sxs-lookup"><span data-stu-id="dc563-704">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="dc563-705">Исправлена проблема с `dns zone import`, при которой пользователям не удавалось импортировать записи А с подстановочным знаком.</span><span class="sxs-lookup"><span data-stu-id="dc563-705">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="dc563-706">Исправлена проблема с `watcher flow-log configure`, при которой не удавалось включить ведение журнала потоков в определенных регионах.</span><span class="sxs-lookup"><span data-stu-id="dc563-706">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-707">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-707">Resource</span></span>
* <span data-ttu-id="dc563-708">Добавлена команда `az rest` для вызовов REST.</span><span class="sxs-lookup"><span data-stu-id="dc563-708">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="dc563-709">Исправлена ошибка, возникавшая при использовании `policy assignment list` с группой ресурсов или уровнем подписки `--scope`.</span><span class="sxs-lookup"><span data-stu-id="dc563-709">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="dc563-710">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="dc563-710">ServiceBus</span></span>
* <span data-ttu-id="dc563-711">Устранена проблема № [9319](https://github.com/azure/azure-cli/issues/9319) с `servicebus topic create --max-size`.</span><span class="sxs-lookup"><span data-stu-id="dc563-711">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-712">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-712">SQL</span></span>
* <span data-ttu-id="dc563-713">Параметр `--location` стал необязательным для `sql [server|mi] create`. Если он не указан, используется расположение группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="dc563-713">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="dc563-714">Исправлена ошибка "Объект NoneType не подлежит итерации" с `sql db list-editions --available`.</span><span class="sxs-lookup"><span data-stu-id="dc563-714">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="dc563-715">SQLVm</span><span class="sxs-lookup"><span data-stu-id="dc563-715">SQLVm</span></span>
* <span data-ttu-id="dc563-716">Критическое изменение. Для `sql vm create` теперь требуется параметр `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="dc563-716">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="dc563-717">Внесены изменения, позволяющие задавать SKU образа SQL при создании или обновлении виртуальной машины SQL.</span><span class="sxs-lookup"><span data-stu-id="dc563-717">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-718">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-718">Storage</span></span>
* <span data-ttu-id="dc563-719">Исправлена проблема с отсутствующим ключом учетной записи для `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="dc563-719">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="dc563-720">Исправлена проблема с `storage blob sync` на платформе Linux.</span><span class="sxs-lookup"><span data-stu-id="dc563-720">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-721">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-721">VM</span></span>
* <span data-ttu-id="dc563-722">[Предварительная версия] Добавлены команды `vm image template` для создания образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="dc563-722">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="dc563-723">4 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-723">June 4, 2019</span></span>

<span data-ttu-id="dc563-724">Версия 2.0.66</span><span class="sxs-lookup"><span data-stu-id="dc563-724">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="dc563-725">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-725">Core</span></span>
* <span data-ttu-id="dc563-726">Исправлена ошибка, из-за которой выполнение команды завершалось со сбоем, если параметр `--output yaml` использовался с параметром `--query`</span><span class="sxs-lookup"><span data-stu-id="dc563-726">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-727">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-727">ACR</span></span>
* <span data-ttu-id="dc563-728">Добавлена группа команд acr pack для создания заданий быстрой сборки с помощью пакетов сборок.</span><span class="sxs-lookup"><span data-stu-id="dc563-728">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-729">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-729">ACS</span></span>
* <span data-ttu-id="dc563-730">Разрешено включение и отключение надстройки панели мониторинга Kubernetes для AKS.</span><span class="sxs-lookup"><span data-stu-id="dc563-730">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="dc563-731">Если подписку нельзя использовать с Azure Red Hat OpenShift, будет отображаться соответствующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="dc563-731">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="dc563-732">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="dc563-732">Batch</span></span>
* <span data-ttu-id="dc563-733">Улучшена обработка ошибок, если не выполнен вход в учетную запись \[[№ 9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[№ 8978](https://github.com/Azure/azure-cli/issues/8978)\].</span><span class="sxs-lookup"><span data-stu-id="dc563-733">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="dc563-734">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="dc563-734">IoT</span></span>
* <span data-ttu-id="dc563-735">Добавлена поддержка для перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="dc563-735">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="dc563-736">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-736">Network</span></span>
* <span data-ttu-id="dc563-737">Добавлены команды `network application-gateway waf-policy` для поддержки настраиваемых правил WAF.</span><span class="sxs-lookup"><span data-stu-id="dc563-737">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="dc563-738">Добавлены аргументы `--waf-policy` и `--max-capacity` для команды `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="dc563-738">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="dc563-739">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-739">Resource</span></span>
* <span data-ttu-id="dc563-740">Улучшен вывод сообщения команды `deployment create` при отсутствии TTY.</span><span class="sxs-lookup"><span data-stu-id="dc563-740">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="dc563-741">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-741">Role</span></span>
* <span data-ttu-id="dc563-742">Обновлен текст справки.</span><span class="sxs-lookup"><span data-stu-id="dc563-742">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="dc563-743">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="dc563-743">Compute</span></span>
* <span data-ttu-id="dc563-744">Добавлена поддержка команды `vm create` для создания виртуальных машин из управляемого образа с номерами LUN дисков данных, которые не начинаются с 0 или для которых пропущены номера.</span><span class="sxs-lookup"><span data-stu-id="dc563-744">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="dc563-745">21 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-745">May 21, 2019</span></span>

<span data-ttu-id="dc563-746">Версия 2.0.65</span><span class="sxs-lookup"><span data-stu-id="dc563-746">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="dc563-747">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-747">Core</span></span>
* <span data-ttu-id="dc563-748">Улучшена функция обратной связи при ошибках аутентификации.</span><span class="sxs-lookup"><span data-stu-id="dc563-748">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="dc563-749">Исправлена проблема, из-за которой интерфейс командной строки загружал расширения, которые не были совместимы с его базовой версией.</span><span class="sxs-lookup"><span data-stu-id="dc563-749">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="dc563-750">Исправлена проблема с запуском и неисправностью `clouds.config`.</span><span class="sxs-lookup"><span data-stu-id="dc563-750">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-751">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-751">ACR</span></span>
* <span data-ttu-id="dc563-752">Добавлена поддержка управляемых удостоверений в Задачи.</span><span class="sxs-lookup"><span data-stu-id="dc563-752">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-753">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-753">ACS</span></span>
* <span data-ttu-id="dc563-754">Исправлена команда `openshift create`, используемая с пользовательским клиентом AAD.</span><span class="sxs-lookup"><span data-stu-id="dc563-754">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-755">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-755">AppService</span></span>
* <span data-ttu-id="dc563-756">[УСТАРЕЛО] Команда `functionapp devops-build` устарела и будет удалена в следующем выпуске.</span><span class="sxs-lookup"><span data-stu-id="dc563-756">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="dc563-757">Внесено изменение в `functionapp devops-pipeline` для получения журнала сборки из Azure DevOps в режиме подробного протоколирования.</span><span class="sxs-lookup"><span data-stu-id="dc563-757">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="dc563-758">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален неподдерживаемый флаг `--use_local_settings` из команды `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="dc563-758">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="dc563-759">Внесено изменение в `webapp up` для возврата выходных данных JSON, если `--logs` не используется.</span><span class="sxs-lookup"><span data-stu-id="dc563-759">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="dc563-760">Добавлена поддержка записи ресурсов по умолчанию в локальную конфигурацию для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="dc563-760">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="dc563-761">Добавлена поддержка `webapp up` для повторного развертывания приложения без использования аргумента `--location`.</span><span class="sxs-lookup"><span data-stu-id="dc563-761">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="dc563-762">Устранена проблема, из-за которой нельзя было создать для Linux номер SKU с планом службы приложений "Бесплатный".</span><span class="sxs-lookup"><span data-stu-id="dc563-762">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="dc563-763">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="dc563-763">BotService</span></span>
* <span data-ttu-id="dc563-764">Внесено изменение для включения поддержки всех регистров в параметрах `--lang` для команд.</span><span class="sxs-lookup"><span data-stu-id="dc563-764">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="dc563-765">Обновлено описание модуля команды.</span><span class="sxs-lookup"><span data-stu-id="dc563-765">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="dc563-766">Потребление</span><span class="sxs-lookup"><span data-stu-id="dc563-766">Consumption</span></span>
* <span data-ttu-id="dc563-767">Добавлен отсутствующий обязательный параметр при выполнении `consumption usage list --billing-period-name`.</span><span class="sxs-lookup"><span data-stu-id="dc563-767">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="dc563-768">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="dc563-768">IoT</span></span>
* <span data-ttu-id="dc563-769">Добавлена поддержка перечисления всех ключей.</span><span class="sxs-lookup"><span data-stu-id="dc563-769">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="dc563-770">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-770">Network</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="dc563-772">Добавлен аргумент `--nat-gateway` для `network vnet subnet [create|update]` для подключения к шлюзу NAT.</span><span class="sxs-lookup"><span data-stu-id="dc563-772">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="dc563-773">Исправлена проблема с `dns zone import`, из-за которой имена записей не сопоставлялись с типом записей.</span><span class="sxs-lookup"><span data-stu-id="dc563-773">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="dc563-774">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="dc563-774">RDBMS</span></span>
* <span data-ttu-id="dc563-775">Добавлена поддержка Postgres и MySQL для георепликации.</span><span class="sxs-lookup"><span data-stu-id="dc563-775">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="dc563-776">RBAC</span><span class="sxs-lookup"><span data-stu-id="dc563-776">RBAC</span></span>
* <span data-ttu-id="dc563-777">Добавлена поддержка области группы управления для `role assignment`.</span><span class="sxs-lookup"><span data-stu-id="dc563-777">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-778">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-778">Storage</span></span>
* <span data-ttu-id="dc563-779">`storage blob sync`: добавьте команду синхронизации для хранилища BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="dc563-779">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="dc563-780">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="dc563-780">Compute</span></span>
* <span data-ttu-id="dc563-781">Добавлен параметр `--computer-name` для `vm create` для установки имени виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="dc563-781">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="dc563-782">Переименован параметр `--ssh-key-value` в `--ssh-key-values` для `[vm|vmss] create` для приема нескольких значений пути или открытого ключа SSH.</span><span class="sxs-lookup"><span data-stu-id="dc563-782">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="dc563-783">__Примечание.__ Это **не** критическое изменение, благодаря которому `--ssh-key-value` будет правильно анализироваться, так как соответствует только `--ssh-key-values`.</span><span class="sxs-lookup"><span data-stu-id="dc563-783">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="dc563-784">Внесено изменение в аргумент `ppg create` для `--type` — теперь он необязательный.</span><span class="sxs-lookup"><span data-stu-id="dc563-784">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="dc563-785">6 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-785">May 6, 2019</span></span>

<span data-ttu-id="dc563-786">Версия 2.0.64</span><span class="sxs-lookup"><span data-stu-id="dc563-786">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-787">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-787">ACS</span></span>
* <span data-ttu-id="dc563-788">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--fqdn` из команд `openshift`.</span><span class="sxs-lookup"><span data-stu-id="dc563-788">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="dc563-789">Внесено изменение для использования общедоступной версии API для Azure Red Hat Openshift.</span><span class="sxs-lookup"><span data-stu-id="dc563-789">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="dc563-790">Добавлен флаг `customer-admin-group-id` в `openshift create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-790">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="dc563-791">[Общедоступная версия.] `(PREVIEW)` больше не используется для `aks create` в параметре `--network-policy`.</span><span class="sxs-lookup"><span data-stu-id="dc563-791">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-792">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-792">Appservice</span></span>
* <span data-ttu-id="dc563-793">[УСТАРЕЛО] Команда `functionapp devops-build` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="dc563-793">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="dc563-794">Команда переименована в `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="dc563-794">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="dc563-795">Исправлен процесс получения правильного имени пользователя для Cloud Shell, приводивший к ошибке выполнения `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="dc563-795">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="dc563-796">Обновлена документация по `appservice plan --sku` в соответствии с поддерживаемыми планами службы приложений.</span><span class="sxs-lookup"><span data-stu-id="dc563-796">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="dc563-797">Добавлены необязательные аргументы для группы ресурсов и план для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="dc563-797">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="dc563-798">Добавлена поддержка `webapp ssh` в соответствии с переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="dc563-798">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="dc563-799">Добавлена поддержка `appserviceplan create` для ценовой категории "Бесплатный" в Linux.</span><span class="sxs-lookup"><span data-stu-id="dc563-799">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="dc563-800">Внесено изменение в `webapp up` для перевода в спящий режим на 30 с после установки параметра приложения `SCM_DO_BUILD_DURING_DEPLOYMENT=true` для обработки холодного запуска Kudu.</span><span class="sxs-lookup"><span data-stu-id="dc563-800">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="dc563-801">Добавлена поддержка среды выполнения `powershell` для `functionapp create` в Windows.</span><span class="sxs-lookup"><span data-stu-id="dc563-801">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="dc563-802">Добавлена команда `create-remote-connection`.</span><span class="sxs-lookup"><span data-stu-id="dc563-802">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="dc563-803">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="dc563-803">Batch</span></span>
* <span data-ttu-id="dc563-804">Исправлена ошибка в проверяющем элементе управления для параметров `--application-package-references`.</span><span class="sxs-lookup"><span data-stu-id="dc563-804">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="dc563-805">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="dc563-805">Botservice</span></span>
* <span data-ttu-id="dc563-806">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` для создания пустого бота веб-приложения по умолчанию (т. е. бот не развертывается в Службе приложений).</span><span class="sxs-lookup"><span data-stu-id="dc563-806">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="dc563-807">Добавлен флаг `--echo` в `bot create` для использования старого поведения с `-v v4`.</span><span class="sxs-lookup"><span data-stu-id="dc563-807">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="dc563-808">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено значение по умолчанию `--version` на `v4`.</span><span class="sxs-lookup"><span data-stu-id="dc563-808">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="dc563-809">__ПРИМЕЧАНИЕ.__ `bot prepare-publish` по-прежнему использует старое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-809">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="dc563-810">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `--lang` — значение `Csharp` больше не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-810">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="dc563-811">Если команда требует `--lang`, который не указан, команда завершит работу с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="dc563-811">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="dc563-812">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в аргументы `--appid` и `--password` для `bot create` — теперь они являются обязательными и их можно создать с помощью `ad app create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-812">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="dc563-813">Добавлена проверка `--appid` и `--password`.</span><span class="sxs-lookup"><span data-stu-id="dc563-813">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="dc563-814">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4`, чтобы не создавать или не использовать учетную запись хранения или Application Insights.</span><span class="sxs-lookup"><span data-stu-id="dc563-814">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="dc563-815">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v3`, чтобы требовать регион, где доступна служба Application Insights.</span><span class="sxs-lookup"><span data-stu-id="dc563-815">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="dc563-816">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot update`, чтобы влиять только на определенные свойства бота.</span><span class="sxs-lookup"><span data-stu-id="dc563-816">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="dc563-817">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в флаг `--lang` для принятия `Javascript` вместо `Node`.</span><span class="sxs-lookup"><span data-stu-id="dc563-817">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="dc563-818">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`Node` больше не используется как допустимое значение `--lang`.</span><span class="sxs-lookup"><span data-stu-id="dc563-818">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="dc563-819">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` — значение `SCM_DO_BUILD_DURING_DEPLOYMENT` больше не равно true.</span><span class="sxs-lookup"><span data-stu-id="dc563-819">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="dc563-820">Все развертывания через Kudu будут работать в соответствии с поведением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-820">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="dc563-821">Внесено изменение в `bot download` для ботов без файлов `.bot`, чтобы создавать файл конфигурации для определенного языка со значениями из параметров приложения для бота.</span><span class="sxs-lookup"><span data-stu-id="dc563-821">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="dc563-822">В команду `bot prepare-deploy` добавлена поддержка параметра `Typescript`.</span><span class="sxs-lookup"><span data-stu-id="dc563-822">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="dc563-823">Добавлено предупреждающее сообщение в `bot prepare-deploy` для ботов `Javascript` и `Typescript`, когда `--code-dir` не содержит `package.json`.</span><span class="sxs-lookup"><span data-stu-id="dc563-823">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="dc563-824">Внесено изменение в `bot prepare-deploy` для возврата `true` при успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="dc563-824">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="dc563-825">Включено ведение подробного журнала для `bot prepare-deploy`.</span><span class="sxs-lookup"><span data-stu-id="dc563-825">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="dc563-826">Добавлены более доступные регионы Application Insights для `az bot create -v v3`.</span><span class="sxs-lookup"><span data-stu-id="dc563-826">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="dc563-827">Configure</span><span class="sxs-lookup"><span data-stu-id="dc563-827">Configure</span></span>
* <span data-ttu-id="dc563-828">Добавлена поддержка конфигурации по умолчанию для аргумента на основе папки.</span><span class="sxs-lookup"><span data-stu-id="dc563-828">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="dc563-829">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="dc563-829">Eventhubs</span></span>
* <span data-ttu-id="dc563-830">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="dc563-830">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="dc563-831">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-831">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="dc563-832">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-832">Network</span></span>
* <span data-ttu-id="dc563-833">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--cache` на `--defer` для `vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-833">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="dc563-834">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="dc563-834">Policy Insights</span></span>
* <span data-ttu-id="dc563-835">Добавлена поддержка `--expand PolicyEvaluationDetails` для результатов оценки политики запросов для ресурса.</span><span class="sxs-lookup"><span data-stu-id="dc563-835">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="dc563-836">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-836">Role</span></span>
* <span data-ttu-id="dc563-837">[УСТАРЕЛО] Внесено изменение в `create-for-rbac` для скрытия аргумента --password (поддержка прекращается в мае 2019 г.).</span><span class="sxs-lookup"><span data-stu-id="dc563-837">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="dc563-838">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="dc563-838">Service Bus</span></span>
* <span data-ttu-id="dc563-839">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="dc563-839">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="dc563-840">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-840">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="dc563-841">Внесено исправление в `topic [create|update]` — теперь `--max-size` поддерживает значения 10, 20, 40 и 80 ГБ для номера SKU ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="dc563-841">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-842">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-842">SQL</span></span>
* <span data-ttu-id="dc563-843">Добавлены команды `sql virtual-cluster [list|show|delete]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-843">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-844">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-844">VM</span></span>
* <span data-ttu-id="dc563-845">Добавлены параметры `--protect-from-scale-in` и `--protect-from-scale-set-actions` для `vmss update`, чтобы включать обновления политики защиты для экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="dc563-845">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="dc563-846">Добавлены параметры `--instance-id` для `vmss update` для включения общего обновления экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="dc563-846">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="dc563-847">Добавлен параметр `--instance-id` для команды `vmss wait`.</span><span class="sxs-lookup"><span data-stu-id="dc563-847">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="dc563-848">Добавлена новая группа команд `ppg` для управления группами размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="dc563-848">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="dc563-849">Добавлен параметр `--ppg` для `[vm|vmss] create` и `vm availability-set create` для управления PPG.</span><span class="sxs-lookup"><span data-stu-id="dc563-849">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="dc563-850">Добавлен параметр `--hyper-v-generation` для команды `image create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-850">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="dc563-851">23 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-851">April 23, 2019</span></span>

<span data-ttu-id="dc563-852">Версия 2.0.63</span><span class="sxs-lookup"><span data-stu-id="dc563-852">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-853">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-853">ACS</span></span>
* <span data-ttu-id="dc563-854">Внесено изменение в `aks get-credentials` для запроса на перезапись повторяющихся значений.</span><span class="sxs-lookup"><span data-stu-id="dc563-854">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="dc563-855">Удалено описание `(PREVIEW)` из команд Dev Spaces aks use-dev-spaces и aks remove-dev-spaces.</span><span class="sxs-lookup"><span data-stu-id="dc563-855">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="dc563-856">AMS</span><span class="sxs-lookup"><span data-stu-id="dc563-856">AMS</span></span>
* <span data-ttu-id="dc563-857">Исправлена ошибка с обновлением фильтров ресурсов и учетных записей.</span><span class="sxs-lookup"><span data-stu-id="dc563-857">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-858">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-858">AppService</span></span>
* <span data-ttu-id="dc563-859">Добавлена поддержка ASE и времени ожидания для `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="dc563-859">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="dc563-860">Добавлена возможность настройки непрерывной интеграции и развертывания в конвейере Azure DevOps из репозитория Github для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="dc563-860">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="dc563-861">Добавлен аргумент `--github-pat` для `functionapp devops-build create` для получения личного маркера доступа Github.</span><span class="sxs-lookup"><span data-stu-id="dc563-861">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="dc563-862">Добавлен аргумент `--github-repository` для `functionapp devops-build create` для подключения репозитория Github, который содержит исходный код приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="dc563-862">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="dc563-863">Исправлена проблема со сбоем `az webapp up --logs` и обновлением .Net Core до версии 2.1 по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-863">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="dc563-864">Удалены ненужные параметры приложения-функции при создании приложения-функции с помощью плана потребления.</span><span class="sxs-lookup"><span data-stu-id="dc563-864">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="dc563-865">Внесены изменения в `webapp up`, чтобы строка ASP по умолчанию добавляла номера в конец для создания плана службы приложений на основе параметров SKU.</span><span class="sxs-lookup"><span data-stu-id="dc563-865">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="dc563-866">Добавлен параметр `-b` для `webapp up` для запуска приложения в браузере.</span><span class="sxs-lookup"><span data-stu-id="dc563-866">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="dc563-867">Внесены изменения в `webapp deployment source config zip` для обработки переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="dc563-867">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="dc563-868">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="dc563-868">Deployment Manager</span></span>
* <span data-ttu-id="dc563-869">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Создание и администрирование артефактов, которые поддерживают развертывания</span><span class="sxs-lookup"><span data-stu-id="dc563-869">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="dc563-870">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="dc563-870">Lab</span></span>
* <span data-ttu-id="dc563-871">Исправлена ошибка, которая приводила к неожиданному завершению работы.</span><span class="sxs-lookup"><span data-stu-id="dc563-871">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="dc563-872">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-872">Network</span></span>
* <span data-ttu-id="dc563-873">Добавлено автоматическое делегирование сервера имен для `dns zone create` в родительском объекте во время создания дочерней зоны.</span><span class="sxs-lookup"><span data-stu-id="dc563-873">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-874">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-874">Resource</span></span>
* <span data-ttu-id="dc563-875">[УСТАРЕЛО] Не рекомендуются к использованию аргументы `--link-id`, `--target-id` и `--filter-string` для `resource link`.</span><span class="sxs-lookup"><span data-stu-id="dc563-875">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="dc563-876">Используйте вместо них аргументы `--link`, `--target` и `--filter`.</span><span class="sxs-lookup"><span data-stu-id="dc563-876">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="dc563-877">Исправлена проблема, из-за которой команды `resource link [create|update]` не работали.</span><span class="sxs-lookup"><span data-stu-id="dc563-877">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="dc563-878">Исправлена проблема, из-за которой удаление с помощью идентификатора ресурса приводило к сбою или ошибке.</span><span class="sxs-lookup"><span data-stu-id="dc563-878">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-879">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-879">SQL</span></span>
* <span data-ttu-id="dc563-880">Добавлена поддержка пользовательского часового пояса в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="dc563-880">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="dc563-881">Внесено изменение, чтобы разрешить использовать имя эластичного пула с `sql db update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-881">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="dc563-882">В команду `sql server [create|update]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="dc563-882">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="dc563-883">Добавлена команда `sql server wait`.</span><span class="sxs-lookup"><span data-stu-id="dc563-883">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-884">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-884">Storage</span></span>
* <span data-ttu-id="dc563-885">Устранена проблема с двойной кодировкой маркеров SAS в `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="dc563-885">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-886">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-886">VM</span></span>
* <span data-ttu-id="dc563-887">Добавлен флаг `--skip-shutdown` для `vm|vmss stop` для выключения виртуальных машин без завершения работы.</span><span class="sxs-lookup"><span data-stu-id="dc563-887">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="dc563-888">Добавлен аргумент `--storage-account-type` для `sig image-version create` настройки типа учетной записи профиля публикации.</span><span class="sxs-lookup"><span data-stu-id="dc563-888">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="dc563-889">Добавлен аргумент `--target-regions` для `sig image-version create` для указания типов учетных записей хранения, связанных с регионами.</span><span class="sxs-lookup"><span data-stu-id="dc563-889">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="dc563-890">9 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-890">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="dc563-891">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-891">Core</span></span>
* <span data-ttu-id="dc563-892">Исправлена проблема, из-за которой для некоторых расширений отображалась версия `Unknown` и ее невозможно было обновить.</span><span class="sxs-lookup"><span data-stu-id="dc563-892">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-893">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-893">ACR</span></span>
* <span data-ttu-id="dc563-894">Добавлена поддержка запуска образа без контекста.</span><span class="sxs-lookup"><span data-stu-id="dc563-894">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="dc563-895">AMS</span><span class="sxs-lookup"><span data-stu-id="dc563-895">AMS</span></span>
* [УСТАРЕЛО]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="dc563-898">Добавлена поддержка новых параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-898">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="dc563-899">Добавлен новый параметр `--filters` для `ams streaming-locator create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-899">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-900">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-900">AppService</span></span>
* <span data-ttu-id="dc563-901">В команду `webapp up` добавлена поддержка параметра `--logs`.</span><span class="sxs-lookup"><span data-stu-id="dc563-901">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="dc563-902">Исправлены ошибки в команде `functionapp devops-build create` при создании файла `azure-pipelines.yml`.</span><span class="sxs-lookup"><span data-stu-id="dc563-902">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="dc563-903">Улучшена обработка и индикаторы ошибок с `unctionapp devops-build create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-903">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="dc563-904">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--local-git` для команды `devops-build`. Обнаружение и обработка локального репозитория Git являются обязательными для создания конвейеров DevOps в Azure.</span><span class="sxs-lookup"><span data-stu-id="dc563-904">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="dc563-905">Добавлена поддержка создания плана функций Linux.</span><span class="sxs-lookup"><span data-stu-id="dc563-905">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="dc563-906">Добавлена возможность менять план для приложения-функции с помощью `functionapp update --plan`.</span><span class="sxs-lookup"><span data-stu-id="dc563-906">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="dc563-907">Добавлена поддержка параметров масштабирования плана "Премиум" для Функций Azure.</span><span class="sxs-lookup"><span data-stu-id="dc563-907">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="dc563-908">CDN</span><span class="sxs-lookup"><span data-stu-id="dc563-908">CDN</span></span>
* <span data-ttu-id="dc563-909">Добавлена поддержка `Microsoft_Standard` и `Standard_ChinaCdn`.</span><span class="sxs-lookup"><span data-stu-id="dc563-909">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="dc563-910">Отзывы</span><span class="sxs-lookup"><span data-stu-id="dc563-910">Feedback</span></span>
* <span data-ttu-id="dc563-911">Внесены изменения в `feedback` для отображения метаданных недавно выполненных команд.</span><span class="sxs-lookup"><span data-stu-id="dc563-911">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="dc563-912">Внесены изменения в `feedback`. Теперь при регистрации проблемы отображается запрос, в соответствии с которым пользователь должен открыть браузер и воспользоваться шаблоном проблемы.</span><span class="sxs-lookup"><span data-stu-id="dc563-912">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="dc563-913">Внесены изменения в `feedback`. Теперь текст проблемы выводится при запуске с параметром --verbose.</span><span class="sxs-lookup"><span data-stu-id="dc563-913">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="dc563-914">Монитор</span><span class="sxs-lookup"><span data-stu-id="dc563-914">Monitor</span></span>
* <span data-ttu-id="dc563-915">Исправлена проблема, из-за которой у параметра count было недопустимое значение в `metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-915">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="dc563-916">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-916">Network</span></span>
* <span data-ttu-id="dc563-917">Исправлен формат таблицы, которая не отображалась с помощью `vnet-gateway list-bgp-peer-status`.</span><span class="sxs-lookup"><span data-stu-id="dc563-917">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="dc563-918">Добавлены команды `list-request-headers` и `list-response-headers` для `application-gateway rewrite-rule`.</span><span class="sxs-lookup"><span data-stu-id="dc563-918">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="dc563-919">Добавлена команда `list-server-variables` для `application-gateway rewrite-rule condition`.</span><span class="sxs-lookup"><span data-stu-id="dc563-919">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="dc563-920">Исправлена проблема, из-за которой обновление состояния соединения на порту ExpressRoute вызывало неизвестное исключение атрибута `express-route port update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-920">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="dc563-921">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="dc563-921">PrivateDNS</span></span>
* <span data-ttu-id="dc563-922">Добавлена команда `network private-dns` для частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="dc563-922">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-923">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-923">Resource</span></span>
* <span data-ttu-id="dc563-924">Исправлена проблема с `deployment create` и `group deployment create`, из-за которой файл параметров с пустым набором параметров не работал.</span><span class="sxs-lookup"><span data-stu-id="dc563-924">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="dc563-925">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-925">Role</span></span>
* <span data-ttu-id="dc563-926">Внесены исправления в `create-for-rbac`. Теперь `--years` обрабатывается правильно.</span><span class="sxs-lookup"><span data-stu-id="dc563-926">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="dc563-927">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `role assignment delete`. Теперь появляется запрос при удалении всех назначений в рамках подписки без дополнительных условий.</span><span class="sxs-lookup"><span data-stu-id="dc563-927">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-928">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-928">SQL</span></span>
* <span data-ttu-id="dc563-929">Команда `sql mi [create|update]` обновлена с помощью свойств proxyOverride и publicDataEndpointEnabled.</span><span class="sxs-lookup"><span data-stu-id="dc563-929">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-930">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-930">Storage</span></span>
* <span data-ttu-id="dc563-931">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален результат выполнения `storage blob delete`.</span><span class="sxs-lookup"><span data-stu-id="dc563-931">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="dc563-932">В команду `storage blob generate-sas` добавлен параметр `--full-uri` для создания полного URI большого двоичного объекта с помощью SAS.</span><span class="sxs-lookup"><span data-stu-id="dc563-932">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="dc563-933">В команду `storage file copy start` добавлен параметр `--file-snapshot` для копирования файла из моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="dc563-933">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="dc563-934">Внесены изменения в `storage blob copy cancel`. Теперь вместо исключения для NoPendingCopyOperation отображается только сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="dc563-934">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="dc563-935">26 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-935">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="dc563-936">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-936">Core</span></span>
* <span data-ttu-id="dc563-937">Устранены проблемы с несовместимостью расширений для разработки.</span><span class="sxs-lookup"><span data-stu-id="dc563-937">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="dc563-938">Функция обработки ошибок теперь указывает клиентам на страницу проблем.</span><span class="sxs-lookup"><span data-stu-id="dc563-938">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="dc563-939">Cloud</span><span class="sxs-lookup"><span data-stu-id="dc563-939">Cloud</span></span>
* <span data-ttu-id="dc563-940">Исправлена ошибка с сообщением о не найденной подписке в `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="dc563-940">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-941">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-941">ACR</span></span>
* <span data-ttu-id="dc563-942">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="dc563-942">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="dc563-943">Добавлено `--auth-mode` в команды `acr build`, `acr run`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-943">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="dc563-944">Добавлена команда acr task credential для управления учетными данными для задачи.</span><span class="sxs-lookup"><span data-stu-id="dc563-944">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="dc563-945">Добавлено --no-wait в команду `acr build`.</span><span class="sxs-lookup"><span data-stu-id="dc563-945">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-946">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-946">AppService</span></span>
* <span data-ttu-id="dc563-947">Исправлена ошибка с `webapp up`, из-за которой нельзя было правильно выполнить запуск из пустого каталога или скрипта неизвестного кода.</span><span class="sxs-lookup"><span data-stu-id="dc563-947">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="dc563-948">Исправлена ошибка, из-за которой не работали слоты для `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="dc563-948">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="dc563-949">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="dc563-949">BOT Service</span></span>
* <span data-ttu-id="dc563-950">Добавлено `bot prepare-deploy` для подготовки к развертыванию ботов с помощью `webapp`.</span><span class="sxs-lookup"><span data-stu-id="dc563-950">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="dc563-951">Изменено `bot create --kind registration` для отображения пароля, если пароль не указан.</span><span class="sxs-lookup"><span data-stu-id="dc563-951">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="dc563-952">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--endpoint` в `bot create --kind registration` на пустую строку (по умолчанию) вместо запрашиваемой.</span><span class="sxs-lookup"><span data-stu-id="dc563-952">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="dc563-953">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="dc563-953">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="dc563-954">CDN</span><span class="sxs-lookup"><span data-stu-id="dc563-954">CDN</span></span>
* <span data-ttu-id="dc563-955">Добавлена поддержка параметра `--no-wait` в команде `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-955">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="dc563-956">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено поведение кэширования строки запроса `cdn endpoint create` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-956">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="dc563-957">IgnoreQueryString больше не используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-957">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="dc563-958">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="dc563-958">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="dc563-959">Сosmos DB</span><span class="sxs-lookup"><span data-stu-id="dc563-959">Cosmosdb</span></span>
* <span data-ttu-id="dc563-960">Добавлена поддержка `--enable-multiple-write-locations` для обновления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="dc563-960">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="dc563-961">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="dc563-961">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="dc563-962">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="dc563-962">Interactive</span></span>
* <span data-ttu-id="dc563-963">Исправлена несовместимость с интерактивным расширением, установленным с помощью azdev.</span><span class="sxs-lookup"><span data-stu-id="dc563-963">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="dc563-964">Монитор</span><span class="sxs-lookup"><span data-stu-id="dc563-964">Monitor</span></span>
* <span data-ttu-id="dc563-965">Внесено изменение, разрешающее использовать значение измерения `*` для `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-965">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="dc563-966">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-966">Network</span></span>
* <span data-ttu-id="dc563-967">Добавлена группа команд `rewrite-rule` для `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="dc563-967">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="dc563-968">Профиль</span><span class="sxs-lookup"><span data-stu-id="dc563-968">Profile</span></span>
* <span data-ttu-id="dc563-969">Включена поддержка учетной записи уровня клиентов для управляемого удостоверения службы для `login`.</span><span class="sxs-lookup"><span data-stu-id="dc563-969">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="dc563-970">Postgres</span><span class="sxs-lookup"><span data-stu-id="dc563-970">Postgres</span></span> 
* <span data-ttu-id="dc563-971">Добавлены команды postgresql `replica` и команда `restart server`.</span><span class="sxs-lookup"><span data-stu-id="dc563-971">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="dc563-972">Внесены изменения для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="dc563-972">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-973">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-973">Resource</span></span>
* <span data-ttu-id="dc563-974">Улучшены табличные выходные данные для `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-974">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="dc563-975">Исправлена проблема с `deployment [create|validate]`, из-за которой secureObject типа не распознавался.</span><span class="sxs-lookup"><span data-stu-id="dc563-975">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="dc563-976">График</span><span class="sxs-lookup"><span data-stu-id="dc563-976">Graph</span></span>
* <span data-ttu-id="dc563-977">Добавлена поддержка параметра `--end-date` в команде `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="dc563-977">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="dc563-978">Добавлена поддержка разрешений для `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="dc563-978">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="dc563-979">Исправлена проблема с `ad app permission list`, из-за которой отсутствовали разрешения.</span><span class="sxs-lookup"><span data-stu-id="dc563-979">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="dc563-980">Изменено `ad sp delete` для пропуска удаления назначения роли, если текущая учетная запись не содержит подписок.</span><span class="sxs-lookup"><span data-stu-id="dc563-980">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="dc563-981">Изменено `ad app create` для использования `--identifier-uris` пустого списка (по умолчанию), если список не указан.</span><span class="sxs-lookup"><span data-stu-id="dc563-981">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-982">носителей.</span><span class="sxs-lookup"><span data-stu-id="dc563-982">storage</span></span>
* <span data-ttu-id="dc563-983">Добавлено `--snapshot` для `storage file download-batch` для скачивания из моментального снимка общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="dc563-983">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="dc563-984">Изменен индикатор выполнения `storage blob [download-batch|upload-batch]`, чтобы обобщить сведения и указать текущий большой двоичный объект.</span><span class="sxs-lookup"><span data-stu-id="dc563-984">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="dc563-985">Исправлена проблема с `storage account update` при обновлении параметров шифрования.</span><span class="sxs-lookup"><span data-stu-id="dc563-985">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="dc563-986">Исправлена проблема со сбоем `storage blob show` при использовании OAuth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="dc563-986">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-987">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-987">VM</span></span>
* <span data-ttu-id="dc563-988">Добавлена команда `image update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-988">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="dc563-989">12 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-989">March 12, 2019</span></span>

<span data-ttu-id="dc563-990">Версия 2.0.60</span><span class="sxs-lookup"><span data-stu-id="dc563-990">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="dc563-991">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-991">Core</span></span>

* <span data-ttu-id="dc563-992">Исправлена недопустимая ошибка в `cloud set` о том, что подписка не найдена.</span><span class="sxs-lookup"><span data-stu-id="dc563-992">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-993">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-993">ACR</span></span>

* <span data-ttu-id="dc563-994">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="dc563-994">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-995">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-995">ACS</span></span>

* <span data-ttu-id="dc563-996">Внесены изменения, в соответствии с которыми параметр `--listen-address` для `aks browse` игнорируется, если он не поддерживается kubectl.</span><span class="sxs-lookup"><span data-stu-id="dc563-996">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="dc563-997">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-997">AppService</span></span>

* <span data-ttu-id="dc563-998">Добавлено `[webapp|functionapp] deployment list-publishing-credentials` для получения URL-адреса публикации Kudu и связанных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="dc563-998">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="dc563-999">Удалена ошибочная инструкция печати для `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-999">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="dc563-1000">Исправлено `functionapp` для настройки правильного образа для среды выполнения в планах службы приложений Linux.</span><span class="sxs-lookup"><span data-stu-id="dc563-1000">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="dc563-1001">Удален тег предварительной версии для `webapp up` и добавлены усовершенствования в команду.</span><span class="sxs-lookup"><span data-stu-id="dc563-1001">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="dc563-1002">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="dc563-1002">Botservice</span></span>

* <span data-ttu-id="dc563-1003">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="dc563-1003">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="dc563-1004">Добавлено `Microsoft-BotFramework-AppId` и `Microsoft-BotFramework-AppPassword` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="dc563-1004">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="dc563-1005">Удалены одинарные кавычки из выходных данных команды `bot publish` в конце `bot create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1005">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="dc563-1006">Изменено `bot publish` для включения поддержки асинхронных операций.</span><span class="sxs-lookup"><span data-stu-id="dc563-1006">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="dc563-1007">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-1007">Container</span></span>

* <span data-ttu-id="dc563-1008">Добавлен аргумент `--no-wait` для команды `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="dc563-1008">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="dc563-1009">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="dc563-1009">EventHub</span></span>

* <span data-ttu-id="dc563-1010">Добавлен флаг `--skip-empty-archives` для `eventhub create|update` для включения поддержки пустых архивов при записи.</span><span class="sxs-lookup"><span data-stu-id="dc563-1010">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="dc563-1011">Поиск</span><span class="sxs-lookup"><span data-stu-id="dc563-1011">Find</span></span>

* <span data-ttu-id="dc563-1012">Основные обновления функций</span><span class="sxs-lookup"><span data-stu-id="dc563-1012">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="dc563-1013">HDInsight</span><span class="sxs-lookup"><span data-stu-id="dc563-1013">HDInsight</span></span>

* <span data-ttu-id="dc563-1014">Добавлен параметр `--storage-account-managed-identity` для `hdinsight create` для включения поддержки MSI ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="dc563-1014">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="dc563-1015">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-1015">Network</span></span>

* <span data-ttu-id="dc563-1016">Исправлена проблема с `vpn-connection update`, когда обновление VPN-подключения между шлюзами в разных подписках завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="dc563-1016">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="dc563-1017">Rdbms</span><span class="sxs-lookup"><span data-stu-id="dc563-1017">Rdbms</span></span>

* <span data-ttu-id="dc563-1018">Незначительные исправления для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="dc563-1018">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="dc563-1019">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-1019">Role</span></span>

* <span data-ttu-id="dc563-1020">Исправлено `role definition update` для использования идентификатора для правильного разрешения определения.</span><span class="sxs-lookup"><span data-stu-id="dc563-1020">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="dc563-1021">Изменено `ad app credential reset` для исключения предположения о том, что субъект-служба приложения всегда существует.</span><span class="sxs-lookup"><span data-stu-id="dc563-1021">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="dc563-1022">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="dc563-1022">Service Fabric</span></span>

* <span data-ttu-id="dc563-1023">Исправлена проблема с `sf cluster list` и невозможностью итерации.</span><span class="sxs-lookup"><span data-stu-id="dc563-1023">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="dc563-1024">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1024">February 26, 2019</span></span>

<span data-ttu-id="dc563-1025">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="dc563-1025">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="dc563-1026">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-1026">Core</span></span>

* <span data-ttu-id="dc563-1027">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="dc563-1027">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-1028">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-1028">ACR</span></span>

* <span data-ttu-id="dc563-1029">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1029">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="dc563-1030">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="dc563-1030">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-1031">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-1031">ACS</span></span>

* <span data-ttu-id="dc563-1032">Добавлен параметр `--listen-address` для команды `aks port-forward`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1032">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-1033">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-1033">AppService</span></span>

* <span data-ttu-id="dc563-1034">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1034">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="dc563-1035">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="dc563-1035">Batch</span></span>
* <span data-ttu-id="dc563-1036">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1036">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="dc563-1037">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1037">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="dc563-1038">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="dc563-1038">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="dc563-1039">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1039">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="dc563-1040">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="dc563-1040">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="dc563-1041">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="dc563-1041">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="dc563-1042">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="dc563-1042">CosmosDB</span></span>

* <span data-ttu-id="dc563-1043">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="dc563-1043">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="dc563-1044">Kusto</span><span class="sxs-lookup"><span data-stu-id="dc563-1044">Kusto</span></span>

* <span data-ttu-id="dc563-1045">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="dc563-1045">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="dc563-1046">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-1046">Network</span></span>

* <span data-ttu-id="dc563-1047">Добавлен аргумент `--express-route-gateway-bypass` для команды `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="dc563-1047">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="dc563-1048">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1048">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="dc563-1049">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1049">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="dc563-1050">Добавлен аргумент `--legacy-mode` в команду `express-route peering [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1050">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="dc563-1051">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1051">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="dc563-1052">Добавлен аргумент `--gateway-default-site` для команды `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="dc563-1052">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="dc563-1053">Добавлены команды `ipsec-policy` для `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1053">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-1054">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-1054">Resource</span></span>

* <span data-ttu-id="dc563-1055">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="dc563-1055">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="dc563-1056">Добавлена поддержка файла параметров на основе URI для `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1056">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="dc563-1057">Добавлена поддержка определений и параметров на основе URI для `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1057">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="dc563-1058">Исправлена обработка параметров и правил для `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1058">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="dc563-1059">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="dc563-1059">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="dc563-1060">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-1060">Role</span></span>

* <span data-ttu-id="dc563-1061">Добавлена поддержка ролей приложений для `ad app [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1061">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1062">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1062">VM</span></span>

* <span data-ttu-id="dc563-1063">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="dc563-1063">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="dc563-1064">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1064">February 12, 2019</span></span>

<span data-ttu-id="dc563-1065">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="dc563-1065">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="dc563-1066">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-1066">Core</span></span>

* <span data-ttu-id="dc563-1067">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="dc563-1067">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="dc563-1068">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="dc563-1068">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-1069">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-1069">ACR</span></span>
* <span data-ttu-id="dc563-1070">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1070">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="dc563-1071">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1071">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-1072">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-1072">ACS</span></span>
* <span data-ttu-id="dc563-1073">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="dc563-1073">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="dc563-1074">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1074">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="dc563-1075">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="dc563-1075">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="dc563-1076">AMS</span><span class="sxs-lookup"><span data-stu-id="dc563-1076">AMS</span></span>
* <span data-ttu-id="dc563-1077">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1077">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="dc563-1078">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1078">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-1079">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-1079">Appservice</span></span>
* <span data-ttu-id="dc563-1080">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="dc563-1080">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="dc563-1081">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="dc563-1081">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="dc563-1082">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1082">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="dc563-1083">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="dc563-1083">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="dc563-1084">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="dc563-1084">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="dc563-1085">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="dc563-1085">Botservice</span></span>
* <span data-ttu-id="dc563-1086">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1086">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="dc563-1087">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1087">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="dc563-1088">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1088">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="dc563-1089">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="dc563-1089">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="dc563-1090">[УСТАРЕЛО] Аргумент `--proj-name` не рекомендуется к использованию. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1090">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="dc563-1091">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="dc563-1091">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="dc563-1092">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="dc563-1092">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="dc563-1093">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="dc563-1093">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="dc563-1094">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="dc563-1094">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="dc563-1095">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="dc563-1095">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="dc563-1096">Key Vault</span><span class="sxs-lookup"><span data-stu-id="dc563-1096">Key Vault</span></span>
* <span data-ttu-id="dc563-1097">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1097">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="dc563-1098">Монитор</span><span class="sxs-lookup"><span data-stu-id="dc563-1098">Monitor</span></span>
* <span data-ttu-id="dc563-1099">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1099">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="dc563-1100">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-1100">Network</span></span>
* <span data-ttu-id="dc563-1101">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="dc563-1101">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="dc563-1102">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="dc563-1102">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="dc563-1103">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="dc563-1103">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="dc563-1104">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1104">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="dc563-1105">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="dc563-1105">Policy Insights</span></span>
* <span data-ttu-id="dc563-1106">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1106">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="dc563-1107">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="dc563-1107">RDBMS</span></span>
* <span data-ttu-id="dc563-1108">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="dc563-1108">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="dc563-1109">Redis</span><span class="sxs-lookup"><span data-stu-id="dc563-1109">Redis</span></span>
* <span data-ttu-id="dc563-1110">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="dc563-1110">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="dc563-1111">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="dc563-1111">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="dc563-1112">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="dc563-1112">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="dc563-1113">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="dc563-1113">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="dc563-1114">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1114">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="dc563-1115">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="dc563-1115">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="dc563-1116">[УСТАРЕЛО] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc563-1116">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="dc563-1117">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-1117">Role</span></span>
* <span data-ttu-id="dc563-1118">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1118">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="dc563-1119">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-1119">SQL VM</span></span>
* <span data-ttu-id="dc563-1120">[УСТАРЕЛО] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="dc563-1120">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1121">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1121">VM</span></span>
* <span data-ttu-id="dc563-1122">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1122">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="dc563-1123">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1123">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="dc563-1124">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="dc563-1124">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="dc563-1125">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1125">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="dc563-1126">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1126">January 31, 2019</span></span>

<span data-ttu-id="dc563-1127">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="dc563-1127">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="dc563-1128">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-1128">Core</span></span>

* <span data-ttu-id="dc563-1129">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="dc563-1129">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="dc563-1130">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1130">January 28, 2019</span></span>

<span data-ttu-id="dc563-1131">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="dc563-1131">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-1132">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-1132">ACR</span></span>
* <span data-ttu-id="dc563-1133">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1133">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-1134">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-1134">ACS</span></span>
* <span data-ttu-id="dc563-1135">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1135">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="dc563-1136">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="dc563-1136">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="dc563-1137">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1137">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="dc563-1138">AMS</span><span class="sxs-lookup"><span data-stu-id="dc563-1138">AMS</span></span>
* <span data-ttu-id="dc563-1139">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1139">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="dc563-1140">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1140">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-1141">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-1141">Appservice</span></span>
* <span data-ttu-id="dc563-1142">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1142">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="dc563-1143">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="dc563-1143">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="dc563-1144">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="dc563-1144">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="dc563-1145">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-1145">Container</span></span>
* <span data-ttu-id="dc563-1146">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1146">Added `container start` command</span></span>
* <span data-ttu-id="dc563-1147">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="dc563-1147">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="dc563-1148">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="dc563-1148">EventGrid</span></span>
* <span data-ttu-id="dc563-1149">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1149">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="dc563-1150">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1150">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="dc563-1151">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="dc563-1151">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="dc563-1152">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="dc563-1152">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="dc563-1153">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="dc563-1153">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="dc563-1154">HDInsight</span><span class="sxs-lookup"><span data-stu-id="dc563-1154">HDInsight</span></span>
* <span data-ttu-id="dc563-1155">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1155">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="dc563-1156">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1156">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="dc563-1157">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1157">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="dc563-1158">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="dc563-1158">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="dc563-1159">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1159">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="dc563-1160">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1160">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="dc563-1161">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="dc563-1161">IoT</span></span>
* <span data-ttu-id="dc563-1162">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="dc563-1162">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="dc563-1163">Kusto</span><span class="sxs-lookup"><span data-stu-id="dc563-1163">Kusto</span></span>
* <span data-ttu-id="dc563-1164">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="dc563-1164">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="dc563-1165">Монитор</span><span class="sxs-lookup"><span data-stu-id="dc563-1165">Monitor</span></span>
* <span data-ttu-id="dc563-1166">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="dc563-1166">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="dc563-1167">Профиль</span><span class="sxs-lookup"><span data-stu-id="dc563-1167">Profile</span></span>
* <span data-ttu-id="dc563-1168">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="dc563-1168">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="dc563-1169">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-1169">Network</span></span>
* <span data-ttu-id="dc563-1170">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1170">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="dc563-1171">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="dc563-1171">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-1172">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-1172">Resource</span></span>
* <span data-ttu-id="dc563-1173">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1173">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="dc563-1174">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1174">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="dc563-1175">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-1175">SQL Virtual Machine</span></span>
* <span data-ttu-id="dc563-1176">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="dc563-1176">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-1177">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-1177">Storage</span></span>
* <span data-ttu-id="dc563-1178">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="dc563-1178">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="dc563-1179">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="dc563-1179">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1180">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1180">VM</span></span>
* <span data-ttu-id="dc563-1181">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="dc563-1181">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="dc563-1182">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1182">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="dc563-1183">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1183">January 15, 2019</span></span>

<span data-ttu-id="dc563-1184">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="dc563-1184">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-1185">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-1185">ACR</span></span>
* <span data-ttu-id="dc563-1186">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="dc563-1186">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="dc563-1187">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="dc563-1187">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="dc563-1188">[УСТАРЕЛО] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="dc563-1188">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="dc563-1189">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-1189">ACS</span></span>
* <span data-ttu-id="dc563-1190">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="dc563-1190">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-1191">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-1191">Appservice</span></span>
* <span data-ttu-id="dc563-1192">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="dc563-1192">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="dc563-1193">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="dc563-1193">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="dc563-1194">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="dc563-1194">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="dc563-1195">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1195">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="dc563-1196">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="dc563-1196">Botservice</span></span>
* <span data-ttu-id="dc563-1197">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1197">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="dc563-1198">Configure</span><span class="sxs-lookup"><span data-stu-id="dc563-1198">Configure</span></span>
* <span data-ttu-id="dc563-1199">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1199">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="dc563-1200">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="dc563-1200">CosmosDB</span></span>
* <span data-ttu-id="dc563-1201">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="dc563-1201">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="dc563-1202">HDInsight</span><span class="sxs-lookup"><span data-stu-id="dc563-1202">HDInsight</span></span>
* <span data-ttu-id="dc563-1203">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="dc563-1203">Added commands for managing applications</span></span>
* <span data-ttu-id="dc563-1204">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1204">Added commands for managing script actions</span></span>
* <span data-ttu-id="dc563-1205">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="dc563-1205">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="dc563-1206">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1206">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="dc563-1207">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-1207">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="dc563-1208">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-1208">Network</span></span>
* <span data-ttu-id="dc563-1209">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="dc563-1209">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="dc563-1210">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="dc563-1210">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="dc563-1211">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="dc563-1211">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="dc563-1212">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1212">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="dc563-1213">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-1213">Role</span></span>
* <span data-ttu-id="dc563-1214">[УСТАРЕЛО] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc563-1214">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="dc563-1215">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="dc563-1215">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="dc563-1216">безопасность</span><span class="sxs-lookup"><span data-stu-id="dc563-1216">Security</span></span>
* <span data-ttu-id="dc563-1217">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="dc563-1217">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-1218">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-1218">Storage</span></span>
* <span data-ttu-id="dc563-1219">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="dc563-1219">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="dc563-1220">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1220">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="dc563-1221">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1221">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="dc563-1222">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1222">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="dc563-1223">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1223">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1224">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1224">VM</span></span>
* <span data-ttu-id="dc563-1225">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="dc563-1225">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="dc563-1226">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1226">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="dc563-1227">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1227">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="dc563-1228">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="dc563-1228">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="dc563-1229">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-1229">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="dc563-1230">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="dc563-1230">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="dc563-1231">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1231">December 20, 2018</span></span>

<span data-ttu-id="dc563-1232">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="dc563-1232">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="dc563-1233">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-1233">Appservice</span></span>
* <span data-ttu-id="dc563-1234">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="dc563-1234">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="dc563-1235">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="dc563-1235">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="dc563-1236">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="dc563-1236">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="dc563-1237">IoT Central</span><span class="sxs-lookup"><span data-stu-id="dc563-1237">IoTCentral</span></span>
* <span data-ttu-id="dc563-1238">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="dc563-1238">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="dc563-1239">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-1239">Role</span></span>
* <span data-ttu-id="dc563-1240">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1240">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-1241">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-1241">SQL</span></span>
* <span data-ttu-id="dc563-1242">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="dc563-1242">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1243">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1243">VM</span></span>
* <span data-ttu-id="dc563-1244">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1244">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="dc563-1245">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1245">December 18, 2018</span></span>

<span data-ttu-id="dc563-1246">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="dc563-1246">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="dc563-1247">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-1247">ACR</span></span>
* <span data-ttu-id="dc563-1248">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="dc563-1248">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="dc563-1249">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="dc563-1249">Condensed the table layout for task list</span></span>
* <span data-ttu-id="dc563-1250">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="dc563-1250">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-1251">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-1251">ACS</span></span>
* <span data-ttu-id="dc563-1252">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1252">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="dc563-1253">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="dc563-1253">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="dc563-1254">[УСТАРЕЛО] Команды `az acs` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="dc563-1254">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="dc563-1255">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1255">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="dc563-1256">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="dc563-1256">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="dc563-1257">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1257">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-1258">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-1258">Appservice</span></span>
* <span data-ttu-id="dc563-1259">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1259">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="dc563-1260">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="dc563-1260">Botservice</span></span>
* <span data-ttu-id="dc563-1261">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1261">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="dc563-1262">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="dc563-1262">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="dc563-1263">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="dc563-1263">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="dc563-1264">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="dc563-1264">Reduced Kudu network calls</span></span>
* <span data-ttu-id="dc563-1265">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="dc563-1265">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="dc563-1266">Потребление</span><span class="sxs-lookup"><span data-stu-id="dc563-1266">Consumption</span></span>
* <span data-ttu-id="dc563-1267">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="dc563-1267">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="dc563-1268">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="dc563-1268">CosmosDB</span></span>
* <span data-ttu-id="dc563-1269">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="dc563-1269">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="dc563-1270">Maps</span><span class="sxs-lookup"><span data-stu-id="dc563-1270">Maps</span></span>
* <span data-ttu-id="dc563-1271">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="dc563-1271">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="dc563-1272">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-1272">Network</span></span>
* <span data-ttu-id="dc563-1273">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1273">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="dc563-1274">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="dc563-1274">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-1275">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-1275">Resource</span></span>
* <span data-ttu-id="dc563-1276">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1276">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="dc563-1277">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1277">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-1278">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-1278">Storage</span></span>
*  <span data-ttu-id="dc563-1279">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="dc563-1279">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1280">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1280">VM</span></span>
* <span data-ttu-id="dc563-1281">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="dc563-1281">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="dc563-1282">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1282">December 4, 2018</span></span>

<span data-ttu-id="dc563-1283">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="dc563-1283">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="dc563-1284">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-1284">Core</span></span>
* <span data-ttu-id="dc563-1285">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="dc563-1285">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="dc563-1286">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="dc563-1286">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-1287">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-1287">Appservice</span></span>
* <span data-ttu-id="dc563-1288">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="dc563-1288">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="dc563-1289">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="dc563-1289">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="dc563-1290">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-1290">Network</span></span>
* <span data-ttu-id="dc563-1291">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="dc563-1291">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="dc563-1292">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-1292">Role</span></span>
* <span data-ttu-id="dc563-1293">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="dc563-1293">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="dc563-1294">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1294">VM</span></span>
* <span data-ttu-id="dc563-1295">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc563-1295">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="dc563-1296">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="dc563-1296">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="dc563-1297">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="dc563-1297">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="dc563-1298">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="dc563-1298">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="dc563-1299">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1299">November 20, 2018</span></span>

<span data-ttu-id="dc563-1300">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="dc563-1300">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="dc563-1301">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-1301">Core</span></span>
* <span data-ttu-id="dc563-1302">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="dc563-1302">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-1303">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-1303">ACR</span></span>
* <span data-ttu-id="dc563-1304">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="dc563-1304">Added context token to task step</span></span>
* <span data-ttu-id="dc563-1305">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="dc563-1305">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="dc563-1306">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1306">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-1307">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-1307">Appservice</span></span>
* <span data-ttu-id="dc563-1308">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="dc563-1308">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="dc563-1309">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-1309">Updated the default `node_version`.</span></span> <span data-ttu-id="dc563-1310">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="dc563-1310">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="dc563-1311">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="dc563-1311">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="dc563-1312">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="dc563-1312">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="dc563-1313">IotCentral</span><span class="sxs-lookup"><span data-stu-id="dc563-1313">IotCentral</span></span>
* <span data-ttu-id="dc563-1314">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="dc563-1314">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="dc563-1315">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="dc563-1315">KeyVault</span></span>
* <span data-ttu-id="dc563-1316">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="dc563-1316">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="dc563-1317">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-1317">Network</span></span>
* <span data-ttu-id="dc563-1318">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1318">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="dc563-1319">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1319">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="dc563-1320">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="dc563-1320">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="dc563-1321">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1321">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="dc563-1322">Rdbms</span><span class="sxs-lookup"><span data-stu-id="dc563-1322">Rdbms</span></span>
* <span data-ttu-id="dc563-1323">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="dc563-1323">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="dc563-1324">RBAC:</span><span class="sxs-lookup"><span data-stu-id="dc563-1324">Rbac</span></span>
* <span data-ttu-id="dc563-1325">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1325">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="dc563-1326">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="dc563-1326">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="dc563-1327">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-1327">Storage</span></span>
* <span data-ttu-id="dc563-1328">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="dc563-1328">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="dc563-1329">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1329">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="dc563-1330">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="dc563-1330">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="dc563-1331">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1331">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1332">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1332">VM</span></span>
* <span data-ttu-id="dc563-1333">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="dc563-1333">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="dc563-1334">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1334">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="dc563-1335">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1335">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="dc563-1336">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="dc563-1336">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="dc563-1337">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1337">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="dc563-1338">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1338">Added `snapshot wait` command</span></span>
* <span data-ttu-id="dc563-1339">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1339">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="dc563-1340">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1340">November 6, 2018</span></span>

<span data-ttu-id="dc563-1341">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="dc563-1341">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="dc563-1342">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-1342">Core</span></span>
* <span data-ttu-id="dc563-1343">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="dc563-1343">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-1344">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-1344">ACR</span></span>
* <span data-ttu-id="dc563-1345">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="dc563-1345">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="dc563-1346">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="dc563-1346">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-1347">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-1347">ACS</span></span>
* <span data-ttu-id="dc563-1348">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-1348">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="dc563-1349">Помощник</span><span class="sxs-lookup"><span data-stu-id="dc563-1349">Advisor</span></span>
* <span data-ttu-id="dc563-1350">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="dc563-1350">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="dc563-1351">AMS</span><span class="sxs-lookup"><span data-stu-id="dc563-1351">AMS</span></span>
* <span data-ttu-id="dc563-1352">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="dc563-1352">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="dc563-1353">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="dc563-1353">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="dc563-1354">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1354">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="dc563-1355">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="dc563-1355">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="dc563-1356">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1356">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="dc563-1357">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1357">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="dc563-1358">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1358">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="dc563-1359">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1359">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="dc563-1360">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1360">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="dc563-1361">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1361">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="dc563-1362">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1362">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="dc563-1363">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1363">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="dc563-1364">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="dc563-1364">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="dc563-1365">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="dc563-1365">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="dc563-1366">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1366">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="dc563-1367">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="dc563-1367">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="dc563-1368">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="dc563-1368">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-1369">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-1369">AppService</span></span>
* <span data-ttu-id="dc563-1370">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="dc563-1370">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="dc563-1371">Configure</span><span class="sxs-lookup"><span data-stu-id="dc563-1371">Configure</span></span>
* <span data-ttu-id="dc563-1372">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="dc563-1372">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="dc563-1373">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-1373">Container</span></span>
* <span data-ttu-id="dc563-1374">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="dc563-1374">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="dc563-1375">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="dc563-1375">EventHub</span></span>
* <span data-ttu-id="dc563-1376">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1376">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="dc563-1377">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="dc563-1377">Interactive</span></span>
* <span data-ttu-id="dc563-1378">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="dc563-1378">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="dc563-1379">Монитор</span><span class="sxs-lookup"><span data-stu-id="dc563-1379">Monitor</span></span>
* <span data-ttu-id="dc563-1380">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1380">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="dc563-1381">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-1381">Network</span></span>
* <span data-ttu-id="dc563-1382">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1382">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="dc563-1383">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="dc563-1383">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="dc563-1384">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1384">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="dc563-1385">Профиль</span><span class="sxs-lookup"><span data-stu-id="dc563-1385">Profile</span></span>
* <span data-ttu-id="dc563-1386">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1386">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="dc563-1387">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="dc563-1387">RDBMS</span></span>
* <span data-ttu-id="dc563-1388">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="dc563-1388">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-1389">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-1389">Resource</span></span>
* <span data-ttu-id="dc563-1390">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1390">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="dc563-1391">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-1391">Role</span></span>
* <span data-ttu-id="dc563-1392">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="dc563-1392">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="dc563-1393">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="dc563-1393">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="dc563-1394">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="dc563-1394">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-1395">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-1395">Storage</span></span>
* <span data-ttu-id="dc563-1396">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1396">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1397">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1397">VM</span></span>
* <span data-ttu-id="dc563-1398">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="dc563-1398">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="dc563-1399">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="dc563-1399">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="dc563-1400">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="dc563-1400">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="dc563-1401">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="dc563-1401">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="dc563-1402">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="dc563-1402">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="dc563-1403">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1403">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="dc563-1404">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1404">October 23, 2018</span></span>

<span data-ttu-id="dc563-1405">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="dc563-1405">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="dc563-1406">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-1406">Core</span></span>
* <span data-ttu-id="dc563-1407">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1407">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="dc563-1408">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1408">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-1409">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-1409">ACR</span></span>
* <span data-ttu-id="dc563-1410">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="dc563-1410">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="dc563-1411">CDN</span><span class="sxs-lookup"><span data-stu-id="dc563-1411">CDN</span></span>
* <span data-ttu-id="dc563-1412">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-1412">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="dc563-1413">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="dc563-1413">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="dc563-1414">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-1414">Container</span></span>
* <span data-ttu-id="dc563-1415">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="dc563-1415">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="dc563-1416">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="dc563-1416">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="dc563-1417">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1417">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="dc563-1418">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="dc563-1418">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="dc563-1419">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="dc563-1419">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="dc563-1420">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="dc563-1420">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="dc563-1421">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1421">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="dc563-1422">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="dc563-1422">CosmosDB</span></span>
* <span data-ttu-id="dc563-1423">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1423">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="dc563-1424">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="dc563-1424">Interactive</span></span>
* <span data-ttu-id="dc563-1425">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="dc563-1425">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="dc563-1426">IoT Central</span><span class="sxs-lookup"><span data-stu-id="dc563-1426">IoT Central</span></span>
* <span data-ttu-id="dc563-1427">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="dc563-1427">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="dc563-1428">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="dc563-1428">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="dc563-1429">Монитор</span><span class="sxs-lookup"><span data-stu-id="dc563-1429">Monitor</span></span>
* <span data-ttu-id="dc563-1430">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="dc563-1430">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="dc563-1431">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="dc563-1431">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="dc563-1432">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="dc563-1432">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="dc563-1433">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="dc563-1433">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="dc563-1434">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1434">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="dc563-1435">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="dc563-1435">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="dc563-1436">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="dc563-1436">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="dc563-1437">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="dc563-1437">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="dc563-1438">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="dc563-1438">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="dc563-1439">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1439">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="dc563-1440">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-1440">Network</span></span>
* <span data-ttu-id="dc563-1441">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="dc563-1441">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="dc563-1442">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="dc563-1442">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="dc563-1443">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="dc563-1443">ServiceBus</span></span>
* <span data-ttu-id="dc563-1444">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="dc563-1444">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-1445">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-1445">SQL</span></span>
* <span data-ttu-id="dc563-1446">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="dc563-1446">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-1447">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-1447">Storage</span></span>
* <span data-ttu-id="dc563-1448">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="dc563-1448">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="dc563-1449">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="dc563-1449">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1450">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1450">VM</span></span>
* <span data-ttu-id="dc563-1451">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="dc563-1451">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="dc563-1452">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="dc563-1452">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="dc563-1453">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="dc563-1453">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="dc563-1454">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1454">October 16, 2018</span></span>

<span data-ttu-id="dc563-1455">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="dc563-1455">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1456">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1456">VM</span></span>
* <span data-ttu-id="dc563-1457">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="dc563-1457">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="dc563-1458">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1458">October 9, 2018</span></span>

<span data-ttu-id="dc563-1459">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="dc563-1459">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="dc563-1460">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-1460">Core</span></span>
* <span data-ttu-id="dc563-1461">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="dc563-1461">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-1462">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-1462">ACR</span></span>
* <span data-ttu-id="dc563-1463">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="dc563-1463">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-1464">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-1464">ACS</span></span>
* <span data-ttu-id="dc563-1465">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="dc563-1465">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="dc563-1466">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="dc563-1466">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="dc563-1467">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1467">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="dc563-1468">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="dc563-1468">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="dc563-1469">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-1469">Container</span></span>
* <span data-ttu-id="dc563-1470">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="dc563-1470">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="dc563-1471">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="dc563-1471">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="dc563-1472">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="dc563-1472">Event Hub</span></span>
* <span data-ttu-id="dc563-1473">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1473">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="dc563-1474">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="dc563-1474">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="dc563-1475">Модули</span><span class="sxs-lookup"><span data-stu-id="dc563-1475">Extensions</span></span>
* <span data-ttu-id="dc563-1476">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="dc563-1476">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="dc563-1477">HDInsight</span><span class="sxs-lookup"><span data-stu-id="dc563-1477">HDInsight</span></span>
* <span data-ttu-id="dc563-1478">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="dc563-1478">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="dc563-1479">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="dc563-1479">IoT</span></span>
* <span data-ttu-id="dc563-1480">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="dc563-1480">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="dc563-1481">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="dc563-1481">KeyVault</span></span>
* <span data-ttu-id="dc563-1482">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="dc563-1482">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="dc563-1483">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-1483">Network</span></span>
* <span data-ttu-id="dc563-1484">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-1484">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="dc563-1485">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="dc563-1485">See #6052</span></span>
* <span data-ttu-id="dc563-1486">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1486">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="dc563-1487">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="dc563-1487">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="dc563-1488">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1488">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="dc563-1489">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1489">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="dc563-1490">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1490">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="dc563-1491">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1491">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="dc563-1492">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-1492">Role</span></span>
* <span data-ttu-id="dc563-1493">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1493">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="dc563-1494">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1494">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="dc563-1495">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="dc563-1495">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="dc563-1496">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="dc563-1496">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="dc563-1497">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="dc563-1497">Service Bus</span></span>
* <span data-ttu-id="dc563-1498">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="dc563-1498">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1499">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1499">VM</span></span>
* <span data-ttu-id="dc563-1500">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1500">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="dc563-1501">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="dc563-1501">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="dc563-1502">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1502">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="dc563-1503">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1503">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="dc563-1504">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="dc563-1504">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="dc563-1505">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="dc563-1505">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="dc563-1506">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1506">September 21, 2018</span></span>

<span data-ttu-id="dc563-1507">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="dc563-1507">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-1508">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-1508">ACR</span></span>
* <span data-ttu-id="dc563-1509">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="dc563-1509">Added ACR Task commands</span></span>
* <span data-ttu-id="dc563-1510">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="dc563-1510">Added quick run command</span></span>
* <span data-ttu-id="dc563-1511">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="dc563-1511">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="dc563-1512">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="dc563-1512">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="dc563-1513">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="dc563-1513">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="dc563-1514">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="dc563-1514">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-1515">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-1515">ACS</span></span>
* <span data-ttu-id="dc563-1516">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="dc563-1516">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="dc563-1517">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="dc563-1517">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-1518">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-1518">AppService</span></span>

* <span data-ttu-id="dc563-1519">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="dc563-1519">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="dc563-1520">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="dc563-1520">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="dc563-1521">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="dc563-1521">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="dc563-1522">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="dc563-1522">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="dc563-1523">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="dc563-1523">Batch</span></span>
* <span data-ttu-id="dc563-1524">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="dc563-1524">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="dc563-1525">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1525">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="dc563-1526">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1526">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="dc563-1527">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="dc563-1527">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="dc563-1528">Batch AI</span><span class="sxs-lookup"><span data-stu-id="dc563-1528">Batch AI</span></span> 
* <span data-ttu-id="dc563-1529">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1529">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="dc563-1530">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="dc563-1530">Cognitive Services</span></span>
* <span data-ttu-id="dc563-1531">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1531">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="dc563-1532">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1532">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="dc563-1533">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1533">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="dc563-1534">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1534">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="dc563-1535">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="dc563-1535">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="dc563-1536">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1536">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="dc563-1537">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-1537">Container</span></span>
* <span data-ttu-id="dc563-1538">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="dc563-1538">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="dc563-1539">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="dc563-1539">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="dc563-1540">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="dc563-1540">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="dc563-1541">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="dc563-1541">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="dc563-1542">Data Lake</span><span class="sxs-lookup"><span data-stu-id="dc563-1542">Datalake</span></span>
* <span data-ttu-id="dc563-1543">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="dc563-1543">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="dc563-1544">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="dc563-1544">Interactive Shell</span></span>
* <span data-ttu-id="dc563-1545">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="dc563-1545">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="dc563-1546">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1546">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="dc563-1547">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="dc563-1547">IoT</span></span>
* <span data-ttu-id="dc563-1548">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="dc563-1548">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="dc563-1549">Key Vault</span><span class="sxs-lookup"><span data-stu-id="dc563-1549">Key Vault</span></span>
* <span data-ttu-id="dc563-1550">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="dc563-1550">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="dc563-1551">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-1551">Network</span></span>
* <span data-ttu-id="dc563-1552">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1552">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="dc563-1553">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="dc563-1553">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="dc563-1554">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="dc563-1554">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="dc563-1555">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1555">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="dc563-1556">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1556">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="dc563-1557">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1557">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="dc563-1558">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="dc563-1558">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="dc563-1559">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1559">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="dc563-1560">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1560">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="dc563-1561">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1561">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="dc563-1562">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1562">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="dc563-1563">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1563">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="dc563-1564">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1564">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="dc563-1565">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="dc563-1565">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="dc563-1566">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1566">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="dc563-1567">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="dc563-1567">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="dc563-1568">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="dc563-1568">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="dc563-1569">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="dc563-1569">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="dc563-1570">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="dc563-1570">RDBMS</span></span>
* <span data-ttu-id="dc563-1571">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="dc563-1571">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="dc563-1572">резервирование.</span><span class="sxs-lookup"><span data-stu-id="dc563-1572">Reservation</span></span>
* <span data-ttu-id="dc563-1573">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1573">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="dc563-1574">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="dc563-1574">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="dc563-1575">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="dc563-1575">Manage App</span></span>
* <span data-ttu-id="dc563-1576">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="dc563-1576">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="dc563-1577">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="dc563-1577">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="dc563-1578">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-1578">Role</span></span>
* <span data-ttu-id="dc563-1579">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="dc563-1579">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="dc563-1580">SignalR</span><span class="sxs-lookup"><span data-stu-id="dc563-1580">SignalR</span></span>
* <span data-ttu-id="dc563-1581">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="dc563-1581">First release</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-1582">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-1582">Storage</span></span>
* <span data-ttu-id="dc563-1583">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="dc563-1583">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="dc563-1584">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="dc563-1584">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1585">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1585">VM</span></span>
* <span data-ttu-id="dc563-1586">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="dc563-1586">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="dc563-1587">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1587">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="dc563-1588">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1588">August 28, 2018</span></span>

<span data-ttu-id="dc563-1589">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="dc563-1589">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="dc563-1590">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-1590">Core</span></span>

* <span data-ttu-id="dc563-1591">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="dc563-1591">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="dc563-1592">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="dc563-1592">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-1593">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-1593">ACR</span></span>

* <span data-ttu-id="dc563-1594">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="dc563-1594">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="dc563-1595">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1595">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-1596">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-1596">ACS</span></span>

* <span data-ttu-id="dc563-1597">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1597">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="dc563-1598">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="dc563-1598">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-1599">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-1599">AppService</span></span>

* <span data-ttu-id="dc563-1600">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="dc563-1600">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="dc563-1601">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="dc563-1601">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="dc563-1602">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="dc563-1602">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="dc563-1603">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="dc563-1603">Backup</span></span>

* <span data-ttu-id="dc563-1604">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="dc563-1604">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="dc563-1605">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="dc563-1605">Bot Service</span></span>

* <span data-ttu-id="dc563-1606">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="dc563-1606">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="dc563-1607">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="dc563-1607">Cognitive Services</span></span>

* <span data-ttu-id="dc563-1608">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="dc563-1608">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="dc563-1609">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="dc563-1609">IoT</span></span>

* <span data-ttu-id="dc563-1610">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="dc563-1610">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="dc563-1611">Монитор</span><span class="sxs-lookup"><span data-stu-id="dc563-1611">Monitor</span></span>

* <span data-ttu-id="dc563-1612">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="dc563-1612">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="dc563-1613">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="dc563-1613">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="dc563-1614">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-1614">Network</span></span>

* <span data-ttu-id="dc563-1615">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="dc563-1615">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-1616">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-1616">Resource</span></span>

* <span data-ttu-id="dc563-1617">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="dc563-1617">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-1618">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-1618">Storage</span></span>

* <span data-ttu-id="dc563-1619">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="dc563-1619">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1620">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1620">VM</span></span>

* <span data-ttu-id="dc563-1621">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="dc563-1621">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="dc563-1622">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1622">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="dc563-1623">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1623">Auguest 14, 2018</span></span>

<span data-ttu-id="dc563-1624">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="dc563-1624">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="dc563-1625">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-1625">Core</span></span>

* <span data-ttu-id="dc563-1626">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1626">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="dc563-1627">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="dc563-1627">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="dc563-1628">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="dc563-1628">Telemetry</span></span>

* <span data-ttu-id="dc563-1629">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="dc563-1629">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-1630">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-1630">ACR</span></span>

* <span data-ttu-id="dc563-1631">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1631">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="dc563-1632">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1632">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-1633">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-1633">ACS</span></span>

* <span data-ttu-id="dc563-1634">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="dc563-1634">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="dc563-1635">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="dc563-1635">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="dc563-1636">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="dc563-1636">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="dc563-1637">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="dc563-1637">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="dc563-1638">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="dc563-1638">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="dc563-1639">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-1639">AppService</span></span>

* <span data-ttu-id="dc563-1640">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1640">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="dc563-1641">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="dc563-1641">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="dc563-1642">Batch AI</span><span class="sxs-lookup"><span data-stu-id="dc563-1642">BatchAI</span></span>

* <span data-ttu-id="dc563-1643">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="dc563-1643">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="dc563-1644">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-1644">Container</span></span>

* <span data-ttu-id="dc563-1645">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="dc563-1645">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="dc563-1646">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="dc563-1646">IoT</span></span>

* <span data-ttu-id="dc563-1647">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="dc563-1647">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="dc563-1648">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1648">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="dc563-1649">IoT Central</span><span class="sxs-lookup"><span data-stu-id="dc563-1649">Iot Central</span></span>

* <span data-ttu-id="dc563-1650">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="dc563-1650">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="dc563-1651">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="dc563-1651">KeyVault</span></span>


* <span data-ttu-id="dc563-1652">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="dc563-1652">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="dc563-1653">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="dc563-1653">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="dc563-1654">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="dc563-1654">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="dc563-1655">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="dc563-1655">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="dc563-1656">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="dc563-1656">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="dc563-1657">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="dc563-1657">Relay</span></span>

* <span data-ttu-id="dc563-1658">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="dc563-1658">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-1659">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-1659">Sql</span></span>

* <span data-ttu-id="dc563-1660">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1660">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-1661">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-1661">Storage</span></span>

* <span data-ttu-id="dc563-1662">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="dc563-1662">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="dc563-1663">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="dc563-1663">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="dc563-1664">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="dc563-1664">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="dc563-1665">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="dc563-1665">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="dc563-1666">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="dc563-1666">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1667">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1667">VM</span></span>

* <span data-ttu-id="dc563-1668">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="dc563-1668">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="dc563-1669">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1669">July 31, 2018</span></span>

<span data-ttu-id="dc563-1670">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="dc563-1670">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-1671">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-1671">ACR</span></span>

* <span data-ttu-id="dc563-1672">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1672">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="dc563-1673">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1673">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-1674">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-1674">ACS</span></span>

* <span data-ttu-id="dc563-1675">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="dc563-1675">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="dc563-1676">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="dc563-1676">Batch</span></span>

* <span data-ttu-id="dc563-1677">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="dc563-1677">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="dc563-1678">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-1678">Container</span></span>

* <span data-ttu-id="dc563-1679">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="dc563-1679">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="dc563-1680">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-1680">Network</span></span>

* <span data-ttu-id="dc563-1681">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="dc563-1681">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="dc563-1682">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-1682">Resource</span></span>

* <span data-ttu-id="dc563-1683">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="dc563-1683">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="dc563-1684">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="dc563-1684">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="dc563-1685">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-1685">Role</span></span>

* <span data-ttu-id="dc563-1686">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="dc563-1686">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="dc563-1687">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="dc563-1687">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="dc563-1688">Поиск</span><span class="sxs-lookup"><span data-stu-id="dc563-1688">Search</span></span>

* <span data-ttu-id="dc563-1689">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="dc563-1689">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="dc563-1690">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="dc563-1690">Service Bus</span></span>

* <span data-ttu-id="dc563-1691">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="dc563-1691">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="dc563-1692">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="dc563-1692">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="dc563-1693">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="dc563-1693">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="dc563-1694">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1694">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-1695">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-1695">Storage</span></span>

* <span data-ttu-id="dc563-1696">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="dc563-1696">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="dc563-1697">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="dc563-1697">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1698">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1698">VM</span></span>

* <span data-ttu-id="dc563-1699">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="dc563-1699">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="dc563-1700">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1700">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="dc563-1701">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="dc563-1701">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="dc563-1702">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="dc563-1702">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="dc563-1703">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1703">July 18, 2018</span></span>

<span data-ttu-id="dc563-1704">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="dc563-1704">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="dc563-1705">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-1705">Core</span></span>

* <span data-ttu-id="dc563-1706">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="dc563-1706">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="dc563-1707">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="dc563-1707">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="dc563-1708">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="dc563-1708">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-1709">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-1709">ACR</span></span>

* <span data-ttu-id="dc563-1710">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="dc563-1710">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="dc563-1711">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1711">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="dc563-1712">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="dc563-1712">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="dc563-1713">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="dc563-1713">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-1714">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-1714">ACS</span></span>

* <span data-ttu-id="dc563-1715">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="dc563-1715">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-1716">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-1716">AppService</span></span>

* <span data-ttu-id="dc563-1717">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="dc563-1717">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="dc563-1718">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="dc563-1718">Batch</span></span>

* <span data-ttu-id="dc563-1719">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="dc563-1719">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="dc563-1720">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="dc563-1720">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="dc563-1721">Batch AI</span><span class="sxs-lookup"><span data-stu-id="dc563-1721">Batch AI</span></span>

* <span data-ttu-id="dc563-1722">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1722">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="dc563-1723">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-1723">Container</span></span>

* <span data-ttu-id="dc563-1724">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="dc563-1724">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="dc563-1725">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="dc563-1725">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="dc563-1726">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-1726">Network</span></span>

* <span data-ttu-id="dc563-1727">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1727">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="dc563-1728">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1728">Added `network nic wait`</span></span>
* <span data-ttu-id="dc563-1729">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="dc563-1729">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="dc563-1730">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="dc563-1730">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="dc563-1731">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-1731">Resource</span></span>

* <span data-ttu-id="dc563-1732">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1732">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="dc563-1733">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1733">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="dc563-1734">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1734">Added `deployment wait` command</span></span>
* <span data-ttu-id="dc563-1735">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="dc563-1735">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-1736">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-1736">SQL</span></span>

* <span data-ttu-id="dc563-1737">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1737">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="dc563-1738">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1738">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="dc563-1739">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1739">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-1740">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-1740">Storage</span></span>

* <span data-ttu-id="dc563-1741">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1741">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1742">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1742">VM</span></span>

* <span data-ttu-id="dc563-1743">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-1743">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="dc563-1744">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1744">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="dc563-1745">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1745">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="dc563-1746">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1746">July 3, 2018</span></span>

<span data-ttu-id="dc563-1747">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="dc563-1747">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="dc563-1748">AKS</span><span class="sxs-lookup"><span data-stu-id="dc563-1748">AKS</span></span>

* <span data-ttu-id="dc563-1749">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="dc563-1749">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="dc563-1750">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1750">July 3, 2018</span></span>

<span data-ttu-id="dc563-1751">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="dc563-1751">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="dc563-1752">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-1752">Core</span></span>

* <span data-ttu-id="dc563-1753">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="dc563-1753">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-1754">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-1754">ACR</span></span>

* <span data-ttu-id="dc563-1755">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="dc563-1755">Added polling build status</span></span>
* <span data-ttu-id="dc563-1756">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="dc563-1756">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="dc563-1757">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1757">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-1758">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-1758">ACS</span></span>

* <span data-ttu-id="dc563-1759">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-1759">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="dc563-1760">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-1760">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="dc563-1761">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1761">Updated options for `aks browse` command.</span></span> <span data-ttu-id="dc563-1762">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1762">Added `--listen-port` support</span></span>
* <span data-ttu-id="dc563-1763">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1763">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="dc563-1764">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="dc563-1764">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="dc563-1765">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1765">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-1766">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-1766">AppService</span></span>

* <span data-ttu-id="dc563-1767">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1767">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="dc563-1768">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="dc563-1768">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="dc563-1769">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="dc563-1769">Backup</span></span>

* <span data-ttu-id="dc563-1770">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="dc563-1770">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="dc563-1771">Batch AI</span><span class="sxs-lookup"><span data-stu-id="dc563-1771">BatchAI</span></span>

* <span data-ttu-id="dc563-1772">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1772">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="dc563-1773">Cloud</span><span class="sxs-lookup"><span data-stu-id="dc563-1773">Cloud</span></span>

* <span data-ttu-id="dc563-1774">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1774">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="dc563-1775">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-1775">Container</span></span>

* <span data-ttu-id="dc563-1776">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="dc563-1776">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="dc563-1777">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1777">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="dc563-1778">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="dc563-1778">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="dc563-1779">Расширение</span><span class="sxs-lookup"><span data-stu-id="dc563-1779">Extension</span></span>

* <span data-ttu-id="dc563-1780">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="dc563-1780">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="dc563-1781">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-1781">Network</span></span>

* <span data-ttu-id="dc563-1782">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="dc563-1782">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="dc563-1783">Rdbms</span><span class="sxs-lookup"><span data-stu-id="dc563-1783">Rdbms</span></span>

* <span data-ttu-id="dc563-1784">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1784">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-1785">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-1785">Resource</span></span>

* <span data-ttu-id="dc563-1786">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1786">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1787">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1787">VM</span></span>

* <span data-ttu-id="dc563-1788">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="dc563-1788">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="dc563-1789">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1789">June 25, 2018</span></span>

<span data-ttu-id="dc563-1790">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="dc563-1790">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="dc563-1791">CLI</span><span class="sxs-lookup"><span data-stu-id="dc563-1791">CLI</span></span>

* <span data-ttu-id="dc563-1792">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="dc563-1792">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="dc563-1793">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1793">June 19, 2018</span></span>

<span data-ttu-id="dc563-1794">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="dc563-1794">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="dc563-1795">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-1795">Core</span></span>

* <span data-ttu-id="dc563-1796">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="dc563-1796">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-1797">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-1797">ACR</span></span>

* <span data-ttu-id="dc563-1798">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1798">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="dc563-1799">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="dc563-1799">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-1800">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-1800">ACS</span></span>

* <span data-ttu-id="dc563-1801">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1801">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="dc563-1802">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1802">Added `--update` support</span></span>
* <span data-ttu-id="dc563-1803">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1803">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="dc563-1804">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1804">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="dc563-1805">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1805">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="dc563-1806">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1806">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="dc563-1807">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1807">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="dc563-1808">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1808">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-1809">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-1809">AppService</span></span>

* <span data-ttu-id="dc563-1810">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="dc563-1810">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="dc563-1811">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1811">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="dc563-1812">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="dc563-1812">Batch</span></span>

* <span data-ttu-id="dc563-1813">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1813">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="dc563-1814">Batch AI</span><span class="sxs-lookup"><span data-stu-id="dc563-1814">Batch AI</span></span>

* <span data-ttu-id="dc563-1815">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="dc563-1815">Added support for workspaces.</span></span> <span data-ttu-id="dc563-1816">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1816">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="dc563-1817">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1817">Added support for experiments.</span></span> <span data-ttu-id="dc563-1818">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="dc563-1818">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="dc563-1819">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="dc563-1819">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="dc563-1820">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1820">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="dc563-1821">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1821">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="dc563-1822">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1822">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="dc563-1823">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="dc563-1823">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="dc563-1824">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1824">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="dc563-1825">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1825">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="dc563-1826">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1826">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="dc563-1827">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1827">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="dc563-1828">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1828">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="dc563-1829">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1829">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="dc563-1830">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="dc563-1830">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="dc563-1831">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1831">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="dc563-1832">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="dc563-1832">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="dc563-1833">[`--config`, `-c`] переименовано в [`--config-file`, `-f`].</span><span class="sxs-lookup"><span data-stu-id="dc563-1833">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="dc563-1834">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="dc563-1834">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="dc563-1835">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="dc563-1835">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="dc563-1836">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="dc563-1836">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="dc563-1837">Maps</span><span class="sxs-lookup"><span data-stu-id="dc563-1837">Maps</span></span>

* <span data-ttu-id="dc563-1838">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1838">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="dc563-1839">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-1839">Network</span></span>

* <span data-ttu-id="dc563-1840">Добавлена поддержка `https` в `network lb probe create` ([№ 6571](https://github.com/Azure/azure-cli/issues/6571)).</span><span class="sxs-lookup"><span data-stu-id="dc563-1840">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="dc563-1841">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="dc563-1841">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="dc563-1842">#6502</span><span class="sxs-lookup"><span data-stu-id="dc563-1842">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="dc563-1843">Резервирование</span><span class="sxs-lookup"><span data-stu-id="dc563-1843">Reservations</span></span>

* <span data-ttu-id="dc563-1844">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1844">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="dc563-1845">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1845">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="dc563-1846">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1846">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="dc563-1847">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1847">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="dc563-1848">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1848">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="dc563-1849">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1849">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="dc563-1850">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-1850">Role</span></span>

* <span data-ttu-id="dc563-1851">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="dc563-1851">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-1852">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-1852">SQL</span></span>

* <span data-ttu-id="dc563-1853">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="dc563-1853">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-1854">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-1854">Storage</span></span>

* <span data-ttu-id="dc563-1855">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="dc563-1855">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1856">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1856">VM</span></span>

* <span data-ttu-id="dc563-1857">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1857">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="dc563-1858">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1858">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="dc563-1859">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="dc563-1859">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="dc563-1860">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1860">June 13, 2018</span></span>

<span data-ttu-id="dc563-1861">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="dc563-1861">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="dc563-1862">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-1862">Core</span></span>

* <span data-ttu-id="dc563-1863">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="dc563-1863">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="dc563-1864">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1864">June 13, 2018</span></span>

<span data-ttu-id="dc563-1865">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="dc563-1865">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="dc563-1866">AKS</span><span class="sxs-lookup"><span data-stu-id="dc563-1866">AKS</span></span>

* <span data-ttu-id="dc563-1867">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="dc563-1867">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="dc563-1868">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="dc563-1868">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="dc563-1869">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="dc563-1869">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="dc563-1870">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="dc563-1870">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="dc563-1871">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="dc563-1871">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-1872">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-1872">AppService</span></span>

* <span data-ttu-id="dc563-1873">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="dc563-1873">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="dc563-1874">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1874">June 5, 2018</span></span>

<span data-ttu-id="dc563-1875">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="dc563-1875">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="dc563-1876">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="dc563-1876">Interactive</span></span>

* <span data-ttu-id="dc563-1877">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="dc563-1877">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="dc563-1878">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1878">June 5, 2018</span></span>

<span data-ttu-id="dc563-1879">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="dc563-1879">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="dc563-1880">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-1880">Core</span></span>

* <span data-ttu-id="dc563-1881">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="dc563-1881">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="dc563-1882">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="dc563-1882">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-1883">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-1883">ACR</span></span>

* <span data-ttu-id="dc563-1884">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="dc563-1884">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="dc563-1885">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1885">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="dc563-1886">AKS</span><span class="sxs-lookup"><span data-stu-id="dc563-1886">AKS</span></span>

* <span data-ttu-id="dc563-1887">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="dc563-1887">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="dc563-1888">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="dc563-1888">Batch</span></span>

* <span data-ttu-id="dc563-1889">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="dc563-1889">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="dc563-1890">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="dc563-1890">IOT</span></span>

* <span data-ttu-id="dc563-1891">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="dc563-1891">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="dc563-1892">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-1892">Network</span></span>

* <span data-ttu-id="dc563-1893">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1893">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="dc563-1894">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="dc563-1894">Policy Insights</span></span>

* <span data-ttu-id="dc563-1895">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="dc563-1895">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="dc563-1896">ARM</span><span class="sxs-lookup"><span data-stu-id="dc563-1896">ARM</span></span>

* <span data-ttu-id="dc563-1897">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1897">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-1898">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-1898">SQL</span></span>

* <span data-ttu-id="dc563-1899">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="dc563-1899">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="dc563-1900">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="dc563-1900">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="dc563-1901">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-1901">Storage</span></span>

* <span data-ttu-id="dc563-1902">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1902">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1903">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1903">VM</span></span>

* <span data-ttu-id="dc563-1904">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1904">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="dc563-1905">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1905">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="dc563-1906">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1906">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="dc563-1907">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1907">May 22, 2018</span></span>

<span data-ttu-id="dc563-1908">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="dc563-1908">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="dc563-1909">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-1909">Core</span></span>

* <span data-ttu-id="dc563-1910">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1910">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-1911">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-1911">ACS</span></span>

* <span data-ttu-id="dc563-1912">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1912">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="dc563-1913">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="dc563-1913">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-1914">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-1914">AppService</span></span>

* <span data-ttu-id="dc563-1915">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="dc563-1915">Improved generic update commands</span></span>
* <span data-ttu-id="dc563-1916">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1916">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="dc563-1917">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-1917">Container</span></span>

* <span data-ttu-id="dc563-1918">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="dc563-1918">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="dc563-1919">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="dc563-1919">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="dc563-1920">Расширение</span><span class="sxs-lookup"><span data-stu-id="dc563-1920">Extension</span></span>

* <span data-ttu-id="dc563-1921">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="dc563-1921">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="dc563-1922">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="dc563-1922">Interactive</span></span>

* <span data-ttu-id="dc563-1923">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="dc563-1923">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="dc563-1924">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="dc563-1924">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="dc563-1925">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="dc563-1925">KeyVault</span></span>

* <span data-ttu-id="dc563-1926">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="dc563-1926">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="dc563-1927">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-1927">Network</span></span>

* <span data-ttu-id="dc563-1928">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="dc563-1928">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="dc563-1929">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="dc563-1929">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-1930">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-1930">SQL</span></span>

* <span data-ttu-id="dc563-1931">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="dc563-1931">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="dc563-1932">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1932">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="dc563-1933">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1933">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="dc563-1934">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="dc563-1934">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="dc563-1935">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="dc563-1935">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="dc563-1936">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1936">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="dc563-1937">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1937">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="dc563-1938">`edition`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1938">`edition`.</span></span> <span data-ttu-id="dc563-1939">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1939">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="dc563-1940">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1940">`elasticPoolName`.</span></span> <span data-ttu-id="dc563-1941">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1941">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="dc563-1942">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="dc563-1942">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="dc563-1943">`edition`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1943">`edition`.</span></span> <span data-ttu-id="dc563-1944">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1944">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="dc563-1945">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1945">`dtu`.</span></span> <span data-ttu-id="dc563-1946">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1946">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="dc563-1947">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1947">`databaseDtuMin`.</span></span> <span data-ttu-id="dc563-1948">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1948">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="dc563-1949">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1949">`databaseDtuMax`.</span></span> <span data-ttu-id="dc563-1950">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1950">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="dc563-1951">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1951">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="dc563-1952">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1952">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-1953">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-1953">Storage</span></span>

* <span data-ttu-id="dc563-1954">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1954">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="dc563-1955">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1955">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-1956">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-1956">VM</span></span>

* <span data-ttu-id="dc563-1957">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1957">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="dc563-1958">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1958">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="dc563-1959">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1959">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="dc563-1960">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="dc563-1960">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="dc563-1961">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1961">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="dc563-1962">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-1962">May 7, 2018</span></span>

<span data-ttu-id="dc563-1963">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="dc563-1963">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="dc563-1964">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-1964">Core</span></span>

* <span data-ttu-id="dc563-1965">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="dc563-1965">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="dc563-1966">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="dc563-1966">Added limited support for positional arguments</span></span>
* <span data-ttu-id="dc563-1967">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1967">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="dc563-1968">#5591</span><span class="sxs-lookup"><span data-stu-id="dc563-1968">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="dc563-1969">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1969">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="dc563-1970">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="dc563-1970">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="dc563-1971">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="dc563-1971">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="dc563-1972">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1972">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="dc563-1973">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="dc563-1973">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-1974">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-1974">ACR</span></span>

* <span data-ttu-id="dc563-1975">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="dc563-1975">Added ACR Build commands</span></span>
* <span data-ttu-id="dc563-1976">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="dc563-1976">Improved resource not found error messages</span></span>
* <span data-ttu-id="dc563-1977">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="dc563-1977">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="dc563-1978">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="dc563-1978">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="dc563-1979">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="dc563-1979">Improved repository commands error messages</span></span>
* <span data-ttu-id="dc563-1980">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="dc563-1980">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-1981">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-1981">ACS</span></span>

* <span data-ttu-id="dc563-1982">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="dc563-1982">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="dc563-1983">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="dc563-1983">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="dc563-1984">AMS</span><span class="sxs-lookup"><span data-stu-id="dc563-1984">AMS</span></span>

* <span data-ttu-id="dc563-1985">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="dc563-1985">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-1986">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-1986">Appservice</span></span>

* <span data-ttu-id="dc563-1987">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="dc563-1987">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="dc563-1988">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-1988">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="dc563-1989">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="dc563-1989">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="dc563-1990">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="dc563-1990">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="dc563-1991">Batch AI</span><span class="sxs-lookup"><span data-stu-id="dc563-1991">Batch AI</span></span>

* <span data-ttu-id="dc563-1992">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="dc563-1992">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="dc563-1993">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="dc563-1993">Cognitive Services</span></span>

* <span data-ttu-id="dc563-1994">Исправлена опечатка в примере для `cognitiveservices account create` ([№ 5603](https://github.com/Azure/azure-cli/issues/5603)).</span><span class="sxs-lookup"><span data-stu-id="dc563-1994">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="dc563-1995">Потребление</span><span class="sxs-lookup"><span data-stu-id="dc563-1995">Consumption</span></span>

* <span data-ttu-id="dc563-1996">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="dc563-1996">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="dc563-1997">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-1997">Container</span></span>

* <span data-ttu-id="dc563-1998">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="dc563-1998">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="dc563-1999">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="dc563-1999">Cosmos DB</span></span>

* <span data-ttu-id="dc563-2000">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="dc563-2000">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="dc563-2001">DMS</span><span class="sxs-lookup"><span data-stu-id="dc563-2001">DMS</span></span>

* <span data-ttu-id="dc563-2002">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="dc563-2002">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="dc563-2003">Расширение</span><span class="sxs-lookup"><span data-stu-id="dc563-2003">Extension</span></span>

* <span data-ttu-id="dc563-2004">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="dc563-2004">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="dc563-2005">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="dc563-2005">Interactive</span></span>

* <span data-ttu-id="dc563-2006">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="dc563-2006">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="dc563-2007">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="dc563-2007">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="dc563-2008">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="dc563-2008">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="dc563-2009">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="dc563-2009">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="dc563-2010">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="dc563-2010">Lab</span></span>

* <span data-ttu-id="dc563-2011">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="dc563-2011">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="dc563-2012">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-2012">Network</span></span>

* <span data-ttu-id="dc563-2013">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="dc563-2013">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="dc563-2014">Профиль</span><span class="sxs-lookup"><span data-stu-id="dc563-2014">Profile</span></span>

* <span data-ttu-id="dc563-2015">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2015">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="dc563-2016">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="dc563-2016">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="dc563-2017">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2017">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="dc563-2018">Redis</span><span class="sxs-lookup"><span data-stu-id="dc563-2018">Redis</span></span>

* <span data-ttu-id="dc563-2019">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2019">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="dc563-2020">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="dc563-2020">Deprecated `redis list-all`.</span></span> <span data-ttu-id="dc563-2021">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2021">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="dc563-2022">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2022">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="dc563-2023">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="dc563-2023">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="dc563-2024">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-2024">Role</span></span>

* <span data-ttu-id="dc563-2025">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="dc563-2025">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-2026">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-2026">Storage</span></span>

* <span data-ttu-id="dc563-2027">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="dc563-2027">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="dc563-2028">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="dc563-2028">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="dc563-2029">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="dc563-2029">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="dc563-2030">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="dc563-2030">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="dc563-2031">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="dc563-2031">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-2032">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-2032">VM</span></span>

* <span data-ttu-id="dc563-2033">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="dc563-2033">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="dc563-2034">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="dc563-2034">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="dc563-2035">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="dc563-2035">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="dc563-2036">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2036">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="dc563-2037">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="dc563-2037">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="dc563-2038">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="dc563-2038">Added write accelerator support</span></span>
* <span data-ttu-id="dc563-2039">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2039">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="dc563-2040">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="dc563-2040">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="dc563-2041">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="dc563-2041">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="dc563-2042">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-2042">April 10, 2018</span></span>

<span data-ttu-id="dc563-2043">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="dc563-2043">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-2044">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-2044">ACR</span></span>

* <span data-ttu-id="dc563-2045">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="dc563-2045">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-2046">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-2046">ACS</span></span>

* <span data-ttu-id="dc563-2047">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="dc563-2047">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-2048">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-2048">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="dc563-2050">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="dc563-2050">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="dc563-2051">Batch AI</span><span class="sxs-lookup"><span data-stu-id="dc563-2051">BatchAI</span></span>

* <span data-ttu-id="dc563-2052">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="dc563-2052">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="dc563-2053">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="dc563-2053">Job level mounting</span></span>
  - <span data-ttu-id="dc563-2054">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="dc563-2054">Environment variables with secret values</span></span>
  - <span data-ttu-id="dc563-2055">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="dc563-2055">Performance counters settings</span></span>
  - <span data-ttu-id="dc563-2056">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="dc563-2056">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="dc563-2057">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="dc563-2057">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="dc563-2058">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="dc563-2058">Usage and limits reporting</span></span>
  - <span data-ttu-id="dc563-2059">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="dc563-2059">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="dc563-2060">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="dc563-2060">Support for custom images</span></span>
  - <span data-ttu-id="dc563-2061">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="dc563-2061">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="dc563-2062">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="dc563-2062">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="dc563-2063">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="dc563-2063">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="dc563-2064">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="dc563-2064">National clouds are supported</span></span>
* <span data-ttu-id="dc563-2065">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="dc563-2065">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="dc563-2066">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="dc563-2066">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="dc563-2067">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="dc563-2067">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="dc563-2068">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="dc563-2068">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="dc563-2069">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="dc563-2069">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="dc563-2070">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="dc563-2070">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="dc563-2071">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2071">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="dc563-2072">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="dc563-2072">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="dc563-2073">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="dc563-2073">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="dc563-2074">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2074">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="dc563-2075">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="dc563-2075">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="dc563-2076">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2076">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="dc563-2077">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2077">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="dc563-2078">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="dc563-2078">Billing</span></span>

* <span data-ttu-id="dc563-2079">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="dc563-2079">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="dc563-2080">Потребление</span><span class="sxs-lookup"><span data-stu-id="dc563-2080">Consumption</span></span>

* <span data-ttu-id="dc563-2081">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2081">Added `marketplace` commands</span></span>
* <span data-ttu-id="dc563-2082">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2082">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="dc563-2083">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2083">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="dc563-2084">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2084">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="dc563-2085">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2085">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="dc563-2086">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2086">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="dc563-2087">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-2087">Container</span></span>

* <span data-ttu-id="dc563-2088">Добавлены параметры подключения тома репозитория Git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2088">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="dc563-2089">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="dc563-2089">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="dc563-2090">Расширение</span><span class="sxs-lookup"><span data-stu-id="dc563-2090">Extension</span></span>

* <span data-ttu-id="dc563-2091">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="dc563-2091">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="dc563-2092">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="dc563-2092">Interactive</span></span>

* <span data-ttu-id="dc563-2093">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="dc563-2093">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="dc563-2094">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="dc563-2094">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="dc563-2095">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2095">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="dc563-2096">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-2096">Network</span></span>

* <span data-ttu-id="dc563-2097">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2097">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="dc563-2098">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2098">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="dc563-2099">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="dc563-2099">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="dc563-2100">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="dc563-2100">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="dc563-2101">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="dc563-2101">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="dc563-2102">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2102">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="dc563-2103">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2103">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="dc563-2104">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="dc563-2104">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="dc563-2105">Профиль</span><span class="sxs-lookup"><span data-stu-id="dc563-2105">Profile</span></span>

* <span data-ttu-id="dc563-2106">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2106">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="dc563-2107">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi` & `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2107">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="dc563-2108">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="dc563-2108">RDBMS</span></span>

* <span data-ttu-id="dc563-2109">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2109">Added `georestore` command</span></span>
* <span data-ttu-id="dc563-2110">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="dc563-2110">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-2111">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-2111">Resource</span></span>

* <span data-ttu-id="dc563-2112">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2112">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="dc563-2113">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2113">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-2114">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-2114">SQL</span></span>

* <span data-ttu-id="dc563-2115">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2115">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-2116">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-2116">Storage</span></span>

* <span data-ttu-id="dc563-2117">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="dc563-2117">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-2118">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-2118">VM</span></span>

* <span data-ttu-id="dc563-2119">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="dc563-2119">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="dc563-2120">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="dc563-2120">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="dc563-2122">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2122">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="dc563-2123">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="dc563-2123">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="dc563-2124">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="dc563-2124">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="dc563-2125">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="dc563-2125">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="dc563-2126">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-2126">March 27, 2018</span></span>

<span data-ttu-id="dc563-2127">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="dc563-2127">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="dc563-2128">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-2128">Core</span></span>

* <span data-ttu-id="dc563-2129">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="dc563-2129">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-2130">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-2130">ACS</span></span>

* <span data-ttu-id="dc563-2131">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="dc563-2131">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-2132">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-2132">Appservice</span></span>

* <span data-ttu-id="dc563-2133">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2133">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="dc563-2134">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2134">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="dc563-2135">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="dc563-2135">Backup</span></span>

* <span data-ttu-id="dc563-2136">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2136">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="dc563-2137">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="dc563-2137">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="dc563-2138">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="dc563-2138">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="dc563-2139">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2139">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="dc563-2140">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-2140">Container</span></span>

* <span data-ttu-id="dc563-2141">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2141">Added `container exec` command.</span></span> <span data-ttu-id="dc563-2142">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="dc563-2142">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="dc563-2143">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="dc563-2143">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="dc563-2144">Расширение</span><span class="sxs-lookup"><span data-stu-id="dc563-2144">Extension</span></span>

* <span data-ttu-id="dc563-2145">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="dc563-2145">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="dc563-2146">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2146">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="dc563-2147">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-2147">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="dc563-2148">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="dc563-2148">Interactive</span></span>

* <span data-ttu-id="dc563-2149">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="dc563-2149">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="dc563-2150">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2150">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="dc563-2151">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="dc563-2151">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="dc563-2152">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="dc563-2152">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="dc563-2153">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="dc563-2153">Lab</span></span>

* <span data-ttu-id="dc563-2154">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2154">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="dc563-2155">Монитор</span><span class="sxs-lookup"><span data-stu-id="dc563-2155">Monitor</span></span>

* <span data-ttu-id="dc563-2156">Добавлена поддержка аргументов `--top`, `--orderby` и `--namespace` для `metrics list` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="dc563-2156">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="dc563-2157">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="dc563-2157">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="dc563-2158">Добавлена поддержка `--namespace` для `metrics list-definitions` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="dc563-2158">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="dc563-2159">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-2159">Network</span></span>

* <span data-ttu-id="dc563-2160">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="dc563-2160">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="dc563-2161">Профиль</span><span class="sxs-lookup"><span data-stu-id="dc563-2161">Profile</span></span>

* <span data-ttu-id="dc563-2162">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2162">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="dc563-2163">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="dc563-2163">RDBMS</span></span>

* <span data-ttu-id="dc563-2164">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="dc563-2164">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-2165">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-2165">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="dc563-2167">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-2167">Role</span></span>

* <span data-ttu-id="dc563-2168">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2168">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="dc563-2169">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="dc563-2169">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="dc563-2170">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="dc563-2170">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="dc563-2171">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2171">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="dc563-2172">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2172">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-2173">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-2173">Storage</span></span>

* <span data-ttu-id="dc563-2174">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="dc563-2174">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="dc563-2175">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="dc563-2175">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-2176">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-2176">VM</span></span>

* <span data-ttu-id="dc563-2177">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="dc563-2177">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="dc563-2178">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2178">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="dc563-2179">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="dc563-2179">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="dc563-2180">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="dc563-2180">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="dc563-2181">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-2181">March 13, 2018</span></span>

<span data-ttu-id="dc563-2182">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="dc563-2182">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-2183">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-2183">ACR</span></span>

* <span data-ttu-id="dc563-2184">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2184">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="dc563-2185">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="dc563-2185">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="dc563-2186">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="dc563-2186">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-2187">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-2187">ACS</span></span>

* <span data-ttu-id="dc563-2188">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="dc563-2188">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="dc563-2189">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="dc563-2189">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="dc563-2190">Помощник</span><span class="sxs-lookup"><span data-stu-id="dc563-2190">Advisor</span></span>

* <span data-ttu-id="dc563-2191">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2191">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="dc563-2192">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2192">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="dc563-2193">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2193">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="dc563-2194">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2194">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="dc563-2195">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2195">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-2196">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-2196">Appservice</span></span>

* <span data-ttu-id="dc563-2197">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="dc563-2197">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="dc563-2198">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2198">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="dc563-2199">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="dc563-2199">Eventhubs</span></span>

* <span data-ttu-id="dc563-2200">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="dc563-2200">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="dc563-2201">Расширение</span><span class="sxs-lookup"><span data-stu-id="dc563-2201">Extension</span></span>

* <span data-ttu-id="dc563-2202">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="dc563-2202">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="dc563-2203">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="dc563-2203">Interactive</span></span>

* <span data-ttu-id="dc563-2204">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="dc563-2204">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="dc563-2205">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="dc563-2205">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="dc563-2206">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="dc563-2206">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="dc563-2207">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="dc563-2207">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="dc563-2208">Монитор</span><span class="sxs-lookup"><span data-stu-id="dc563-2208">Monitor</span></span>

* <span data-ttu-id="dc563-2209">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="dc563-2209">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="dc563-2210">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2210">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="dc563-2211">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2211">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="dc563-2212">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2212">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="dc563-2213">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-2213">Network</span></span>

* <span data-ttu-id="dc563-2214">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2214">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="dc563-2215">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="dc563-2215">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="dc563-2216">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2216">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="dc563-2217">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2217">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="dc563-2218">Профиль</span><span class="sxs-lookup"><span data-stu-id="dc563-2218">Profile</span></span>

* <span data-ttu-id="dc563-2219">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="dc563-2219">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="dc563-2220">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2220">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="dc563-2221">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="dc563-2221">RDBMS</span></span>

* <span data-ttu-id="dc563-2222">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="dc563-2222">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="dc563-2223">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="dc563-2223">Service Bus</span></span>

* <span data-ttu-id="dc563-2224">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="dc563-2224">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-2225">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-2225">Storage</span></span>

* <span data-ttu-id="dc563-2226">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="dc563-2226">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="dc563-2227">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="dc563-2227">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-2228">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-2228">VM</span></span>

* <span data-ttu-id="dc563-2229">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="dc563-2229">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="dc563-2230">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="dc563-2230">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="dc563-2231">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2231">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="dc563-2232">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="dc563-2232">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="dc563-2233">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="dc563-2233">February 27, 2018</span></span>

<span data-ttu-id="dc563-2234">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="dc563-2234">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="dc563-2235">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-2235">Core</span></span>

* <span data-ttu-id="dc563-2236">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="dc563-2236">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="dc563-2237">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="dc563-2237">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="dc563-2238">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2238">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-2239">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-2239">ACS</span></span>

* <span data-ttu-id="dc563-2240">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-2240">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="dc563-2241">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="dc563-2241">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="dc563-2242">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2242">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="dc563-2243">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2243">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-2244">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-2244">Appservice</span></span>

* <span data-ttu-id="dc563-2245">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="dc563-2245">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="dc563-2246">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="dc563-2246">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="dc563-2247">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="dc563-2247">Cognitive Services</span></span>

* <span data-ttu-id="dc563-2248">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="dc563-2248">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="dc563-2249">Потребление</span><span class="sxs-lookup"><span data-stu-id="dc563-2249">Consumption</span></span>

* <span data-ttu-id="dc563-2250">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="dc563-2250">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="dc563-2251">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="dc563-2251">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="dc563-2252">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-2252">Container</span></span>

* <span data-ttu-id="dc563-2253">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="dc563-2253">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="dc563-2254">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-2254">Network</span></span>

* <span data-ttu-id="dc563-2255">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2255">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-2256">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-2256">Resource</span></span>

* <span data-ttu-id="dc563-2257">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="dc563-2257">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="dc563-2258">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-2258">Role</span></span>

* <span data-ttu-id="dc563-2259">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="dc563-2259">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-2260">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-2260">SQL</span></span>

* <span data-ttu-id="dc563-2261">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="dc563-2261">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-2262">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-2262">Storage</span></span>

* <span data-ttu-id="dc563-2263">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2263">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-2264">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-2264">VM</span></span>

* <span data-ttu-id="dc563-2265">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="dc563-2265">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="dc563-2266">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-2266">February 13, 2018</span></span>

<span data-ttu-id="dc563-2267">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="dc563-2267">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="dc563-2268">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-2268">Core</span></span>

* <span data-ttu-id="dc563-2269">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="dc563-2269">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-2270">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-2270">ACS</span></span>

* <span data-ttu-id="dc563-2271">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="dc563-2271">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="dc563-2272">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2272">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="dc563-2273">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="dc563-2273">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="dc563-2274">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="dc563-2274">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="dc563-2275">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="dc563-2275">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="dc563-2276">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2276">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="dc563-2277">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="dc563-2277">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="dc563-2278">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2278">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-2279">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-2279">Appservice</span></span>

* <span data-ttu-id="dc563-2280">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="dc563-2280">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="dc563-2281">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2281">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="dc563-2282">CDN</span><span class="sxs-lookup"><span data-stu-id="dc563-2282">CDN</span></span>

* <span data-ttu-id="dc563-2283">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2283">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="dc563-2284">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-2284">Container</span></span>

* <span data-ttu-id="dc563-2285">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="dc563-2285">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="dc563-2286">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="dc563-2286">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="dc563-2287">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="dc563-2287">CosmosDB</span></span>

* <span data-ttu-id="dc563-2288">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="dc563-2288">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="dc563-2289">Расширение</span><span class="sxs-lookup"><span data-stu-id="dc563-2289">Extension</span></span>

* <span data-ttu-id="dc563-2290">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2290">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="dc563-2291">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2291">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="dc563-2292">Отзывы</span><span class="sxs-lookup"><span data-stu-id="dc563-2292">Feedback</span></span>

* <span data-ttu-id="dc563-2293">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="dc563-2293">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="dc563-2294">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="dc563-2294">Interactive</span></span>

* <span data-ttu-id="dc563-2295">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="dc563-2295">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="dc563-2296">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="dc563-2296">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="dc563-2297">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="dc563-2297">IoT</span></span>

* <span data-ttu-id="dc563-2298">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="dc563-2298">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="dc563-2299">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="dc563-2299">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="dc563-2300">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2300">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="dc563-2301">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="dc563-2301">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="dc563-2302">Монитор</span><span class="sxs-lookup"><span data-stu-id="dc563-2302">Monitor</span></span>

* <span data-ttu-id="dc563-2303">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2303">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="dc563-2304">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-2304">Network</span></span>

* <span data-ttu-id="dc563-2305">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="dc563-2305">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="dc563-2306">Профиль</span><span class="sxs-lookup"><span data-stu-id="dc563-2306">Profile</span></span>

* <span data-ttu-id="dc563-2307">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="dc563-2307">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-2308">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-2308">Resource</span></span>

* <span data-ttu-id="dc563-2309">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2309">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="dc563-2310">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-2310">Role</span></span>

* <span data-ttu-id="dc563-2311">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="dc563-2311">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-2312">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-2312">SQL</span></span>

* <span data-ttu-id="dc563-2313">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2313">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="dc563-2314">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2314">Added `sql db rename`</span></span>
* <span data-ttu-id="dc563-2315">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="dc563-2315">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-2316">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-2316">Storage</span></span>

* <span data-ttu-id="dc563-2317">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="dc563-2317">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-2318">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-2318">VM</span></span>

* <span data-ttu-id="dc563-2319">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="dc563-2319">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="dc563-2320">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="dc563-2320">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="dc563-2321">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="dc563-2321">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="dc563-2322">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-2322">January 31, 2018</span></span>

<span data-ttu-id="dc563-2323">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="dc563-2323">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="dc563-2324">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-2324">Core</span></span>

* <span data-ttu-id="dc563-2325">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="dc563-2325">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="dc563-2326">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="dc563-2326">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="dc563-2327">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="dc563-2327">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="dc563-2328">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="dc563-2328">Use `--verbose` to see</span></span>
* <span data-ttu-id="dc563-2329">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="dc563-2329">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-2330">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-2330">ACS</span></span>

* <span data-ttu-id="dc563-2331">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2331">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="dc563-2332">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2332">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-2333">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-2333">Appservice</span></span>

* <span data-ttu-id="dc563-2334">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="dc563-2334">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="dc563-2335">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="dc563-2335">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="dc563-2336">CDN</span><span class="sxs-lookup"><span data-stu-id="dc563-2336">CDN</span></span>

* <span data-ttu-id="dc563-2337">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2337">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="dc563-2338">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="dc563-2338">CosmosDB</span></span>

* <span data-ttu-id="dc563-2339">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="dc563-2339">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="dc563-2340">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="dc563-2340">Interactive</span></span>

* <span data-ttu-id="dc563-2341">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="dc563-2341">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="dc563-2342">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-2342">Network</span></span>

* <span data-ttu-id="dc563-2343">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2343">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="dc563-2344">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-2344">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="dc563-2345">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2345">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="dc563-2346">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2346">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="dc563-2347">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2347">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="dc563-2348">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="dc563-2348">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="dc563-2349">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="dc563-2349">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="dc563-2350">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="dc563-2350">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="dc563-2351">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2351">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="dc563-2352">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2352">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="dc563-2353">Профиль</span><span class="sxs-lookup"><span data-stu-id="dc563-2353">Profile</span></span>

* <span data-ttu-id="dc563-2354">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="dc563-2354">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-2355">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-2355">Resource</span></span>

* <span data-ttu-id="dc563-2356">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="dc563-2356">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-2357">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-2357">Storage</span></span>

* <span data-ttu-id="dc563-2358">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="dc563-2358">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="dc563-2359">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="dc563-2359">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="dc563-2360">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2360">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="dc563-2361">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2361">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="dc563-2362">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="dc563-2362">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-2363">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-2363">VM</span></span>

* <span data-ttu-id="dc563-2364">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="dc563-2364">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="dc563-2365">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="dc563-2365">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="dc563-2366">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="dc563-2366">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="dc563-2367">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2367">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="dc563-2368">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-2368">January 17, 2018</span></span>

<span data-ttu-id="dc563-2369">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="dc563-2369">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-2370">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-2370">ACR</span></span>

* <span data-ttu-id="dc563-2371">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="dc563-2371">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="dc563-2372">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="dc563-2372">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-2373">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-2373">ACS</span></span>

* <span data-ttu-id="dc563-2374">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2374">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="dc563-2375">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="dc563-2375">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-2376">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-2376">Appservice</span></span>

* <span data-ttu-id="dc563-2377">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="dc563-2377">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="dc563-2378">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="dc563-2378">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="dc563-2379">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2379">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="dc563-2380">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="dc563-2380">Backup</span></span>

* <span data-ttu-id="dc563-2381">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="dc563-2381">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="dc563-2382">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="dc563-2382">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="dc563-2383">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="dc563-2383">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="dc563-2384">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="dc563-2384">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="dc563-2385">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="dc563-2385">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="dc563-2386">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="dc563-2386">Batch</span></span>

* <span data-ttu-id="dc563-2387">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="dc563-2387">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="dc563-2388">Cloud</span><span class="sxs-lookup"><span data-stu-id="dc563-2388">Cloud</span></span>

* <span data-ttu-id="dc563-2389">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="dc563-2389">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="dc563-2390">Потребление</span><span class="sxs-lookup"><span data-stu-id="dc563-2390">Consumption</span></span>

* <span data-ttu-id="dc563-2391">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2391">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="dc563-2392">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="dc563-2392">Event Grid</span></span>

* <span data-ttu-id="dc563-2393">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2393">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="dc563-2394">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2394">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="dc563-2395">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2395">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="dc563-2396">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2396">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="dc563-2397">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2397">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="dc563-2398">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2398">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="dc563-2399">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2399">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="dc563-2400">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="dc563-2400">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="dc563-2401">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="dc563-2401">Interactive</span></span>

* <span data-ttu-id="dc563-2402">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="dc563-2402">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="dc563-2403">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="dc563-2403">Fixed errors on startup</span></span>
* <span data-ttu-id="dc563-2404">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="dc563-2404">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="dc563-2405">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="dc563-2405">IoT</span></span>

* <span data-ttu-id="dc563-2406">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="dc563-2406">Added support for device provisioning service</span></span>
* <span data-ttu-id="dc563-2407">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="dc563-2407">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="dc563-2408">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="dc563-2408">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="dc563-2409">Монитор</span><span class="sxs-lookup"><span data-stu-id="dc563-2409">Monitor</span></span>

* <span data-ttu-id="dc563-2410">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="dc563-2410">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="dc563-2411">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2411">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="dc563-2412">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="dc563-2412">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="dc563-2413">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-2413">Network</span></span>

* <span data-ttu-id="dc563-2414">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="dc563-2414">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="dc563-2415">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="dc563-2415">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="dc563-2416">Профиль</span><span class="sxs-lookup"><span data-stu-id="dc563-2416">Profile</span></span>

* <span data-ttu-id="dc563-2417">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="dc563-2417">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="dc563-2418">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-2418">Role</span></span>

* <span data-ttu-id="dc563-2419">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="dc563-2419">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="dc563-2420">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="dc563-2420">Service Fabric</span></span>

* <span data-ttu-id="dc563-2421">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="dc563-2421">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="dc563-2422">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="dc563-2422">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-2423">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-2423">VM</span></span>

* <span data-ttu-id="dc563-2424">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2424">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="dc563-2425">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="dc563-2425">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="dc563-2426">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2426">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="dc563-2427">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="dc563-2427">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="dc563-2428">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="dc563-2428">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="dc563-2429">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2429">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="dc563-2430">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2430">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="dc563-2431">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2431">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="dc563-2432">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-2432">December 19, 2017</span></span>

<span data-ttu-id="dc563-2433">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="dc563-2433">Version 2.0.23</span></span>

* <span data-ttu-id="dc563-2434">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="dc563-2434">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="dc563-2435">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-2435">Container</span></span>

* <span data-ttu-id="dc563-2436">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="dc563-2436">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="dc563-2437">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-2437">Network</span></span>

* <span data-ttu-id="dc563-2438">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="dc563-2438">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="dc563-2439">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="dc563-2439">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-2440">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-2440">Storage</span></span>

* <span data-ttu-id="dc563-2441">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="dc563-2441">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-2442">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-2442">VM</span></span>

* <span data-ttu-id="dc563-2443">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="dc563-2443">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="dc563-2444">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-2444">December 5, 2017</span></span>

<span data-ttu-id="dc563-2445">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="dc563-2445">Version 2.0.22</span></span>

* <span data-ttu-id="dc563-2446">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2446">Removed `az component` commands.</span></span> <span data-ttu-id="dc563-2447">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2447">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="dc563-2448">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-2448">Core</span></span>
* <span data-ttu-id="dc563-2449">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="dc563-2449">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="dc563-2450">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="dc563-2450">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-2451">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-2451">ACS</span></span>

* <span data-ttu-id="dc563-2452">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2452">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="dc563-2453">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2453">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="dc563-2454">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="dc563-2454">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="dc563-2455">Помощник</span><span class="sxs-lookup"><span data-stu-id="dc563-2455">Advisor</span></span>

* <span data-ttu-id="dc563-2456">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="dc563-2456">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-2457">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-2457">Appservice</span></span>

* <span data-ttu-id="dc563-2458">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2458">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="dc563-2459">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="dc563-2459">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="dc563-2460">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2460">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="dc563-2461">Потребление</span><span class="sxs-lookup"><span data-stu-id="dc563-2461">Consumption</span></span>

* <span data-ttu-id="dc563-2462">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="dc563-2462">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="dc563-2463">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-2463">Container</span></span>

* <span data-ttu-id="dc563-2464">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="dc563-2464">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="dc563-2465">Монитор</span><span class="sxs-lookup"><span data-stu-id="dc563-2465">Monitor</span></span>

* <span data-ttu-id="dc563-2466">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="dc563-2466">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-2467">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-2467">Resource</span></span>

* <span data-ttu-id="dc563-2468">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="dc563-2468">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="dc563-2469">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-2469">Role</span></span>

* <span data-ttu-id="dc563-2470">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2470">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="dc563-2471">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="dc563-2471">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="dc563-2472">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2472">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-2473">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-2473">SQL</span></span>

* <span data-ttu-id="dc563-2474">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2474">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="dc563-2475">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2475">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-2476">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-2476">VM</span></span>

* <span data-ttu-id="dc563-2477">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2477">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="dc563-2478">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-2478">November 14, 2017</span></span>

<span data-ttu-id="dc563-2479">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="dc563-2479">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-2480">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-2480">ACR</span></span>

* <span data-ttu-id="dc563-2481">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="dc563-2481">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="dc563-2482">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-2482">ACS</span></span>

* <span data-ttu-id="dc563-2483">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="dc563-2483">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="dc563-2484">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="dc563-2484">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="dc563-2485">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2485">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="dc563-2486">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="dc563-2486">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="dc563-2487">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="dc563-2487">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-2488">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-2488">Appservice</span></span>

* <span data-ttu-id="dc563-2489">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="dc563-2489">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="dc563-2490">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2490">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="dc563-2491">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2491">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="dc563-2492">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2492">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="dc563-2493">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="dc563-2493">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="dc563-2494">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="dc563-2494">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="dc563-2495">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="dc563-2495">Batch</span></span>

* <span data-ttu-id="dc563-2496">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2496">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="dc563-2497">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="dc563-2497">Batchai</span></span>

* <span data-ttu-id="dc563-2498">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2498">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="dc563-2499">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2499">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="dc563-2500">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2500">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="dc563-2501">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2501">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="dc563-2502">Cloud</span><span class="sxs-lookup"><span data-stu-id="dc563-2502">Cloud</span></span>

* <span data-ttu-id="dc563-2503">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="dc563-2503">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="dc563-2504">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-2504">Container</span></span>

* <span data-ttu-id="dc563-2505">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="dc563-2505">Added support to open multiple ports</span></span>
* <span data-ttu-id="dc563-2506">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="dc563-2506">Added container group restart policy</span></span>
* <span data-ttu-id="dc563-2507">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="dc563-2507">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="dc563-2508">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="dc563-2508">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="dc563-2509">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="dc563-2509">Data Lake Analytics</span></span>

* <span data-ttu-id="dc563-2510">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="dc563-2510">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="dc563-2511">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="dc563-2511">Data Lake Store</span></span>

* <span data-ttu-id="dc563-2512">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="dc563-2512">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="dc563-2513">Расширение</span><span class="sxs-lookup"><span data-stu-id="dc563-2513">Extension</span></span>

* <span data-ttu-id="dc563-2514">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="dc563-2514">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="dc563-2515">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="dc563-2515">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="dc563-2516">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="dc563-2516">IoT</span></span>

* <span data-ttu-id="dc563-2517">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="dc563-2517">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="dc563-2518">Монитор</span><span class="sxs-lookup"><span data-stu-id="dc563-2518">Monitor</span></span>

* <span data-ttu-id="dc563-2519">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2519">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="dc563-2520">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-2520">Network</span></span>

* <span data-ttu-id="dc563-2521">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="dc563-2521">Added support for CAA DNS records</span></span>
* <span data-ttu-id="dc563-2522">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2522">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="dc563-2523">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="dc563-2523">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="dc563-2524">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2524">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="dc563-2525">Резервирование</span><span class="sxs-lookup"><span data-stu-id="dc563-2525">Reservations</span></span>

* <span data-ttu-id="dc563-2526">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="dc563-2526">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-2527">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-2527">Resource</span></span>

* <span data-ttu-id="dc563-2528">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2528">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-2529">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-2529">SQL</span></span>

* <span data-ttu-id="dc563-2530">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2530">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-2531">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-2531">Storage</span></span>

* <span data-ttu-id="dc563-2532">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-2532">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="dc563-2533">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="dc563-2533">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="dc563-2534">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2534">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="dc563-2535">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2535">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="dc563-2536">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2536">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="dc563-2537">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2537">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="dc563-2538">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2538">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-2539">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-2539">VM</span></span>

* <span data-ttu-id="dc563-2540">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2540">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="dc563-2541">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="dc563-2541">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="dc563-2542">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2542">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="dc563-2543">Переименование `vm format-secret` в `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="dc563-2543">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="dc563-2544">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="dc563-2544">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="dc563-2545">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-2545">October 24, 2017</span></span>

<span data-ttu-id="dc563-2546">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="dc563-2546">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="dc563-2547">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-2547">Core</span></span>

* <span data-ttu-id="dc563-2548">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="dc563-2548">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-2549">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-2549">ACR</span></span>

* <span data-ttu-id="dc563-2550">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="dc563-2550">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="dc563-2551">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="dc563-2551">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="dc563-2552">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="dc563-2552">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-2553">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-2553">ACS</span></span>

* <span data-ttu-id="dc563-2554">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="dc563-2554">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="dc563-2555">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="dc563-2555">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-2556">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-2556">Appservice</span></span>

* <span data-ttu-id="dc563-2557">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="dc563-2557">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="dc563-2558">Компонент</span><span class="sxs-lookup"><span data-stu-id="dc563-2558">Component</span></span>

* <span data-ttu-id="dc563-2559">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="dc563-2559">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="dc563-2560">Монитор</span><span class="sxs-lookup"><span data-stu-id="dc563-2560">Monitor</span></span>

* <span data-ttu-id="dc563-2561">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2561">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-2562">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-2562">Resource</span></span>

* <span data-ttu-id="dc563-2563">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="dc563-2563">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="dc563-2564">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="dc563-2564">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-2565">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-2565">VM</span></span>

* <span data-ttu-id="dc563-2566">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="dc563-2566">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="dc563-2567">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-2567">October 9, 2017</span></span>

<span data-ttu-id="dc563-2568">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="dc563-2568">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="dc563-2569">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-2569">Core</span></span>

* <span data-ttu-id="dc563-2570">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="dc563-2570">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-2571">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-2571">Appservice</span></span>

* <span data-ttu-id="dc563-2572">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2572">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="dc563-2573">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="dc563-2573">Batch</span></span>

* <span data-ttu-id="dc563-2574">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="dc563-2574">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="dc563-2575">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="dc563-2575">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="dc563-2576">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="dc563-2576">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="dc563-2577">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="dc563-2577">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="dc563-2578">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="dc563-2578">Batchai</span></span>

* <span data-ttu-id="dc563-2579">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="dc563-2579">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="dc563-2580">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="dc563-2580">Keyvault</span></span>

* <span data-ttu-id="dc563-2581">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="dc563-2581">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="dc563-2582">(#4448)</span><span class="sxs-lookup"><span data-stu-id="dc563-2582">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="dc563-2583">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-2583">Network</span></span>

* <span data-ttu-id="dc563-2584">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="dc563-2584">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="dc563-2585">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="dc563-2585">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-2586">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-2586">Resource</span></span>

* <span data-ttu-id="dc563-2587">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2587">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="dc563-2588">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="dc563-2588">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="dc563-2589">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="dc563-2589">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="dc563-2590">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="dc563-2590">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-2591">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-2591">Sql</span></span>

* <span data-ttu-id="dc563-2592">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="dc563-2592">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="dc563-2593">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="dc563-2593">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="dc563-2594">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="dc563-2594">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-2595">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-2595">Storage</span></span>

* <span data-ttu-id="dc563-2596">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="dc563-2596">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-2597">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="dc563-2597">Vm</span></span>

* <span data-ttu-id="dc563-2598">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="dc563-2598">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="dc563-2599">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2599">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="dc563-2600">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2600">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="dc563-2601">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2601">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="dc563-2602">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="dc563-2602">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="dc563-2603">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-2603">September 22, 2017</span></span>

<span data-ttu-id="dc563-2604">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="dc563-2604">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-2605">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-2605">Resource</span></span>

* <span data-ttu-id="dc563-2606">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="dc563-2606">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="dc563-2607">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="dc563-2607">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="dc563-2608">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="dc563-2608">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="dc563-2609">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2609">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="dc563-2610">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-2610">Network</span></span>

* <span data-ttu-id="dc563-2611">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="dc563-2611">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="dc563-2612">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="dc563-2612">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="dc563-2613">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="dc563-2613">Added `asg` application security group commands</span></span>
* <span data-ttu-id="dc563-2614">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="dc563-2614">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="dc563-2615">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="dc563-2615">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="dc563-2616">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="dc563-2616">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="dc563-2617">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2617">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-2618">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-2618">Storage</span></span>

* <span data-ttu-id="dc563-2619">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="dc563-2619">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="dc563-2620">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="dc563-2620">Eventgrid</span></span>

* <span data-ttu-id="dc563-2621">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="dc563-2621">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-2622">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-2622">SQL</span></span>

* <span data-ttu-id="dc563-2623">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="dc563-2623">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="dc563-2624">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="dc563-2624">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="dc563-2625">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="dc563-2625">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="dc563-2626">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="dc563-2626">Keyvault</span></span>

* <span data-ttu-id="dc563-2627">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="dc563-2627">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-2628">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-2628">VM</span></span>

* <span data-ttu-id="dc563-2629">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="dc563-2629">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="dc563-2630">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="dc563-2630">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="dc563-2631">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="dc563-2631">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="dc563-2632">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="dc563-2632">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="dc563-2633">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="dc563-2633">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="dc563-2634">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="dc563-2634">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-2635">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-2635">ACS</span></span>

* <span data-ttu-id="dc563-2636">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="dc563-2636">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-2637">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-2637">Appservice</span></span>

* <span data-ttu-id="dc563-2638">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="dc563-2638">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="dc563-2639">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="dc563-2639">Backup</span></span>

* <span data-ttu-id="dc563-2640">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="dc563-2640">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="dc563-2641">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-2641">September 11, 2017</span></span>

<span data-ttu-id="dc563-2642">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="dc563-2642">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="dc563-2643">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-2643">Core</span></span>

* <span data-ttu-id="dc563-2644">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="dc563-2644">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="dc563-2645">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="dc563-2645">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-2646">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-2646">Acs</span></span>

* <span data-ttu-id="dc563-2647">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2647">Added `acs list-locations` command</span></span>
* <span data-ttu-id="dc563-2648">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-2648">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-2649">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-2649">Appservice</span></span>

* <span data-ttu-id="dc563-2650">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="dc563-2650">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="dc563-2651">CDN</span><span class="sxs-lookup"><span data-stu-id="dc563-2651">CDN</span></span>

* <span data-ttu-id="dc563-2652">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2652">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="dc563-2653">Расширение</span><span class="sxs-lookup"><span data-stu-id="dc563-2653">Extension</span></span>

* <span data-ttu-id="dc563-2654">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="dc563-2654">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="dc563-2655">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="dc563-2655">Keyvault</span></span>

* <span data-ttu-id="dc563-2656">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2656">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="dc563-2657">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-2657">Network</span></span>

* <span data-ttu-id="dc563-2658">Переименование `vnet list-private-access-services` в `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="dc563-2658">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="dc563-2659">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2659">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="dc563-2660">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2660">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="dc563-2661">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2661">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="dc563-2662">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2662">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-2663">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-2663">Resource</span></span>

* <span data-ttu-id="dc563-2664">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2664">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="dc563-2665">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2665">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="dc563-2666">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="dc563-2666">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="dc563-2667">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="dc563-2667">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-2668">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-2668">SQL</span></span>

* <span data-ttu-id="dc563-2669">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2669">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-2670">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-2670">VM</span></span>

* <span data-ttu-id="dc563-2671">Исправлено: Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="dc563-2671">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="dc563-2672">Исправлено: Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="dc563-2672">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="dc563-2673">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2673">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="dc563-2674">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="dc563-2674">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="dc563-2675">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="dc563-2675">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="dc563-2676">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-2676">August 31, 2017</span></span>

<span data-ttu-id="dc563-2677">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="dc563-2677">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="dc563-2678">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="dc563-2678">Keyvault</span></span>

* <span data-ttu-id="dc563-2679">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2679">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="dc563-2680">Sf</span><span class="sxs-lookup"><span data-stu-id="dc563-2680">Sf</span></span>

* <span data-ttu-id="dc563-2681">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="dc563-2681">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-2682">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-2682">Storage</span></span>

* <span data-ttu-id="dc563-2683">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="dc563-2683">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="dc563-2684">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="dc563-2684">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="dc563-2685">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-2685">August 28, 2017</span></span>

<span data-ttu-id="dc563-2686">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="dc563-2686">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="dc563-2687">CLI</span><span class="sxs-lookup"><span data-stu-id="dc563-2687">CLI</span></span>

* <span data-ttu-id="dc563-2688">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="dc563-2688">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-2689">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-2689">ACS</span></span>

* <span data-ttu-id="dc563-2690">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="dc563-2690">Corrected preview regions</span></span>
* <span data-ttu-id="dc563-2691">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2691">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="dc563-2692">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="dc563-2692">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-2693">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-2693">Appservice</span></span>

* <span data-ttu-id="dc563-2694">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2694">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="dc563-2695">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2695">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="dc563-2696">Предоставлен параметр `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2696">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="dc563-2697">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="dc563-2697">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="dc563-2698">Исправлено: Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="dc563-2698">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="dc563-2699">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="dc563-2699">IoT</span></span>

* <span data-ttu-id="dc563-2700">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="dc563-2700">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="dc563-2701">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-2701">Network</span></span>

* <span data-ttu-id="dc563-2702">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2702">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="dc563-2703">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2703">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="dc563-2704">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2704">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="dc563-2705">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2705">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="dc563-2706">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2706">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="dc563-2707">Профиль</span><span class="sxs-lookup"><span data-stu-id="dc563-2707">Profile</span></span>

* <span data-ttu-id="dc563-2708">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="dc563-2708">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="dc563-2709">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="dc563-2709">Service Fabric</span></span>

* <span data-ttu-id="dc563-2710">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="dc563-2710">Preview release</span></span>
* <span data-ttu-id="dc563-2711">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="dc563-2711">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="dc563-2712">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="dc563-2712">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="dc563-2713">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2713">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-2714">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-2714">Storage</span></span>

* <span data-ttu-id="dc563-2715">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="dc563-2715">Enabled setting blob tier</span></span>
* <span data-ttu-id="dc563-2716">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="dc563-2716">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="dc563-2717">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2717">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="dc563-2718">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="dc563-2718">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="dc563-2719">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2719">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="dc563-2720">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2720">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-2721">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-2721">VM</span></span>

* <span data-ttu-id="dc563-2722">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2722">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="dc563-2723">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2723">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="dc563-2724">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="dc563-2724">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="dc563-2725">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="dc563-2725">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="dc563-2726">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="dc563-2726">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="dc563-2727">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2727">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="dc563-2728">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-2728">August 15, 2017</span></span>

<span data-ttu-id="dc563-2729">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="dc563-2729">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-2730">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-2730">ACS</span></span>

* <span data-ttu-id="dc563-2731">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="dc563-2731">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-2732">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-2732">Appservice</span></span>

* <span data-ttu-id="dc563-2733">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="dc563-2733">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="dc563-2734">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="dc563-2734">Event Grid</span></span>

* <span data-ttu-id="dc563-2735">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="dc563-2735">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="dc563-2736">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-2736">August 11, 2017</span></span>

<span data-ttu-id="dc563-2737">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="dc563-2737">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-2738">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-2738">ACS</span></span>

* <span data-ttu-id="dc563-2739">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="dc563-2739">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="dc563-2740">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="dc563-2740">Batch</span></span>

* <span data-ttu-id="dc563-2741">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="dc563-2741">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="dc563-2742">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="dc563-2742">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="dc563-2743">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="dc563-2743">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="dc563-2744">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="dc563-2744">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="dc563-2745">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="dc563-2745">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="dc563-2746">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="dc563-2746">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="dc563-2747">Компонент</span><span class="sxs-lookup"><span data-stu-id="dc563-2747">Component</span></span>

* <span data-ttu-id="dc563-2748">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="dc563-2748">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="dc563-2749">Контейнер</span><span class="sxs-lookup"><span data-stu-id="dc563-2749">Container</span></span>

* <span data-ttu-id="dc563-2750">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="dc563-2750">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="dc563-2751">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="dc563-2751">Data Lake Store</span></span>

* <span data-ttu-id="dc563-2752">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="dc563-2752">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="dc563-2753">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="dc563-2753">Event Grid</span></span>

* <span data-ttu-id="dc563-2754">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="dc563-2754">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="dc563-2755">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-2755">Network</span></span>

* <span data-ttu-id="dc563-2756">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="dc563-2756">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="dc563-2757">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2757">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="dc563-2758">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2758">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="dc563-2759">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2759">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="dc563-2760">Профиль</span><span class="sxs-lookup"><span data-stu-id="dc563-2760">Profile</span></span>

* <span data-ttu-id="dc563-2761">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="dc563-2761">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-2762">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-2762">Storage</span></span>

* <span data-ttu-id="dc563-2763">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="dc563-2763">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-2764">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-2764">VM</span></span>

* <span data-ttu-id="dc563-2765">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="dc563-2765">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="dc563-2766">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2766">Exposed `list-skus` command</span></span>
* <span data-ttu-id="dc563-2767">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="dc563-2767">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="dc563-2768">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="dc563-2768">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="dc563-2769">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="dc563-2769">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="dc563-2770">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-2770">July 28, 2017</span></span>

<span data-ttu-id="dc563-2771">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="dc563-2771">Version 2.0.12</span></span>

* <span data-ttu-id="dc563-2772">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="dc563-2772">Added container commands</span></span>
* <span data-ttu-id="dc563-2773">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="dc563-2773">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="dc563-2774">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-2774">Core</span></span>

* <span data-ttu-id="dc563-2775">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="dc563-2775">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="dc563-2776">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="dc563-2776">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="dc563-2777">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="dc563-2777">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="dc563-2778">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="dc563-2778">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="dc563-2779">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="dc563-2779">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="dc563-2780">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="dc563-2780">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="dc563-2781">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="dc563-2781">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="dc563-2782">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="dc563-2782">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="dc563-2783">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="dc563-2783">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="dc563-2784">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="dc563-2784">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="dc563-2785">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="dc563-2785">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="dc563-2786">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="dc563-2786">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="dc563-2787">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="dc563-2787">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="dc563-2788">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="dc563-2788">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="dc563-2789">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="dc563-2789">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="dc563-2790">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="dc563-2790">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="dc563-2791">ACR</span><span class="sxs-lookup"><span data-stu-id="dc563-2791">ACR</span></span>

* <span data-ttu-id="dc563-2792">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="dc563-2792">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="dc563-2793">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="dc563-2793">Support SKU update for managed registries</span></span>
* <span data-ttu-id="dc563-2794">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="dc563-2794">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="dc563-2795">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="dc563-2795">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="dc563-2796">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="dc563-2796">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="dc563-2797">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="dc563-2797">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-2798">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-2798">ACS</span></span>

* <span data-ttu-id="dc563-2799">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="dc563-2799">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-2800">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="dc563-2800">Appservice</span></span>

* <span data-ttu-id="dc563-2801">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="dc563-2801">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="dc563-2802">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="dc563-2802">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="dc563-2803">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2803">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="dc563-2804">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="dc563-2804">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="dc563-2805">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="dc563-2805">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="dc563-2806">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="dc563-2806">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="dc563-2807">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="dc563-2807">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="dc563-2808">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="dc563-2808">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="dc563-2809">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="dc563-2809">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="dc563-2810">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2810">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="dc563-2811">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="dc563-2811">Batch</span></span>

* <span data-ttu-id="dc563-2812">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="dc563-2812">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="dc563-2813">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2813">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="dc563-2814">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2814">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="dc563-2815">CDN</span><span class="sxs-lookup"><span data-stu-id="dc563-2815">CDN</span></span>

* <span data-ttu-id="dc563-2816">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="dc563-2816">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="dc563-2817">Cloud</span><span class="sxs-lookup"><span data-stu-id="dc563-2817">Cloud</span></span>

* <span data-ttu-id="dc563-2818">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="dc563-2818">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="dc563-2819">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="dc563-2819">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="dc563-2820">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="dc563-2820">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="dc563-2821">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="dc563-2821">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="dc563-2822">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2822">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="dc563-2823">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="dc563-2823">CosmosDB</span></span>

* <span data-ttu-id="dc563-2824">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="dc563-2824">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="dc563-2825">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="dc563-2825">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="dc563-2826">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="dc563-2826">Data Lake Analytics</span></span>

* <span data-ttu-id="dc563-2827">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2827">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="dc563-2828">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2828">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="dc563-2829">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2829">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="dc563-2830">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="dc563-2830">Data Lake Store</span></span>

* <span data-ttu-id="dc563-2831">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2831">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="dc563-2832">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="dc563-2832">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="dc563-2833">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2833">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="dc563-2834">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="dc563-2834">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="dc563-2835">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="dc563-2835">Interactive</span></span>

* <span data-ttu-id="dc563-2836">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="dc563-2836">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="dc563-2837">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="dc563-2837">Increased test coverage</span></span>
* <span data-ttu-id="dc563-2838">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="dc563-2838">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="dc563-2839">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="dc563-2839">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="dc563-2840">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="dc563-2840">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="dc563-2841">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="dc563-2841">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="dc563-2842">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="dc563-2842">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="dc563-2843">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2843">Added `--progress` flag</span></span>
* <span data-ttu-id="dc563-2844">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2844">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="dc563-2845">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="dc563-2845">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="dc563-2846">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="dc563-2846">IoT</span></span>

* <span data-ttu-id="dc563-2847">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="dc563-2847">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="dc563-2848">(3934).</span><span class="sxs-lookup"><span data-stu-id="dc563-2848">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="dc563-2849">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="dc563-2849">Key vault</span></span>

* <span data-ttu-id="dc563-2850">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="dc563-2850">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="dc563-2851">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2851">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="dc563-2852">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="dc563-2852">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="dc563-2853">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2853">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="dc563-2854">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2854">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="dc563-2855">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="dc563-2855">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="dc563-2856">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="dc563-2856">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="dc563-2857">(3307).</span><span class="sxs-lookup"><span data-stu-id="dc563-2857">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="dc563-2858">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="dc563-2858">Lab</span></span>

* <span data-ttu-id="dc563-2859">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2859">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="dc563-2860">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2860">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="dc563-2861">Монитор</span><span class="sxs-lookup"><span data-stu-id="dc563-2861">Monitor</span></span>

* <span data-ttu-id="dc563-2862">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="dc563-2862">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="dc563-2863">Переименование `monitor alert-rule-incidents list` в `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="dc563-2863">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="dc563-2864">Переименование `monitor alert-rule-incidents show` в `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="dc563-2864">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="dc563-2865">Переименование `monitor metric-defintions list` в `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="dc563-2865">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="dc563-2866">Переименование `monitor alert-rules` в `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="dc563-2866">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="dc563-2867">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="dc563-2867">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="dc563-2868">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="dc563-2868">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="dc563-2869">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="dc563-2869">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="dc563-2870">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="dc563-2870">`location` no longer required</span></span>
  * <span data-ttu-id="dc563-2871">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="dc563-2871">Add name and ID support for target</span></span>
  * <span data-ttu-id="dc563-2872">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="dc563-2872">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="dc563-2873">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="dc563-2873">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="dc563-2874">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="dc563-2874">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="dc563-2875">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="dc563-2875">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="dc563-2876">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2876">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="dc563-2877">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2877">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="dc563-2878">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-2878">Network</span></span>

* <span data-ttu-id="dc563-2879">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2879">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="dc563-2880">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2880">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="dc563-2881">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="dc563-2881">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="dc563-2882">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2882">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="dc563-2883">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2883">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="dc563-2884">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2884">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="dc563-2885">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2885">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="dc563-2886">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2886">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="dc563-2887">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2887">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="dc563-2888">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2888">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="dc563-2889">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2889">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="dc563-2890">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2890">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="dc563-2891">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2891">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="dc563-2892">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2892">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="dc563-2893">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2893">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="dc563-2894">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2894">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="dc563-2895">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="dc563-2895">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="dc563-2896">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2896">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="dc563-2897">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2897">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="dc563-2898">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2898">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="dc563-2899">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2899">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="dc563-2900">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2900">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="dc563-2901">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2901">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="dc563-2902">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="dc563-2902">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="dc563-2903">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="dc563-2903">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="dc563-2904">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="dc563-2904">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="dc563-2905">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="dc563-2905">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="dc563-2906">Профиль</span><span class="sxs-lookup"><span data-stu-id="dc563-2906">Profile</span></span>

* <span data-ttu-id="dc563-2907">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="dc563-2907">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="dc563-2908">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="dc563-2908">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="dc563-2909">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="dc563-2909">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="dc563-2910">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="dc563-2910">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="dc563-2911">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="dc563-2911">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="dc563-2912">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="dc563-2912">RDBMS</span></span>

* <span data-ttu-id="dc563-2913">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="dc563-2913">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="dc563-2914">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="dc563-2914">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="dc563-2915">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="dc563-2915">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="dc563-2916">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="dc563-2916">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-2917">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-2917">Resource</span></span>

* <span data-ttu-id="dc563-2918">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2918">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="dc563-2919">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2919">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="dc563-2920">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2920">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="dc563-2921">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2921">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="dc563-2922">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="dc563-2922">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="dc563-2923">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2923">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="dc563-2924">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="dc563-2924">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="dc563-2925">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2925">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="dc563-2926">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-2926">Role</span></span>

* <span data-ttu-id="dc563-2927">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="dc563-2927">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="dc563-2928">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="dc563-2928">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="dc563-2929">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="dc563-2929">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="dc563-2930">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="dc563-2930">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="dc563-2931">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2931">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="dc563-2932">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="dc563-2932">Service Fabric</span></span>
* <span data-ttu-id="dc563-2933">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="dc563-2933">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="dc563-2934">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="dc563-2934">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="dc563-2935">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="dc563-2935">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-2936">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-2936">SQL</span></span>

* <span data-ttu-id="dc563-2937">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2937">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="dc563-2938">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2938">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="dc563-2939">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2939">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-2940">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-2940">Storage</span></span>

* <span data-ttu-id="dc563-2941">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="dc563-2941">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="dc563-2942">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="dc563-2942">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="dc563-2943">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="dc563-2943">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="dc563-2944">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="dc563-2944">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="dc563-2945">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="dc563-2945">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="dc563-2946">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="dc563-2946">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-2947">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-2947">VM</span></span>

* <span data-ttu-id="dc563-2948">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="dc563-2948">Support configuring nsg</span></span>
* <span data-ttu-id="dc563-2949">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="dc563-2949">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="dc563-2950">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="dc563-2950">Support managed service identities</span></span>
* <span data-ttu-id="dc563-2951">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="dc563-2951">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="dc563-2952">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="dc563-2952">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="dc563-2953">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-2953">May 10, 2017</span></span>

<span data-ttu-id="dc563-2954">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="dc563-2954">Version 2.0.6</span></span>

* <span data-ttu-id="dc563-2955">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="dc563-2955">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="dc563-2956">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="dc563-2956">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="dc563-2957">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="dc563-2957">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="dc563-2958">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="dc563-2958">Include Cognitive Services module</span></span>
* <span data-ttu-id="dc563-2959">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="dc563-2959">Include Service Fabric module</span></span>
* <span data-ttu-id="dc563-2960">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="dc563-2960">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="dc563-2961">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="dc563-2961">Add support for CDN commands</span></span>
* <span data-ttu-id="dc563-2962">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="dc563-2962">Remove Container module</span></span>
* <span data-ttu-id="dc563-2963">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="dc563-2963">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="dc563-2964">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="dc563-2964">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="dc563-2965">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-2965">Core</span></span>

* <span data-ttu-id="dc563-2966">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="dc563-2966">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="dc563-2967">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([#2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="dc563-2967">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="dc563-2968">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="dc563-2968">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="dc563-2969">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="dc563-2969">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="dc563-2970">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="dc563-2970">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="dc563-2971">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="dc563-2971">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="dc563-2972">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="dc563-2972">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="dc563-2973">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="dc563-2973">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="dc563-2974">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="dc563-2974">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="dc563-2975">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="dc563-2975">core: Improved performance</span></span>
* <span data-ttu-id="dc563-2976">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="dc563-2976">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="dc563-2977">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="dc563-2977">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-2978">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-2978">ACS</span></span>

* <span data-ttu-id="dc563-2979">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="dc563-2979">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="dc563-2980">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="dc563-2980">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="dc563-2981">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="dc563-2981">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="dc563-2982">Удален профиль Windows перед вызовом метода PUT для команды scale ([#2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="dc563-2982">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-2983">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-2983">AppService</span></span>

* <span data-ttu-id="dc563-2984">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="dc563-2984">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="dc563-2985">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="dc563-2985">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="dc563-2986">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="dc563-2986">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="dc563-2987">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="dc563-2987">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="dc563-2988">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="dc563-2988">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="dc563-2989">Включена поддержка настройки строк подключения ([#2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="dc563-2989">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="dc563-2990">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="dc563-2990">support slot swap with preview</span></span>
* <span data-ttu-id="dc563-2991">Устранены ошибки из команд службы приложений ([#2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="dc563-2991">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="dc563-2992">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([#2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="dc563-2992">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="dc563-2993">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="dc563-2993">CosmosDB</span></span>

* <span data-ttu-id="dc563-2994">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="dc563-2994">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="dc563-2995">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="dc563-2995">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="dc563-2996">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="dc563-2996">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="dc563-2997">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="dc563-2997">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="dc563-2998">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="dc563-2998">Data Lake Analytics</span></span>

* <span data-ttu-id="dc563-2999">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="dc563-2999">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="dc563-3000">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="dc563-3000">Add support for new catalog item type: package.</span></span> <span data-ttu-id="dc563-3001">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="dc563-3001">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="dc563-3002">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="dc563-3002">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="dc563-3003">Таблица</span><span class="sxs-lookup"><span data-stu-id="dc563-3003">Table</span></span>
  * <span data-ttu-id="dc563-3004">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="dc563-3004">Table valued function</span></span>
  * <span data-ttu-id="dc563-3005">Представление</span><span class="sxs-lookup"><span data-stu-id="dc563-3005">View</span></span>
  * <span data-ttu-id="dc563-3006">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="dc563-3006">Table Statistics.</span></span> <span data-ttu-id="dc563-3007">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="dc563-3007">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="dc563-3008">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="dc563-3008">Data Lake Store</span></span>

* <span data-ttu-id="dc563-3009">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="dc563-3009">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="dc563-3010">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3010">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="dc563-3011">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="dc563-3011">missed help for access show.</span></span> <span data-ttu-id="dc563-3012">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="dc563-3012">adding it.</span></span> <span data-ttu-id="dc563-3013">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="dc563-3013">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="dc563-3014">Поиск</span><span class="sxs-lookup"><span data-stu-id="dc563-3014">Find</span></span>

* <span data-ttu-id="dc563-3015">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="dc563-3015">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="dc563-3016">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="dc563-3016">KeyVault</span></span>

* <span data-ttu-id="dc563-3017">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="dc563-3017">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="dc563-3018">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="dc563-3018">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="dc563-3019">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="dc563-3019">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="dc563-3020">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="dc563-3020">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="dc563-3021">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3021">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="dc563-3022">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="dc563-3022">Lab</span></span>

* <span data-ttu-id="dc563-3023">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="dc563-3023">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="dc563-3024">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="dc563-3024">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="dc563-3025">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="dc563-3025">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="dc563-3026">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="dc563-3026">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="dc563-3027">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="dc563-3027">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="dc563-3028">Монитор</span><span class="sxs-lookup"><span data-stu-id="dc563-3028">Monitor</span></span>

* <span data-ttu-id="dc563-3029">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3029">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="dc563-3030">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3030">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="dc563-3031">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-3031">Network</span></span>

* <span data-ttu-id="dc563-3032">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="dc563-3032">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="dc563-3033">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-3033">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="dc563-3034">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="dc563-3034">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="dc563-3035">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="dc563-3035">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="dc563-3036">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="dc563-3036">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="dc563-3037">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="dc563-3037">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="dc563-3038">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="dc563-3038">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="dc563-3039">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="dc563-3039">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="dc563-3040">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="dc563-3040">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="dc563-3041">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="dc563-3041">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="dc563-3042">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="dc563-3042">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="dc563-3043">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-3043">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="dc563-3044">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="dc563-3044">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="dc563-3045">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="dc563-3045">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="dc563-3046">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="dc563-3046">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="dc563-3047">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="dc563-3047">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="dc563-3048">Профиль</span><span class="sxs-lookup"><span data-stu-id="dc563-3048">Profile</span></span>

* <span data-ttu-id="dc563-3049">Включена поддержка входа при отсутствии подписок ([#2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3049">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="dc563-3050">Включена поддержка сокращенных имен параметров в команде az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3050">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="dc563-3051">Redis</span><span class="sxs-lookup"><span data-stu-id="dc563-3051">Redis</span></span>

* <span data-ttu-id="dc563-3052">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="dc563-3052">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="dc563-3053">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="dc563-3053">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="dc563-3054">Ресурс</span><span class="sxs-lookup"><span data-stu-id="dc563-3054">Resource</span></span>

* <span data-ttu-id="dc563-3055">Добавлены команды определения managedapp и managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3055">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="dc563-3056">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3056">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="dc563-3057">Включена поддержка создания универсального ресурса ([#2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3057">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="dc563-3058">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="dc563-3058">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="dc563-3059">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="dc563-3059">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="dc563-3060">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="dc563-3060">Add docs for az lock update.</span></span> <span data-ttu-id="dc563-3061">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="dc563-3061">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="dc563-3062">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="dc563-3062">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="dc563-3063">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="dc563-3063">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="dc563-3064">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="dc563-3064">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="dc563-3065">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="dc563-3065">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="dc563-3066">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([#2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3066">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="dc563-3067">Роль</span><span class="sxs-lookup"><span data-stu-id="dc563-3067">Role</span></span>

* <span data-ttu-id="dc563-3068">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([#2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3068">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="dc563-3069">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3069">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="dc563-3070">Роль: устранены проблемы при обновлении определения роли ([#2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3070">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="dc563-3071">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="dc563-3071">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="dc563-3072">SQL</span><span class="sxs-lookup"><span data-stu-id="dc563-3072">SQL</span></span>

* <span data-ttu-id="dc563-3073">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="dc563-3073">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="dc563-3074">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3074">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="dc563-3075">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-3075">Storage</span></span>

* <span data-ttu-id="dc563-3076">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="dc563-3076">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="dc563-3077">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="dc563-3077">Add support for incremental blob copy</span></span>
* <span data-ttu-id="dc563-3078">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="dc563-3078">Add support for large block blob upload</span></span>
* <span data-ttu-id="dc563-3079">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="dc563-3079">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-3080">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-3080">VM</span></span>

* <span data-ttu-id="dc563-3081">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="dc563-3081">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="dc563-3082">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="dc563-3082">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="dc563-3083">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="dc563-3083">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="dc563-3084">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="dc563-3084">az vm/vmss disk</span></span>
  3. <span data-ttu-id="dc563-3085">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="dc563-3085">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="dc563-3086">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="dc563-3086">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="dc563-3087">vm/vmss: добавлена поддержка создания из образа Marketplace, для которого требуются сведения о плане ([#1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3087">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="dc563-3088">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-3088">April 3, 2017</span></span>

<span data-ttu-id="dc563-3089">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="dc563-3089">Version 2.0.2</span></span>

<span data-ttu-id="dc563-3090">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="dc563-3090">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="dc563-3091">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="dc563-3091">Core</span></span>

* <span data-ttu-id="dc563-3092">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-3092">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="dc563-3093">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3093">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="dc563-3094">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3094">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="dc563-3095">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3095">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="dc563-3096">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3096">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="dc563-3097">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="dc563-3097">Add prompting for missing template parameters.</span></span> <span data-ttu-id="dc563-3098">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3098">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="dc563-3099">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="dc563-3099">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="dc563-3100">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="dc563-3100">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="dc563-3101">ACS</span><span class="sxs-lookup"><span data-stu-id="dc563-3101">ACS</span></span>

* <span data-ttu-id="dc563-3102">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3102">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="dc563-3103">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="dc563-3103">Add support for ssh key password prompting.</span></span> <span data-ttu-id="dc563-3104">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3104">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="dc563-3105">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="dc563-3105">Add support for windows clusters.</span></span> <span data-ttu-id="dc563-3106">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3106">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="dc563-3107">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="dc563-3107">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="dc563-3108">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3108">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="dc563-3109">AppService</span><span class="sxs-lookup"><span data-stu-id="dc563-3109">AppService</span></span>

* <span data-ttu-id="dc563-3110">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3110">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="dc563-3111">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3111">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="dc563-3112">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3112">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="dc563-3113">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3113">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="dc563-3114">Data Lake</span><span class="sxs-lookup"><span data-stu-id="dc563-3114">DataLake</span></span>

* <span data-ttu-id="dc563-3115">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="dc563-3115">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="dc563-3116">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="dc563-3116">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="dc563-3117">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="dc563-3117">DocuemntDB</span></span>

* <span data-ttu-id="dc563-3118">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3118">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="dc563-3119">ВМ</span><span class="sxs-lookup"><span data-stu-id="dc563-3119">VM</span></span>

* <span data-ttu-id="dc563-3120">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3120">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="dc563-3121">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3121">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="dc563-3122">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3122">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="dc563-3123">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3123">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="dc563-3124">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3124">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="dc563-3125">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3125">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="dc563-3126">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="dc563-3126">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="dc563-3127">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="dc563-3127">February 27, 2017</span></span>

<span data-ttu-id="dc563-3128">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="dc563-3128">Version 2.0.0</span></span>

<span data-ttu-id="dc563-3129">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="dc563-3129">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="dc563-3130">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="dc563-3130">Container Service (acs)</span></span>
- <span data-ttu-id="dc563-3131">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="dc563-3131">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="dc563-3132">Сеть</span><span class="sxs-lookup"><span data-stu-id="dc563-3132">Networking</span></span>
- <span data-ttu-id="dc563-3133">Память</span><span class="sxs-lookup"><span data-stu-id="dc563-3133">Storage</span></span>

<span data-ttu-id="dc563-3134">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="dc563-3134">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="dc563-3135">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="dc563-3135">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="dc563-3136">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="dc563-3136">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="dc563-3137">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="dc563-3137">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="dc563-3138">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="dc563-3138">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="dc563-3139">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="dc563-3139">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="dc563-3140">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="dc563-3140">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="dc563-3141">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="dc563-3141">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="dc563-3142">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="dc563-3142">Provide feedback from the command line with the `az feedback` command</span></span>

