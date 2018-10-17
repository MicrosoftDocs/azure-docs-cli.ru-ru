---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/09/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 0aec9dce0eda007c71df3693b39c7ec8cc9856cd
ms.sourcegitcommit: 0fc354c24454f5c9c5ff4b7296ad7b18ffdf31b1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2018
ms.locfileid: "48904792"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="78ff8-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="78ff8-103">Azure CLI release notes</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="78ff8-104">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-104">October 9, 2018</span></span>

<span data-ttu-id="78ff8-105">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="78ff8-105">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="78ff8-106">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-106">Core</span></span>
* <span data-ttu-id="78ff8-107">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="78ff8-107">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="78ff8-108">ACR</span><span class="sxs-lookup"><span data-stu-id="78ff8-108">ACR</span></span>
* <span data-ttu-id="78ff8-109">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="78ff8-109">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-110">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-110">ACS</span></span>
* <span data-ttu-id="78ff8-111">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="78ff8-111">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="78ff8-112">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="78ff8-112">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="78ff8-113">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-113">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="78ff8-114">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="78ff8-114">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="78ff8-115">Контейнер</span><span class="sxs-lookup"><span data-stu-id="78ff8-115">Container</span></span>
* <span data-ttu-id="78ff8-116">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="78ff8-116">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="78ff8-117">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="78ff8-117">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="78ff8-118">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="78ff8-118">Event Hub</span></span>
* <span data-ttu-id="78ff8-119">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-119">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="78ff8-120">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="78ff8-120">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="78ff8-121">расширения.</span><span class="sxs-lookup"><span data-stu-id="78ff8-121">Extensions</span></span>
* <span data-ttu-id="78ff8-122">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="78ff8-122">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="78ff8-123">HDInsight</span><span class="sxs-lookup"><span data-stu-id="78ff8-123">HDInsight</span></span>
* <span data-ttu-id="78ff8-124">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="78ff8-124">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="78ff8-125">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="78ff8-125">IoT</span></span>
* <span data-ttu-id="78ff8-126">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="78ff8-126">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="78ff8-127">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="78ff8-127">KeyVault</span></span>
* <span data-ttu-id="78ff8-128">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="78ff8-128">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-129">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-129">Network</span></span>
* <span data-ttu-id="78ff8-130">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="78ff8-130">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="78ff8-131">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="78ff8-131">See #6052</span></span>
* <span data-ttu-id="78ff8-132">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-132">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="78ff8-133">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="78ff8-133">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="78ff8-134">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-134">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="78ff8-135">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-135">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="78ff8-136">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-136">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="78ff8-137">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-137">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="78ff8-138">Роль</span><span class="sxs-lookup"><span data-stu-id="78ff8-138">Role</span></span>
* <span data-ttu-id="78ff8-139">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-139">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="78ff8-140">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-140">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="78ff8-141">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="78ff8-141">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="78ff8-142">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="78ff8-142">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="78ff8-143">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="78ff8-143">Service Bus</span></span>
* <span data-ttu-id="78ff8-144">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="78ff8-144">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-145">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-145">VM</span></span>
* <span data-ttu-id="78ff8-146">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-146">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="78ff8-147">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="78ff8-147">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="78ff8-148">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-148">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="78ff8-149">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-149">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="78ff8-150">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="78ff8-150">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="78ff8-151">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="78ff8-151">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="78ff8-152">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-152">September 21, 2018</span></span>

<span data-ttu-id="78ff8-153">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="78ff8-153">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="78ff8-154">ACR</span><span class="sxs-lookup"><span data-stu-id="78ff8-154">ACR</span></span>
* <span data-ttu-id="78ff8-155">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="78ff8-155">Added ACR Task commands</span></span>
* <span data-ttu-id="78ff8-156">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="78ff8-156">Added quick run command</span></span>
* <span data-ttu-id="78ff8-157">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="78ff8-157">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="78ff8-158">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="78ff8-158">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="78ff8-159">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="78ff8-159">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="78ff8-160">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="78ff8-160">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-161">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-161">ACS</span></span>
* <span data-ttu-id="78ff8-162">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="78ff8-162">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="78ff8-163">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="78ff8-163">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-164">AppService</span><span class="sxs-lookup"><span data-stu-id="78ff8-164">AppService</span></span>

* <span data-ttu-id="78ff8-165">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="78ff8-165">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="78ff8-166">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="78ff8-166">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="78ff8-167">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="78ff8-167">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="78ff8-168">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="78ff8-168">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="78ff8-169">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="78ff8-169">Batch</span></span>
* <span data-ttu-id="78ff8-170">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="78ff8-170">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="78ff8-171">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-171">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="78ff8-172">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-172">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="78ff8-173">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="78ff8-173">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="78ff8-174">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="78ff8-174">Batch AI</span></span> 
* <span data-ttu-id="78ff8-175">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-175">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="78ff8-176">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="78ff8-176">Cognitive Services</span></span>
* <span data-ttu-id="78ff8-177">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-177">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="78ff8-178">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-178">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="78ff8-179">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-179">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="78ff8-180">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-180">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="78ff8-181">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="78ff8-181">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="78ff8-182">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-182">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="78ff8-183">Контейнер</span><span class="sxs-lookup"><span data-stu-id="78ff8-183">Container</span></span>
* <span data-ttu-id="78ff8-184">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="78ff8-184">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="78ff8-185">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="78ff8-185">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="78ff8-186">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="78ff8-186">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="78ff8-187">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="78ff8-187">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="78ff8-188">Data Lake</span><span class="sxs-lookup"><span data-stu-id="78ff8-188">Datalake</span></span>
* <span data-ttu-id="78ff8-189">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="78ff8-189">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="78ff8-190">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="78ff8-190">Interactive Shell</span></span>
* <span data-ttu-id="78ff8-191">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="78ff8-191">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="78ff8-192">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-192">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="78ff8-193">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="78ff8-193">IoT</span></span>
* <span data-ttu-id="78ff8-194">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="78ff8-194">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="78ff8-195">Key Vault</span><span class="sxs-lookup"><span data-stu-id="78ff8-195">Key Vault</span></span>
* <span data-ttu-id="78ff8-196">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="78ff8-196">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-197">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-197">Network</span></span>
* <span data-ttu-id="78ff8-198">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-198">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="78ff8-199">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="78ff8-199">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="78ff8-200">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="78ff8-200">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="78ff8-201">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-201">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="78ff8-202">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-202">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="78ff8-203">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-203">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="78ff8-204">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="78ff8-204">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="78ff8-205">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-205">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="78ff8-206">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-206">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="78ff8-207">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-207">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="78ff8-208">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-208">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="78ff8-209">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-209">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="78ff8-210">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры`--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-210">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="78ff8-211">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="78ff8-211">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="78ff8-212">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-212">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="78ff8-213">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="78ff8-213">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="78ff8-214">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="78ff8-214">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="78ff8-215">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="78ff8-215">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="78ff8-216">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="78ff8-216">RDBMS</span></span>
* <span data-ttu-id="78ff8-217">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="78ff8-217">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="78ff8-218">резервирование.</span><span class="sxs-lookup"><span data-stu-id="78ff8-218">Reservation</span></span>
* <span data-ttu-id="78ff8-219">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-219">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="78ff8-220">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="78ff8-220">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="78ff8-221">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="78ff8-221">Manage App</span></span>
* <span data-ttu-id="78ff8-222">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="78ff8-222">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="78ff8-223">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="78ff8-223">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="78ff8-224">Роль</span><span class="sxs-lookup"><span data-stu-id="78ff8-224">Role</span></span>
* <span data-ttu-id="78ff8-225">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="78ff8-225">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="78ff8-226">SignalR</span><span class="sxs-lookup"><span data-stu-id="78ff8-226">SignalR</span></span>
* <span data-ttu-id="78ff8-227">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="78ff8-227">First release</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-228">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-228">Storage</span></span>
* <span data-ttu-id="78ff8-229">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="78ff8-229">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="78ff8-230">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="78ff8-230">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-231">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-231">VM</span></span>
* <span data-ttu-id="78ff8-232">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="78ff8-232">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="78ff8-233">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-233">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="78ff8-234">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-234">August 28, 2018</span></span>

<span data-ttu-id="78ff8-235">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="78ff8-235">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="78ff8-236">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-236">Core</span></span>

* <span data-ttu-id="78ff8-237">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="78ff8-237">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="78ff8-238">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="78ff8-238">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="78ff8-239">ACR</span><span class="sxs-lookup"><span data-stu-id="78ff8-239">ACR</span></span>

* <span data-ttu-id="78ff8-240">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="78ff8-240">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="78ff8-241">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-241">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-242">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-242">ACS</span></span>

* <span data-ttu-id="78ff8-243">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-243">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="78ff8-244">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="78ff8-244">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-245">AppService</span><span class="sxs-lookup"><span data-stu-id="78ff8-245">AppService</span></span>

* <span data-ttu-id="78ff8-246">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="78ff8-246">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="78ff8-247">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="78ff8-247">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="78ff8-248">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="78ff8-248">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="78ff8-249">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="78ff8-249">Backup</span></span>

* <span data-ttu-id="78ff8-250">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="78ff8-250">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="78ff8-251">Служба Bot Service</span><span class="sxs-lookup"><span data-stu-id="78ff8-251">Bot Service</span></span>

* <span data-ttu-id="78ff8-252">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="78ff8-252">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="78ff8-253">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="78ff8-253">Cognitive Services</span></span>

* <span data-ttu-id="78ff8-254">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="78ff8-254">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="78ff8-255">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="78ff8-255">IoT</span></span>

* <span data-ttu-id="78ff8-256">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="78ff8-256">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="78ff8-257">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="78ff8-257">Monitor</span></span>

* <span data-ttu-id="78ff8-258">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="78ff8-258">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="78ff8-259">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="78ff8-259">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-260">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-260">Network</span></span>

* <span data-ttu-id="78ff8-261">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="78ff8-261">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="78ff8-262">Ресурс</span><span class="sxs-lookup"><span data-stu-id="78ff8-262">Resource</span></span>

* <span data-ttu-id="78ff8-263">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="78ff8-263">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-264">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-264">Storage</span></span>

* <span data-ttu-id="78ff8-265">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="78ff8-265">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-266">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-266">VM</span></span>

* <span data-ttu-id="78ff8-267">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="78ff8-267">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="78ff8-268">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-268">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="78ff8-269">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-269">Auguest 14, 2018</span></span>

<span data-ttu-id="78ff8-270">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="78ff8-270">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="78ff8-271">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-271">Core</span></span>

* <span data-ttu-id="78ff8-272">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-272">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="78ff8-273">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="78ff8-273">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="78ff8-274">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="78ff8-274">Telemetry</span></span>

* <span data-ttu-id="78ff8-275">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="78ff8-275">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="78ff8-276">ACR</span><span class="sxs-lookup"><span data-stu-id="78ff8-276">ACR</span></span>

* <span data-ttu-id="78ff8-277">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-277">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="78ff8-278">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-278">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-279">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-279">ACS</span></span>

* <span data-ttu-id="78ff8-280">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="78ff8-280">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="78ff8-281">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="78ff8-281">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="78ff8-282">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="78ff8-282">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="78ff8-283">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="78ff8-283">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="78ff8-284">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="78ff8-284">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="78ff8-285">AppService</span><span class="sxs-lookup"><span data-stu-id="78ff8-285">AppService</span></span>

* <span data-ttu-id="78ff8-286">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-286">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="78ff8-287">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="78ff8-287">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="78ff8-288">Batch AI</span><span class="sxs-lookup"><span data-stu-id="78ff8-288">BatchAI</span></span>

* <span data-ttu-id="78ff8-289">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="78ff8-289">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="78ff8-290">Контейнер</span><span class="sxs-lookup"><span data-stu-id="78ff8-290">Container</span></span>

* <span data-ttu-id="78ff8-291">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="78ff8-291">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="78ff8-292">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="78ff8-292">IoT</span></span>

* <span data-ttu-id="78ff8-293">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="78ff8-293">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="78ff8-294">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-294">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="78ff8-295">IoT Central</span><span class="sxs-lookup"><span data-stu-id="78ff8-295">Iot Central</span></span>

* <span data-ttu-id="78ff8-296">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="78ff8-296">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="78ff8-297">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="78ff8-297">KeyVault</span></span>


