---
title: Заметки о выпуске Azure CLI 2.0
description: Узнайте о последних обновлениях в Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/21/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: f6dd04e088651527b1ac13e719b7fc3c5522b310
ms.sourcegitcommit: d93b0a2bcfb0d164ef90d6d4618f0552609a8ea6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/20/2018
ms.locfileid: "46470071"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="c4228-103">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="c4228-103">Azure CLI 2.0 release notes</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="c4228-104">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-104">September 21, 2018</span></span>

<span data-ttu-id="c4228-105">Версия 20.46</span><span class="sxs-lookup"><span data-stu-id="c4228-105">Version 20.46</span></span>

### <a name="acr"></a><span data-ttu-id="c4228-106">ACR</span><span class="sxs-lookup"><span data-stu-id="c4228-106">ACR</span></span>
* <span data-ttu-id="c4228-107">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="c4228-107">Added ACR Task commands</span></span>
* <span data-ttu-id="c4228-108">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="c4228-108">Added quick run command</span></span>
* <span data-ttu-id="c4228-109">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="c4228-109">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="c4228-110">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="c4228-110">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="c4228-111">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="c4228-111">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="c4228-112">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="c4228-112">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-113">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-113">ACS</span></span>
* <span data-ttu-id="c4228-114">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="c4228-114">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="c4228-115">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="c4228-115">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-116">AppService</span><span class="sxs-lookup"><span data-stu-id="c4228-116">AppService</span></span>