* <span data-ttu-id="78ff8-298">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="78ff8-298">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="78ff8-299">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="78ff8-299">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="78ff8-300">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="78ff8-300">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="78ff8-301">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="78ff8-301">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="78ff8-302">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="78ff8-302">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="78ff8-303">Передача</span><span class="sxs-lookup"><span data-stu-id="78ff8-303">Relay</span></span>

* <span data-ttu-id="78ff8-304">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="78ff8-304">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="78ff8-305">SQL</span><span class="sxs-lookup"><span data-stu-id="78ff8-305">Sql</span></span>

* <span data-ttu-id="78ff8-306">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-306">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-307">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-307">Storage</span></span>

* <span data-ttu-id="78ff8-308">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="78ff8-308">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="78ff8-309">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="78ff8-309">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="78ff8-310">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="78ff8-310">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="78ff8-311">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="78ff8-311">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="78ff8-312">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="78ff8-312">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-313">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-313">VM</span></span>

* <span data-ttu-id="78ff8-314">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="78ff8-314">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="78ff8-315">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-315">July 31, 2018</span></span>

<span data-ttu-id="78ff8-316">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="78ff8-316">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="78ff8-317">ACR</span><span class="sxs-lookup"><span data-stu-id="78ff8-317">ACR</span></span>

* <span data-ttu-id="78ff8-318">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-318">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="78ff8-319">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-319">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-320">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-320">ACS</span></span>

* <span data-ttu-id="78ff8-321">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="78ff8-321">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="78ff8-322">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="78ff8-322">Batch</span></span>

* <span data-ttu-id="78ff8-323">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="78ff8-323">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="78ff8-324">Контейнер</span><span class="sxs-lookup"><span data-stu-id="78ff8-324">Container</span></span>

* <span data-ttu-id="78ff8-325">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="78ff8-325">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-326">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-326">Network</span></span>

* <span data-ttu-id="78ff8-327">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="78ff8-327">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="78ff8-328">Ресурс</span><span class="sxs-lookup"><span data-stu-id="78ff8-328">Resource</span></span>

* <span data-ttu-id="78ff8-329">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="78ff8-329">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="78ff8-330">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="78ff8-330">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="78ff8-331">Роль</span><span class="sxs-lookup"><span data-stu-id="78ff8-331">Role</span></span>

* <span data-ttu-id="78ff8-332">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="78ff8-332">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="78ff8-333">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="78ff8-333">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="78ff8-334">поиска</span><span class="sxs-lookup"><span data-stu-id="78ff8-334">Search</span></span>

* <span data-ttu-id="78ff8-335">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="78ff8-335">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="78ff8-336">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="78ff8-336">Service Bus</span></span>

* <span data-ttu-id="78ff8-337">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="78ff8-337">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="78ff8-338">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="78ff8-338">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="78ff8-339">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="78ff8-339">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="78ff8-340">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-340">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-341">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-341">Storage</span></span>

* <span data-ttu-id="78ff8-342">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="78ff8-342">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="78ff8-343">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="78ff8-343">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-344">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-344">VM</span></span>

* <span data-ttu-id="78ff8-345">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="78ff8-345">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="78ff8-346">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-346">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="78ff8-347">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="78ff8-347">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="78ff8-348">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="78ff8-348">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="78ff8-349">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-349">July 18, 2018</span></span>

<span data-ttu-id="78ff8-350">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="78ff8-350">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="78ff8-351">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-351">Core</span></span>

* <span data-ttu-id="78ff8-352">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="78ff8-352">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="78ff8-353">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="78ff8-353">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="78ff8-354">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="78ff8-354">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="78ff8-355">ACR</span><span class="sxs-lookup"><span data-stu-id="78ff8-355">ACR</span></span>

* <span data-ttu-id="78ff8-356">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="78ff8-356">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="78ff8-357">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-357">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="78ff8-358">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="78ff8-358">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="78ff8-359">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="78ff8-359">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-360">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-360">ACS</span></span>

* <span data-ttu-id="78ff8-361">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="78ff8-361">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-362">AppService</span><span class="sxs-lookup"><span data-stu-id="78ff8-362">AppService</span></span>

* <span data-ttu-id="78ff8-363">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="78ff8-363">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="78ff8-364">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="78ff8-364">Batch</span></span>

* <span data-ttu-id="78ff8-365">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="78ff8-365">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="78ff8-366">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="78ff8-366">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="78ff8-367">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="78ff8-367">Batch AI</span></span>

* <span data-ttu-id="78ff8-368">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-368">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="78ff8-369">Контейнер</span><span class="sxs-lookup"><span data-stu-id="78ff8-369">Container</span></span>

* <span data-ttu-id="78ff8-370">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="78ff8-370">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="78ff8-371">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="78ff8-371">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-372">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-372">Network</span></span>

* <span data-ttu-id="78ff8-373">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-373">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="78ff8-374">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-374">Added `network nic wait`</span></span>
* <span data-ttu-id="78ff8-375">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="78ff8-375">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="78ff8-376">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="78ff8-376">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="78ff8-377">Ресурс</span><span class="sxs-lookup"><span data-stu-id="78ff8-377">Resource</span></span>

* <span data-ttu-id="78ff8-378">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-378">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="78ff8-379">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-379">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="78ff8-380">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-380">Added `deployment wait` command</span></span>
* <span data-ttu-id="78ff8-381">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="78ff8-381">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="78ff8-382">SQL</span><span class="sxs-lookup"><span data-stu-id="78ff8-382">SQL</span></span>

* <span data-ttu-id="78ff8-383">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-383">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="78ff8-384">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-384">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="78ff8-385">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-385">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-386">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-386">Storage</span></span>

* <span data-ttu-id="78ff8-387">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-387">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-388">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-388">VM</span></span>

* <span data-ttu-id="78ff8-389">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="78ff8-389">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="78ff8-390">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-390">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="78ff8-391">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-391">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="78ff8-392">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-392">July 3, 2018</span></span>

<span data-ttu-id="78ff8-393">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="78ff8-393">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="78ff8-394">AKS</span><span class="sxs-lookup"><span data-stu-id="78ff8-394">AKS</span></span>

* <span data-ttu-id="78ff8-395">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="78ff8-395">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="78ff8-396">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-396">July 3, 2018</span></span>

<span data-ttu-id="78ff8-397">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="78ff8-397">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="78ff8-398">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-398">Core</span></span>

* <span data-ttu-id="78ff8-399">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="78ff8-399">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="78ff8-400">ACR</span><span class="sxs-lookup"><span data-stu-id="78ff8-400">ACR</span></span>

* <span data-ttu-id="78ff8-401">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="78ff8-401">Added polling build status</span></span>
* <span data-ttu-id="78ff8-402">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="78ff8-402">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="78ff8-403">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-403">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-404">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-404">ACS</span></span>

* <span data-ttu-id="78ff8-405">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="78ff8-405">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="78ff8-406">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="78ff8-406">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="78ff8-407">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-407">Updated options for `aks browse` command.</span></span> <span data-ttu-id="78ff8-408">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-408">Added `--listen-port` support</span></span>
* <span data-ttu-id="78ff8-409">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-409">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="78ff8-410">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="78ff8-410">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="78ff8-411">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-411">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-412">AppService</span><span class="sxs-lookup"><span data-stu-id="78ff8-412">AppService</span></span>

* <span data-ttu-id="78ff8-413">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-413">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="78ff8-414">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="78ff8-414">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="78ff8-415">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="78ff8-415">Backup</span></span>

* <span data-ttu-id="78ff8-416">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="78ff8-416">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="78ff8-417">Batch AI</span><span class="sxs-lookup"><span data-stu-id="78ff8-417">BatchAI</span></span>

* <span data-ttu-id="78ff8-418">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-418">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="78ff8-419">Облако</span><span class="sxs-lookup"><span data-stu-id="78ff8-419">Cloud</span></span>

* <span data-ttu-id="78ff8-420">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-420">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="78ff8-421">Контейнер</span><span class="sxs-lookup"><span data-stu-id="78ff8-421">Container</span></span>

* <span data-ttu-id="78ff8-422">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="78ff8-422">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="78ff8-423">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-423">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="78ff8-424">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="78ff8-424">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="78ff8-425">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="78ff8-425">Extension</span></span>

* <span data-ttu-id="78ff8-426">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="78ff8-426">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-427">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-427">Network</span></span>

* <span data-ttu-id="78ff8-428">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-428">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="78ff8-429">Rdbms</span><span class="sxs-lookup"><span data-stu-id="78ff8-429">Rdbms</span></span>

* <span data-ttu-id="78ff8-430">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-430">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="78ff8-431">Ресурс</span><span class="sxs-lookup"><span data-stu-id="78ff8-431">Resource</span></span>

* <span data-ttu-id="78ff8-432">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-432">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-433">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-433">VM</span></span>

* <span data-ttu-id="78ff8-434">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="78ff8-434">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="78ff8-435">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-435">June 25, 2018</span></span>

<span data-ttu-id="78ff8-436">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="78ff8-436">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="78ff8-437">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="78ff8-437">CLI</span></span>

* <span data-ttu-id="78ff8-438">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="78ff8-438">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="78ff8-439">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-439">June 19, 2018</span></span>

<span data-ttu-id="78ff8-440">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="78ff8-440">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="78ff8-441">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-441">Core</span></span>

* <span data-ttu-id="78ff8-442">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="78ff8-442">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="78ff8-443">ACR</span><span class="sxs-lookup"><span data-stu-id="78ff8-443">ACR</span></span>

* <span data-ttu-id="78ff8-444">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-444">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="78ff8-445">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="78ff8-445">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-446">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-446">ACS</span></span>

* <span data-ttu-id="78ff8-447">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-447">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="78ff8-448">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-448">Added `--update` support</span></span>
* <span data-ttu-id="78ff8-449">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-449">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="78ff8-450">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-450">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="78ff8-451">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-451">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="78ff8-452">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-452">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="78ff8-453">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-453">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="78ff8-454">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-454">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-455">AppService</span><span class="sxs-lookup"><span data-stu-id="78ff8-455">AppService</span></span>

* <span data-ttu-id="78ff8-456">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="78ff8-456">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="78ff8-457">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-457">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="78ff8-458">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="78ff8-458">Batch</span></span>

* <span data-ttu-id="78ff8-459">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-459">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="78ff8-460">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="78ff8-460">Batch AI</span></span>

* <span data-ttu-id="78ff8-461">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="78ff8-461">Added support for workspaces.</span></span> <span data-ttu-id="78ff8-462">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-462">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="78ff8-463">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-463">Added support for experiments.</span></span> <span data-ttu-id="78ff8-464">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="78ff8-464">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="78ff8-465">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="78ff8-465">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="78ff8-466">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-466">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="78ff8-467">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-467">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="78ff8-468">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-468">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="78ff8-469">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="78ff8-469">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="78ff8-470">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-470">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="78ff8-471">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-471">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="78ff8-472">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-472">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="78ff8-473">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-473">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="78ff8-474">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-474">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="78ff8-475">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-475">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="78ff8-476">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="78ff8-476">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="78ff8-477">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-477">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="78ff8-478">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="78ff8-478">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="78ff8-479">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="78ff8-479">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="78ff8-480">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="78ff8-480">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="78ff8-481">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="78ff8-481">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="78ff8-482">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="78ff8-482">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="78ff8-483">Карты</span><span class="sxs-lookup"><span data-stu-id="78ff8-483">Maps</span></span>

* <span data-ttu-id="78ff8-484">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-484">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-485">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-485">Network</span></span>

* <span data-ttu-id="78ff8-486">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="78ff8-486">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="78ff8-487">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="78ff8-487">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="78ff8-488">#6502</span><span class="sxs-lookup"><span data-stu-id="78ff8-488">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="78ff8-489">Резервирование</span><span class="sxs-lookup"><span data-stu-id="78ff8-489">Reservations</span></span>

* <span data-ttu-id="78ff8-490">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-490">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="78ff8-491">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-491">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="78ff8-492">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-492">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="78ff8-493">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-493">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="78ff8-494">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-494">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="78ff8-495">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-495">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="78ff8-496">Роль</span><span class="sxs-lookup"><span data-stu-id="78ff8-496">Role</span></span>

* <span data-ttu-id="78ff8-497">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="78ff8-497">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="78ff8-498">SQL</span><span class="sxs-lookup"><span data-stu-id="78ff8-498">SQL</span></span>

* <span data-ttu-id="78ff8-499">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="78ff8-499">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-500">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-500">Storage</span></span>

* <span data-ttu-id="78ff8-501">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="78ff8-501">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-502">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-502">VM</span></span>

* <span data-ttu-id="78ff8-503">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-503">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="78ff8-504">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-504">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="78ff8-505">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="78ff8-505">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="78ff8-506">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-506">June 13, 2018</span></span>

<span data-ttu-id="78ff8-507">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="78ff8-507">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="78ff8-508">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-508">Core</span></span>

* <span data-ttu-id="78ff8-509">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="78ff8-509">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="78ff8-510">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-510">June 13, 2018</span></span>

<span data-ttu-id="78ff8-511">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="78ff8-511">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="78ff8-512">AKS</span><span class="sxs-lookup"><span data-stu-id="78ff8-512">AKS</span></span>

* <span data-ttu-id="78ff8-513">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="78ff8-513">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="78ff8-514">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="78ff8-514">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="78ff8-515">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="78ff8-515">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="78ff8-516">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="78ff8-516">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="78ff8-517">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="78ff8-517">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-518">AppService</span><span class="sxs-lookup"><span data-stu-id="78ff8-518">AppService</span></span>

* <span data-ttu-id="78ff8-519">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="78ff8-519">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="78ff8-520">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-520">June 5, 2018</span></span>

<span data-ttu-id="78ff8-521">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="78ff8-521">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="78ff8-522">Interactive</span><span class="sxs-lookup"><span data-stu-id="78ff8-522">Interactive</span></span>

* <span data-ttu-id="78ff8-523">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="78ff8-523">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="78ff8-524">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-524">June 5, 2018</span></span>

<span data-ttu-id="78ff8-525">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="78ff8-525">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="78ff8-526">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-526">Core</span></span>

* <span data-ttu-id="78ff8-527">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="78ff8-527">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="78ff8-528">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="78ff8-528">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="78ff8-529">ACR</span><span class="sxs-lookup"><span data-stu-id="78ff8-529">ACR</span></span>

* <span data-ttu-id="78ff8-530">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="78ff8-530">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="78ff8-531">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-531">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="78ff8-532">AKS</span><span class="sxs-lookup"><span data-stu-id="78ff8-532">AKS</span></span>

* <span data-ttu-id="78ff8-533">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="78ff8-533">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="78ff8-534">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="78ff8-534">Batch</span></span>

* <span data-ttu-id="78ff8-535">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="78ff8-535">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="78ff8-536">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="78ff8-536">IOT</span></span>

* <span data-ttu-id="78ff8-537">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="78ff8-537">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-538">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-538">Network</span></span>

* <span data-ttu-id="78ff8-539">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-539">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="78ff8-540">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="78ff8-540">Policy Insights</span></span>

* <span data-ttu-id="78ff8-541">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="78ff8-541">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="78ff8-542">ARM</span><span class="sxs-lookup"><span data-stu-id="78ff8-542">ARM</span></span>

* <span data-ttu-id="78ff8-543">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-543">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="78ff8-544">SQL</span><span class="sxs-lookup"><span data-stu-id="78ff8-544">SQL</span></span>

* <span data-ttu-id="78ff8-545">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="78ff8-545">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="78ff8-546">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="78ff8-546">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="78ff8-547">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-547">Storage</span></span>

* <span data-ttu-id="78ff8-548">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-548">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-549">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-549">VM</span></span>

* <span data-ttu-id="78ff8-550">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-550">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="78ff8-551">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-551">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="78ff8-552">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-552">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="78ff8-553">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-553">May 22, 2018</span></span>

<span data-ttu-id="78ff8-554">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="78ff8-554">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="78ff8-555">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-555">Core</span></span>

* <span data-ttu-id="78ff8-556">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-556">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-557">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-557">ACS</span></span>

* <span data-ttu-id="78ff8-558">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-558">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="78ff8-559">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="78ff8-559">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-560">AppService</span><span class="sxs-lookup"><span data-stu-id="78ff8-560">AppService</span></span>

* <span data-ttu-id="78ff8-561">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="78ff8-561">Improved generic update commands</span></span>
* <span data-ttu-id="78ff8-562">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-562">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="78ff8-563">Контейнер</span><span class="sxs-lookup"><span data-stu-id="78ff8-563">Container</span></span>

* <span data-ttu-id="78ff8-564">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="78ff8-564">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="78ff8-565">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="78ff8-565">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="78ff8-566">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="78ff8-566">Extension</span></span>

* <span data-ttu-id="78ff8-567">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="78ff8-567">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="78ff8-568">Interactive</span><span class="sxs-lookup"><span data-stu-id="78ff8-568">Interactive</span></span>

* <span data-ttu-id="78ff8-569">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="78ff8-569">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="78ff8-570">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="78ff8-570">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="78ff8-571">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="78ff8-571">KeyVault</span></span>

* <span data-ttu-id="78ff8-572">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="78ff8-572">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-573">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-573">Network</span></span>

* <span data-ttu-id="78ff8-574">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="78ff8-574">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="78ff8-575">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="78ff8-575">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="78ff8-576">SQL</span><span class="sxs-lookup"><span data-stu-id="78ff8-576">SQL</span></span>

* <span data-ttu-id="78ff8-577">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="78ff8-577">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="78ff8-578">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-578">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="78ff8-579">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-579">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="78ff8-580">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="78ff8-580">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="78ff8-581">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="78ff8-581">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="78ff8-582">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-582">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="78ff8-583">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-583">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="78ff8-584">`edition`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-584">`edition`.</span></span> <span data-ttu-id="78ff8-585">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-585">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="78ff8-586">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-586">`elasticPoolName`.</span></span> <span data-ttu-id="78ff8-587">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-587">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="78ff8-588">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="78ff8-588">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="78ff8-589">`edition`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-589">`edition`.</span></span> <span data-ttu-id="78ff8-590">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-590">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="78ff8-591">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-591">`dtu`.</span></span> <span data-ttu-id="78ff8-592">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-592">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="78ff8-593">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-593">`databaseDtuMin`.</span></span> <span data-ttu-id="78ff8-594">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-594">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="78ff8-595">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-595">`databaseDtuMax`.</span></span> <span data-ttu-id="78ff8-596">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-596">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="78ff8-597">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-597">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="78ff8-598">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-598">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-599">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-599">Storage</span></span>

* <span data-ttu-id="78ff8-600">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-600">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="78ff8-601">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-601">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-602">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-602">VM</span></span>

* <span data-ttu-id="78ff8-603">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-603">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="78ff8-604">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-604">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="78ff8-605">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-605">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="78ff8-606">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="78ff8-606">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="78ff8-607">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-607">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="78ff8-608">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-608">May 7, 2018</span></span>

<span data-ttu-id="78ff8-609">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="78ff8-609">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="78ff8-610">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-610">Core</span></span>

* <span data-ttu-id="78ff8-611">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="78ff8-611">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="78ff8-612">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-612">Added limited support for positional arguments</span></span>
* <span data-ttu-id="78ff8-613">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-613">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="78ff8-614">#5591</span><span class="sxs-lookup"><span data-stu-id="78ff8-614">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="78ff8-615">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-615">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="78ff8-616">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="78ff8-616">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="78ff8-617">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="78ff8-617">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="78ff8-618">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-618">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="78ff8-619">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="78ff8-619">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="78ff8-620">ACR</span><span class="sxs-lookup"><span data-stu-id="78ff8-620">ACR</span></span>

* <span data-ttu-id="78ff8-621">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="78ff8-621">Added ACR Build commands</span></span>
* <span data-ttu-id="78ff8-622">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="78ff8-622">Improved resource not found error messages</span></span>
* <span data-ttu-id="78ff8-623">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="78ff8-623">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="78ff8-624">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="78ff8-624">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="78ff8-625">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="78ff8-625">Improved repository commands error messages</span></span>
* <span data-ttu-id="78ff8-626">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="78ff8-626">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-627">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-627">ACS</span></span>

* <span data-ttu-id="78ff8-628">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="78ff8-628">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="78ff8-629">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="78ff8-629">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="78ff8-630">AMS</span><span class="sxs-lookup"><span data-stu-id="78ff8-630">AMS</span></span>

* <span data-ttu-id="78ff8-631">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="78ff8-631">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-632">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="78ff8-632">Appservice</span></span>

* <span data-ttu-id="78ff8-633">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="78ff8-633">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="78ff8-634">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-634">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="78ff8-635">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="78ff8-635">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="78ff8-636">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="78ff8-636">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="78ff8-637">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="78ff8-637">Batch AI</span></span>

* <span data-ttu-id="78ff8-638">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="78ff8-638">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="78ff8-639">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="78ff8-639">Cognitive Services</span></span>

* <span data-ttu-id="78ff8-640">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="78ff8-640">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="78ff8-641">Потребление</span><span class="sxs-lookup"><span data-stu-id="78ff8-641">Consumption</span></span>

* <span data-ttu-id="78ff8-642">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="78ff8-642">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="78ff8-643">Контейнер</span><span class="sxs-lookup"><span data-stu-id="78ff8-643">Container</span></span>

* <span data-ttu-id="78ff8-644">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="78ff8-644">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="78ff8-645">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="78ff8-645">Cosmos DB</span></span>

* <span data-ttu-id="78ff8-646">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="78ff8-646">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="78ff8-647">DMS</span><span class="sxs-lookup"><span data-stu-id="78ff8-647">DMS</span></span>

* <span data-ttu-id="78ff8-648">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="78ff8-648">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="78ff8-649">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="78ff8-649">Extension</span></span>

* <span data-ttu-id="78ff8-650">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="78ff8-650">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="78ff8-651">Interactive</span><span class="sxs-lookup"><span data-stu-id="78ff8-651">Interactive</span></span>

* <span data-ttu-id="78ff8-652">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="78ff8-652">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="78ff8-653">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="78ff8-653">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="78ff8-654">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="78ff8-654">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="78ff8-655">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="78ff8-655">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="78ff8-656">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="78ff8-656">Lab</span></span>

* <span data-ttu-id="78ff8-657">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="78ff8-657">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-658">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-658">Network</span></span>

* <span data-ttu-id="78ff8-659">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="78ff8-659">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="78ff8-660">Профиль</span><span class="sxs-lookup"><span data-stu-id="78ff8-660">Profile</span></span>

* <span data-ttu-id="78ff8-661">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-661">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="78ff8-662">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="78ff8-662">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="78ff8-663">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-663">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="78ff8-664">Redis</span><span class="sxs-lookup"><span data-stu-id="78ff8-664">Redis</span></span>

* <span data-ttu-id="78ff8-665">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-665">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="78ff8-666">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="78ff8-666">Deprecated `redis list-all`.</span></span> <span data-ttu-id="78ff8-667">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-667">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="78ff8-668">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-668">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="78ff8-669">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="78ff8-669">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="78ff8-670">Роль</span><span class="sxs-lookup"><span data-stu-id="78ff8-670">Role</span></span>

* <span data-ttu-id="78ff8-671">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="78ff8-671">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-672">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-672">Storage</span></span>

* <span data-ttu-id="78ff8-673">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="78ff8-673">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="78ff8-674">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="78ff8-674">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="78ff8-675">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="78ff8-675">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="78ff8-676">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="78ff8-676">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="78ff8-677">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="78ff8-677">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-678">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-678">VM</span></span>

* <span data-ttu-id="78ff8-679">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="78ff8-679">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="78ff8-680">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="78ff8-680">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="78ff8-681">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="78ff8-681">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="78ff8-682">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-682">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="78ff8-683">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="78ff8-683">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="78ff8-684">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="78ff8-684">Added write accelerator support</span></span>
* <span data-ttu-id="78ff8-685">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-685">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="78ff8-686">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="78ff8-686">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="78ff8-687">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="78ff8-687">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="78ff8-688">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-688">April 10, 2018</span></span>

<span data-ttu-id="78ff8-689">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="78ff8-689">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="78ff8-690">ACR</span><span class="sxs-lookup"><span data-stu-id="78ff8-690">ACR</span></span>

* <span data-ttu-id="78ff8-691">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="78ff8-691">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-692">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-692">ACS</span></span>

* <span data-ttu-id="78ff8-693">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="78ff8-693">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-694">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="78ff8-694">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="78ff8-696">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="78ff8-696">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="78ff8-697">Batch AI</span><span class="sxs-lookup"><span data-stu-id="78ff8-697">BatchAI</span></span>