* <span data-ttu-id="c4228-117">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="c4228-117">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="c4228-118">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="c4228-118">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="c4228-119">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="c4228-119">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="c4228-120">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="c4228-120">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="c4228-121">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="c4228-121">Batch</span></span>
* <span data-ttu-id="c4228-122">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="c4228-122">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="c4228-123">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="c4228-123">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="c4228-124">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-124">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="c4228-125">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="c4228-125">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c4228-126">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="c4228-126">Batch AI</span></span> 
* <span data-ttu-id="c4228-127">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-127">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c4228-128">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c4228-128">Cognitive Services</span></span>
* <span data-ttu-id="c4228-129">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="c4228-129">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="c4228-130">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="c4228-130">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="c4228-131">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="c4228-131">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="c4228-132">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="c4228-132">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="c4228-133">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="c4228-133">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="c4228-134">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="c4228-134">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="c4228-135">Контейнер</span><span class="sxs-lookup"><span data-stu-id="c4228-135">Container</span></span>
* <span data-ttu-id="c4228-136">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="c4228-136">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="c4228-137">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="c4228-137">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="c4228-138">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="c4228-138">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="c4228-139">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="c4228-139">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="c4228-140">Data Lake</span><span class="sxs-lookup"><span data-stu-id="c4228-140">Datalake</span></span>
* <span data-ttu-id="c4228-141">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="c4228-141">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="c4228-142">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="c4228-142">Interactive Shell</span></span>
* <span data-ttu-id="c4228-143">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="c4228-143">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="c4228-144">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="c4228-144">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="c4228-145">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="c4228-145">IoT</span></span>
* <span data-ttu-id="c4228-146">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="c4228-146">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="c4228-147">Key Vault</span><span class="sxs-lookup"><span data-stu-id="c4228-147">Key Vault</span></span>
* <span data-ttu-id="c4228-148">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="c4228-148">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="c4228-149">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-149">Network</span></span>
* <span data-ttu-id="c4228-150">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="c4228-150">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="c4228-151">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="c4228-151">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="c4228-152">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="c4228-152">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="c4228-153">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="c4228-153">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="c4228-154">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-154">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="c4228-155">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-155">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="c4228-156">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="c4228-156">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="c4228-157">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="c4228-157">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="c4228-158">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="c4228-158">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="c4228-159">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="c4228-159">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="c4228-160">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="c4228-160">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="c4228-161">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="c4228-161">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="c4228-162">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры`--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="c4228-162">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="c4228-163">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="c4228-163">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="c4228-164">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="c4228-164">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="c4228-165">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="c4228-165">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="c4228-166">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="c4228-166">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="c4228-167">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="c4228-167">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="c4228-168">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="c4228-168">RDBMS</span></span>
* <span data-ttu-id="c4228-169">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="c4228-169">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="c4228-170">резервирование.</span><span class="sxs-lookup"><span data-stu-id="c4228-170">Reservation</span></span>
* <span data-ttu-id="c4228-171">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c4228-171">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="c4228-172">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="c4228-172">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="c4228-173">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="c4228-173">Manage App</span></span>
* <span data-ttu-id="c4228-174">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="c4228-174">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="c4228-175">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="c4228-175">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="c4228-176">Роль</span><span class="sxs-lookup"><span data-stu-id="c4228-176">Role</span></span>
* <span data-ttu-id="c4228-177">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="c4228-177">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="c4228-178">SignalR</span><span class="sxs-lookup"><span data-stu-id="c4228-178">SignalR</span></span>
* <span data-ttu-id="c4228-179">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="c4228-179">First release</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-180">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-180">Storage</span></span>
* <span data-ttu-id="c4228-181">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="c4228-181">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="c4228-182">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="c4228-182">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-183">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-183">VM</span></span>
* <span data-ttu-id="c4228-184">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="c4228-184">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="c4228-185">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="c4228-185">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="c4228-186">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-186">August 28, 2018</span></span>

<span data-ttu-id="c4228-187">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="c4228-187">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="c4228-188">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-188">Core</span></span>

* <span data-ttu-id="c4228-189">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="c4228-189">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="c4228-190">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="c4228-190">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="c4228-191">ACR</span><span class="sxs-lookup"><span data-stu-id="c4228-191">ACR</span></span>

* <span data-ttu-id="c4228-192">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="c4228-192">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="c4228-193">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="c4228-193">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-194">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-194">ACS</span></span>

* <span data-ttu-id="c4228-195">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="c4228-195">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="c4228-196">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="c4228-196">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-197">AppService</span><span class="sxs-lookup"><span data-stu-id="c4228-197">AppService</span></span>

* <span data-ttu-id="c4228-198">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="c4228-198">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="c4228-199">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="c4228-199">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="c4228-200">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="c4228-200">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="c4228-201">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="c4228-201">Backup</span></span>

* <span data-ttu-id="c4228-202">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="c4228-202">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="c4228-203">Служба Bot Service</span><span class="sxs-lookup"><span data-stu-id="c4228-203">Bot Service</span></span>

* <span data-ttu-id="c4228-204">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="c4228-204">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c4228-205">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c4228-205">Cognitive Services</span></span>

* <span data-ttu-id="c4228-206">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="c4228-206">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="c4228-207">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="c4228-207">IoT</span></span>

* <span data-ttu-id="c4228-208">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="c4228-208">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="c4228-209">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="c4228-209">Monitor</span></span>

* <span data-ttu-id="c4228-210">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="c4228-210">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="c4228-211">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="c4228-211">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="c4228-212">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-212">Network</span></span>

* <span data-ttu-id="c4228-213">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="c4228-213">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="c4228-214">Ресурс</span><span class="sxs-lookup"><span data-stu-id="c4228-214">Resource</span></span>

* <span data-ttu-id="c4228-215">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="c4228-215">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-216">Хранилище</span><span class="sxs-lookup"><span data-stu-id="c4228-216">Storage</span></span>

* <span data-ttu-id="c4228-217">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="c4228-217">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-218">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-218">VM</span></span>

* <span data-ttu-id="c4228-219">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="c4228-219">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="c4228-220">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-220">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="c4228-221">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-221">Auguest 14, 2018</span></span>

<span data-ttu-id="c4228-222">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="c4228-222">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="c4228-223">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-223">Core</span></span>

* <span data-ttu-id="c4228-224">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="c4228-224">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="c4228-225">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="c4228-225">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="c4228-226">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="c4228-226">Telemetry</span></span>

* <span data-ttu-id="c4228-227">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="c4228-227">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="c4228-228">ACR</span><span class="sxs-lookup"><span data-stu-id="c4228-228">ACR</span></span>

* <span data-ttu-id="c4228-229">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="c4228-229">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="c4228-230">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="c4228-230">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-231">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-231">ACS</span></span>

* <span data-ttu-id="c4228-232">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="c4228-232">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="c4228-233">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="c4228-233">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="c4228-234">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="c4228-234">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="c4228-235">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="c4228-235">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="c4228-236">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="c4228-236">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="c4228-237">AppService</span><span class="sxs-lookup"><span data-stu-id="c4228-237">AppService</span></span>

* <span data-ttu-id="c4228-238">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c4228-238">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="c4228-239">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="c4228-239">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="c4228-240">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c4228-240">BatchAI</span></span>

* <span data-ttu-id="c4228-241">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="c4228-241">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="c4228-242">Контейнер</span><span class="sxs-lookup"><span data-stu-id="c4228-242">Container</span></span>

* <span data-ttu-id="c4228-243">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="c4228-243">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="c4228-244">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="c4228-244">IoT</span></span>

* <span data-ttu-id="c4228-245">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="c4228-245">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="c4228-246">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="c4228-246">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="c4228-247">IoT Central</span><span class="sxs-lookup"><span data-stu-id="c4228-247">Iot Central</span></span>

* <span data-ttu-id="c4228-248">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="c4228-248">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="c4228-249">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="c4228-249">KeyVault</span></span>


* <span data-ttu-id="c4228-250">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="c4228-250">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="c4228-251">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="c4228-251">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="c4228-252">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="c4228-252">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="c4228-253">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="c4228-253">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="c4228-254">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="c4228-254">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="c4228-255">Передача</span><span class="sxs-lookup"><span data-stu-id="c4228-255">Relay</span></span>

* <span data-ttu-id="c4228-256">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="c4228-256">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="c4228-257">SQL</span><span class="sxs-lookup"><span data-stu-id="c4228-257">Sql</span></span>

* <span data-ttu-id="c4228-258">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="c4228-258">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-259">Хранилище</span><span class="sxs-lookup"><span data-stu-id="c4228-259">Storage</span></span>

* <span data-ttu-id="c4228-260">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="c4228-260">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="c4228-261">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="c4228-261">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="c4228-262">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="c4228-262">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="c4228-263">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="c4228-263">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="c4228-264">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="c4228-264">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-265">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-265">VM</span></span>

* <span data-ttu-id="c4228-266">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="c4228-266">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="c4228-267">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-267">July 31, 2018</span></span>

<span data-ttu-id="c4228-268">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="c4228-268">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="c4228-269">ACR</span><span class="sxs-lookup"><span data-stu-id="c4228-269">ACR</span></span>

* <span data-ttu-id="c4228-270">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="c4228-270">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="c4228-271">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="c4228-271">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-272">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-272">ACS</span></span>

* <span data-ttu-id="c4228-273">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="c4228-273">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="c4228-274">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="c4228-274">Batch</span></span>

* <span data-ttu-id="c4228-275">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="c4228-275">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="c4228-276">Контейнер</span><span class="sxs-lookup"><span data-stu-id="c4228-276">Container</span></span>

* <span data-ttu-id="c4228-277">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="c4228-277">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="c4228-278">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-278">Network</span></span>

* <span data-ttu-id="c4228-279">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="c4228-279">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="c4228-280">Ресурс</span><span class="sxs-lookup"><span data-stu-id="c4228-280">Resource</span></span>

* <span data-ttu-id="c4228-281">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="c4228-281">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="c4228-282">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="c4228-282">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="c4228-283">Роль</span><span class="sxs-lookup"><span data-stu-id="c4228-283">Role</span></span>

* <span data-ttu-id="c4228-284">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="c4228-284">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="c4228-285">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="c4228-285">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="c4228-286">поиска</span><span class="sxs-lookup"><span data-stu-id="c4228-286">Search</span></span>

* <span data-ttu-id="c4228-287">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="c4228-287">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="c4228-288">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="c4228-288">Service Bus</span></span>

* <span data-ttu-id="c4228-289">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="c4228-289">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="c4228-290">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="c4228-290">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="c4228-291">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="c4228-291">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="c4228-292">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="c4228-292">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-293">Хранилище</span><span class="sxs-lookup"><span data-stu-id="c4228-293">Storage</span></span>

* <span data-ttu-id="c4228-294">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="c4228-294">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="c4228-295">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="c4228-295">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-296">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-296">VM</span></span>

* <span data-ttu-id="c4228-297">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="c4228-297">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="c4228-298">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="c4228-298">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="c4228-299">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="c4228-299">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="c4228-300">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="c4228-300">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="c4228-301">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-301">July 18, 2018</span></span>

<span data-ttu-id="c4228-302">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="c4228-302">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="c4228-303">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-303">Core</span></span>

* <span data-ttu-id="c4228-304">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="c4228-304">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="c4228-305">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="c4228-305">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="c4228-306">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="c4228-306">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="c4228-307">ACR</span><span class="sxs-lookup"><span data-stu-id="c4228-307">ACR</span></span>

* <span data-ttu-id="c4228-308">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="c4228-308">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="c4228-309">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-309">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="c4228-310">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="c4228-310">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="c4228-311">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="c4228-311">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-312">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-312">ACS</span></span>

* <span data-ttu-id="c4228-313">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="c4228-313">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-314">AppService</span><span class="sxs-lookup"><span data-stu-id="c4228-314">AppService</span></span>

* <span data-ttu-id="c4228-315">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="c4228-315">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="c4228-316">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="c4228-316">Batch</span></span>

* <span data-ttu-id="c4228-317">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="c4228-317">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="c4228-318">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="c4228-318">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c4228-319">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="c4228-319">Batch AI</span></span>

* <span data-ttu-id="c4228-320">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="c4228-320">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="c4228-321">Контейнер</span><span class="sxs-lookup"><span data-stu-id="c4228-321">Container</span></span>

* <span data-ttu-id="c4228-322">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="c4228-322">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="c4228-323">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="c4228-323">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="c4228-324">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-324">Network</span></span>

* <span data-ttu-id="c4228-325">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="c4228-325">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="c4228-326">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="c4228-326">Added `network nic wait`</span></span>
* <span data-ttu-id="c4228-327">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="c4228-327">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="c4228-328">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="c4228-328">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="c4228-329">Ресурс</span><span class="sxs-lookup"><span data-stu-id="c4228-329">Resource</span></span>

* <span data-ttu-id="c4228-330">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="c4228-330">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="c4228-331">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="c4228-331">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="c4228-332">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="c4228-332">Added `deployment wait` command</span></span>
* <span data-ttu-id="c4228-333">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="c4228-333">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="c4228-334">SQL</span><span class="sxs-lookup"><span data-stu-id="c4228-334">SQL</span></span>

* <span data-ttu-id="c4228-335">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-335">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="c4228-336">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="c4228-336">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="c4228-337">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="c4228-337">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-338">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-338">Storage</span></span>

* <span data-ttu-id="c4228-339">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="c4228-339">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-340">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-340">VM</span></span>

* <span data-ttu-id="c4228-341">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c4228-341">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="c4228-342">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-342">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="c4228-343">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="c4228-343">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="c4228-344">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-344">July 3, 2018</span></span>

<span data-ttu-id="c4228-345">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="c4228-345">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="c4228-346">AKS</span><span class="sxs-lookup"><span data-stu-id="c4228-346">AKS</span></span>

* <span data-ttu-id="c4228-347">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="c4228-347">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="c4228-348">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-348">July 3, 2018</span></span>

<span data-ttu-id="c4228-349">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="c4228-349">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="c4228-350">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-350">Core</span></span>

* <span data-ttu-id="c4228-351">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="c4228-351">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="c4228-352">ACR</span><span class="sxs-lookup"><span data-stu-id="c4228-352">ACR</span></span>

* <span data-ttu-id="c4228-353">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="c4228-353">Added polling build status</span></span>
* <span data-ttu-id="c4228-354">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="c4228-354">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="c4228-355">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="c4228-355">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-356">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-356">ACS</span></span>

* <span data-ttu-id="c4228-357">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c4228-357">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="c4228-358">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c4228-358">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="c4228-359">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="c4228-359">Updated options for `aks browse` command.</span></span> <span data-ttu-id="c4228-360">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="c4228-360">Added `--listen-port` support</span></span>
* <span data-ttu-id="c4228-361">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="c4228-361">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="c4228-362">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="c4228-362">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="c4228-363">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="c4228-363">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-364">AppService</span><span class="sxs-lookup"><span data-stu-id="c4228-364">AppService</span></span>

* <span data-ttu-id="c4228-365">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="c4228-365">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="c4228-366">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="c4228-366">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="c4228-367">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="c4228-367">Backup</span></span>

* <span data-ttu-id="c4228-368">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="c4228-368">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="c4228-369">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c4228-369">BatchAI</span></span>

* <span data-ttu-id="c4228-370">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="c4228-370">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="c4228-371">Облако</span><span class="sxs-lookup"><span data-stu-id="c4228-371">Cloud</span></span>

* <span data-ttu-id="c4228-372">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="c4228-372">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="c4228-373">Контейнер</span><span class="sxs-lookup"><span data-stu-id="c4228-373">Container</span></span>

* <span data-ttu-id="c4228-374">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="c4228-374">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="c4228-375">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="c4228-375">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="c4228-376">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="c4228-376">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="c4228-377">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="c4228-377">Extension</span></span>

* <span data-ttu-id="c4228-378">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="c4228-378">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="c4228-379">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-379">Network</span></span>

* <span data-ttu-id="c4228-380">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="c4228-380">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="c4228-381">Rdbms</span><span class="sxs-lookup"><span data-stu-id="c4228-381">Rdbms</span></span>

* <span data-ttu-id="c4228-382">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="c4228-382">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="c4228-383">Ресурс</span><span class="sxs-lookup"><span data-stu-id="c4228-383">Resource</span></span>

* <span data-ttu-id="c4228-384">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="c4228-384">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-385">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-385">VM</span></span>

* <span data-ttu-id="c4228-386">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="c4228-386">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="c4228-387">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-387">June 25, 2018</span></span>

<span data-ttu-id="c4228-388">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="c4228-388">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="c4228-389">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="c4228-389">CLI</span></span>

* <span data-ttu-id="c4228-390">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="c4228-390">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="c4228-391">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-391">June 19, 2018</span></span>

<span data-ttu-id="c4228-392">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="c4228-392">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="c4228-393">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-393">Core</span></span>

* <span data-ttu-id="c4228-394">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="c4228-394">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="c4228-395">ACR</span><span class="sxs-lookup"><span data-stu-id="c4228-395">ACR</span></span>

* <span data-ttu-id="c4228-396">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="c4228-396">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="c4228-397">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="c4228-397">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-398">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-398">ACS</span></span>

* <span data-ttu-id="c4228-399">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="c4228-399">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="c4228-400">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-400">Added `--update` support</span></span>
* <span data-ttu-id="c4228-401">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="c4228-401">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="c4228-402">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="c4228-402">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="c4228-403">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="c4228-403">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="c4228-404">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="c4228-404">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="c4228-405">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="c4228-405">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="c4228-406">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="c4228-406">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-407">AppService</span><span class="sxs-lookup"><span data-stu-id="c4228-407">AppService</span></span>

* <span data-ttu-id="c4228-408">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="c4228-408">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="c4228-409">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c4228-409">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="c4228-410">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="c4228-410">Batch</span></span>

* <span data-ttu-id="c4228-411">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="c4228-411">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c4228-412">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="c4228-412">Batch AI</span></span>

* <span data-ttu-id="c4228-413">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="c4228-413">Added support for workspaces.</span></span> <span data-ttu-id="c4228-414">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c4228-414">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="c4228-415">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="c4228-415">Added support for experiments.</span></span> <span data-ttu-id="c4228-416">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="c4228-416">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="c4228-417">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="c4228-417">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="c4228-418">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="c4228-418">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="c4228-419">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="c4228-419">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="c4228-420">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="c4228-420">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="c4228-421">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="c4228-421">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="c4228-422">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="c4228-422">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="c4228-423">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-423">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="c4228-424">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="c4228-424">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="c4228-425">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-425">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="c4228-426">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="c4228-426">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="c4228-427">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="c4228-427">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="c4228-428">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="c4228-428">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="c4228-429">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-429">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="c4228-430">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="c4228-430">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="c4228-431">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="c4228-431">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="c4228-432">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="c4228-432">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="c4228-433">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="c4228-433">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="c4228-434">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="c4228-434">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="c4228-435">Карты</span><span class="sxs-lookup"><span data-stu-id="c4228-435">Maps</span></span>

* <span data-ttu-id="c4228-436">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="c4228-436">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="c4228-437">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-437">Network</span></span>

* <span data-ttu-id="c4228-438">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="c4228-438">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="c4228-439">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="c4228-439">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="c4228-440">#6502</span><span class="sxs-lookup"><span data-stu-id="c4228-440">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="c4228-441">Резервирование</span><span class="sxs-lookup"><span data-stu-id="c4228-441">Reservations</span></span>

* <span data-ttu-id="c4228-442">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="c4228-442">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="c4228-443">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="c4228-443">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="c4228-444">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="c4228-444">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="c4228-445">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="c4228-445">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="c4228-446">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="c4228-446">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="c4228-447">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-447">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="c4228-448">Роль</span><span class="sxs-lookup"><span data-stu-id="c4228-448">Role</span></span>

* <span data-ttu-id="c4228-449">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="c4228-449">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="c4228-450">SQL</span><span class="sxs-lookup"><span data-stu-id="c4228-450">SQL</span></span>

* <span data-ttu-id="c4228-451">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="c4228-451">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-452">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-452">Storage</span></span>

* <span data-ttu-id="c4228-453">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="c4228-453">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-454">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-454">VM</span></span>

* <span data-ttu-id="c4228-455">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-455">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="c4228-456">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="c4228-456">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="c4228-457">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="c4228-457">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="c4228-458">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-458">June 13, 2018</span></span>

<span data-ttu-id="c4228-459">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="c4228-459">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="c4228-460">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-460">Core</span></span>

* <span data-ttu-id="c4228-461">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="c4228-461">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="c4228-462">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-462">June 13, 2018</span></span>

<span data-ttu-id="c4228-463">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="c4228-463">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="c4228-464">AKS</span><span class="sxs-lookup"><span data-stu-id="c4228-464">AKS</span></span>

* <span data-ttu-id="c4228-465">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="c4228-465">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="c4228-466">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="c4228-466">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="c4228-467">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="c4228-467">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="c4228-468">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="c4228-468">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="c4228-469">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c4228-469">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-470">AppService</span><span class="sxs-lookup"><span data-stu-id="c4228-470">AppService</span></span>

* <span data-ttu-id="c4228-471">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="c4228-471">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="c4228-472">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-472">June 5, 2018</span></span>

<span data-ttu-id="c4228-473">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="c4228-473">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="c4228-474">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4228-474">Interactive</span></span>

* <span data-ttu-id="c4228-475">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="c4228-475">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="c4228-476">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-476">June 5, 2018</span></span>

<span data-ttu-id="c4228-477">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="c4228-477">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="c4228-478">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-478">Core</span></span>

* <span data-ttu-id="c4228-479">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="c4228-479">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="c4228-480">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="c4228-480">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="c4228-481">ACR</span><span class="sxs-lookup"><span data-stu-id="c4228-481">ACR</span></span>

* <span data-ttu-id="c4228-482">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="c4228-482">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="c4228-483">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="c4228-483">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="c4228-484">AKS</span><span class="sxs-lookup"><span data-stu-id="c4228-484">AKS</span></span>

* <span data-ttu-id="c4228-485">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="c4228-485">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="c4228-486">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="c4228-486">Batch</span></span>

* <span data-ttu-id="c4228-487">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="c4228-487">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="c4228-488">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="c4228-488">IOT</span></span>

* <span data-ttu-id="c4228-489">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="c4228-489">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="c4228-490">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-490">Network</span></span>

* <span data-ttu-id="c4228-491">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="c4228-491">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="c4228-492">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="c4228-492">Policy Insights</span></span>

* <span data-ttu-id="c4228-493">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="c4228-493">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="c4228-494">ARM</span><span class="sxs-lookup"><span data-stu-id="c4228-494">ARM</span></span>

* <span data-ttu-id="c4228-495">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="c4228-495">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="c4228-496">SQL</span><span class="sxs-lookup"><span data-stu-id="c4228-496">SQL</span></span>

* <span data-ttu-id="c4228-497">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="c4228-497">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="c4228-498">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="c4228-498">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="c4228-499">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-499">Storage</span></span>

* <span data-ttu-id="c4228-500">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="c4228-500">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-501">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-501">VM</span></span>

* <span data-ttu-id="c4228-502">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="c4228-502">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="c4228-503">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-503">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="c4228-504">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-504">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="c4228-505">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-505">May 22, 2018</span></span>

<span data-ttu-id="c4228-506">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="c4228-506">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="c4228-507">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-507">Core</span></span>

* <span data-ttu-id="c4228-508">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="c4228-508">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-509">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-509">ACS</span></span>

* <span data-ttu-id="c4228-510">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="c4228-510">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="c4228-511">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="c4228-511">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-512">AppService</span><span class="sxs-lookup"><span data-stu-id="c4228-512">AppService</span></span>

* <span data-ttu-id="c4228-513">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="c4228-513">Improved generic update commands</span></span>
* <span data-ttu-id="c4228-514">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="c4228-514">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="c4228-515">Контейнер</span><span class="sxs-lookup"><span data-stu-id="c4228-515">Container</span></span>

* <span data-ttu-id="c4228-516">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="c4228-516">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="c4228-517">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="c4228-517">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="c4228-518">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="c4228-518">Extension</span></span>

* <span data-ttu-id="c4228-519">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="c4228-519">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="c4228-520">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4228-520">Interactive</span></span>

* <span data-ttu-id="c4228-521">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="c4228-521">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="c4228-522">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="c4228-522">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="c4228-523">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="c4228-523">KeyVault</span></span>

* <span data-ttu-id="c4228-524">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="c4228-524">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="c4228-525">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-525">Network</span></span>

* <span data-ttu-id="c4228-526">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="c4228-526">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="c4228-527">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="c4228-527">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="c4228-528">SQL</span><span class="sxs-lookup"><span data-stu-id="c4228-528">SQL</span></span>

* <span data-ttu-id="c4228-529">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="c4228-529">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="c4228-530">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="c4228-530">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="c4228-531">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="c4228-531">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="c4228-532">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="c4228-532">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="c4228-533">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="c4228-533">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="c4228-534">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="c4228-534">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="c4228-535">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="c4228-535">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="c4228-536">`edition`.</span><span class="sxs-lookup"><span data-stu-id="c4228-536">`edition`.</span></span> <span data-ttu-id="c4228-537">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="c4228-537">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="c4228-538">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="c4228-538">`elasticPoolName`.</span></span> <span data-ttu-id="c4228-539">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="c4228-539">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="c4228-540">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="c4228-540">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="c4228-541">`edition`.</span><span class="sxs-lookup"><span data-stu-id="c4228-541">`edition`.</span></span> <span data-ttu-id="c4228-542">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="c4228-542">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="c4228-543">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="c4228-543">`dtu`.</span></span> <span data-ttu-id="c4228-544">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="c4228-544">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="c4228-545">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="c4228-545">`databaseDtuMin`.</span></span> <span data-ttu-id="c4228-546">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="c4228-546">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="c4228-547">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="c4228-547">`databaseDtuMax`.</span></span> <span data-ttu-id="c4228-548">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="c4228-548">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="c4228-549">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="c4228-549">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="c4228-550">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="c4228-550">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-551">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-551">Storage</span></span>

* <span data-ttu-id="c4228-552">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="c4228-552">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="c4228-553">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="c4228-553">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-554">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-554">VM</span></span>

* <span data-ttu-id="c4228-555">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-555">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="c4228-556">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="c4228-556">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="c4228-557">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="c4228-557">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="c4228-558">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="c4228-558">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="c4228-559">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-559">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="c4228-560">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-560">May 7, 2018</span></span>

<span data-ttu-id="c4228-561">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="c4228-561">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="c4228-562">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-562">Core</span></span>

* <span data-ttu-id="c4228-563">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="c4228-563">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="c4228-564">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="c4228-564">Added limited support for positional arguments</span></span>
* <span data-ttu-id="c4228-565">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="c4228-565">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="c4228-566">#5591</span><span class="sxs-lookup"><span data-stu-id="c4228-566">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="c4228-567">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="c4228-567">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="c4228-568">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="c4228-568">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="c4228-569">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="c4228-569">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="c4228-570">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="c4228-570">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="c4228-571">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="c4228-571">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="c4228-572">ACR</span><span class="sxs-lookup"><span data-stu-id="c4228-572">ACR</span></span>

* <span data-ttu-id="c4228-573">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="c4228-573">Added ACR Build commands</span></span>
* <span data-ttu-id="c4228-574">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="c4228-574">Improved resource not found error messages</span></span>
* <span data-ttu-id="c4228-575">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="c4228-575">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="c4228-576">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="c4228-576">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="c4228-577">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="c4228-577">Improved repository commands error messages</span></span>
* <span data-ttu-id="c4228-578">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="c4228-578">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-579">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-579">ACS</span></span>

* <span data-ttu-id="c4228-580">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="c4228-580">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="c4228-581">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="c4228-581">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="c4228-582">AMS</span><span class="sxs-lookup"><span data-stu-id="c4228-582">AMS</span></span>

* <span data-ttu-id="c4228-583">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="c4228-583">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-584">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="c4228-584">Appservice</span></span>

* <span data-ttu-id="c4228-585">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="c4228-585">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="c4228-586">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-586">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="c4228-587">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="c4228-587">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="c4228-588">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="c4228-588">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="c4228-589">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="c4228-589">Batch AI</span></span>

* <span data-ttu-id="c4228-590">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="c4228-590">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c4228-591">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c4228-591">Cognitive Services</span></span>

* <span data-ttu-id="c4228-592">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="c4228-592">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="c4228-593">Потребление</span><span class="sxs-lookup"><span data-stu-id="c4228-593">Consumption</span></span>

* <span data-ttu-id="c4228-594">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="c4228-594">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="c4228-595">Контейнер</span><span class="sxs-lookup"><span data-stu-id="c4228-595">Container</span></span>

* <span data-ttu-id="c4228-596">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="c4228-596">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="c4228-597">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="c4228-597">Cosmos DB</span></span>

* <span data-ttu-id="c4228-598">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c4228-598">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="c4228-599">DMS</span><span class="sxs-lookup"><span data-stu-id="c4228-599">DMS</span></span>

* <span data-ttu-id="c4228-600">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="c4228-600">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="c4228-601">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="c4228-601">Extension</span></span>

* <span data-ttu-id="c4228-602">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="c4228-602">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="c4228-603">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4228-603">Interactive</span></span>

* <span data-ttu-id="c4228-604">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="c4228-604">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="c4228-605">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="c4228-605">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="c4228-606">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="c4228-606">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="c4228-607">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="c4228-607">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="c4228-608">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="c4228-608">Lab</span></span>

* <span data-ttu-id="c4228-609">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="c4228-609">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="c4228-610">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-610">Network</span></span>

* <span data-ttu-id="c4228-611">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="c4228-611">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="c4228-612">Профиль</span><span class="sxs-lookup"><span data-stu-id="c4228-612">Profile</span></span>

* <span data-ttu-id="c4228-613">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-613">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="c4228-614">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="c4228-614">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="c4228-615">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="c4228-615">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="c4228-616">Redis</span><span class="sxs-lookup"><span data-stu-id="c4228-616">Redis</span></span>

* <span data-ttu-id="c4228-617">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="c4228-617">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="c4228-618">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="c4228-618">Deprecated `redis list-all`.</span></span> <span data-ttu-id="c4228-619">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="c4228-619">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="c4228-620">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="c4228-620">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="c4228-621">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="c4228-621">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="c4228-622">Роль</span><span class="sxs-lookup"><span data-stu-id="c4228-622">Role</span></span>

* <span data-ttu-id="c4228-623">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="c4228-623">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-624">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-624">Storage</span></span>

* <span data-ttu-id="c4228-625">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="c4228-625">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="c4228-626">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="c4228-626">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="c4228-627">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="c4228-627">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="c4228-628">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="c4228-628">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="c4228-629">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="c4228-629">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-630">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-630">VM</span></span>

* <span data-ttu-id="c4228-631">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="c4228-631">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="c4228-632">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="c4228-632">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="c4228-633">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="c4228-633">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="c4228-634">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="c4228-634">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="c4228-635">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="c4228-635">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="c4228-636">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="c4228-636">Added write accelerator support</span></span>
* <span data-ttu-id="c4228-637">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="c4228-637">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="c4228-638">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="c4228-638">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="c4228-639">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="c4228-639">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="c4228-640">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-640">April 10, 2018</span></span>

<span data-ttu-id="c4228-641">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="c4228-641">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="c4228-642">ACR</span><span class="sxs-lookup"><span data-stu-id="c4228-642">ACR</span></span>

* <span data-ttu-id="c4228-643">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="c4228-643">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-644">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-644">ACS</span></span>

* <span data-ttu-id="c4228-645">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="c4228-645">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-646">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="c4228-646">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="c4228-648">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="c4228-648">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="c4228-649">Batch AI</span><span class="sxs-lookup"><span data-stu-id="c4228-649">BatchAI</span></span>

* <span data-ttu-id="c4228-650">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="c4228-650">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="c4228-651">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="c4228-651">Job level mounting</span></span>
 - <span data-ttu-id="c4228-652">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="c4228-652">Environment variables with secret values</span></span>
 - <span data-ttu-id="c4228-653">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="c4228-653">Performance counters settings</span></span>
 - <span data-ttu-id="c4228-654">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="c4228-654">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="c4228-655">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="c4228-655">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="c4228-656">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="c4228-656">Usage and limits reporting</span></span>
 - <span data-ttu-id="c4228-657">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="c4228-657">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="c4228-658">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="c4228-658">Support for custom images</span></span>
 - <span data-ttu-id="c4228-659">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="c4228-659">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="c4228-660">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="c4228-660">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="c4228-661">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="c4228-661">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="c4228-662">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="c4228-662">National clouds are supported</span></span>
* <span data-ttu-id="c4228-663">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="c4228-663">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="c4228-664">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="c4228-664">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="c4228-665">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="c4228-665">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="c4228-666">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="c4228-666">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="c4228-667">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="c4228-667">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="c4228-668">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="c4228-668">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="c4228-669">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="c4228-669">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="c4228-670">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="c4228-670">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="c4228-671">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="c4228-671">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="c4228-672">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-672">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="c4228-673">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="c4228-673">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="c4228-674">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="c4228-674">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="c4228-675">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-675">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="c4228-676">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="c4228-676">Billing</span></span>

* <span data-ttu-id="c4228-677">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="c4228-677">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="c4228-678">Потребление</span><span class="sxs-lookup"><span data-stu-id="c4228-678">Consumption</span></span>

* <span data-ttu-id="c4228-679">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="c4228-679">Added `marketplace` commands</span></span>
* <span data-ttu-id="c4228-680">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="c4228-680">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="c4228-681">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="c4228-681">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="c4228-682">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="c4228-682">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="c4228-683">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="c4228-683">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="c4228-684">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="c4228-684">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="c4228-685">Контейнер</span><span class="sxs-lookup"><span data-stu-id="c4228-685">Container</span></span>

* <span data-ttu-id="c4228-686">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="c4228-686">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="c4228-687">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="c4228-687">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="c4228-688">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="c4228-688">Extension</span></span>

* <span data-ttu-id="c4228-689">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="c4228-689">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="c4228-690">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4228-690">Interactive</span></span>

* <span data-ttu-id="c4228-691">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="c4228-691">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="c4228-692">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="c4228-692">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="c4228-693">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="c4228-693">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="c4228-694">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-694">Network</span></span>

* <span data-ttu-id="c4228-695">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-695">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="c4228-696">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-696">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="c4228-697">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="c4228-697">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="c4228-698">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="c4228-698">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="c4228-699">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="c4228-699">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="c4228-700">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-700">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="c4228-701">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-701">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="c4228-702">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="c4228-702">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="c4228-703">Профиль</span><span class="sxs-lookup"><span data-stu-id="c4228-703">Profile</span></span>

* <span data-ttu-id="c4228-704">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="c4228-704">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="c4228-705">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="c4228-705">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="c4228-706">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="c4228-706">RDBMS</span></span>

* <span data-ttu-id="c4228-707">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="c4228-707">Added `georestore` command</span></span>
* <span data-ttu-id="c4228-708">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-708">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="c4228-709">Ресурс</span><span class="sxs-lookup"><span data-stu-id="c4228-709">Resource</span></span>

* <span data-ttu-id="c4228-710">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-710">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="c4228-711">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-711">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="c4228-712">SQL</span><span class="sxs-lookup"><span data-stu-id="c4228-712">SQL</span></span>

* <span data-ttu-id="c4228-713">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="c4228-713">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-714">Хранилище</span><span class="sxs-lookup"><span data-stu-id="c4228-714">Storage</span></span>

* <span data-ttu-id="c4228-715">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="c4228-715">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-716">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-716">VM</span></span>

* <span data-ttu-id="c4228-717">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="c4228-717">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="c4228-718">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="c4228-718">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="c4228-720">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-720">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="c4228-721">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-721">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="c4228-722">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="c4228-722">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="c4228-723">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="c4228-723">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="c4228-724">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-724">March 27, 2018</span></span>

<span data-ttu-id="c4228-725">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="c4228-725">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="c4228-726">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-726">Core</span></span>

* <span data-ttu-id="c4228-727">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="c4228-727">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-728">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-728">ACS</span></span>

* <span data-ttu-id="c4228-729">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="c4228-729">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-730">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="c4228-730">Appservice</span></span>

* <span data-ttu-id="c4228-731">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-731">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="c4228-732">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-732">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="c4228-733">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="c4228-733">Backup</span></span>

* <span data-ttu-id="c4228-734">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="c4228-734">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="c4228-735">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="c4228-735">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="c4228-736">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="c4228-736">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="c4228-737">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="c4228-737">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="c4228-738">Контейнер</span><span class="sxs-lookup"><span data-stu-id="c4228-738">Container</span></span>

* <span data-ttu-id="c4228-739">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="c4228-739">Added `container exec` command.</span></span> <span data-ttu-id="c4228-740">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="c4228-740">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="c4228-741">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="c4228-741">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="c4228-742">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="c4228-742">Extension</span></span>

* <span data-ttu-id="c4228-743">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="c4228-743">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="c4228-744">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="c4228-744">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="c4228-745">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c4228-745">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="c4228-746">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4228-746">Interactive</span></span>

* <span data-ttu-id="c4228-747">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="c4228-747">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="c4228-748">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="c4228-748">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="c4228-749">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="c4228-749">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="c4228-750">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="c4228-750">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="c4228-751">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="c4228-751">Lab</span></span>

* <span data-ttu-id="c4228-752">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="c4228-752">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="c4228-753">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="c4228-753">Monitor</span></span>

* <span data-ttu-id="c4228-754">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="c4228-754">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="c4228-755">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="c4228-755">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="c4228-756">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="c4228-756">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="c4228-757">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-757">Network</span></span>

* <span data-ttu-id="c4228-758">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="c4228-758">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="c4228-759">Профиль</span><span class="sxs-lookup"><span data-stu-id="c4228-759">Profile</span></span>

* <span data-ttu-id="c4228-760">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="c4228-760">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="c4228-761">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="c4228-761">RDBMS</span></span>

* <span data-ttu-id="c4228-762">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="c4228-762">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="c4228-763">Ресурс</span><span class="sxs-lookup"><span data-stu-id="c4228-763">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="c4228-765">Роль</span><span class="sxs-lookup"><span data-stu-id="c4228-765">Role</span></span>

* <span data-ttu-id="c4228-766">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-766">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="c4228-767">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="c4228-767">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="c4228-768">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="c4228-768">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="c4228-769">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-769">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="c4228-770">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="c4228-770">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-771">Хранилище</span><span class="sxs-lookup"><span data-stu-id="c4228-771">Storage</span></span>

* <span data-ttu-id="c4228-772">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="c4228-772">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="c4228-773">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049): проблемы, когда при отправке добавочного большого двоичного объекта игнорируются параметры условия.</span><span class="sxs-lookup"><span data-stu-id="c4228-773">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-774">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-774">VM</span></span>

* <span data-ttu-id="c4228-775">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="c4228-775">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="c4228-776">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-776">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="c4228-777">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="c4228-777">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="c4228-778">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="c4228-778">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="c4228-779">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-779">March 13, 2018</span></span>

<span data-ttu-id="c4228-780">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="c4228-780">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="c4228-781">ACR</span><span class="sxs-lookup"><span data-stu-id="c4228-781">ACR</span></span>

* <span data-ttu-id="c4228-782">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="c4228-782">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="c4228-783">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="c4228-783">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="c4228-784">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="c4228-784">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-785">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-785">ACS</span></span>

* <span data-ttu-id="c4228-786">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="c4228-786">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="c4228-787">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="c4228-787">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="c4228-788">Помощник</span><span class="sxs-lookup"><span data-stu-id="c4228-788">Advisor</span></span>

* <span data-ttu-id="c4228-789">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="c4228-789">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="c4228-790">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-790">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="c4228-791">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="c4228-791">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="c4228-792">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="c4228-792">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="c4228-793">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="c4228-793">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-794">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="c4228-794">Appservice</span></span>

* <span data-ttu-id="c4228-795">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="c4228-795">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="c4228-796">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-796">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="c4228-797">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="c4228-797">Eventhubs</span></span>

* <span data-ttu-id="c4228-798">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="c4228-798">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="c4228-799">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="c4228-799">Extension</span></span>

* <span data-ttu-id="c4228-800">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="c4228-800">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="c4228-801">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4228-801">Interactive</span></span>

* <span data-ttu-id="c4228-802">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625): теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="c4228-802">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="c4228-803">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016): при использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="c4228-803">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="c4228-804">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688): если при загрузке таблицы команд возникало исключение, опережающий ввод не выполнялся.</span><span class="sxs-lookup"><span data-stu-id="c4228-804">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="c4228-805">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="c4228-805">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="c4228-806">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="c4228-806">Monitor</span></span>

* <span data-ttu-id="c4228-807">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="c4228-807">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="c4228-808">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="c4228-808">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="c4228-809">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="c4228-809">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="c4228-810">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="c4228-810">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="c4228-811">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-811">Network</span></span>

* <span data-ttu-id="c4228-812">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-812">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="c4228-813">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="c4228-813">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="c4228-814">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="c4228-814">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="c4228-815">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="c4228-815">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="c4228-816">Профиль</span><span class="sxs-lookup"><span data-stu-id="c4228-816">Profile</span></span>

* <span data-ttu-id="c4228-817">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="c4228-817">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="c4228-818">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="c4228-818">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="c4228-819">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="c4228-819">RDBMS</span></span>

* <span data-ttu-id="c4228-820">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="c4228-820">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="c4228-821">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="c4228-821">Service Bus</span></span>

* <span data-ttu-id="c4228-822">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="c4228-822">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-823">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-823">Storage</span></span>

* <span data-ttu-id="c4228-824">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="c4228-824">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="c4228-825">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286): при пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="c4228-825">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-826">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-826">VM</span></span>

* <span data-ttu-id="c4228-827">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="c4228-827">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="c4228-828">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="c4228-828">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="c4228-829">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-829">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="c4228-830">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="c4228-830">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="c4228-831">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="c4228-831">February 27, 2018</span></span>

<span data-ttu-id="c4228-832">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="c4228-832">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="c4228-833">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-833">Core</span></span>

* <span data-ttu-id="c4228-834">Исправлена ошибка с установкой Homebrew [#5184](https://github.com/Azure/azure-cli/issues/5184).</span><span class="sxs-lookup"><span data-stu-id="c4228-834">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="c4228-835">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="c4228-835">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="c4228-836">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="c4228-836">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-837">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-837">ACS</span></span>

* <span data-ttu-id="c4228-838">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c4228-838">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="c4228-839">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="c4228-839">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="c4228-840">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="c4228-840">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="c4228-841">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="c4228-841">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-842">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="c4228-842">Appservice</span></span>

* <span data-ttu-id="c4228-843">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="c4228-843">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="c4228-844">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="c4228-844">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="c4228-845">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="c4228-845">Cognitive Services</span></span>

* <span data-ttu-id="c4228-846">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="c4228-846">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="c4228-847">Потребление</span><span class="sxs-lookup"><span data-stu-id="c4228-847">Consumption</span></span>

* <span data-ttu-id="c4228-848">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="c4228-848">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="c4228-849">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="c4228-849">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="c4228-850">Контейнер</span><span class="sxs-lookup"><span data-stu-id="c4228-850">Container</span></span>

* <span data-ttu-id="c4228-851">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="c4228-851">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="c4228-852">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-852">Network</span></span>

* <span data-ttu-id="c4228-853">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559): отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="c4228-853">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="c4228-854">Ресурс</span><span class="sxs-lookup"><span data-stu-id="c4228-854">Resource</span></span>

* <span data-ttu-id="c4228-855">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="c4228-855">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="c4228-856">Роль</span><span class="sxs-lookup"><span data-stu-id="c4228-856">Role</span></span>

* <span data-ttu-id="c4228-857">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="c4228-857">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="c4228-858">SQL</span><span class="sxs-lookup"><span data-stu-id="c4228-858">SQL</span></span>

* <span data-ttu-id="c4228-859">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="c4228-859">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-860">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-860">Storage</span></span>

* <span data-ttu-id="c4228-861">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-861">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-862">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-862">VM</span></span>

* <span data-ttu-id="c4228-863">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="c4228-863">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="c4228-864">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-864">February 13, 2018</span></span>

<span data-ttu-id="c4228-865">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="c4228-865">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="c4228-866">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-866">Core</span></span>

* <span data-ttu-id="c4228-867">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="c4228-867">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-868">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-868">ACS</span></span>

* <span data-ttu-id="c4228-869">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="c4228-869">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="c4228-870">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-870">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="c4228-871">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="c4228-871">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="c4228-872">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="c4228-872">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="c4228-873">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="c4228-873">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="c4228-874">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="c4228-874">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="c4228-875">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="c4228-875">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="c4228-876">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="c4228-876">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-877">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="c4228-877">Appservice</span></span>

* <span data-ttu-id="c4228-878">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="c4228-878">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="c4228-879">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="c4228-879">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="c4228-880">CDN</span><span class="sxs-lookup"><span data-stu-id="c4228-880">CDN</span></span>

* <span data-ttu-id="c4228-881">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-881">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="c4228-882">Контейнер</span><span class="sxs-lookup"><span data-stu-id="c4228-882">Container</span></span>

* <span data-ttu-id="c4228-883">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="c4228-883">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="c4228-884">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="c4228-884">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c4228-885">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c4228-885">CosmosDB</span></span>

* <span data-ttu-id="c4228-886">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="c4228-886">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="c4228-887">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="c4228-887">Extension</span></span>

* <span data-ttu-id="c4228-888">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-888">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="c4228-889">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-889">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="c4228-890">Отзыв</span><span class="sxs-lookup"><span data-stu-id="c4228-890">Feedback</span></span>

* <span data-ttu-id="c4228-891">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="c4228-891">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="c4228-892">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4228-892">Interactive</span></span>

* <span data-ttu-id="c4228-893">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="c4228-893">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="c4228-894">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="c4228-894">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="c4228-895">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="c4228-895">IoT</span></span>

* <span data-ttu-id="c4228-896">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="c4228-896">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="c4228-897">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="c4228-897">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="c4228-898">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-898">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="c4228-899">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="c4228-899">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="c4228-900">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="c4228-900">Monitor</span></span>

* <span data-ttu-id="c4228-901">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-901">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="c4228-902">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-902">Network</span></span>

* <span data-ttu-id="c4228-903">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="c4228-903">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="c4228-904">Профиль</span><span class="sxs-lookup"><span data-stu-id="c4228-904">Profile</span></span>

* <span data-ttu-id="c4228-905">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="c4228-905">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="c4228-906">Ресурс</span><span class="sxs-lookup"><span data-stu-id="c4228-906">Resource</span></span>

* <span data-ttu-id="c4228-907">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="c4228-907">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="c4228-908">Роль</span><span class="sxs-lookup"><span data-stu-id="c4228-908">Role</span></span>

* <span data-ttu-id="c4228-909">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="c4228-909">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="c4228-910">SQL</span><span class="sxs-lookup"><span data-stu-id="c4228-910">SQL</span></span>

* <span data-ttu-id="c4228-911">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="c4228-911">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="c4228-912">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="c4228-912">Added `sql db rename`</span></span>
* <span data-ttu-id="c4228-913">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="c4228-913">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-914">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-914">Storage</span></span>

* <span data-ttu-id="c4228-915">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="c4228-915">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-916">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-916">VM</span></span>

* <span data-ttu-id="c4228-917">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="c4228-917">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="c4228-918">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="c4228-918">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="c4228-919">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="c4228-919">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="c4228-920">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-920">January 31, 2018</span></span>

<span data-ttu-id="c4228-921">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="c4228-921">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="c4228-922">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-922">Core</span></span>

* <span data-ttu-id="c4228-923">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="c4228-923">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="c4228-924">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="c4228-924">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="c4228-925">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="c4228-925">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="c4228-926">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="c4228-926">Use `--verbose` to see</span></span>
* <span data-ttu-id="c4228-927">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="c4228-927">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-928">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-928">ACS</span></span>

* <span data-ttu-id="c4228-929">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="c4228-929">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="c4228-930">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="c4228-930">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-931">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="c4228-931">Appservice</span></span>

* <span data-ttu-id="c4228-932">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="c4228-932">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="c4228-933">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="c4228-933">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="c4228-934">CDN</span><span class="sxs-lookup"><span data-stu-id="c4228-934">CDN</span></span>

* <span data-ttu-id="c4228-935">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-935">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c4228-936">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c4228-936">CosmosDB</span></span>

* <span data-ttu-id="c4228-937">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="c4228-937">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="c4228-938">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4228-938">Interactive</span></span>

* <span data-ttu-id="c4228-939">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="c4228-939">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="c4228-940">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-940">Network</span></span>

* <span data-ttu-id="c4228-941">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-941">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="c4228-942">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c4228-942">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="c4228-943">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-943">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="c4228-944">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-944">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="c4228-945">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="c4228-945">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="c4228-946">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="c4228-946">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="c4228-947">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="c4228-947">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="c4228-948">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="c4228-948">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="c4228-949">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="c4228-949">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="c4228-950">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="c4228-950">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="c4228-951">Профиль</span><span class="sxs-lookup"><span data-stu-id="c4228-951">Profile</span></span>

* <span data-ttu-id="c4228-952">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="c4228-952">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="c4228-953">Ресурс</span><span class="sxs-lookup"><span data-stu-id="c4228-953">Resource</span></span>

* <span data-ttu-id="c4228-954">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="c4228-954">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-955">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-955">Storage</span></span>

* <span data-ttu-id="c4228-956">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="c4228-956">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="c4228-957">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="c4228-957">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="c4228-958">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="c4228-958">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="c4228-959">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-959">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="c4228-960">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="c4228-960">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-961">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-961">VM</span></span>

* <span data-ttu-id="c4228-962">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="c4228-962">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="c4228-963">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="c4228-963">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="c4228-964">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="c4228-964">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="c4228-965">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-965">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="c4228-966">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-966">January 17, 2018</span></span>

<span data-ttu-id="c4228-967">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="c4228-967">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="c4228-968">ACR</span><span class="sxs-lookup"><span data-stu-id="c4228-968">ACR</span></span>

* <span data-ttu-id="c4228-969">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="c4228-969">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="c4228-970">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="c4228-970">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-971">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-971">ACS</span></span>

* <span data-ttu-id="c4228-972">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="c4228-972">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="c4228-973">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="c4228-973">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-974">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="c4228-974">Appservice</span></span>

* <span data-ttu-id="c4228-975">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="c4228-975">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="c4228-976">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="c4228-976">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="c4228-977">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="c4228-977">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="c4228-978">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="c4228-978">Backup</span></span>

* <span data-ttu-id="c4228-979">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="c4228-979">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="c4228-980">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="c4228-980">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="c4228-981">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="c4228-981">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="c4228-982">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="c4228-982">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="c4228-983">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="c4228-983">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="c4228-984">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="c4228-984">Batch</span></span>

* <span data-ttu-id="c4228-985">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="c4228-985">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="c4228-986">Облако</span><span class="sxs-lookup"><span data-stu-id="c4228-986">Cloud</span></span>

* <span data-ttu-id="c4228-987">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="c4228-987">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="c4228-988">Потребление</span><span class="sxs-lookup"><span data-stu-id="c4228-988">Consumption</span></span>

* <span data-ttu-id="c4228-989">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="c4228-989">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="c4228-990">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="c4228-990">Event Grid</span></span>

* <span data-ttu-id="c4228-991">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="c4228-991">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="c4228-992">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="c4228-992">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="c4228-993">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="c4228-993">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="c4228-994">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="c4228-994">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="c4228-995">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-995">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="c4228-996">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-996">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="c4228-997">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="c4228-997">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="c4228-998">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="c4228-998">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="c4228-999">Interactive</span><span class="sxs-lookup"><span data-stu-id="c4228-999">Interactive</span></span>

* <span data-ttu-id="c4228-1000">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="c4228-1000">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="c4228-1001">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="c4228-1001">Fixed errors on startup</span></span>
* <span data-ttu-id="c4228-1002">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="c4228-1002">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="c4228-1003">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="c4228-1003">IoT</span></span>

* <span data-ttu-id="c4228-1004">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="c4228-1004">Added support for device provisioning service</span></span>
* <span data-ttu-id="c4228-1005">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="c4228-1005">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="c4228-1006">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="c4228-1006">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="c4228-1007">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="c4228-1007">Monitor</span></span>

* <span data-ttu-id="c4228-1008">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="c4228-1008">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="c4228-1009">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1009">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="c4228-1010">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="c4228-1010">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="c4228-1011">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-1011">Network</span></span>

* <span data-ttu-id="c4228-1012">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="c4228-1012">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="c4228-1013">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="c4228-1013">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="c4228-1014">Профиль</span><span class="sxs-lookup"><span data-stu-id="c4228-1014">Profile</span></span>

* <span data-ttu-id="c4228-1015">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="c4228-1015">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="c4228-1016">Роль</span><span class="sxs-lookup"><span data-stu-id="c4228-1016">Role</span></span>

* <span data-ttu-id="c4228-1017">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="c4228-1017">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c4228-1018">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c4228-1018">Service Fabric</span></span>

* <span data-ttu-id="c4228-1019">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="c4228-1019">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="c4228-1020">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="c4228-1020">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-1021">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-1021">VM</span></span>

* <span data-ttu-id="c4228-1022">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1022">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="c4228-1023">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="c4228-1023">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="c4228-1024">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1024">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="c4228-1025">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="c4228-1025">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="c4228-1026">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="c4228-1026">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="c4228-1027">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1027">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="c4228-1028">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1028">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="c4228-1029">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1029">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="c4228-1030">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-1030">December 19, 2017</span></span>

<span data-ttu-id="c4228-1031">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="c4228-1031">Version 2.0.23</span></span>

* <span data-ttu-id="c4228-1032">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="c4228-1032">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="c4228-1033">Контейнер</span><span class="sxs-lookup"><span data-stu-id="c4228-1033">Container</span></span>

* <span data-ttu-id="c4228-1034">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="c4228-1034">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="c4228-1035">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-1035">Network</span></span>

* <span data-ttu-id="c4228-1036">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4228-1036">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="c4228-1037">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4228-1037">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-1038">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-1038">Storage</span></span>

* <span data-ttu-id="c4228-1039">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="c4228-1039">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-1040">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-1040">VM</span></span>

* <span data-ttu-id="c4228-1041">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="c4228-1041">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="c4228-1042">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-1042">December 5, 2017</span></span>

<span data-ttu-id="c4228-1043">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="c4228-1043">Version 2.0.22</span></span>

* <span data-ttu-id="c4228-1044">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1044">Removed `az component` commands.</span></span> <span data-ttu-id="c4228-1045">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1045">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="c4228-1046">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-1046">Core</span></span>
* <span data-ttu-id="c4228-1047">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="c4228-1047">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="c4228-1048">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="c4228-1048">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-1049">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-1049">ACS</span></span>

* <span data-ttu-id="c4228-1050">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1050">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="c4228-1051">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1051">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="c4228-1052">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="c4228-1052">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="c4228-1053">Помощник</span><span class="sxs-lookup"><span data-stu-id="c4228-1053">Advisor</span></span>

* <span data-ttu-id="c4228-1054">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="c4228-1054">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-1055">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="c4228-1055">Appservice</span></span>

* <span data-ttu-id="c4228-1056">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1056">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="c4228-1057">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="c4228-1057">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="c4228-1058">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1058">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="c4228-1059">Потребление</span><span class="sxs-lookup"><span data-stu-id="c4228-1059">Consumption</span></span>

* <span data-ttu-id="c4228-1060">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="c4228-1060">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="c4228-1061">Контейнер</span><span class="sxs-lookup"><span data-stu-id="c4228-1061">Container</span></span>

* <span data-ttu-id="c4228-1062">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="c4228-1062">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="c4228-1063">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="c4228-1063">Monitor</span></span>

* <span data-ttu-id="c4228-1064">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="c4228-1064">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="c4228-1065">Ресурс</span><span class="sxs-lookup"><span data-stu-id="c4228-1065">Resource</span></span>

* <span data-ttu-id="c4228-1066">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="c4228-1066">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="c4228-1067">Роль</span><span class="sxs-lookup"><span data-stu-id="c4228-1067">Role</span></span>

* <span data-ttu-id="c4228-1068">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1068">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="c4228-1069">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="c4228-1069">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="c4228-1070">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1070">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="c4228-1071">SQL</span><span class="sxs-lookup"><span data-stu-id="c4228-1071">SQL</span></span>

* <span data-ttu-id="c4228-1072">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1072">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="c4228-1073">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1073">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-1074">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-1074">VM</span></span>

* <span data-ttu-id="c4228-1075">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1075">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="c4228-1076">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-1076">November 14, 2017</span></span>

<span data-ttu-id="c4228-1077">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="c4228-1077">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="c4228-1078">ACR</span><span class="sxs-lookup"><span data-stu-id="c4228-1078">ACR</span></span>

* <span data-ttu-id="c4228-1079">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="c4228-1079">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="c4228-1080">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-1080">ACS</span></span>

* <span data-ttu-id="c4228-1081">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="c4228-1081">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="c4228-1082">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="c4228-1082">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="c4228-1083">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1083">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="c4228-1084">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="c4228-1084">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="c4228-1085">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="c4228-1085">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-1086">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="c4228-1086">Appservice</span></span>

* <span data-ttu-id="c4228-1087">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="c4228-1087">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="c4228-1088">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1088">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="c4228-1089">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1089">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="c4228-1090">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1090">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="c4228-1091">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="c4228-1091">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="c4228-1092">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="c4228-1092">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="c4228-1093">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="c4228-1093">Batch</span></span>

* <span data-ttu-id="c4228-1094">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1094">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="c4228-1095">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="c4228-1095">Batchai</span></span>

* <span data-ttu-id="c4228-1096">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1096">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="c4228-1097">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1097">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="c4228-1098">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1098">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="c4228-1099">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1099">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="c4228-1100">Облако</span><span class="sxs-lookup"><span data-stu-id="c4228-1100">Cloud</span></span>

* <span data-ttu-id="c4228-1101">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="c4228-1101">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="c4228-1102">Контейнер</span><span class="sxs-lookup"><span data-stu-id="c4228-1102">Container</span></span>

* <span data-ttu-id="c4228-1103">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="c4228-1103">Added support to open multiple ports</span></span>
* <span data-ttu-id="c4228-1104">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="c4228-1104">Added container group restart policy</span></span>
* <span data-ttu-id="c4228-1105">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="c4228-1105">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="c4228-1106">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="c4228-1106">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c4228-1107">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c4228-1107">Data Lake Analytics</span></span>

* <span data-ttu-id="c4228-1108">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="c4228-1108">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c4228-1109">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c4228-1109">Data Lake Store</span></span>

* <span data-ttu-id="c4228-1110">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="c4228-1110">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="c4228-1111">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="c4228-1111">Extension</span></span>

* <span data-ttu-id="c4228-1112">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="c4228-1112">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="c4228-1113">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="c4228-1113">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="c4228-1114">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="c4228-1114">IoT</span></span>

* <span data-ttu-id="c4228-1115">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="c4228-1115">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="c4228-1116">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="c4228-1116">Monitor</span></span>

* <span data-ttu-id="c4228-1117">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1117">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="c4228-1118">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-1118">Network</span></span>

* <span data-ttu-id="c4228-1119">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="c4228-1119">Added support for CAA DNS records</span></span>
* <span data-ttu-id="c4228-1120">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1120">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="c4228-1121">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="c4228-1121">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="c4228-1122">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1122">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="c4228-1123">Резервирование</span><span class="sxs-lookup"><span data-stu-id="c4228-1123">Reservations</span></span>

* <span data-ttu-id="c4228-1124">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="c4228-1124">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="c4228-1125">Ресурс</span><span class="sxs-lookup"><span data-stu-id="c4228-1125">Resource</span></span>

* <span data-ttu-id="c4228-1126">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1126">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="c4228-1127">SQL</span><span class="sxs-lookup"><span data-stu-id="c4228-1127">SQL</span></span>

* <span data-ttu-id="c4228-1128">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1128">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-1129">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-1129">Storage</span></span>

* <span data-ttu-id="c4228-1130">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c4228-1130">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="c4228-1131">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="c4228-1131">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="c4228-1132">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1132">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="c4228-1133">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1133">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="c4228-1134">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1134">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="c4228-1135">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1135">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="c4228-1136">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1136">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-1137">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-1137">VM</span></span>

* <span data-ttu-id="c4228-1138">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1138">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="c4228-1139">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="c4228-1139">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="c4228-1140">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1140">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="c4228-1141">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1141">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="c4228-1142">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="c4228-1142">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="c4228-1143">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-1143">October 24, 2017</span></span>

<span data-ttu-id="c4228-1144">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="c4228-1144">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="c4228-1145">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-1145">Core</span></span>

* <span data-ttu-id="c4228-1146">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="c4228-1146">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="c4228-1147">ACR</span><span class="sxs-lookup"><span data-stu-id="c4228-1147">ACR</span></span>

* <span data-ttu-id="c4228-1148">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="c4228-1148">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="c4228-1149">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="c4228-1149">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="c4228-1150">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="c4228-1150">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-1151">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-1151">ACS</span></span>

* <span data-ttu-id="c4228-1152">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="c4228-1152">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="c4228-1153">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="c4228-1153">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-1154">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="c4228-1154">Appservice</span></span>

* <span data-ttu-id="c4228-1155">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="c4228-1155">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="c4228-1156">Компонент</span><span class="sxs-lookup"><span data-stu-id="c4228-1156">Component</span></span>

* <span data-ttu-id="c4228-1157">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="c4228-1157">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="c4228-1158">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="c4228-1158">Monitor</span></span>

* <span data-ttu-id="c4228-1159">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1159">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="c4228-1160">Ресурс</span><span class="sxs-lookup"><span data-stu-id="c4228-1160">Resource</span></span>

* <span data-ttu-id="c4228-1161">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="c4228-1161">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="c4228-1162">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="c4228-1162">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-1163">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-1163">VM</span></span>

* <span data-ttu-id="c4228-1164">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="c4228-1164">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="c4228-1165">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-1165">October 9, 2017</span></span>

<span data-ttu-id="c4228-1166">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="c4228-1166">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="c4228-1167">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-1167">Core</span></span>

* <span data-ttu-id="c4228-1168">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="c4228-1168">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-1169">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="c4228-1169">Appservice</span></span>

* <span data-ttu-id="c4228-1170">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1170">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="c4228-1171">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="c4228-1171">Batch</span></span>

* <span data-ttu-id="c4228-1172">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="c4228-1172">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="c4228-1173">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="c4228-1173">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="c4228-1174">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="c4228-1174">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="c4228-1175">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="c4228-1175">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="c4228-1176">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="c4228-1176">Batchai</span></span>

* <span data-ttu-id="c4228-1177">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="c4228-1177">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="c4228-1178">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="c4228-1178">Keyvault</span></span>

* <span data-ttu-id="c4228-1179">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="c4228-1179">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="c4228-1180">(#4448)</span><span class="sxs-lookup"><span data-stu-id="c4228-1180">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="c4228-1181">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-1181">Network</span></span>

* <span data-ttu-id="c4228-1182">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="c4228-1182">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="c4228-1183">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="c4228-1183">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="c4228-1184">Ресурс</span><span class="sxs-lookup"><span data-stu-id="c4228-1184">Resource</span></span>

* <span data-ttu-id="c4228-1185">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1185">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="c4228-1186">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="c4228-1186">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="c4228-1187">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="c4228-1187">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="c4228-1188">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="c4228-1188">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="c4228-1189">SQL</span><span class="sxs-lookup"><span data-stu-id="c4228-1189">Sql</span></span>

* <span data-ttu-id="c4228-1190">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="c4228-1190">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="c4228-1191">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="c4228-1191">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="c4228-1192">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="c4228-1192">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-1193">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-1193">Storage</span></span>

* <span data-ttu-id="c4228-1194">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c4228-1194">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-1195">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="c4228-1195">Vm</span></span>

* <span data-ttu-id="c4228-1196">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="c4228-1196">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="c4228-1197">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1197">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="c4228-1198">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1198">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="c4228-1199">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1199">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="c4228-1200">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="c4228-1200">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="c4228-1201">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-1201">September 22, 2017</span></span>

<span data-ttu-id="c4228-1202">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="c4228-1202">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="c4228-1203">Ресурс</span><span class="sxs-lookup"><span data-stu-id="c4228-1203">Resource</span></span>

* <span data-ttu-id="c4228-1204">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="c4228-1204">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="c4228-1205">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="c4228-1205">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="c4228-1206">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="c4228-1206">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="c4228-1207">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1207">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="c4228-1208">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-1208">Network</span></span>

* <span data-ttu-id="c4228-1209">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="c4228-1209">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="c4228-1210">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="c4228-1210">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="c4228-1211">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="c4228-1211">Added `asg` application security group commands</span></span>
* <span data-ttu-id="c4228-1212">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="c4228-1212">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="c4228-1213">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4228-1213">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="c4228-1214">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4228-1214">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="c4228-1215">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1215">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-1216">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-1216">Storage</span></span>

* <span data-ttu-id="c4228-1217">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="c4228-1217">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="c4228-1218">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="c4228-1218">Eventgrid</span></span>

* <span data-ttu-id="c4228-1219">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="c4228-1219">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="c4228-1220">SQL</span><span class="sxs-lookup"><span data-stu-id="c4228-1220">SQL</span></span>

* <span data-ttu-id="c4228-1221">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="c4228-1221">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="c4228-1222">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="c4228-1222">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="c4228-1223">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="c4228-1223">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="c4228-1224">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="c4228-1224">Keyvault</span></span>

* <span data-ttu-id="c4228-1225">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="c4228-1225">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-1226">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-1226">VM</span></span>

* <span data-ttu-id="c4228-1227">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="c4228-1227">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="c4228-1228">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="c4228-1228">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="c4228-1229">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="c4228-1229">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="c4228-1230">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="c4228-1230">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="c4228-1231">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="c4228-1231">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="c4228-1232">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="c4228-1232">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-1233">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-1233">ACS</span></span>

* <span data-ttu-id="c4228-1234">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="c4228-1234">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-1235">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="c4228-1235">Appservice</span></span>

* <span data-ttu-id="c4228-1236">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="c4228-1236">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="c4228-1237">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="c4228-1237">Backup</span></span>

* <span data-ttu-id="c4228-1238">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="c4228-1238">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="c4228-1239">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-1239">September 11, 2017</span></span>

<span data-ttu-id="c4228-1240">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="c4228-1240">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="c4228-1241">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-1241">Core</span></span>

* <span data-ttu-id="c4228-1242">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="c4228-1242">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="c4228-1243">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="c4228-1243">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-1244">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-1244">Acs</span></span>

* <span data-ttu-id="c4228-1245">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1245">Added `acs list-locations` command</span></span>
* <span data-ttu-id="c4228-1246">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c4228-1246">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-1247">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="c4228-1247">Appservice</span></span>

* <span data-ttu-id="c4228-1248">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="c4228-1248">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="c4228-1249">CDN</span><span class="sxs-lookup"><span data-stu-id="c4228-1249">CDN</span></span>

* <span data-ttu-id="c4228-1250">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1250">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="c4228-1251">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="c4228-1251">Extension</span></span>

* <span data-ttu-id="c4228-1252">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="c4228-1252">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="c4228-1253">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="c4228-1253">Keyvault</span></span>

* <span data-ttu-id="c4228-1254">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1254">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="c4228-1255">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-1255">Network</span></span>

* <span data-ttu-id="c4228-1256">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1256">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="c4228-1257">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1257">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="c4228-1258">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1258">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="c4228-1259">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1259">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="c4228-1260">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1260">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="c4228-1261">Ресурс</span><span class="sxs-lookup"><span data-stu-id="c4228-1261">Resource</span></span>

* <span data-ttu-id="c4228-1262">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1262">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="c4228-1263">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1263">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="c4228-1264">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="c4228-1264">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="c4228-1265">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="c4228-1265">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="c4228-1266">SQL</span><span class="sxs-lookup"><span data-stu-id="c4228-1266">SQL</span></span>

* <span data-ttu-id="c4228-1267">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1267">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-1268">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-1268">VM</span></span>

* <span data-ttu-id="c4228-1269">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="c4228-1269">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="c4228-1270">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="c4228-1270">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="c4228-1271">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1271">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="c4228-1272">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="c4228-1272">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="c4228-1273">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="c4228-1273">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="c4228-1274">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-1274">August 31, 2017</span></span>

<span data-ttu-id="c4228-1275">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="c4228-1275">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="c4228-1276">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="c4228-1276">Keyvault</span></span>

* <span data-ttu-id="c4228-1277">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1277">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="c4228-1278">Sf</span><span class="sxs-lookup"><span data-stu-id="c4228-1278">Sf</span></span>

* <span data-ttu-id="c4228-1279">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="c4228-1279">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-1280">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-1280">Storage</span></span>

* <span data-ttu-id="c4228-1281">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="c4228-1281">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="c4228-1282">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="c4228-1282">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="c4228-1283">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-1283">August 28, 2017</span></span>

<span data-ttu-id="c4228-1284">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="c4228-1284">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="c4228-1285">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="c4228-1285">CLI</span></span>

* <span data-ttu-id="c4228-1286">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="c4228-1286">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-1287">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-1287">ACS</span></span>

* <span data-ttu-id="c4228-1288">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="c4228-1288">Corrected preview regions</span></span>
* <span data-ttu-id="c4228-1289">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1289">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="c4228-1290">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="c4228-1290">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-1291">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="c4228-1291">Appservice</span></span>

* <span data-ttu-id="c4228-1292">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1292">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="c4228-1293">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1293">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="c4228-1294">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1294">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="c4228-1295">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="c4228-1295">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="c4228-1296">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="c4228-1296">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="c4228-1297">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="c4228-1297">IoT</span></span>

* <span data-ttu-id="c4228-1298">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="c4228-1298">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="c4228-1299">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-1299">Network</span></span>

* <span data-ttu-id="c4228-1300">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1300">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="c4228-1301">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1301">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="c4228-1302">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1302">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="c4228-1303">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1303">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="c4228-1304">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1304">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="c4228-1305">Профиль</span><span class="sxs-lookup"><span data-stu-id="c4228-1305">Profile</span></span>

* <span data-ttu-id="c4228-1306">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="c4228-1306">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c4228-1307">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c4228-1307">Service Fabric</span></span>

* <span data-ttu-id="c4228-1308">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="c4228-1308">Preview release</span></span>
* <span data-ttu-id="c4228-1309">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="c4228-1309">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="c4228-1310">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="c4228-1310">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="c4228-1311">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1311">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-1312">Хранилище</span><span class="sxs-lookup"><span data-stu-id="c4228-1312">Storage</span></span>

* <span data-ttu-id="c4228-1313">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="c4228-1313">Enabled setting blob tier</span></span>
* <span data-ttu-id="c4228-1314">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="c4228-1314">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="c4228-1315">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1315">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="c4228-1316">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="c4228-1316">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="c4228-1317">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1317">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="c4228-1318">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1318">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-1319">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-1319">VM</span></span>

* <span data-ttu-id="c4228-1320">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1320">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="c4228-1321">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1321">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="c4228-1322">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="c4228-1322">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="c4228-1323">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="c4228-1323">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="c4228-1324">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="c4228-1324">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="c4228-1325">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1325">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="c4228-1326">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-1326">August 15, 2017</span></span>

<span data-ttu-id="c4228-1327">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="c4228-1327">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-1328">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-1328">ACS</span></span>

* <span data-ttu-id="c4228-1329">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="c4228-1329">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-1330">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="c4228-1330">Appservice</span></span>

* <span data-ttu-id="c4228-1331">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="c4228-1331">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="c4228-1332">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="c4228-1332">Event Grid</span></span>

* <span data-ttu-id="c4228-1333">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="c4228-1333">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="c4228-1334">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-1334">August 11, 2017</span></span>

<span data-ttu-id="c4228-1335">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="c4228-1335">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-1336">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-1336">ACS</span></span>

* <span data-ttu-id="c4228-1337">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="c4228-1337">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="c4228-1338">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="c4228-1338">Batch</span></span>

* <span data-ttu-id="c4228-1339">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="c4228-1339">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="c4228-1340">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="c4228-1340">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="c4228-1341">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c4228-1341">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="c4228-1342">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="c4228-1342">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="c4228-1343">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="c4228-1343">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="c4228-1344">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="c4228-1344">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="c4228-1345">Компонент</span><span class="sxs-lookup"><span data-stu-id="c4228-1345">Component</span></span>

* <span data-ttu-id="c4228-1346">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="c4228-1346">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="c4228-1347">Контейнер</span><span class="sxs-lookup"><span data-stu-id="c4228-1347">Container</span></span>

* <span data-ttu-id="c4228-1348">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="c4228-1348">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="c4228-1349">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c4228-1349">Data Lake Store</span></span>

* <span data-ttu-id="c4228-1350">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="c4228-1350">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="c4228-1351">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="c4228-1351">Event Grid</span></span>

* <span data-ttu-id="c4228-1352">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="c4228-1352">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="c4228-1353">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-1353">Network</span></span>

* <span data-ttu-id="c4228-1354">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="c4228-1354">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="c4228-1355">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1355">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="c4228-1356">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1356">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="c4228-1357">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1357">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="c4228-1358">Профиль</span><span class="sxs-lookup"><span data-stu-id="c4228-1358">Profile</span></span>

* <span data-ttu-id="c4228-1359">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="c4228-1359">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-1360">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-1360">Storage</span></span>

* <span data-ttu-id="c4228-1361">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="c4228-1361">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-1362">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-1362">VM</span></span>

* <span data-ttu-id="c4228-1363">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="c4228-1363">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="c4228-1364">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1364">Exposed `list-skus` command</span></span>
* <span data-ttu-id="c4228-1365">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="c4228-1365">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="c4228-1366">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-1366">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="c4228-1367">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="c4228-1367">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="c4228-1368">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-1368">July 28, 2017</span></span>

<span data-ttu-id="c4228-1369">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="c4228-1369">Version 2.0.12</span></span>

* <span data-ttu-id="c4228-1370">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="c4228-1370">Added container commands</span></span>
* <span data-ttu-id="c4228-1371">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c4228-1371">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="c4228-1372">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-1372">Core</span></span>

* <span data-ttu-id="c4228-1373">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="c4228-1373">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="c4228-1374">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="c4228-1374">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="c4228-1375">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="c4228-1375">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="c4228-1376">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="c4228-1376">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="c4228-1377">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="c4228-1377">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="c4228-1378">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="c4228-1378">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="c4228-1379">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="c4228-1379">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="c4228-1380">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="c4228-1380">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="c4228-1381">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="c4228-1381">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="c4228-1382">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="c4228-1382">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="c4228-1383">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="c4228-1383">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="c4228-1384">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="c4228-1384">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="c4228-1385">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="c4228-1385">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="c4228-1386">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="c4228-1386">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="c4228-1387">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="c4228-1387">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="c4228-1388">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="c4228-1388">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="c4228-1389">ACR</span><span class="sxs-lookup"><span data-stu-id="c4228-1389">ACR</span></span>

* <span data-ttu-id="c4228-1390">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="c4228-1390">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="c4228-1391">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="c4228-1391">Support SKU update for managed registries</span></span>
* <span data-ttu-id="c4228-1392">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="c4228-1392">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="c4228-1393">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="c4228-1393">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="c4228-1394">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="c4228-1394">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="c4228-1395">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="c4228-1395">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-1396">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-1396">ACS</span></span>

* <span data-ttu-id="c4228-1397">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="c4228-1397">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-1398">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="c4228-1398">Appservice</span></span>

* <span data-ttu-id="c4228-1399">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="c4228-1399">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="c4228-1400">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="c4228-1400">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="c4228-1401">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1401">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="c4228-1402">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="c4228-1402">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="c4228-1403">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="c4228-1403">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="c4228-1404">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="c4228-1404">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="c4228-1405">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="c4228-1405">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="c4228-1406">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="c4228-1406">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="c4228-1407">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="c4228-1407">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="c4228-1408">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1408">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="c4228-1409">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="c4228-1409">Batch</span></span>

* <span data-ttu-id="c4228-1410">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="c4228-1410">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="c4228-1411">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1411">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="c4228-1412">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1412">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="c4228-1413">CDN</span><span class="sxs-lookup"><span data-stu-id="c4228-1413">CDN</span></span>

* <span data-ttu-id="c4228-1414">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="c4228-1414">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="c4228-1415">Облако</span><span class="sxs-lookup"><span data-stu-id="c4228-1415">Cloud</span></span>

* <span data-ttu-id="c4228-1416">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="c4228-1416">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="c4228-1417">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="c4228-1417">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="c4228-1418">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="c4228-1418">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="c4228-1419">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="c4228-1419">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="c4228-1420">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1420">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c4228-1421">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c4228-1421">CosmosDB</span></span>

* <span data-ttu-id="c4228-1422">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="c4228-1422">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="c4228-1423">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="c4228-1423">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c4228-1424">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c4228-1424">Data Lake Analytics</span></span>

* <span data-ttu-id="c4228-1425">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1425">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="c4228-1426">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1426">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="c4228-1427">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1427">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c4228-1428">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c4228-1428">Data Lake Store</span></span>

* <span data-ttu-id="c4228-1429">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1429">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="c4228-1430">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="c4228-1430">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="c4228-1431">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1431">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="c4228-1432">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="c4228-1432">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="c4228-1433">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="c4228-1433">Interactive</span></span>

* <span data-ttu-id="c4228-1434">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="c4228-1434">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="c4228-1435">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="c4228-1435">Increased test coverage</span></span>
* <span data-ttu-id="c4228-1436">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="c4228-1436">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="c4228-1437">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="c4228-1437">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="c4228-1438">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="c4228-1438">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="c4228-1439">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="c4228-1439">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="c4228-1440">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="c4228-1440">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="c4228-1441">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1441">Added `--progress` flag</span></span>
* <span data-ttu-id="c4228-1442">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1442">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="c4228-1443">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="c4228-1443">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="c4228-1444">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="c4228-1444">IoT</span></span>

* <span data-ttu-id="c4228-1445">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="c4228-1445">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="c4228-1446">(3934).</span><span class="sxs-lookup"><span data-stu-id="c4228-1446">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="c4228-1447">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="c4228-1447">Key vault</span></span>

* <span data-ttu-id="c4228-1448">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="c4228-1448">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="c4228-1449">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1449">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="c4228-1450">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="c4228-1450">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="c4228-1451">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="c4228-1451">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="c4228-1452">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1452">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="c4228-1453">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="c4228-1453">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="c4228-1454">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="c4228-1454">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="c4228-1455">(3307).</span><span class="sxs-lookup"><span data-stu-id="c4228-1455">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="c4228-1456">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="c4228-1456">Lab</span></span>

* <span data-ttu-id="c4228-1457">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1457">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="c4228-1458">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1458">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="c4228-1459">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="c4228-1459">Monitor</span></span>

* <span data-ttu-id="c4228-1460">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="c4228-1460">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="c4228-1461">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1461">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="c4228-1462">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1462">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="c4228-1463">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1463">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="c4228-1464">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1464">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="c4228-1465">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="c4228-1465">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="c4228-1466">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="c4228-1466">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="c4228-1467">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="c4228-1467">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="c4228-1468">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="c4228-1468">`location` no longer required</span></span>
  * <span data-ttu-id="c4228-1469">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="c4228-1469">Add name and ID support for target</span></span>
  * <span data-ttu-id="c4228-1470">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="c4228-1470">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="c4228-1471">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="c4228-1471">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="c4228-1472">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="c4228-1472">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="c4228-1473">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="c4228-1473">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="c4228-1474">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1474">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="c4228-1475">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1475">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="c4228-1476">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-1476">Network</span></span>

* <span data-ttu-id="c4228-1477">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1477">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="c4228-1478">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1478">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="c4228-1479">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="c4228-1479">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="c4228-1480">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1480">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="c4228-1481">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1481">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="c4228-1482">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1482">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="c4228-1483">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1483">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="c4228-1484">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1484">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="c4228-1485">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1485">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="c4228-1486">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1486">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="c4228-1487">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1487">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="c4228-1488">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1488">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="c4228-1489">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1489">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="c4228-1490">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1490">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="c4228-1491">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1491">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="c4228-1492">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1492">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="c4228-1493">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="c4228-1493">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="c4228-1494">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1494">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="c4228-1495">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1495">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="c4228-1496">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1496">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="c4228-1497">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1497">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="c4228-1498">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1498">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="c4228-1499">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1499">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="c4228-1500">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="c4228-1500">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="c4228-1501">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="c4228-1501">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="c4228-1502">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="c4228-1502">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="c4228-1503">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="c4228-1503">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="c4228-1504">Профиль</span><span class="sxs-lookup"><span data-stu-id="c4228-1504">Profile</span></span>

* <span data-ttu-id="c4228-1505">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="c4228-1505">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="c4228-1506">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="c4228-1506">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="c4228-1507">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="c4228-1507">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="c4228-1508">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="c4228-1508">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="c4228-1509">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="c4228-1509">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="c4228-1510">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="c4228-1510">RDBMS</span></span>

* <span data-ttu-id="c4228-1511">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="c4228-1511">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="c4228-1512">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="c4228-1512">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="c4228-1513">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="c4228-1513">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="c4228-1514">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="c4228-1514">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="c4228-1515">Ресурс</span><span class="sxs-lookup"><span data-stu-id="c4228-1515">Resource</span></span>

* <span data-ttu-id="c4228-1516">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1516">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="c4228-1517">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1517">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="c4228-1518">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1518">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="c4228-1519">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1519">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="c4228-1520">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="c4228-1520">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="c4228-1521">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1521">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="c4228-1522">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="c4228-1522">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="c4228-1523">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1523">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="c4228-1524">Роль</span><span class="sxs-lookup"><span data-stu-id="c4228-1524">Role</span></span>

* <span data-ttu-id="c4228-1525">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="c4228-1525">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="c4228-1526">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="c4228-1526">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="c4228-1527">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="c4228-1527">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="c4228-1528">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="c4228-1528">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="c4228-1529">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1529">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="c4228-1530">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="c4228-1530">Service Fabric</span></span>
* <span data-ttu-id="c4228-1531">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="c4228-1531">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="c4228-1532">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="c4228-1532">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="c4228-1533">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="c4228-1533">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="c4228-1534">SQL</span><span class="sxs-lookup"><span data-stu-id="c4228-1534">SQL</span></span>

* <span data-ttu-id="c4228-1535">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1535">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="c4228-1536">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1536">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="c4228-1537">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1537">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-1538">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-1538">Storage</span></span>

* <span data-ttu-id="c4228-1539">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="c4228-1539">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="c4228-1540">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="c4228-1540">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="c4228-1541">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="c4228-1541">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="c4228-1542">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="c4228-1542">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="c4228-1543">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="c4228-1543">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="c4228-1544">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="c4228-1544">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-1545">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-1545">VM</span></span>

* <span data-ttu-id="c4228-1546">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="c4228-1546">Support configuring nsg</span></span>
* <span data-ttu-id="c4228-1547">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="c4228-1547">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="c4228-1548">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="c4228-1548">Support managed service identities</span></span>
* <span data-ttu-id="c4228-1549">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1549">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="c4228-1550">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="c4228-1550">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="c4228-1551">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-1551">May 10, 2017</span></span>

<span data-ttu-id="c4228-1552">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="c4228-1552">Version 2.0.6</span></span>

* <span data-ttu-id="c4228-1553">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="c4228-1553">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="c4228-1554">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="c4228-1554">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="c4228-1555">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="c4228-1555">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="c4228-1556">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="c4228-1556">Include Cognitive Services module</span></span>
* <span data-ttu-id="c4228-1557">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="c4228-1557">Include Service Fabric module</span></span>
* <span data-ttu-id="c4228-1558">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="c4228-1558">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="c4228-1559">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="c4228-1559">Add support for CDN commands</span></span>
* <span data-ttu-id="c4228-1560">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="c4228-1560">Remove Container module</span></span>
* <span data-ttu-id="c4228-1561">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1561">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="c4228-1562">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1562">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="c4228-1563">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-1563">Core</span></span>

* <span data-ttu-id="c4228-1564">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="c4228-1564">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="c4228-1565">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([#2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1565">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="c4228-1566">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1566">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="c4228-1567">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1567">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="c4228-1568">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1568">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="c4228-1569">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1569">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="c4228-1570">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1570">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="c4228-1571">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1571">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="c4228-1572">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1572">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="c4228-1573">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="c4228-1573">core: Improved performance</span></span>
* <span data-ttu-id="c4228-1574">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="c4228-1574">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="c4228-1575">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="c4228-1575">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-1576">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-1576">ACS</span></span>

* <span data-ttu-id="c4228-1577">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="c4228-1577">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="c4228-1578">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="c4228-1578">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="c4228-1579">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="c4228-1579">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="c4228-1580">Удален профиль Windows перед вызовом метода PUT для команды scale ([#2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1580">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-1581">AppService</span><span class="sxs-lookup"><span data-stu-id="c4228-1581">AppService</span></span>

* <span data-ttu-id="c4228-1582">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="c4228-1582">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="c4228-1583">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="c4228-1583">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="c4228-1584">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="c4228-1584">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="c4228-1585">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="c4228-1585">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="c4228-1586">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="c4228-1586">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="c4228-1587">Включена поддержка настройки строк подключения ([#2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1587">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="c4228-1588">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="c4228-1588">support slot swap with preview</span></span>
* <span data-ttu-id="c4228-1589">Устранены ошибки из команд службы приложений ([#2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1589">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="c4228-1590">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([#2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1590">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="c4228-1591">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c4228-1591">CosmosDB</span></span>

* <span data-ttu-id="c4228-1592">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="c4228-1592">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="c4228-1593">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="c4228-1593">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="c4228-1594">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="c4228-1594">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="c4228-1595">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="c4228-1595">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="c4228-1596">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="c4228-1596">Data Lake Analytics</span></span>

* <span data-ttu-id="c4228-1597">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="c4228-1597">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="c4228-1598">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="c4228-1598">Add support for new catalog item type: package.</span></span> <span data-ttu-id="c4228-1599">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1599">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="c4228-1600">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="c4228-1600">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="c4228-1601">Таблица</span><span class="sxs-lookup"><span data-stu-id="c4228-1601">Table</span></span>
  * <span data-ttu-id="c4228-1602">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="c4228-1602">Table valued function</span></span>
  * <span data-ttu-id="c4228-1603">Просмотр</span><span class="sxs-lookup"><span data-stu-id="c4228-1603">View</span></span>
  * <span data-ttu-id="c4228-1604">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="c4228-1604">Table Statistics.</span></span> <span data-ttu-id="c4228-1605">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="c4228-1605">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="c4228-1606">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="c4228-1606">Data Lake Store</span></span>

* <span data-ttu-id="c4228-1607">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="c4228-1607">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="c4228-1608">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1608">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="c4228-1609">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="c4228-1609">missed help for access show.</span></span> <span data-ttu-id="c4228-1610">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="c4228-1610">adding it.</span></span> <span data-ttu-id="c4228-1611">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="c4228-1611">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="c4228-1612">Поиск</span><span class="sxs-lookup"><span data-stu-id="c4228-1612">Find</span></span>

* <span data-ttu-id="c4228-1613">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="c4228-1613">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="c4228-1614">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="c4228-1614">KeyVault</span></span>

* <span data-ttu-id="c4228-1615">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="c4228-1615">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="c4228-1616">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="c4228-1616">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="c4228-1617">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="c4228-1617">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="c4228-1618">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="c4228-1618">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="c4228-1619">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1619">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="c4228-1620">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="c4228-1620">Lab</span></span>

* <span data-ttu-id="c4228-1621">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="c4228-1621">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="c4228-1622">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="c4228-1622">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="c4228-1623">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="c4228-1623">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="c4228-1624">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="c4228-1624">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="c4228-1625">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="c4228-1625">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="c4228-1626">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="c4228-1626">Monitor</span></span>

* <span data-ttu-id="c4228-1627">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1627">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="c4228-1628">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1628">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="c4228-1629">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-1629">Network</span></span>

* <span data-ttu-id="c4228-1630">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1630">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="c4228-1631">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1631">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="c4228-1632">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="c4228-1632">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="c4228-1633">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="c4228-1633">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="c4228-1634">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="c4228-1634">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="c4228-1635">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="c4228-1635">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="c4228-1636">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="c4228-1636">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="c4228-1637">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="c4228-1637">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="c4228-1638">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1638">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="c4228-1639">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="c4228-1639">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="c4228-1640">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1640">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="c4228-1641">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1641">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="c4228-1642">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="c4228-1642">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="c4228-1643">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="c4228-1643">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="c4228-1644">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="c4228-1644">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="c4228-1645">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="c4228-1645">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="c4228-1646">Профиль</span><span class="sxs-lookup"><span data-stu-id="c4228-1646">Profile</span></span>

* <span data-ttu-id="c4228-1647">Включена поддержка входа при отсутствии подписок ([#2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1647">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="c4228-1648">Включена поддержка сокращенных имен параметров в команде az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1648">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="c4228-1649">Redis</span><span class="sxs-lookup"><span data-stu-id="c4228-1649">Redis</span></span>

* <span data-ttu-id="c4228-1650">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="c4228-1650">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="c4228-1651">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="c4228-1651">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="c4228-1652">Ресурс</span><span class="sxs-lookup"><span data-stu-id="c4228-1652">Resource</span></span>

* <span data-ttu-id="c4228-1653">Добавлены команды определения managedapp и managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1653">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="c4228-1654">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1654">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="c4228-1655">Включена поддержка создания универсального ресурса ([#2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1655">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="c4228-1656">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="c4228-1656">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="c4228-1657">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="c4228-1657">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="c4228-1658">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="c4228-1658">Add docs for az lock update.</span></span> <span data-ttu-id="c4228-1659">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="c4228-1659">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="c4228-1660">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="c4228-1660">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="c4228-1661">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="c4228-1661">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="c4228-1662">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="c4228-1662">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="c4228-1663">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="c4228-1663">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="c4228-1664">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([#2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1664">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="c4228-1665">Роль</span><span class="sxs-lookup"><span data-stu-id="c4228-1665">Role</span></span>

* <span data-ttu-id="c4228-1666">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([#2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1666">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="c4228-1667">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1667">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="c4228-1668">Роль: устранены проблемы при обновлении определения роли ([#2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1668">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="c4228-1669">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="c4228-1669">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="c4228-1670">SQL</span><span class="sxs-lookup"><span data-stu-id="c4228-1670">SQL</span></span>

* <span data-ttu-id="c4228-1671">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="c4228-1671">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="c4228-1672">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1672">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="c4228-1673">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-1673">Storage</span></span>

* <span data-ttu-id="c4228-1674">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1674">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="c4228-1675">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="c4228-1675">Add support for incremental blob copy</span></span>
* <span data-ttu-id="c4228-1676">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="c4228-1676">Add support for large block blob upload</span></span>
* <span data-ttu-id="c4228-1677">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="c4228-1677">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-1678">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-1678">VM</span></span>

* <span data-ttu-id="c4228-1679">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="c4228-1679">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="c4228-1680">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="c4228-1680">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="c4228-1681">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="c4228-1681">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="c4228-1682">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="c4228-1682">az vm/vmss disk</span></span>
  3. <span data-ttu-id="c4228-1683">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="c4228-1683">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="c4228-1684">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="c4228-1684">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="c4228-1685">vm/vmss: добавлена поддержка создания из образа Marketplace, для которого требуются сведения о плане ([#1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1685">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="c4228-1686">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-1686">April 3, 2017</span></span>

<span data-ttu-id="c4228-1687">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="c4228-1687">Version 2.0.2</span></span>

<span data-ttu-id="c4228-1688">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="c4228-1688">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="c4228-1689">Core</span><span class="sxs-lookup"><span data-stu-id="c4228-1689">Core</span></span>

* <span data-ttu-id="c4228-1690">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c4228-1690">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="c4228-1691">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1691">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="c4228-1692">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1692">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="c4228-1693">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1693">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="c4228-1694">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1694">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="c4228-1695">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="c4228-1695">Add prompting for missing template parameters.</span></span> <span data-ttu-id="c4228-1696">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1696">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="c4228-1697">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c4228-1697">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="c4228-1698">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="c4228-1698">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="c4228-1699">ACS</span><span class="sxs-lookup"><span data-stu-id="c4228-1699">ACS</span></span>

* <span data-ttu-id="c4228-1700">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1700">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="c4228-1701">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="c4228-1701">Add support for ssh key password prompting.</span></span> <span data-ttu-id="c4228-1702">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1702">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="c4228-1703">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="c4228-1703">Add support for windows clusters.</span></span> <span data-ttu-id="c4228-1704">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1704">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="c4228-1705">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="c4228-1705">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="c4228-1706">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1706">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="c4228-1707">AppService</span><span class="sxs-lookup"><span data-stu-id="c4228-1707">AppService</span></span>

* <span data-ttu-id="c4228-1708">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1708">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="c4228-1709">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1709">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="c4228-1710">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1710">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="c4228-1711">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1711">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="c4228-1712">Data Lake</span><span class="sxs-lookup"><span data-stu-id="c4228-1712">DataLake</span></span>

* <span data-ttu-id="c4228-1713">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="c4228-1713">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="c4228-1714">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="c4228-1714">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="c4228-1715">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="c4228-1715">DocuemntDB</span></span>

* <span data-ttu-id="c4228-1716">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1716">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="c4228-1717">ВМ</span><span class="sxs-lookup"><span data-stu-id="c4228-1717">VM</span></span>

* <span data-ttu-id="c4228-1718">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1718">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="c4228-1719">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1719">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="c4228-1720">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1720">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="c4228-1721">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1721">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="c4228-1722">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1722">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="c4228-1723">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1723">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="c4228-1724">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="c4228-1724">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="c4228-1725">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="c4228-1725">February 27, 2017</span></span>

<span data-ttu-id="c4228-1726">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="c4228-1726">Version 2.0.0</span></span>

<span data-ttu-id="c4228-1727">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="c4228-1727">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="c4228-1728">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="c4228-1728">Container Service (acs)</span></span>
- <span data-ttu-id="c4228-1729">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="c4228-1729">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="c4228-1730">Сеть</span><span class="sxs-lookup"><span data-stu-id="c4228-1730">Networking</span></span>
- <span data-ttu-id="c4228-1731">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="c4228-1731">Storage</span></span>

<span data-ttu-id="c4228-1732">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1732">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="c4228-1733">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="c4228-1733">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="c4228-1734">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="c4228-1734">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="c4228-1735">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="c4228-1735">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="c4228-1736">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="c4228-1736">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="c4228-1737">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="c4228-1737">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="c4228-1738">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="c4228-1738">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="c4228-1739">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="c4228-1739">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="c4228-1740">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="c4228-1740">Provide feedback from the command line with the `az feedback` command</span></span>