* <span data-ttu-id="78ff8-698">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="78ff8-698">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="78ff8-699">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="78ff8-699">Job level mounting</span></span>
 - <span data-ttu-id="78ff8-700">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-700">Environment variables with secret values</span></span>
 - <span data-ttu-id="78ff8-701">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="78ff8-701">Performance counters settings</span></span>
 - <span data-ttu-id="78ff8-702">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="78ff8-702">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="78ff8-703">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-703">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="78ff8-704">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="78ff8-704">Usage and limits reporting</span></span>
 - <span data-ttu-id="78ff8-705">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-705">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="78ff8-706">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-706">Support for custom images</span></span>
 - <span data-ttu-id="78ff8-707">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="78ff8-707">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="78ff8-708">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="78ff8-708">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="78ff8-709">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-709">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="78ff8-710">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="78ff8-710">National clouds are supported</span></span>
* <span data-ttu-id="78ff8-711">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="78ff8-711">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="78ff8-712">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="78ff8-712">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="78ff8-713">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="78ff8-713">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="78ff8-714">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="78ff8-714">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="78ff8-715">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="78ff8-715">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="78ff8-716">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="78ff8-716">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="78ff8-717">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-717">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="78ff8-718">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="78ff8-718">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="78ff8-719">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="78ff8-719">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="78ff8-720">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-720">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="78ff8-721">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="78ff8-721">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="78ff8-722">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-722">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="78ff8-723">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-723">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="78ff8-724">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="78ff8-724">Billing</span></span>

* <span data-ttu-id="78ff8-725">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="78ff8-725">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="78ff8-726">Потребление</span><span class="sxs-lookup"><span data-stu-id="78ff8-726">Consumption</span></span>

* <span data-ttu-id="78ff8-727">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-727">Added `marketplace` commands</span></span>
* <span data-ttu-id="78ff8-728">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-728">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="78ff8-729">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-729">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="78ff8-730">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-730">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="78ff8-731">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-731">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="78ff8-732">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-732">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="78ff8-733">Контейнер</span><span class="sxs-lookup"><span data-stu-id="78ff8-733">Container</span></span>

* <span data-ttu-id="78ff8-734">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-734">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="78ff8-735">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="78ff8-735">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="78ff8-736">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="78ff8-736">Extension</span></span>

* <span data-ttu-id="78ff8-737">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="78ff8-737">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="78ff8-738">Interactive</span><span class="sxs-lookup"><span data-stu-id="78ff8-738">Interactive</span></span>

* <span data-ttu-id="78ff8-739">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="78ff8-739">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="78ff8-740">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="78ff8-740">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="78ff8-741">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-741">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-742">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-742">Network</span></span>

* <span data-ttu-id="78ff8-743">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-743">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="78ff8-744">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-744">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="78ff8-745">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="78ff8-745">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="78ff8-746">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="78ff8-746">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="78ff8-747">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="78ff8-747">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="78ff8-748">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-748">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="78ff8-749">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-749">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="78ff8-750">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="78ff8-750">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="78ff8-751">Профиль</span><span class="sxs-lookup"><span data-stu-id="78ff8-751">Profile</span></span>

* <span data-ttu-id="78ff8-752">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-752">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="78ff8-753">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-753">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="78ff8-754">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="78ff8-754">RDBMS</span></span>

* <span data-ttu-id="78ff8-755">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-755">Added `georestore` command</span></span>
* <span data-ttu-id="78ff8-756">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="78ff8-756">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="78ff8-757">Ресурс</span><span class="sxs-lookup"><span data-stu-id="78ff8-757">Resource</span></span>

* <span data-ttu-id="78ff8-758">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-758">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="78ff8-759">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-759">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="78ff8-760">SQL</span><span class="sxs-lookup"><span data-stu-id="78ff8-760">SQL</span></span>

* <span data-ttu-id="78ff8-761">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-761">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-762">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-762">Storage</span></span>

* <span data-ttu-id="78ff8-763">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="78ff8-763">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-764">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-764">VM</span></span>

* <span data-ttu-id="78ff8-765">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="78ff8-765">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="78ff8-766">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="78ff8-766">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="78ff8-768">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-768">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="78ff8-769">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="78ff8-769">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="78ff8-770">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="78ff8-770">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="78ff8-771">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="78ff8-771">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="78ff8-772">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-772">March 27, 2018</span></span>

<span data-ttu-id="78ff8-773">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="78ff8-773">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="78ff8-774">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-774">Core</span></span>

* <span data-ttu-id="78ff8-775">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="78ff8-775">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-776">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-776">ACS</span></span>

* <span data-ttu-id="78ff8-777">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="78ff8-777">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-778">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="78ff8-778">Appservice</span></span>

* <span data-ttu-id="78ff8-779">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-779">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="78ff8-780">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-780">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="78ff8-781">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="78ff8-781">Backup</span></span>

* <span data-ttu-id="78ff8-782">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-782">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="78ff8-783">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="78ff8-783">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="78ff8-784">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="78ff8-784">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="78ff8-785">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-785">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="78ff8-786">Контейнер</span><span class="sxs-lookup"><span data-stu-id="78ff8-786">Container</span></span>

* <span data-ttu-id="78ff8-787">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-787">Added `container exec` command.</span></span> <span data-ttu-id="78ff8-788">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="78ff8-788">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="78ff8-789">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="78ff8-789">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="78ff8-790">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="78ff8-790">Extension</span></span>

* <span data-ttu-id="78ff8-791">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="78ff8-791">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="78ff8-792">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-792">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="78ff8-793">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="78ff8-793">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="78ff8-794">Interactive</span><span class="sxs-lookup"><span data-stu-id="78ff8-794">Interactive</span></span>

* <span data-ttu-id="78ff8-795">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="78ff8-795">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="78ff8-796">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-796">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="78ff8-797">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="78ff8-797">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="78ff8-798">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="78ff8-798">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="78ff8-799">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="78ff8-799">Lab</span></span>

* <span data-ttu-id="78ff8-800">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-800">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="78ff8-801">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="78ff8-801">Monitor</span></span>

* <span data-ttu-id="78ff8-802">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="78ff8-802">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="78ff8-803">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="78ff8-803">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="78ff8-804">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="78ff8-804">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-805">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-805">Network</span></span>

* <span data-ttu-id="78ff8-806">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="78ff8-806">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="78ff8-807">Профиль</span><span class="sxs-lookup"><span data-stu-id="78ff8-807">Profile</span></span>

* <span data-ttu-id="78ff8-808">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-808">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="78ff8-809">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="78ff8-809">RDBMS</span></span>

* <span data-ttu-id="78ff8-810">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="78ff8-810">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="78ff8-811">Ресурс</span><span class="sxs-lookup"><span data-stu-id="78ff8-811">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="78ff8-813">Роль</span><span class="sxs-lookup"><span data-stu-id="78ff8-813">Role</span></span>

* <span data-ttu-id="78ff8-814">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-814">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="78ff8-815">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="78ff8-815">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="78ff8-816">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="78ff8-816">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="78ff8-817">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-817">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="78ff8-818">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-818">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-819">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-819">Storage</span></span>

* <span data-ttu-id="78ff8-820">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="78ff8-820">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="78ff8-821">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049): проблемы, когда при отправке добавочного большого двоичного объекта игнорируются параметры условия.</span><span class="sxs-lookup"><span data-stu-id="78ff8-821">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-822">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-822">VM</span></span>

* <span data-ttu-id="78ff8-823">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="78ff8-823">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="78ff8-824">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-824">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="78ff8-825">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="78ff8-825">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="78ff8-826">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="78ff8-826">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="78ff8-827">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-827">March 13, 2018</span></span>

<span data-ttu-id="78ff8-828">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="78ff8-828">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="78ff8-829">ACR</span><span class="sxs-lookup"><span data-stu-id="78ff8-829">ACR</span></span>

* <span data-ttu-id="78ff8-830">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-830">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="78ff8-831">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="78ff8-831">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="78ff8-832">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="78ff8-832">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-833">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-833">ACS</span></span>

* <span data-ttu-id="78ff8-834">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="78ff8-834">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="78ff8-835">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="78ff8-835">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="78ff8-836">Помощник</span><span class="sxs-lookup"><span data-stu-id="78ff8-836">Advisor</span></span>

* <span data-ttu-id="78ff8-837">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-837">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="78ff8-838">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-838">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="78ff8-839">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-839">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="78ff8-840">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-840">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="78ff8-841">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-841">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-842">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="78ff8-842">Appservice</span></span>

* <span data-ttu-id="78ff8-843">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="78ff8-843">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="78ff8-844">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-844">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="78ff8-845">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="78ff8-845">Eventhubs</span></span>

* <span data-ttu-id="78ff8-846">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="78ff8-846">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="78ff8-847">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="78ff8-847">Extension</span></span>

* <span data-ttu-id="78ff8-848">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="78ff8-848">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="78ff8-849">Interactive</span><span class="sxs-lookup"><span data-stu-id="78ff8-849">Interactive</span></span>

* <span data-ttu-id="78ff8-850">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625): теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="78ff8-850">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="78ff8-851">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016): при использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="78ff8-851">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="78ff8-852">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688): если при загрузке таблицы команд возникало исключение, опережающий ввод не выполнялся.</span><span class="sxs-lookup"><span data-stu-id="78ff8-852">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="78ff8-853">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="78ff8-853">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="78ff8-854">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="78ff8-854">Monitor</span></span>

* <span data-ttu-id="78ff8-855">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="78ff8-855">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="78ff8-856">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-856">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="78ff8-857">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-857">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="78ff8-858">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-858">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-859">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-859">Network</span></span>

* <span data-ttu-id="78ff8-860">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-860">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="78ff8-861">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="78ff8-861">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="78ff8-862">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-862">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="78ff8-863">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-863">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="78ff8-864">Профиль</span><span class="sxs-lookup"><span data-stu-id="78ff8-864">Profile</span></span>

* <span data-ttu-id="78ff8-865">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="78ff8-865">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="78ff8-866">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-866">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="78ff8-867">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="78ff8-867">RDBMS</span></span>

* <span data-ttu-id="78ff8-868">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="78ff8-868">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="78ff8-869">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="78ff8-869">Service Bus</span></span>

* <span data-ttu-id="78ff8-870">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="78ff8-870">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-871">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-871">Storage</span></span>

* <span data-ttu-id="78ff8-872">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="78ff8-872">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="78ff8-873">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286): при пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="78ff8-873">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-874">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-874">VM</span></span>

* <span data-ttu-id="78ff8-875">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="78ff8-875">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="78ff8-876">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="78ff8-876">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="78ff8-877">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-877">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="78ff8-878">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="78ff8-878">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="78ff8-879">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="78ff8-879">February 27, 2018</span></span>

<span data-ttu-id="78ff8-880">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="78ff8-880">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="78ff8-881">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-881">Core</span></span>

* <span data-ttu-id="78ff8-882">Исправлена ошибка с установкой Homebrew [#5184](https://github.com/Azure/azure-cli/issues/5184).</span><span class="sxs-lookup"><span data-stu-id="78ff8-882">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="78ff8-883">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="78ff8-883">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="78ff8-884">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-884">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-885">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-885">ACS</span></span>

* <span data-ttu-id="78ff8-886">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="78ff8-886">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="78ff8-887">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="78ff8-887">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="78ff8-888">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-888">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="78ff8-889">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-889">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-890">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="78ff8-890">Appservice</span></span>

* <span data-ttu-id="78ff8-891">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="78ff8-891">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="78ff8-892">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="78ff8-892">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="78ff8-893">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="78ff8-893">Cognitive Services</span></span>

* <span data-ttu-id="78ff8-894">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="78ff8-894">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="78ff8-895">Потребление</span><span class="sxs-lookup"><span data-stu-id="78ff8-895">Consumption</span></span>

* <span data-ttu-id="78ff8-896">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="78ff8-896">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="78ff8-897">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="78ff8-897">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="78ff8-898">Контейнер</span><span class="sxs-lookup"><span data-stu-id="78ff8-898">Container</span></span>

* <span data-ttu-id="78ff8-899">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="78ff8-899">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-900">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-900">Network</span></span>

* <span data-ttu-id="78ff8-901">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559): отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-901">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="78ff8-902">Ресурс</span><span class="sxs-lookup"><span data-stu-id="78ff8-902">Resource</span></span>

* <span data-ttu-id="78ff8-903">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="78ff8-903">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="78ff8-904">Роль</span><span class="sxs-lookup"><span data-stu-id="78ff8-904">Role</span></span>

* <span data-ttu-id="78ff8-905">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="78ff8-905">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="78ff8-906">SQL</span><span class="sxs-lookup"><span data-stu-id="78ff8-906">SQL</span></span>

* <span data-ttu-id="78ff8-907">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-907">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-908">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-908">Storage</span></span>

* <span data-ttu-id="78ff8-909">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-909">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-910">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-910">VM</span></span>

* <span data-ttu-id="78ff8-911">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="78ff8-911">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="78ff8-912">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-912">February 13, 2018</span></span>

<span data-ttu-id="78ff8-913">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="78ff8-913">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="78ff8-914">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-914">Core</span></span>

* <span data-ttu-id="78ff8-915">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="78ff8-915">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-916">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-916">ACS</span></span>

* <span data-ttu-id="78ff8-917">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="78ff8-917">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="78ff8-918">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-918">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="78ff8-919">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="78ff8-919">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="78ff8-920">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="78ff8-920">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="78ff8-921">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="78ff8-921">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="78ff8-922">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-922">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="78ff8-923">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="78ff8-923">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="78ff8-924">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-924">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-925">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="78ff8-925">Appservice</span></span>

* <span data-ttu-id="78ff8-926">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="78ff8-926">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="78ff8-927">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-927">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="78ff8-928">CDN</span><span class="sxs-lookup"><span data-stu-id="78ff8-928">CDN</span></span>

* <span data-ttu-id="78ff8-929">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-929">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="78ff8-930">Контейнер</span><span class="sxs-lookup"><span data-stu-id="78ff8-930">Container</span></span>

* <span data-ttu-id="78ff8-931">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="78ff8-931">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="78ff8-932">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="78ff8-932">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="78ff8-933">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="78ff8-933">CosmosDB</span></span>

* <span data-ttu-id="78ff8-934">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="78ff8-934">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="78ff8-935">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="78ff8-935">Extension</span></span>

* <span data-ttu-id="78ff8-936">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-936">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="78ff8-937">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-937">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="78ff8-938">Отзыв</span><span class="sxs-lookup"><span data-stu-id="78ff8-938">Feedback</span></span>

* <span data-ttu-id="78ff8-939">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="78ff8-939">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="78ff8-940">Interactive</span><span class="sxs-lookup"><span data-stu-id="78ff8-940">Interactive</span></span>

* <span data-ttu-id="78ff8-941">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="78ff8-941">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="78ff8-942">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="78ff8-942">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="78ff8-943">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="78ff8-943">IoT</span></span>

* <span data-ttu-id="78ff8-944">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="78ff8-944">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="78ff8-945">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="78ff8-945">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="78ff8-946">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-946">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="78ff8-947">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="78ff8-947">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="78ff8-948">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="78ff8-948">Monitor</span></span>

* <span data-ttu-id="78ff8-949">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-949">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-950">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-950">Network</span></span>

* <span data-ttu-id="78ff8-951">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="78ff8-951">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="78ff8-952">Профиль</span><span class="sxs-lookup"><span data-stu-id="78ff8-952">Profile</span></span>

* <span data-ttu-id="78ff8-953">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="78ff8-953">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="78ff8-954">Ресурс</span><span class="sxs-lookup"><span data-stu-id="78ff8-954">Resource</span></span>

* <span data-ttu-id="78ff8-955">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-955">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="78ff8-956">Роль</span><span class="sxs-lookup"><span data-stu-id="78ff8-956">Role</span></span>

* <span data-ttu-id="78ff8-957">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="78ff8-957">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="78ff8-958">SQL</span><span class="sxs-lookup"><span data-stu-id="78ff8-958">SQL</span></span>

* <span data-ttu-id="78ff8-959">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-959">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="78ff8-960">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-960">Added `sql db rename`</span></span>
* <span data-ttu-id="78ff8-961">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="78ff8-961">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-962">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-962">Storage</span></span>

* <span data-ttu-id="78ff8-963">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="78ff8-963">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-964">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-964">VM</span></span>

* <span data-ttu-id="78ff8-965">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="78ff8-965">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="78ff8-966">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="78ff8-966">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="78ff8-967">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="78ff8-967">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="78ff8-968">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-968">January 31, 2018</span></span>

<span data-ttu-id="78ff8-969">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="78ff8-969">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="78ff8-970">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-970">Core</span></span>

* <span data-ttu-id="78ff8-971">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="78ff8-971">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="78ff8-972">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="78ff8-972">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="78ff8-973">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="78ff8-973">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="78ff8-974">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="78ff8-974">Use `--verbose` to see</span></span>
* <span data-ttu-id="78ff8-975">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="78ff8-975">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-976">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-976">ACS</span></span>

* <span data-ttu-id="78ff8-977">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-977">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="78ff8-978">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-978">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-979">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="78ff8-979">Appservice</span></span>

* <span data-ttu-id="78ff8-980">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="78ff8-980">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="78ff8-981">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="78ff8-981">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="78ff8-982">CDN</span><span class="sxs-lookup"><span data-stu-id="78ff8-982">CDN</span></span>

* <span data-ttu-id="78ff8-983">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-983">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="78ff8-984">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="78ff8-984">CosmosDB</span></span>

* <span data-ttu-id="78ff8-985">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="78ff8-985">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="78ff8-986">Interactive</span><span class="sxs-lookup"><span data-stu-id="78ff8-986">Interactive</span></span>

* <span data-ttu-id="78ff8-987">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="78ff8-987">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-988">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-988">Network</span></span>

* <span data-ttu-id="78ff8-989">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-989">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="78ff8-990">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="78ff8-990">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="78ff8-991">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-991">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="78ff8-992">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-992">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="78ff8-993">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-993">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="78ff8-994">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="78ff8-994">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="78ff8-995">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="78ff8-995">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="78ff8-996">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="78ff8-996">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="78ff8-997">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-997">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="78ff8-998">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-998">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="78ff8-999">Профиль</span><span class="sxs-lookup"><span data-stu-id="78ff8-999">Profile</span></span>

* <span data-ttu-id="78ff8-1000">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1000">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="78ff8-1001">Ресурс</span><span class="sxs-lookup"><span data-stu-id="78ff8-1001">Resource</span></span>

* <span data-ttu-id="78ff8-1002">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1002">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-1003">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-1003">Storage</span></span>

* <span data-ttu-id="78ff8-1004">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1004">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="78ff8-1005">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1005">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="78ff8-1006">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1006">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="78ff8-1007">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1007">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="78ff8-1008">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1008">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-1009">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-1009">VM</span></span>

* <span data-ttu-id="78ff8-1010">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1010">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="78ff8-1011">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1011">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="78ff8-1012">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1012">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="78ff8-1013">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1013">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="78ff8-1014">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1014">January 17, 2018</span></span>

<span data-ttu-id="78ff8-1015">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="78ff8-1015">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="78ff8-1016">ACR</span><span class="sxs-lookup"><span data-stu-id="78ff8-1016">ACR</span></span>

* <span data-ttu-id="78ff8-1017">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1017">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="78ff8-1018">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1018">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-1019">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-1019">ACS</span></span>

* <span data-ttu-id="78ff8-1020">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1020">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="78ff8-1021">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1021">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-1022">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="78ff8-1022">Appservice</span></span>

* <span data-ttu-id="78ff8-1023">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1023">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="78ff8-1024">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1024">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="78ff8-1025">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1025">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="78ff8-1026">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="78ff8-1026">Backup</span></span>

* <span data-ttu-id="78ff8-1027">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1027">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="78ff8-1028">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1028">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="78ff8-1029">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1029">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="78ff8-1030">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1030">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="78ff8-1031">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1031">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="78ff8-1032">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="78ff8-1032">Batch</span></span>

* <span data-ttu-id="78ff8-1033">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1033">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="78ff8-1034">Облако</span><span class="sxs-lookup"><span data-stu-id="78ff8-1034">Cloud</span></span>

* <span data-ttu-id="78ff8-1035">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1035">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="78ff8-1036">Потребление</span><span class="sxs-lookup"><span data-stu-id="78ff8-1036">Consumption</span></span>

* <span data-ttu-id="78ff8-1037">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1037">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="78ff8-1038">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="78ff8-1038">Event Grid</span></span>

* <span data-ttu-id="78ff8-1039">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1039">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="78ff8-1040">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1040">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="78ff8-1041">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1041">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="78ff8-1042">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1042">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="78ff8-1043">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1043">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="78ff8-1044">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1044">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="78ff8-1045">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1045">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="78ff8-1046">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1046">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="78ff8-1047">Interactive</span><span class="sxs-lookup"><span data-stu-id="78ff8-1047">Interactive</span></span>

* <span data-ttu-id="78ff8-1048">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1048">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="78ff8-1049">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1049">Fixed errors on startup</span></span>
* <span data-ttu-id="78ff8-1050">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1050">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="78ff8-1051">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="78ff8-1051">IoT</span></span>

* <span data-ttu-id="78ff8-1052">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1052">Added support for device provisioning service</span></span>
* <span data-ttu-id="78ff8-1053">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1053">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="78ff8-1054">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1054">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="78ff8-1055">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="78ff8-1055">Monitor</span></span>

* <span data-ttu-id="78ff8-1056">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1056">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="78ff8-1057">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1057">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="78ff8-1058">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1058">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-1059">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-1059">Network</span></span>

* <span data-ttu-id="78ff8-1060">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1060">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="78ff8-1061">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1061">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="78ff8-1062">Профиль</span><span class="sxs-lookup"><span data-stu-id="78ff8-1062">Profile</span></span>

* <span data-ttu-id="78ff8-1063">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1063">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="78ff8-1064">Роль</span><span class="sxs-lookup"><span data-stu-id="78ff8-1064">Role</span></span>

* <span data-ttu-id="78ff8-1065">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1065">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="78ff8-1066">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="78ff8-1066">Service Fabric</span></span>

* <span data-ttu-id="78ff8-1067">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1067">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="78ff8-1068">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1068">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-1069">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-1069">VM</span></span>

* <span data-ttu-id="78ff8-1070">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1070">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="78ff8-1071">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="78ff8-1071">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="78ff8-1072">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1072">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="78ff8-1073">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1073">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="78ff8-1074">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1074">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="78ff8-1075">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1075">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="78ff8-1076">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1076">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="78ff8-1077">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1077">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="78ff8-1078">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1078">December 19, 2017</span></span>

<span data-ttu-id="78ff8-1079">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="78ff8-1079">Version 2.0.23</span></span>

* <span data-ttu-id="78ff8-1080">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1080">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="78ff8-1081">Контейнер</span><span class="sxs-lookup"><span data-stu-id="78ff8-1081">Container</span></span>

* <span data-ttu-id="78ff8-1082">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1082">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-1083">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-1083">Network</span></span>

* <span data-ttu-id="78ff8-1084">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1084">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="78ff8-1085">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1085">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-1086">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-1086">Storage</span></span>

* <span data-ttu-id="78ff8-1087">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1087">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-1088">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-1088">VM</span></span>

* <span data-ttu-id="78ff8-1089">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1089">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="78ff8-1090">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1090">December 5, 2017</span></span>

<span data-ttu-id="78ff8-1091">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="78ff8-1091">Version 2.0.22</span></span>

* <span data-ttu-id="78ff8-1092">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1092">Removed `az component` commands.</span></span> <span data-ttu-id="78ff8-1093">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1093">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="78ff8-1094">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-1094">Core</span></span>
* <span data-ttu-id="78ff8-1095">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1095">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="78ff8-1096">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1096">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-1097">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-1097">ACS</span></span>

* <span data-ttu-id="78ff8-1098">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1098">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="78ff8-1099">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1099">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="78ff8-1100">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1100">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="78ff8-1101">Помощник</span><span class="sxs-lookup"><span data-stu-id="78ff8-1101">Advisor</span></span>

* <span data-ttu-id="78ff8-1102">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="78ff8-1102">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-1103">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="78ff8-1103">Appservice</span></span>

* <span data-ttu-id="78ff8-1104">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1104">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="78ff8-1105">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1105">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="78ff8-1106">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1106">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="78ff8-1107">Потребление</span><span class="sxs-lookup"><span data-stu-id="78ff8-1107">Consumption</span></span>

* <span data-ttu-id="78ff8-1108">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1108">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="78ff8-1109">Контейнер</span><span class="sxs-lookup"><span data-stu-id="78ff8-1109">Container</span></span>

* <span data-ttu-id="78ff8-1110">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1110">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="78ff8-1111">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="78ff8-1111">Monitor</span></span>

* <span data-ttu-id="78ff8-1112">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1112">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="78ff8-1113">Ресурс</span><span class="sxs-lookup"><span data-stu-id="78ff8-1113">Resource</span></span>

* <span data-ttu-id="78ff8-1114">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1114">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="78ff8-1115">Роль</span><span class="sxs-lookup"><span data-stu-id="78ff8-1115">Role</span></span>

* <span data-ttu-id="78ff8-1116">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1116">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="78ff8-1117">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1117">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="78ff8-1118">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1118">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="78ff8-1119">SQL</span><span class="sxs-lookup"><span data-stu-id="78ff8-1119">SQL</span></span>

* <span data-ttu-id="78ff8-1120">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1120">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="78ff8-1121">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1121">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-1122">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-1122">VM</span></span>

* <span data-ttu-id="78ff8-1123">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1123">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="78ff8-1124">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1124">November 14, 2017</span></span>

<span data-ttu-id="78ff8-1125">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="78ff8-1125">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="78ff8-1126">ACR</span><span class="sxs-lookup"><span data-stu-id="78ff8-1126">ACR</span></span>

* <span data-ttu-id="78ff8-1127">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1127">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="78ff8-1128">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-1128">ACS</span></span>

* <span data-ttu-id="78ff8-1129">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1129">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="78ff8-1130">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1130">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="78ff8-1131">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1131">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="78ff8-1132">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1132">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="78ff8-1133">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1133">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-1134">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="78ff8-1134">Appservice</span></span>

* <span data-ttu-id="78ff8-1135">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1135">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="78ff8-1136">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1136">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="78ff8-1137">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1137">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="78ff8-1138">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1138">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="78ff8-1139">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="78ff8-1139">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="78ff8-1140">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1140">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="78ff8-1141">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="78ff8-1141">Batch</span></span>

* <span data-ttu-id="78ff8-1142">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1142">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="78ff8-1143">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="78ff8-1143">Batchai</span></span>

* <span data-ttu-id="78ff8-1144">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1144">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="78ff8-1145">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1145">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="78ff8-1146">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1146">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="78ff8-1147">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1147">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="78ff8-1148">Облако</span><span class="sxs-lookup"><span data-stu-id="78ff8-1148">Cloud</span></span>

* <span data-ttu-id="78ff8-1149">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1149">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="78ff8-1150">Контейнер</span><span class="sxs-lookup"><span data-stu-id="78ff8-1150">Container</span></span>

* <span data-ttu-id="78ff8-1151">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1151">Added support to open multiple ports</span></span>
* <span data-ttu-id="78ff8-1152">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1152">Added container group restart policy</span></span>
* <span data-ttu-id="78ff8-1153">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1153">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="78ff8-1154">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1154">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="78ff8-1155">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="78ff8-1155">Data Lake Analytics</span></span>

* <span data-ttu-id="78ff8-1156">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1156">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="78ff8-1157">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="78ff8-1157">Data Lake Store</span></span>

* <span data-ttu-id="78ff8-1158">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1158">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="78ff8-1159">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="78ff8-1159">Extension</span></span>

* <span data-ttu-id="78ff8-1160">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1160">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="78ff8-1161">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1161">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="78ff8-1162">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="78ff8-1162">IoT</span></span>

* <span data-ttu-id="78ff8-1163">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1163">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="78ff8-1164">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="78ff8-1164">Monitor</span></span>

* <span data-ttu-id="78ff8-1165">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1165">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-1166">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-1166">Network</span></span>

* <span data-ttu-id="78ff8-1167">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1167">Added support for CAA DNS records</span></span>
* <span data-ttu-id="78ff8-1168">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1168">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="78ff8-1169">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1169">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="78ff8-1170">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1170">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="78ff8-1171">Резервирование</span><span class="sxs-lookup"><span data-stu-id="78ff8-1171">Reservations</span></span>

* <span data-ttu-id="78ff8-1172">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="78ff8-1172">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="78ff8-1173">Ресурс</span><span class="sxs-lookup"><span data-stu-id="78ff8-1173">Resource</span></span>

* <span data-ttu-id="78ff8-1174">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1174">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="78ff8-1175">SQL</span><span class="sxs-lookup"><span data-stu-id="78ff8-1175">SQL</span></span>

* <span data-ttu-id="78ff8-1176">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1176">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-1177">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-1177">Storage</span></span>

* <span data-ttu-id="78ff8-1178">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1178">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="78ff8-1179">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1179">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="78ff8-1180">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1180">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="78ff8-1181">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1181">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="78ff8-1182">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1182">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="78ff8-1183">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1183">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="78ff8-1184">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1184">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-1185">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-1185">VM</span></span>

* <span data-ttu-id="78ff8-1186">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1186">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="78ff8-1187">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1187">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="78ff8-1188">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1188">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="78ff8-1189">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1189">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="78ff8-1190">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1190">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="78ff8-1191">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1191">October 24, 2017</span></span>

<span data-ttu-id="78ff8-1192">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="78ff8-1192">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="78ff8-1193">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-1193">Core</span></span>

* <span data-ttu-id="78ff8-1194">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1194">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="78ff8-1195">ACR</span><span class="sxs-lookup"><span data-stu-id="78ff8-1195">ACR</span></span>

* <span data-ttu-id="78ff8-1196">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1196">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="78ff8-1197">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="78ff8-1197">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="78ff8-1198">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="78ff8-1198">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-1199">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-1199">ACS</span></span>

* <span data-ttu-id="78ff8-1200">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1200">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="78ff8-1201">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1201">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-1202">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="78ff8-1202">Appservice</span></span>

* <span data-ttu-id="78ff8-1203">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1203">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="78ff8-1204">Компонент</span><span class="sxs-lookup"><span data-stu-id="78ff8-1204">Component</span></span>

* <span data-ttu-id="78ff8-1205">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="78ff8-1205">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="78ff8-1206">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="78ff8-1206">Monitor</span></span>

* <span data-ttu-id="78ff8-1207">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1207">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="78ff8-1208">Ресурс</span><span class="sxs-lookup"><span data-stu-id="78ff8-1208">Resource</span></span>

* <span data-ttu-id="78ff8-1209">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1209">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="78ff8-1210">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="78ff8-1210">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-1211">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-1211">VM</span></span>

* <span data-ttu-id="78ff8-1212">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1212">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="78ff8-1213">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1213">October 9, 2017</span></span>

<span data-ttu-id="78ff8-1214">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="78ff8-1214">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="78ff8-1215">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-1215">Core</span></span>

* <span data-ttu-id="78ff8-1216">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1216">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-1217">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="78ff8-1217">Appservice</span></span>

* <span data-ttu-id="78ff8-1218">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1218">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="78ff8-1219">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="78ff8-1219">Batch</span></span>

* <span data-ttu-id="78ff8-1220">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="78ff8-1220">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="78ff8-1221">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1221">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="78ff8-1222">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1222">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="78ff8-1223">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1223">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="78ff8-1224">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="78ff8-1224">Batchai</span></span>

* <span data-ttu-id="78ff8-1225">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="78ff8-1225">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="78ff8-1226">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="78ff8-1226">Keyvault</span></span>

* <span data-ttu-id="78ff8-1227">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1227">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="78ff8-1228">(#4448)</span><span class="sxs-lookup"><span data-stu-id="78ff8-1228">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="78ff8-1229">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-1229">Network</span></span>

* <span data-ttu-id="78ff8-1230">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1230">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="78ff8-1231">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1231">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="78ff8-1232">Ресурс</span><span class="sxs-lookup"><span data-stu-id="78ff8-1232">Resource</span></span>

* <span data-ttu-id="78ff8-1233">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1233">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="78ff8-1234">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1234">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="78ff8-1235">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1235">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="78ff8-1236">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1236">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="78ff8-1237">SQL</span><span class="sxs-lookup"><span data-stu-id="78ff8-1237">Sql</span></span>

* <span data-ttu-id="78ff8-1238">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1238">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="78ff8-1239">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1239">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="78ff8-1240">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1240">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-1241">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-1241">Storage</span></span>

* <span data-ttu-id="78ff8-1242">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1242">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-1243">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="78ff8-1243">Vm</span></span>

* <span data-ttu-id="78ff8-1244">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1244">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="78ff8-1245">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1245">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="78ff8-1246">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1246">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="78ff8-1247">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1247">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="78ff8-1248">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1248">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="78ff8-1249">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1249">September 22, 2017</span></span>

<span data-ttu-id="78ff8-1250">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="78ff8-1250">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="78ff8-1251">Ресурс</span><span class="sxs-lookup"><span data-stu-id="78ff8-1251">Resource</span></span>

* <span data-ttu-id="78ff8-1252">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="78ff8-1252">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="78ff8-1253">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="78ff8-1253">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="78ff8-1254">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1254">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="78ff8-1255">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1255">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-1256">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-1256">Network</span></span>

* <span data-ttu-id="78ff8-1257">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1257">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="78ff8-1258">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1258">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="78ff8-1259">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1259">Added `asg` application security group commands</span></span>
* <span data-ttu-id="78ff8-1260">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1260">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="78ff8-1261">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1261">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="78ff8-1262">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1262">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="78ff8-1263">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1263">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-1264">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-1264">Storage</span></span>

* <span data-ttu-id="78ff8-1265">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="78ff8-1265">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="78ff8-1266">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="78ff8-1266">Eventgrid</span></span>

* <span data-ttu-id="78ff8-1267">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="78ff8-1267">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="78ff8-1268">SQL</span><span class="sxs-lookup"><span data-stu-id="78ff8-1268">SQL</span></span>

* <span data-ttu-id="78ff8-1269">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1269">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="78ff8-1270">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="78ff8-1270">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="78ff8-1271">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1271">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="78ff8-1272">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="78ff8-1272">Keyvault</span></span>

* <span data-ttu-id="78ff8-1273">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="78ff8-1273">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-1274">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-1274">VM</span></span>

* <span data-ttu-id="78ff8-1275">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1275">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="78ff8-1276">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="78ff8-1276">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="78ff8-1277">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1277">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="78ff8-1278">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1278">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="78ff8-1279">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1279">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="78ff8-1280">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1280">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-1281">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-1281">ACS</span></span>

* <span data-ttu-id="78ff8-1282">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="78ff8-1282">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-1283">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="78ff8-1283">Appservice</span></span>

* <span data-ttu-id="78ff8-1284">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="78ff8-1284">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="78ff8-1285">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="78ff8-1285">Backup</span></span>

* <span data-ttu-id="78ff8-1286">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1286">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="78ff8-1287">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1287">September 11, 2017</span></span>

<span data-ttu-id="78ff8-1288">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="78ff8-1288">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="78ff8-1289">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-1289">Core</span></span>

* <span data-ttu-id="78ff8-1290">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1290">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="78ff8-1291">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1291">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-1292">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-1292">Acs</span></span>

* <span data-ttu-id="78ff8-1293">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1293">Added `acs list-locations` command</span></span>
* <span data-ttu-id="78ff8-1294">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1294">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-1295">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="78ff8-1295">Appservice</span></span>

* <span data-ttu-id="78ff8-1296">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1296">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="78ff8-1297">CDN</span><span class="sxs-lookup"><span data-stu-id="78ff8-1297">CDN</span></span>

* <span data-ttu-id="78ff8-1298">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1298">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="78ff8-1299">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="78ff8-1299">Extension</span></span>

* <span data-ttu-id="78ff8-1300">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="78ff8-1300">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="78ff8-1301">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="78ff8-1301">Keyvault</span></span>

* <span data-ttu-id="78ff8-1302">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1302">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-1303">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-1303">Network</span></span>

* <span data-ttu-id="78ff8-1304">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1304">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="78ff8-1305">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1305">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="78ff8-1306">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1306">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="78ff8-1307">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1307">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="78ff8-1308">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1308">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="78ff8-1309">Ресурс</span><span class="sxs-lookup"><span data-stu-id="78ff8-1309">Resource</span></span>

* <span data-ttu-id="78ff8-1310">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1310">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="78ff8-1311">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1311">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="78ff8-1312">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1312">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="78ff8-1313">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1313">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="78ff8-1314">SQL</span><span class="sxs-lookup"><span data-stu-id="78ff8-1314">SQL</span></span>

* <span data-ttu-id="78ff8-1315">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1315">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-1316">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-1316">VM</span></span>

* <span data-ttu-id="78ff8-1317">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1317">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="78ff8-1318">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1318">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="78ff8-1319">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1319">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="78ff8-1320">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1320">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="78ff8-1321">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1321">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="78ff8-1322">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1322">August 31, 2017</span></span>

<span data-ttu-id="78ff8-1323">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="78ff8-1323">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="78ff8-1324">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="78ff8-1324">Keyvault</span></span>

* <span data-ttu-id="78ff8-1325">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1325">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="78ff8-1326">Sf</span><span class="sxs-lookup"><span data-stu-id="78ff8-1326">Sf</span></span>

* <span data-ttu-id="78ff8-1327">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1327">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-1328">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-1328">Storage</span></span>

* <span data-ttu-id="78ff8-1329">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1329">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="78ff8-1330">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1330">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="78ff8-1331">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1331">August 28, 2017</span></span>

<span data-ttu-id="78ff8-1332">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="78ff8-1332">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="78ff8-1333">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="78ff8-1333">CLI</span></span>

* <span data-ttu-id="78ff8-1334">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1334">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-1335">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-1335">ACS</span></span>

* <span data-ttu-id="78ff8-1336">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1336">Corrected preview regions</span></span>
* <span data-ttu-id="78ff8-1337">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1337">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="78ff8-1338">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1338">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-1339">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="78ff8-1339">Appservice</span></span>

* <span data-ttu-id="78ff8-1340">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1340">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="78ff8-1341">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1341">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="78ff8-1342">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1342">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="78ff8-1343">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1343">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="78ff8-1344">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1344">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="78ff8-1345">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="78ff8-1345">IoT</span></span>

* <span data-ttu-id="78ff8-1346">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1346">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-1347">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-1347">Network</span></span>

* <span data-ttu-id="78ff8-1348">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1348">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="78ff8-1349">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1349">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="78ff8-1350">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1350">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="78ff8-1351">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1351">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="78ff8-1352">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1352">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="78ff8-1353">Профиль</span><span class="sxs-lookup"><span data-stu-id="78ff8-1353">Profile</span></span>

* <span data-ttu-id="78ff8-1354">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1354">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="78ff8-1355">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="78ff8-1355">Service Fabric</span></span>

* <span data-ttu-id="78ff8-1356">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1356">Preview release</span></span>
* <span data-ttu-id="78ff8-1357">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1357">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="78ff8-1358">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1358">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="78ff8-1359">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1359">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-1360">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-1360">Storage</span></span>

* <span data-ttu-id="78ff8-1361">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1361">Enabled setting blob tier</span></span>
* <span data-ttu-id="78ff8-1362">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1362">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="78ff8-1363">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1363">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="78ff8-1364">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1364">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="78ff8-1365">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1365">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="78ff8-1366">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1366">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-1367">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-1367">VM</span></span>

* <span data-ttu-id="78ff8-1368">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1368">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="78ff8-1369">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1369">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="78ff8-1370">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1370">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="78ff8-1371">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1371">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="78ff8-1372">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1372">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="78ff8-1373">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1373">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="78ff8-1374">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1374">August 15, 2017</span></span>

<span data-ttu-id="78ff8-1375">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="78ff8-1375">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-1376">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-1376">ACS</span></span>

* <span data-ttu-id="78ff8-1377">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1377">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-1378">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="78ff8-1378">Appservice</span></span>

* <span data-ttu-id="78ff8-1379">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1379">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="78ff8-1380">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="78ff8-1380">Event Grid</span></span>

* <span data-ttu-id="78ff8-1381">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1381">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="78ff8-1382">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1382">August 11, 2017</span></span>

<span data-ttu-id="78ff8-1383">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="78ff8-1383">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-1384">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-1384">ACS</span></span>

* <span data-ttu-id="78ff8-1385">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1385">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="78ff8-1386">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="78ff8-1386">Batch</span></span>

* <span data-ttu-id="78ff8-1387">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1387">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="78ff8-1388">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1388">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="78ff8-1389">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1389">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="78ff8-1390">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1390">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="78ff8-1391">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1391">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="78ff8-1392">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1392">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="78ff8-1393">Компонент</span><span class="sxs-lookup"><span data-stu-id="78ff8-1393">Component</span></span>

* <span data-ttu-id="78ff8-1394">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1394">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="78ff8-1395">Контейнер</span><span class="sxs-lookup"><span data-stu-id="78ff8-1395">Container</span></span>

* <span data-ttu-id="78ff8-1396">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1396">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="78ff8-1397">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="78ff8-1397">Data Lake Store</span></span>

* <span data-ttu-id="78ff8-1398">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1398">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="78ff8-1399">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="78ff8-1399">Event Grid</span></span>

* <span data-ttu-id="78ff8-1400">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="78ff8-1400">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-1401">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-1401">Network</span></span>

* <span data-ttu-id="78ff8-1402">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1402">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="78ff8-1403">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1403">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="78ff8-1404">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1404">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="78ff8-1405">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1405">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="78ff8-1406">Профиль</span><span class="sxs-lookup"><span data-stu-id="78ff8-1406">Profile</span></span>

* <span data-ttu-id="78ff8-1407">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1407">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-1408">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-1408">Storage</span></span>

* <span data-ttu-id="78ff8-1409">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1409">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-1410">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-1410">VM</span></span>

* <span data-ttu-id="78ff8-1411">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1411">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="78ff8-1412">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1412">Exposed `list-skus` command</span></span>
* <span data-ttu-id="78ff8-1413">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1413">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="78ff8-1414">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1414">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="78ff8-1415">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1415">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="78ff8-1416">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1416">July 28, 2017</span></span>

<span data-ttu-id="78ff8-1417">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="78ff8-1417">Version 2.0.12</span></span>

* <span data-ttu-id="78ff8-1418">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1418">Added container commands</span></span>
* <span data-ttu-id="78ff8-1419">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1419">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="78ff8-1420">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-1420">Core</span></span>

* <span data-ttu-id="78ff8-1421">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1421">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="78ff8-1422">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1422">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="78ff8-1423">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1423">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="78ff8-1424">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1424">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="78ff8-1425">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1425">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="78ff8-1426">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1426">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="78ff8-1427">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1427">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="78ff8-1428">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1428">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="78ff8-1429">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1429">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="78ff8-1430">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1430">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="78ff8-1431">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1431">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="78ff8-1432">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1432">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="78ff8-1433">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1433">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="78ff8-1434">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1434">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="78ff8-1435">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1435">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="78ff8-1436">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1436">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="78ff8-1437">ACR</span><span class="sxs-lookup"><span data-stu-id="78ff8-1437">ACR</span></span>

* <span data-ttu-id="78ff8-1438">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1438">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="78ff8-1439">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1439">Support SKU update for managed registries</span></span>
* <span data-ttu-id="78ff8-1440">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1440">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="78ff8-1441">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1441">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="78ff8-1442">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1442">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="78ff8-1443">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1443">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-1444">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-1444">ACS</span></span>

* <span data-ttu-id="78ff8-1445">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1445">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-1446">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="78ff8-1446">Appservice</span></span>

* <span data-ttu-id="78ff8-1447">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1447">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="78ff8-1448">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1448">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="78ff8-1449">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1449">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="78ff8-1450">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1450">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="78ff8-1451">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1451">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="78ff8-1452">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1452">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="78ff8-1453">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1453">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="78ff8-1454">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1454">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="78ff8-1455">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1455">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="78ff8-1456">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1456">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="78ff8-1457">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="78ff8-1457">Batch</span></span>

* <span data-ttu-id="78ff8-1458">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1458">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="78ff8-1459">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1459">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="78ff8-1460">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1460">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="78ff8-1461">CDN</span><span class="sxs-lookup"><span data-stu-id="78ff8-1461">CDN</span></span>

* <span data-ttu-id="78ff8-1462">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1462">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="78ff8-1463">Облако</span><span class="sxs-lookup"><span data-stu-id="78ff8-1463">Cloud</span></span>

* <span data-ttu-id="78ff8-1464">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1464">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="78ff8-1465">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1465">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="78ff8-1466">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1466">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="78ff8-1467">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1467">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="78ff8-1468">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1468">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="78ff8-1469">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="78ff8-1469">CosmosDB</span></span>

* <span data-ttu-id="78ff8-1470">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1470">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="78ff8-1471">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1471">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="78ff8-1472">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="78ff8-1472">Data Lake Analytics</span></span>

* <span data-ttu-id="78ff8-1473">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1473">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="78ff8-1474">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1474">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="78ff8-1475">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1475">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="78ff8-1476">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="78ff8-1476">Data Lake Store</span></span>

* <span data-ttu-id="78ff8-1477">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1477">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="78ff8-1478">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1478">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="78ff8-1479">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1479">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="78ff8-1480">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1480">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="78ff8-1481">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="78ff8-1481">Interactive</span></span>

* <span data-ttu-id="78ff8-1482">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1482">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="78ff8-1483">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1483">Increased test coverage</span></span>
* <span data-ttu-id="78ff8-1484">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1484">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="78ff8-1485">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1485">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="78ff8-1486">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1486">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="78ff8-1487">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1487">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="78ff8-1488">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1488">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="78ff8-1489">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1489">Added `--progress` flag</span></span>
* <span data-ttu-id="78ff8-1490">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1490">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="78ff8-1491">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1491">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="78ff8-1492">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="78ff8-1492">IoT</span></span>

* <span data-ttu-id="78ff8-1493">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="78ff8-1493">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="78ff8-1494">(3934).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1494">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="78ff8-1495">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="78ff8-1495">Key vault</span></span>

* <span data-ttu-id="78ff8-1496">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="78ff8-1496">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="78ff8-1497">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1497">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="78ff8-1498">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="78ff8-1498">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="78ff8-1499">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="78ff8-1499">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="78ff8-1500">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1500">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="78ff8-1501">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1501">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="78ff8-1502">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="78ff8-1502">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="78ff8-1503">(3307).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1503">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="78ff8-1504">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="78ff8-1504">Lab</span></span>

* <span data-ttu-id="78ff8-1505">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1505">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="78ff8-1506">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1506">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="78ff8-1507">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="78ff8-1507">Monitor</span></span>

* <span data-ttu-id="78ff8-1508">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1508">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="78ff8-1509">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1509">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="78ff8-1510">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1510">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="78ff8-1511">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1511">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="78ff8-1512">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1512">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="78ff8-1513">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="78ff8-1513">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="78ff8-1514">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="78ff8-1514">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="78ff8-1515">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="78ff8-1515">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="78ff8-1516">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="78ff8-1516">`location` no longer required</span></span>
  * <span data-ttu-id="78ff8-1517">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="78ff8-1517">Add name and ID support for target</span></span>
  * <span data-ttu-id="78ff8-1518">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="78ff8-1518">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="78ff8-1519">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="78ff8-1519">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="78ff8-1520">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="78ff8-1520">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="78ff8-1521">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1521">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="78ff8-1522">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1522">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="78ff8-1523">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1523">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-1524">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-1524">Network</span></span>

* <span data-ttu-id="78ff8-1525">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1525">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="78ff8-1526">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1526">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="78ff8-1527">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1527">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="78ff8-1528">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1528">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="78ff8-1529">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1529">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="78ff8-1530">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1530">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="78ff8-1531">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1531">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="78ff8-1532">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1532">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="78ff8-1533">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1533">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="78ff8-1534">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1534">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="78ff8-1535">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1535">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="78ff8-1536">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1536">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="78ff8-1537">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1537">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="78ff8-1538">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1538">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="78ff8-1539">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1539">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="78ff8-1540">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1540">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="78ff8-1541">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1541">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="78ff8-1542">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1542">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="78ff8-1543">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1543">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="78ff8-1544">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1544">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="78ff8-1545">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1545">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="78ff8-1546">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1546">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="78ff8-1547">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1547">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="78ff8-1548">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1548">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="78ff8-1549">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1549">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="78ff8-1550">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1550">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="78ff8-1551">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1551">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="78ff8-1552">Профиль</span><span class="sxs-lookup"><span data-stu-id="78ff8-1552">Profile</span></span>

* <span data-ttu-id="78ff8-1553">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1553">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="78ff8-1554">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1554">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="78ff8-1555">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1555">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="78ff8-1556">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1556">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="78ff8-1557">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1557">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="78ff8-1558">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="78ff8-1558">RDBMS</span></span>

* <span data-ttu-id="78ff8-1559">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1559">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="78ff8-1560">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1560">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="78ff8-1561">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1561">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="78ff8-1562">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1562">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="78ff8-1563">Ресурс</span><span class="sxs-lookup"><span data-stu-id="78ff8-1563">Resource</span></span>

* <span data-ttu-id="78ff8-1564">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1564">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="78ff8-1565">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1565">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="78ff8-1566">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1566">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="78ff8-1567">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1567">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="78ff8-1568">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1568">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="78ff8-1569">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1569">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="78ff8-1570">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1570">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="78ff8-1571">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1571">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="78ff8-1572">Роль</span><span class="sxs-lookup"><span data-stu-id="78ff8-1572">Role</span></span>

* <span data-ttu-id="78ff8-1573">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1573">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="78ff8-1574">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1574">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="78ff8-1575">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1575">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="78ff8-1576">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1576">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="78ff8-1577">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1577">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="78ff8-1578">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="78ff8-1578">Service Fabric</span></span>
* <span data-ttu-id="78ff8-1579">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1579">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="78ff8-1580">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1580">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="78ff8-1581">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1581">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="78ff8-1582">SQL</span><span class="sxs-lookup"><span data-stu-id="78ff8-1582">SQL</span></span>

* <span data-ttu-id="78ff8-1583">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1583">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="78ff8-1584">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1584">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="78ff8-1585">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1585">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-1586">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-1586">Storage</span></span>

* <span data-ttu-id="78ff8-1587">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1587">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="78ff8-1588">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1588">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="78ff8-1589">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1589">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="78ff8-1590">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="78ff8-1590">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="78ff8-1591">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1591">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="78ff8-1592">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1592">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-1593">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-1593">VM</span></span>

* <span data-ttu-id="78ff8-1594">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1594">Support configuring nsg</span></span>
* <span data-ttu-id="78ff8-1595">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1595">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="78ff8-1596">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1596">Support managed service identities</span></span>
* <span data-ttu-id="78ff8-1597">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1597">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="78ff8-1598">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1598">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="78ff8-1599">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1599">May 10, 2017</span></span>

<span data-ttu-id="78ff8-1600">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="78ff8-1600">Version 2.0.6</span></span>

* <span data-ttu-id="78ff8-1601">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1601">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="78ff8-1602">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1602">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="78ff8-1603">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1603">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="78ff8-1604">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1604">Include Cognitive Services module</span></span>
* <span data-ttu-id="78ff8-1605">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1605">Include Service Fabric module</span></span>
* <span data-ttu-id="78ff8-1606">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1606">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="78ff8-1607">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1607">Add support for CDN commands</span></span>
* <span data-ttu-id="78ff8-1608">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1608">Remove Container module</span></span>
* <span data-ttu-id="78ff8-1609">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1609">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="78ff8-1610">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1610">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="78ff8-1611">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-1611">Core</span></span>

* <span data-ttu-id="78ff8-1612">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1612">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="78ff8-1613">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1613">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="78ff8-1614">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1614">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="78ff8-1615">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1615">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="78ff8-1616">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1616">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="78ff8-1617">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1617">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="78ff8-1618">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1618">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="78ff8-1619">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1619">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="78ff8-1620">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1620">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="78ff8-1621">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1621">core: Improved performance</span></span>
* <span data-ttu-id="78ff8-1622">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1622">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="78ff8-1623">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1623">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-1624">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-1624">ACS</span></span>

* <span data-ttu-id="78ff8-1625">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1625">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="78ff8-1626">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1626">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="78ff8-1627">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1627">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="78ff8-1628">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1628">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-1629">AppService</span><span class="sxs-lookup"><span data-stu-id="78ff8-1629">AppService</span></span>

* <span data-ttu-id="78ff8-1630">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1630">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="78ff8-1631">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1631">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="78ff8-1632">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1632">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="78ff8-1633">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1633">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="78ff8-1634">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1634">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="78ff8-1635">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1635">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="78ff8-1636">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1636">support slot swap with preview</span></span>
* <span data-ttu-id="78ff8-1637">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1637">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="78ff8-1638">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1638">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="78ff8-1639">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="78ff8-1639">CosmosDB</span></span>

* <span data-ttu-id="78ff8-1640">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1640">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="78ff8-1641">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1641">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="78ff8-1642">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1642">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="78ff8-1643">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1643">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="78ff8-1644">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="78ff8-1644">Data Lake Analytics</span></span>

* <span data-ttu-id="78ff8-1645">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1645">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="78ff8-1646">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1646">Add support for new catalog item type: package.</span></span> <span data-ttu-id="78ff8-1647">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1647">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="78ff8-1648">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="78ff8-1648">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="78ff8-1649">Таблица</span><span class="sxs-lookup"><span data-stu-id="78ff8-1649">Table</span></span>
  * <span data-ttu-id="78ff8-1650">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="78ff8-1650">Table valued function</span></span>
  * <span data-ttu-id="78ff8-1651">Просмотр</span><span class="sxs-lookup"><span data-stu-id="78ff8-1651">View</span></span>
  * <span data-ttu-id="78ff8-1652">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1652">Table Statistics.</span></span> <span data-ttu-id="78ff8-1653">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1653">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="78ff8-1654">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="78ff8-1654">Data Lake Store</span></span>

* <span data-ttu-id="78ff8-1655">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1655">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="78ff8-1656">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1656">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="78ff8-1657">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1657">missed help for access show.</span></span> <span data-ttu-id="78ff8-1658">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1658">adding it.</span></span> <span data-ttu-id="78ff8-1659">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="78ff8-1659">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="78ff8-1660">Поиск</span><span class="sxs-lookup"><span data-stu-id="78ff8-1660">Find</span></span>

* <span data-ttu-id="78ff8-1661">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1661">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="78ff8-1662">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="78ff8-1662">KeyVault</span></span>

* <span data-ttu-id="78ff8-1663">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1663">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="78ff8-1664">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1664">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="78ff8-1665">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1665">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="78ff8-1666">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1666">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="78ff8-1667">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1667">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="78ff8-1668">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="78ff8-1668">Lab</span></span>

* <span data-ttu-id="78ff8-1669">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1669">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="78ff8-1670">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1670">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="78ff8-1671">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1671">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="78ff8-1672">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1672">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="78ff8-1673">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1673">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="78ff8-1674">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="78ff8-1674">Monitor</span></span>

* <span data-ttu-id="78ff8-1675">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1675">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="78ff8-1676">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1676">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="78ff8-1677">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-1677">Network</span></span>

* <span data-ttu-id="78ff8-1678">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1678">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="78ff8-1679">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1679">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="78ff8-1680">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1680">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="78ff8-1681">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1681">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="78ff8-1682">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1682">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="78ff8-1683">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1683">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="78ff8-1684">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1684">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="78ff8-1685">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1685">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="78ff8-1686">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1686">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="78ff8-1687">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="78ff8-1687">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="78ff8-1688">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1688">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="78ff8-1689">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1689">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="78ff8-1690">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1690">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="78ff8-1691">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1691">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="78ff8-1692">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1692">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="78ff8-1693">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1693">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="78ff8-1694">Профиль</span><span class="sxs-lookup"><span data-stu-id="78ff8-1694">Profile</span></span>

* <span data-ttu-id="78ff8-1695">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1695">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="78ff8-1696">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1696">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="78ff8-1697">Redis</span><span class="sxs-lookup"><span data-stu-id="78ff8-1697">Redis</span></span>

* <span data-ttu-id="78ff8-1698">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1698">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="78ff8-1699">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1699">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="78ff8-1700">Ресурс</span><span class="sxs-lookup"><span data-stu-id="78ff8-1700">Resource</span></span>

* <span data-ttu-id="78ff8-1701">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1701">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="78ff8-1702">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1702">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="78ff8-1703">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1703">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="78ff8-1704">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1704">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="78ff8-1705">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="78ff8-1705">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="78ff8-1706">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1706">Add docs for az lock update.</span></span> <span data-ttu-id="78ff8-1707">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="78ff8-1707">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="78ff8-1708">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1708">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="78ff8-1709">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="78ff8-1709">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="78ff8-1710">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1710">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="78ff8-1711">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="78ff8-1711">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="78ff8-1712">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1712">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="78ff8-1713">Роль</span><span class="sxs-lookup"><span data-stu-id="78ff8-1713">Role</span></span>

* <span data-ttu-id="78ff8-1714">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1714">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="78ff8-1715">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1715">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="78ff8-1716">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1716">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="78ff8-1717">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1717">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="78ff8-1718">SQL</span><span class="sxs-lookup"><span data-stu-id="78ff8-1718">SQL</span></span>

* <span data-ttu-id="78ff8-1719">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1719">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="78ff8-1720">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1720">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="78ff8-1721">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-1721">Storage</span></span>

* <span data-ttu-id="78ff8-1722">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1722">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="78ff8-1723">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1723">Add support for incremental blob copy</span></span>
* <span data-ttu-id="78ff8-1724">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1724">Add support for large block blob upload</span></span>
* <span data-ttu-id="78ff8-1725">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1725">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-1726">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-1726">VM</span></span>

* <span data-ttu-id="78ff8-1727">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1727">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="78ff8-1728">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="78ff8-1728">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="78ff8-1729">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="78ff8-1729">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="78ff8-1730">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="78ff8-1730">az vm/vmss disk</span></span>
  3. <span data-ttu-id="78ff8-1731">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1731">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="78ff8-1732">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1732">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="78ff8-1733">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1733">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="78ff8-1734">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1734">April 3, 2017</span></span>

<span data-ttu-id="78ff8-1735">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="78ff8-1735">Version 2.0.2</span></span>

<span data-ttu-id="78ff8-1736">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1736">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="78ff8-1737">Core</span><span class="sxs-lookup"><span data-stu-id="78ff8-1737">Core</span></span>

* <span data-ttu-id="78ff8-1738">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1738">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="78ff8-1739">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1739">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="78ff8-1740">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1740">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="78ff8-1741">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1741">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="78ff8-1742">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1742">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="78ff8-1743">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="78ff8-1743">Add prompting for missing template parameters.</span></span> <span data-ttu-id="78ff8-1744">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1744">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="78ff8-1745">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1745">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="78ff8-1746">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1746">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="78ff8-1747">ACS</span><span class="sxs-lookup"><span data-stu-id="78ff8-1747">ACS</span></span>

* <span data-ttu-id="78ff8-1748">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1748">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="78ff8-1749">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="78ff8-1749">Add support for ssh key password prompting.</span></span> <span data-ttu-id="78ff8-1750">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1750">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="78ff8-1751">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="78ff8-1751">Add support for windows clusters.</span></span> <span data-ttu-id="78ff8-1752">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1752">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="78ff8-1753">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="78ff8-1753">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="78ff8-1754">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1754">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="78ff8-1755">AppService</span><span class="sxs-lookup"><span data-stu-id="78ff8-1755">AppService</span></span>

* <span data-ttu-id="78ff8-1756">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1756">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="78ff8-1757">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1757">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="78ff8-1758">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1758">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="78ff8-1759">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1759">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="78ff8-1760">Data Lake</span><span class="sxs-lookup"><span data-stu-id="78ff8-1760">DataLake</span></span>

* <span data-ttu-id="78ff8-1761">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1761">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="78ff8-1762">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1762">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="78ff8-1763">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="78ff8-1763">DocuemntDB</span></span>

* <span data-ttu-id="78ff8-1764">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1764">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="78ff8-1765">ВМ</span><span class="sxs-lookup"><span data-stu-id="78ff8-1765">VM</span></span>

* <span data-ttu-id="78ff8-1766">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1766">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="78ff8-1767">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1767">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="78ff8-1768">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1768">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="78ff8-1769">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1769">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="78ff8-1770">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1770">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="78ff8-1771">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1771">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="78ff8-1772">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1772">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="78ff8-1773">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1773">February 27, 2017</span></span>

<span data-ttu-id="78ff8-1774">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="78ff8-1774">Version 2.0.0</span></span>

<span data-ttu-id="78ff8-1775">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="78ff8-1775">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="78ff8-1776">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="78ff8-1776">Container Service (acs)</span></span>
- <span data-ttu-id="78ff8-1777">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="78ff8-1777">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="78ff8-1778">Сеть</span><span class="sxs-lookup"><span data-stu-id="78ff8-1778">Networking</span></span>
- <span data-ttu-id="78ff8-1779">Хранилище</span><span class="sxs-lookup"><span data-stu-id="78ff8-1779">Storage</span></span>

<span data-ttu-id="78ff8-1780">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1780">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="78ff8-1781">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1781">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="78ff8-1782">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1782">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="78ff8-1783">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1783">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="78ff8-1784">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="78ff8-1784">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="78ff8-1785">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="78ff8-1785">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="78ff8-1786">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="78ff8-1786">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="78ff8-1787">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="78ff8-1787">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="78ff8-1788">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="78ff8-1788">Provide feedback from the command line with the `az feedback` command</span></span>

