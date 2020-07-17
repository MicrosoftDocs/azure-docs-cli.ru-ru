---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 07/14/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: cf9c4e1a86b3315d45a7533f67b731ee2f3d6bc0
ms.sourcegitcommit: 857d0f19fd87d37d134efdf0dda0e7003260938b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "86308684"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="82d30-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="82d30-103">Azure CLI release notes</span></span>

# <a name="current-release-notes"></a>[<span data-ttu-id="82d30-104">Заметки о текущем выпуске</span><span class="sxs-lookup"><span data-stu-id="82d30-104">Current release notes</span></span>](#tab/azure-cli)

## <a name="july-14-2020"></a><span data-ttu-id="82d30-105">14 июля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-105">July 14, 2020</span></span>

<span data-ttu-id="82d30-106">Версия 2.9.0</span><span class="sxs-lookup"><span data-stu-id="82d30-106">Version 2.9.0</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-107">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-107">ACR</span></span>

* <span data-ttu-id="82d30-108">Обработка ссылки на артефакт журнала из реестра для потоковой передачи журналов.</span><span class="sxs-lookup"><span data-stu-id="82d30-108">Handle log artifact link from Registry to stream logs</span></span>
* <span data-ttu-id="82d30-109">Устарели команды helm2.</span><span class="sxs-lookup"><span data-stu-id="82d30-109">Deprecate helm2 commands</span></span>

### <a name="aks"></a><span data-ttu-id="82d30-110">AKS</span><span class="sxs-lookup"><span data-stu-id="82d30-110">AKS</span></span>

* <span data-ttu-id="82d30-111">`az aks create`: добавлен аргумент --enable-aad.</span><span class="sxs-lookup"><span data-stu-id="82d30-111">`az aks create`: add --enable-aad argument</span></span>
* <span data-ttu-id="82d30-112">`az aks update`: добавлен аргумент --enable-aad.</span><span class="sxs-lookup"><span data-stu-id="82d30-112">`az aks update`: add --enable-aad argument</span></span>

### <a name="apim"></a><span data-ttu-id="82d30-113">APIM</span><span class="sxs-lookup"><span data-stu-id="82d30-113">APIM</span></span>

* <span data-ttu-id="82d30-114">Добавлены общие команды az apim api.</span><span class="sxs-lookup"><span data-stu-id="82d30-114">Added general az apim api commands</span></span>

### <a name="appconfig"></a><span data-ttu-id="82d30-115">AppConfig</span><span class="sxs-lookup"><span data-stu-id="82d30-115">AppConfig</span></span>

* <span data-ttu-id="82d30-116">Добавлен пример для использования --fields в appconfig revision.</span><span class="sxs-lookup"><span data-stu-id="82d30-116">Add example for using --fields in appconfig revision</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-117">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-117">AppService</span></span>

* <span data-ttu-id="82d30-118">`az functionapp create`: включена поддержка Java 11 и PowerShell 7.</span><span class="sxs-lookup"><span data-stu-id="82d30-118">`az functionapp create`: Added support for Java 11 and Powershell 7.</span></span> <span data-ttu-id="82d30-119">Включена поддержка API стеков.</span><span class="sxs-lookup"><span data-stu-id="82d30-119">Added Stacks API Support.</span></span>
* <span data-ttu-id="82d30-120">Исправлена ошибка № 14208, из-за которой создание многоконтейнерного приложения завершается сбоем.</span><span class="sxs-lookup"><span data-stu-id="82d30-120">Fix #14208 multi-container app creation fails</span></span>
* <span data-ttu-id="82d30-121">Исправлена ошибка с az webapp create, связанная с использованием вписанных в код стеков среды выполнения.</span><span class="sxs-lookup"><span data-stu-id="82d30-121">Fix az webapp create - use hardcoded runtime stacks</span></span>

### <a name="arm"></a><span data-ttu-id="82d30-122">ARM</span><span class="sxs-lookup"><span data-stu-id="82d30-122">ARM</span></span>

* <span data-ttu-id="82d30-123">`az resource tag`: исправлена ошибка, связанная с добавлением тегов к ресурсам с помощью типа ресурса `Microsoft.ContainerInstance/containerGroups`.</span><span class="sxs-lookup"><span data-stu-id="82d30-123">`az resource tag`: Fix the problem of tagging resources with resource type `Microsoft.ContainerInstance/containerGroups`</span></span>

### <a name="compute"></a><span data-ttu-id="82d30-124">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="82d30-124">Compute</span></span>

* <span data-ttu-id="82d30-125">Выполнено обновление версии дисков до 2020-05-01 и вычислительных ресурсов до 2020-06-01.</span><span class="sxs-lookup"><span data-stu-id="82d30-125">Bump version disks 2020-05-01, compute 2020-06-01</span></span>
* <span data-ttu-id="82d30-126">Включено двойное шифрование набора шифрования диска.</span><span class="sxs-lookup"><span data-stu-id="82d30-126">Double encryption of disk encryption set</span></span>
* <span data-ttu-id="82d30-127">`az vmss update`: включена поддержка определения межклиентского образа.</span><span class="sxs-lookup"><span data-stu-id="82d30-127">`az vmss update`: support specify cross tenant image.</span></span>
* <span data-ttu-id="82d30-128">`az sig image-version create`: включена поддержка определения межклиентского образа.</span><span class="sxs-lookup"><span data-stu-id="82d30-128">`az sig image-version create`: support specify cross tenant image.</span></span>
* <span data-ttu-id="82d30-129">vm/vmss create. Включено шифрование кэша и передаваемых данных для дисков ОС и данных и временных дисков для виртуальных машин и Масштабируемых наборов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="82d30-129">vm/vmss create: Encryption of cache & data-in-transit for OS/Data disks and temp disks for VM & VMSS</span></span>
* <span data-ttu-id="82d30-130">Добавлена операция имитации удаления для виртуальных машин и Масштабируемых наборов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="82d30-130">Add simulate-eviction operation for VM and VMSS</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82d30-131">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-131">CosmosDB</span></span>

* <span data-ttu-id="82d30-132">Последние компоненты: Autoscale, IpRules, EnableFreeTier и EnableAnalyticalStorage.</span><span class="sxs-lookup"><span data-stu-id="82d30-132">Recent features: Autoscale, IpRules, EnableFreeTier and EnableAnalyticalStorage</span></span>

### <a name="eventgrid"></a><span data-ttu-id="82d30-133">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="82d30-133">EventGrid</span></span>

* <span data-ttu-id="82d30-134">Включена поддержка CLI для 2020-04-01-preview и отмечены предварительные версии функций как is_Preview=true.</span><span class="sxs-lookup"><span data-stu-id="82d30-134">Add CLI support for 2020-04-01-preview and mark preview features with is_Preview=True</span></span>

### <a name="find"></a><span data-ttu-id="82d30-135">Поиск</span><span class="sxs-lookup"><span data-stu-id="82d30-135">Find</span></span>

* <span data-ttu-id="82d30-136">Исправлена ошибка № 14094, связанная с az find. Исправлена ошибка, из-за которой не удается войти при отключенной телеметрии.</span><span class="sxs-lookup"><span data-stu-id="82d30-136">Fix #14094 az find Fix Queries failing when not logged in and when telemetry is disabled</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82d30-137">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82d30-137">HDInsight</span></span>

* <span data-ttu-id="82d30-138">Добавлены две команды для перезагрузки узла HDInsight.</span><span class="sxs-lookup"><span data-stu-id="82d30-138">Add two commands to support hdinsight node reboot feature</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-139">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-139">Monitor</span></span>

* <span data-ttu-id="82d30-140">Удален флаг предварительной версии для команд в рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="82d30-140">Remove preview flag for commands under Log Analytics workspace</span></span>
* <span data-ttu-id="82d30-141">`az monitor diagnostic-settings subscription`: включена поддержка параметров диагностики для подписки.</span><span class="sxs-lookup"><span data-stu-id="82d30-141">`az monitor diagnostic-settings subscription`: Support diagnositc settings for subscription</span></span>
* <span data-ttu-id="82d30-142">`az monitor metrics`: включена поддержка символов "," и "|" в именах метрик.</span><span class="sxs-lookup"><span data-stu-id="82d30-142">`az monitor metrics`: support ',' and '|' in metric name</span></span>
* <span data-ttu-id="82d30-143">`az monitor log-analytics workspace data-export`: включена поддержка экспорта данных аналитики журнала.</span><span class="sxs-lookup"><span data-stu-id="82d30-143">`az monitor log-analytics workspace data-export`: support log analytics data export</span></span>

### <a name="network"></a><span data-ttu-id="82d30-144">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-144">Network</span></span>

* <span data-ttu-id="82d30-145">`az network application-gateway frontend-ip update`: Устарел параметр --public-ip-address.</span><span class="sxs-lookup"><span data-stu-id="82d30-145">`az network application-gateway frontend-ip update`: Deprecating the --public-ip-address parameter</span></span>
* <span data-ttu-id="82d30-146">Выполнено обновление azure-mgmt-network до 11.0.0.</span><span class="sxs-lookup"><span data-stu-id="82d30-146">Bump azure-mgmt-network to 11.0.0</span></span>
* <span data-ttu-id="82d30-147">`az network express-route gateway connection`: включена конфигурация маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="82d30-147">`az network express-route gateway connection`: support routing configuration</span></span>
* <span data-ttu-id="82d30-148">`az network virtual-appliance`: Включена поддержка сетевого виртуального устройства Azure.</span><span class="sxs-lookup"><span data-stu-id="82d30-148">`az network virtual-appliance`: Support Azure network virtual appliance.</span></span>
* <span data-ttu-id="82d30-149">Включена поддержка компонента Приватного канала в Шлюзе приложений.</span><span class="sxs-lookup"><span data-stu-id="82d30-149">Application Gateway support private link feature</span></span>

### <a name="policyinsights"></a><span data-ttu-id="82d30-150">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="82d30-150">PolicyInsights</span></span>

* <span data-ttu-id="82d30-151">`az policy state`: добавлена команда trigger-scan для активации оценки соответствия политикам.</span><span class="sxs-lookup"><span data-stu-id="82d30-151">`az policy state`: add trigger-scan command to trigger policy compliance evaluations</span></span>
* <span data-ttu-id="82d30-152">`az policy state list`: предоставлены версии сущностей политики в каждой записи соответствия.</span><span class="sxs-lookup"><span data-stu-id="82d30-152">`az policy state list`: expose versions of policy entities in each compliance record</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-153">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-153">Profile</span></span>

* <span data-ttu-id="82d30-154">`az account get-access-token`: включено отображение expiresOn для управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="82d30-154">`az account get-access-token`: Show expiresOn for Managed Identity</span></span>

### <a name="rdbms"></a><span data-ttu-id="82d30-155">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="82d30-155">RDBMS</span></span>

* <span data-ttu-id="82d30-156">Включена поддержка минимальной версии TLS.</span><span class="sxs-lookup"><span data-stu-id="82d30-156">Support Minimum TLS version</span></span>
* <span data-ttu-id="82d30-157">Включено шифрование инфраструктуры для Azure Postgres и MySQL</span><span class="sxs-lookup"><span data-stu-id="82d30-157">Add Infrastructure Encryption for Azure Postgres and MySQL</span></span>

### <a name="security"></a><span data-ttu-id="82d30-158">Безопасность</span><span class="sxs-lookup"><span data-stu-id="82d30-158">Security</span></span>

* <span data-ttu-id="82d30-159">Добавлены команды allowed_connections.</span><span class="sxs-lookup"><span data-stu-id="82d30-159">Add allowed_connections commands</span></span>
* <span data-ttu-id="82d30-160">Добавлены команды адаптивного усиления защиты сети.</span><span class="sxs-lookup"><span data-stu-id="82d30-160">Add Adaptive network hardeningss commands</span></span>
* <span data-ttu-id="82d30-161">Добавлены команды adaptive_application_controls.</span><span class="sxs-lookup"><span data-stu-id="82d30-161">Add adaptive_application_controls commands</span></span>
* <span data-ttu-id="82d30-162">Добавлены команды REST az security iot-solution/iot-alerts/iot-recommendations/iot-analytics в Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="82d30-162">Addition of az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST to Azure CLI</span></span>
* <span data-ttu-id="82d30-163">Добавлен интерфейс командной строки для обеспечения соответствия нормативным требованиям.</span><span class="sxs-lookup"><span data-stu-id="82d30-163">Add regulatory compliance CLI</span></span>

### <a name="signalr"></a><span data-ttu-id="82d30-164">SignalR</span><span class="sxs-lookup"><span data-stu-id="82d30-164">SignalR</span></span>

* <span data-ttu-id="82d30-165">Добавлены возможности, включая управление подключениями к частным конечным точкам, сетевыми правилами и вышестоящими компонентами.</span><span class="sxs-lookup"><span data-stu-id="82d30-165">Add features including managing private endpoint connections, network rules and upstream</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-166">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-166">SQL</span></span>

* <span data-ttu-id="82d30-167">`az sql mi create`, `az sql mi update`: добавлен параметр `--tags` для поддержки тегов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="82d30-167">`az sql mi create`, `az sql mi update`: Add `--tags` parameter to support resource tagging</span></span>
* <span data-ttu-id="82d30-168">`az sql mi failover`: включена поддержка отработки отказа с основного сайта на дополнительный.</span><span class="sxs-lookup"><span data-stu-id="82d30-168">`az sql mi failover`: Support failover from primary or secondary point</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-169">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-169">Storage</span></span>

* <span data-ttu-id="82d30-170">`az storage account create/update`: добавлен параметр --allow-blob-public-access для включения и отключения общего доступа к большим двоичным объектам и контейнерам.</span><span class="sxs-lookup"><span data-stu-id="82d30-170">`az storage account create/update`: Add --allow-blob-public-access to allow or disallow public access for blob and containers</span></span>
* <span data-ttu-id="82d30-171">`az storage account create/update`: добавлен параметр `--min-tls-version` для настройки минимальной версии TLS, используемой при выполнении запросов к хранилищу.</span><span class="sxs-lookup"><span data-stu-id="82d30-171">`az storage account create/update`: Add `--min-tls-version` to support setting the minimum TLS version to be permitted on requests to storage.</span></span>
* <span data-ttu-id="82d30-172">Удален возврат учетных данных маркера.</span><span class="sxs-lookup"><span data-stu-id="82d30-172">Remove check in token credential</span></span>
* <span data-ttu-id="82d30-173">Исправлено имя учетной записи хранения в примерах.</span><span class="sxs-lookup"><span data-stu-id="82d30-173">Fix the storage account name in examples</span></span>

### <a name="webapp"></a><span data-ttu-id="82d30-174">Веб-приложения</span><span class="sxs-lookup"><span data-stu-id="82d30-174">Webapp</span></span>

* <span data-ttu-id="82d30-175">Исправление. az webapp log deployment show: возврат журналов развертывания вместо метаданных журнала.</span><span class="sxs-lookup"><span data-stu-id="82d30-175">Bugfix: az webapp log deployment show - return deployment logs instead of log metadata</span></span>
* <span data-ttu-id="82d30-176">Исправление. az webapp vnet-integration add: исправлена обработка ошибок при неправильном имени виртуальной сети и включена поддержка идентификатора ресурса виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="82d30-176">Bugfix: az webapp vnet-integration add - fix error handling if bad vnet name, support vnet resource ID</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="82d30-177">23 июня 2020 года</span><span class="sxs-lookup"><span data-stu-id="82d30-177">June 23, 2020</span></span>

<span data-ttu-id="82d30-178">Версия 2.8.0</span><span class="sxs-lookup"><span data-stu-id="82d30-178">Version 2.8.0</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-179">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-179">ACR</span></span>

* <span data-ttu-id="82d30-180">Добавлена поддержка отключения конечных точек региона и отключения маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="82d30-180">Add support for region endpoint disable / routing disable</span></span>
* <span data-ttu-id="82d30-181">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.]  `az acr login --expose-token` не принимает имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="82d30-181">[BREAKING CHANGE] `az acr login --expose-token` does not accept username and password</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-182">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-182">ACS</span></span>

* <span data-ttu-id="82d30-183">Удален частный кластер и API 2019-10-27-preview.</span><span class="sxs-lookup"><span data-stu-id="82d30-183">Remove private cluster and 2019-10-27-preview API</span></span>

### <a name="aks"></a><span data-ttu-id="82d30-184">AKS</span><span class="sxs-lookup"><span data-stu-id="82d30-184">AKS</span></span>

* <span data-ttu-id="82d30-185">Включена поддержка параметра --yes для команды az aks upgrade.</span><span class="sxs-lookup"><span data-stu-id="82d30-185">Support --yes for az aks upgrade</span></span>
* <span data-ttu-id="82d30-186">Отменено изменение SKU виртуальной машины по умолчанию на Standard_D2s_v3 (№ 13541).</span><span class="sxs-lookup"><span data-stu-id="82d30-186">Revert "change default vm sku to Standard_D2s_v3 (#13541)"</span></span>
* <span data-ttu-id="82d30-187">Добавлена команда az aks update --uptime-sla.</span><span class="sxs-lookup"><span data-stu-id="82d30-187">Add "az aks update --uptime-sla"</span></span>
* <span data-ttu-id="82d30-188">Исправлена опечатка в команде az aks update.</span><span class="sxs-lookup"><span data-stu-id="82d30-188">Fix typo in az aks update command</span></span>
* <span data-ttu-id="82d30-189">Включена поддержка пула агентов узла 0 и блокировка ручного масштабирования для пула с поддержкой CAS.</span><span class="sxs-lookup"><span data-stu-id="82d30-189">Change to support 0 node agent pool and block manual scale for CAS enabled pool</span></span>
* <span data-ttu-id="82d30-190">Исправлена опечатка в VirtualMachineScaleSets и обновлены ссылки на версии Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="82d30-190">Fix typo on VirtualMachineScaleSets and update references to Kubernetes versions</span></span>

### <a name="ams"></a><span data-ttu-id="82d30-191">AMS</span><span class="sxs-lookup"><span data-stu-id="82d30-191">AMS</span></span>

* <span data-ttu-id="82d30-192">Изменен текст справки по параметру --expires.</span><span class="sxs-lookup"><span data-stu-id="82d30-192">CHANGE help text for "--expiry" parameter.</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-193">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-193">AppService</span></span>

* <span data-ttu-id="82d30-194">`az webapp log deployment show`: включено отображение журнала последнего развертывания или журналов конкретного развертывания, если указан идентификатор развертывания.</span><span class="sxs-lookup"><span data-stu-id="82d30-194">`az webapp log deployment show`: Show the latest deployment log, or the deployment logs of a specific deployment if deployment-id is specified</span></span>
* <span data-ttu-id="82d30-195">`az webapp log deployment list`: список доступных журналов развертывания.</span><span class="sxs-lookup"><span data-stu-id="82d30-195">`az webapp log deployment list`: List of deployment logs available</span></span>
* <span data-ttu-id="82d30-196">Исправление: ошибка поверхности при указании недопустимого имени веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="82d30-196">Fix: Surface error when invalid webapp name provided</span></span>
* <span data-ttu-id="82d30-197">Исправлена ошибка № 13261, и-за которой az webapp list-runtimes использует статический список до появления новых доступных API стеков.</span><span class="sxs-lookup"><span data-stu-id="82d30-197">Fix #13261 az webapp list-runtimes use static list until new Available Stacks API is available</span></span>
* <span data-ttu-id="82d30-198">`az appservice ase create`: исправлена ошибка создания № 13361.</span><span class="sxs-lookup"><span data-stu-id="82d30-198">`az appservice ase create`: Fix create issue #13361</span></span>
* <span data-ttu-id="82d30-199">`az appservice ase list-addresses`: исправлена ошибка изменения SDK № 13140.</span><span class="sxs-lookup"><span data-stu-id="82d30-199">`az appservice ase list-addresses`: Fix change of SDK #13140.</span></span>
* <span data-ttu-id="82d30-200">Исправлена ошибка создания слота или веб-приложения для контейнеров Windows.</span><span class="sxs-lookup"><span data-stu-id="82d30-200">Fix webapp/slot creation for Windows Containers</span></span>
* <span data-ttu-id="82d30-201">`az webapp auth update`: добавлен необязательный параметр для обновления версии среды выполнения.</span><span class="sxs-lookup"><span data-stu-id="82d30-201">`az webapp auth update`: Add optional parameter to update runtime-version</span></span>
* <span data-ttu-id="82d30-202">Включена поддержка перечисления, удаления, утверждения и отклонения подключения к частной конечной точке для веб-приложения в интерфейсе командной строки.</span><span class="sxs-lookup"><span data-stu-id="82d30-202">Support list, delete, approve and reject private endpoint connection for webapp in CLI</span></span>
* <span data-ttu-id="82d30-203">Исправлена ошибка № 13888: включена поддержка команд get, list, create для статических веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="82d30-203">Fix #13888 : Add support for Static WebApps: get, list, create commands</span></span>
* <span data-ttu-id="82d30-204">Улучшены сообщения об ошибках для подключения туннеля SSH.</span><span class="sxs-lookup"><span data-stu-id="82d30-204">Improved error messages for SSH Tunnel Connection</span></span>

### <a name="arm"></a><span data-ttu-id="82d30-205">ARM</span><span class="sxs-lookup"><span data-stu-id="82d30-205">ARM</span></span>

* <span data-ttu-id="82d30-206">`az tag`: добавлены примеры для параметра -h.</span><span class="sxs-lookup"><span data-stu-id="82d30-206">`az tag`: Add examples for -h</span></span>
* <span data-ttu-id="82d30-207">`az deployment group/sub what-if`: добавлен параметр --exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="82d30-207">`az deployment group/sub what-if`: Add --exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="82d30-208">`az deployment group/sub/mg/tenant create`: добавлен параметр --what-if-exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="82d30-208">`az deployment group/sub/mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="82d30-209">`az deployment group/sub/mg/tenant validate`: улучшен формат отображения сообщений об ошибках.</span><span class="sxs-lookup"><span data-stu-id="82d30-209">`az deployment group/sub/mg/tenant validate`: Show error messages in a better format.</span></span>
* <span data-ttu-id="82d30-210">`az group export`: добавлены новые параметры `--skip-resource-name-params` и `--skip-all-params` для включения поддержки параметризации с целью пропуска.</span><span class="sxs-lookup"><span data-stu-id="82d30-210">`az group export`: Add new parameters `--skip-resource-name-params` and `--skip-all-params` to support skip parameterization</span></span>
* <span data-ttu-id="82d30-211">Добавлена команда az feature unregister api.</span><span class="sxs-lookup"><span data-stu-id="82d30-211">Add az feature unregister api</span></span>

### <a name="aro"></a><span data-ttu-id="82d30-212">ARO</span><span class="sxs-lookup"><span data-stu-id="82d30-212">ARO</span></span>

* <span data-ttu-id="82d30-213">Добавлены атрибуты Public и Private в параметры для получения справки по видимости входящего трафика или сервера API.</span><span class="sxs-lookup"><span data-stu-id="82d30-213">Add Public, Private to params for help with ingress/apiserver visibility</span></span>

### <a name="batch"></a><span data-ttu-id="82d30-214">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-214">Batch</span></span>

* <span data-ttu-id="82d30-215">`az batch account create`: добавлен новый параметр `--public-network-access`.</span><span class="sxs-lookup"><span data-stu-id="82d30-215">`az batch account create`: Add new parameter `--public-network-access`</span></span>
* <span data-ttu-id="82d30-216">`az batch account create`: добавлен новый параметр `--identity-type`.</span><span class="sxs-lookup"><span data-stu-id="82d30-216">`az batch account create`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="82d30-217">`az batch account set`: добавлен новый параметр `--identity-type`.</span><span class="sxs-lookup"><span data-stu-id="82d30-217">`az batch account set`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="82d30-218">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az batch pool create. При создании пула с помощью пользовательского образа свойство --image теперь может ссылаться только на образ Общей коллекции образов.</span><span class="sxs-lookup"><span data-stu-id="82d30-218">[BREAKING CHANGE] az batch pool create: When creating a pool using a custom image, the --image property of can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="82d30-219">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az batch pool create. При создании пула с параметром --json-file и указании networkConfiguration свойство publicIPs было перемещено в новое свойство publicIPAddressConfiguration.</span><span class="sxs-lookup"><span data-stu-id="82d30-219">[BREAKING CHANGE] az batch pool create: When creating a pool with --json-file option and specifying a networkConfiguration, the publicIPs property has moved in to a new property publicIPAddressConfiguration.</span></span> <span data-ttu-id="82d30-220">Это новое свойство также поддерживает новое свойство ipAddressProvisioningType, которое определяет, как пул должен выделять IP-адреса, и свойство publicIPs, которое позволяет настроить список ресурсов PublicIP для использования, когда для ipAddressProvisioningType указано значение UserManaged.</span><span class="sxs-lookup"><span data-stu-id="82d30-220">This new property also supports a new ipAddressProvisioningType property which specifies how the pool should allocate IP's and a publicIPs property which allows for configuration of a list of PublicIP resources to use in the case ipAddressProvisioningType is set to UserManaged</span></span>
* <span data-ttu-id="82d30-221">`az network private-link-resource`: включена поддержка ресурса Microsoft.Batch batchAccount.</span><span class="sxs-lookup"><span data-stu-id="82d30-221">`az network private-link-resource`: Add support for the Microsoft.Batch batchAccount resource</span></span>
* <span data-ttu-id="82d30-222">`az network private-endpoint-connection`: включена поддержка ресурса Microsoft.Batch batchAccount.</span><span class="sxs-lookup"><span data-stu-id="82d30-222">`az network private-endpoint-connection`: Add support for the Microsoft.Batch batchAccount resource</span></span>

### <a name="cdn"></a><span data-ttu-id="82d30-223">CDN</span><span class="sxs-lookup"><span data-stu-id="82d30-223">CDN</span></span>

* <span data-ttu-id="82d30-224">`az cdn custom-domain enable-https`: включена поддержка BYOC.</span><span class="sxs-lookup"><span data-stu-id="82d30-224">`az cdn custom-domain enable-https`: Add BYOC support.</span></span>
* <span data-ttu-id="82d30-225">`az cdn custom-domain enable-https`: исправлена ошибка включения пользовательского HTTPS с использованием управляемых CDN сертификатов для SKU Standard_Verizon и Standard_Microsoft.</span><span class="sxs-lookup"><span data-stu-id="82d30-225">`az cdn custom-domain enable-https`: Fix enabling custom HTTPS with CDN managed certificates for Standard_Verizon and Standard_Microsoft SKUs.</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="82d30-226">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="82d30-226">Cognitive Services</span></span>

* <span data-ttu-id="82d30-227">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.]  `az cognitiveservices account` теперь имеет единую структуру для всех команд.</span><span class="sxs-lookup"><span data-stu-id="82d30-227">[BREAKING CHANGE] `az cognitiveservices account` now have a unified structure for all commands.</span></span>
* <span data-ttu-id="82d30-228">`az cognitiveservices account identity`: добавлена возможность управления удостоверениями для Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="82d30-228">`az cognitiveservices account identity`: Add identity management for Cognitive Services.</span></span>

### <a name="compute"></a><span data-ttu-id="82d30-229">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="82d30-229">Compute</span></span>

* <span data-ttu-id="82d30-230">`az image builder`: обновлена версия API до 2020-02-14.</span><span class="sxs-lookup"><span data-stu-id="82d30-230">`az image builder`: Upgrade API version to 2020-02-14</span></span>
* <span data-ttu-id="82d30-231">`az image builder create`: добавлен параметр `--identity` для включения поддержки конфигурации удостоверений.</span><span class="sxs-lookup"><span data-stu-id="82d30-231">`az image builder create`: Add `--identity` to support identity configuration</span></span>
* <span data-ttu-id="82d30-232">`az image builder customizer add`: включена поддержка настройщика Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="82d30-232">`az image builder customizer add`: Support Windows update customizer</span></span>
* <span data-ttu-id="82d30-233">Новая команда `az image builder cancel`.</span><span class="sxs-lookup"><span data-stu-id="82d30-233">New command `az image builder cancel`</span></span>
* <span data-ttu-id="82d30-234">Включено отображение предупреждения, когда пользователь развертывает VMSS, прикрепленные к конкретной версии образа, а не к последней.</span><span class="sxs-lookup"><span data-stu-id="82d30-234">Show a warning when a user deploys a VMSS pinned to a specific image version rather than latest</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="82d30-235">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-235">Cosmos DB</span></span>

* <span data-ttu-id="82d30-236">`az cosmosdb`: добавлена команда exists в базу данных и группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="82d30-236">`az cosmosdb`: Add exists command to database and container groups</span></span>
* <span data-ttu-id="82d30-237">Разрешено создание фиксированных коллекций.</span><span class="sxs-lookup"><span data-stu-id="82d30-237">Allow creating fixed collections</span></span>

### <a name="eventhub"></a><span data-ttu-id="82d30-238">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="82d30-238">EventHub</span></span>

* <span data-ttu-id="82d30-239">`az eventhubs namespace create` : добавлены параметры управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="82d30-239">`az eventhubs namespace create` : Add managed identity parameters</span></span>

### <a name="extension"></a><span data-ttu-id="82d30-240">Расширение</span><span class="sxs-lookup"><span data-stu-id="82d30-240">Extension</span></span>

* <span data-ttu-id="82d30-241">Добавлен параметр --version для включения поддержки установки из конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="82d30-241">Add --version to support to install from a specific version</span></span>
* <span data-ttu-id="82d30-242">Включены расширения CLI для включения пакетов в пространство имен Azure.</span><span class="sxs-lookup"><span data-stu-id="82d30-242">Enable CLI extensions to include packages in the 'azure' namespace</span></span>

### <a name="iot-hub"></a><span data-ttu-id="82d30-243">Центр Интернета вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-243">Iot Hub</span></span>

* <span data-ttu-id="82d30-244">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az iot hub job: удалены устаревшие команды заданий.</span><span class="sxs-lookup"><span data-stu-id="82d30-244">[BREAKING CHANGE] az iot hub job: Remove deprecated job commands</span></span>

### <a name="keyvault"></a><span data-ttu-id="82d30-245">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="82d30-245">KeyVault</span></span>

* <span data-ttu-id="82d30-246">`az keyvault key import`: включена поддержка импорта из строк с помощью двух новых параметров.</span><span class="sxs-lookup"><span data-stu-id="82d30-246">`az keyvault key import`: Supports importing from strings via two new parameters.</span></span>
* <span data-ttu-id="82d30-247">Включена поддержка шифрования и расшифровки строк или байтов с помощью хранимых ключей.</span><span class="sxs-lookup"><span data-stu-id="82d30-247">Support string/bytes encryption and decryption with stored keys</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-248">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-248">Monitor</span></span>

* <span data-ttu-id="82d30-249">Включена поддержка возможности не дожидаться создания кластера.</span><span class="sxs-lookup"><span data-stu-id="82d30-249">Support no wait for cluster creation</span></span>
* <span data-ttu-id="82d30-250">`az monitor log-analytics workspace saved-search`: включена поддержка новых команд для сохраненного поиска.</span><span class="sxs-lookup"><span data-stu-id="82d30-250">`az monitor log-analytics workspace saved-search`: Support new commands for saved search</span></span>

### <a name="network"></a><span data-ttu-id="82d30-251">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-251">Network</span></span>

* <span data-ttu-id="82d30-252">`az network application-gateway address-pool update`: уточнено справочное сообщение и добавлены примеры.</span><span class="sxs-lookup"><span data-stu-id="82d30-252">`az network application-gateway address-pool update`: Refine help message and add examples.</span></span>
* <span data-ttu-id="82d30-253">`az network vnet create`: включена поддержка аргумента --nsg.</span><span class="sxs-lookup"><span data-stu-id="82d30-253">`az network vnet create`: Support --nsg argument</span></span>
* <span data-ttu-id="82d30-254">`az network lb address-pool`: включена поддержка создания внутреннего пула балансировки нагрузки с внутренним адресом.</span><span class="sxs-lookup"><span data-stu-id="82d30-254">`az network lb address-pool`: Support create lb backend pool with backend address.</span></span>
* <span data-ttu-id="82d30-255">`az network application-gateway address-pool`: исправлена ошибка с аргументом --add.</span><span class="sxs-lookup"><span data-stu-id="82d30-255">`az network application-gateway address-pool`: Fix for --add argument</span></span>

### <a name="rbac"></a><span data-ttu-id="82d30-256">RBAC</span><span class="sxs-lookup"><span data-stu-id="82d30-256">RBAC</span></span>

* <span data-ttu-id="82d30-257">`az ad sp create-for-rabc`: включена поддержка имен с пробелом, косой чертой и обратной косой чертой.</span><span class="sxs-lookup"><span data-stu-id="82d30-257">`az ad sp create-for-rabc`: Support name with space, slash and back slash</span></span>
* <span data-ttu-id="82d30-258">`az ad sp create-for-rbac`: уточнено сообщение об ошибке при указании недопустимой области пользователем.</span><span class="sxs-lookup"><span data-stu-id="82d30-258">`az ad sp create-for-rbac`: Refine error message when user specify an invalid scope</span></span>

### <a name="security"></a><span data-ttu-id="82d30-259">Безопасность</span><span class="sxs-lookup"><span data-stu-id="82d30-259">Security</span></span>

* <span data-ttu-id="82d30-260">Добавлены команды оценки безопасности.</span><span class="sxs-lookup"><span data-stu-id="82d30-260">Add security assessment commands</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-261">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-261">SQL</span></span>

* <span data-ttu-id="82d30-262">`az sql db ltr-policy/ltr-backup`: обновление и отображение политик долгосрочного хранения, отображение и удаление долгосрочных резервных копий, восстановление долгосрочных резервных копий.</span><span class="sxs-lookup"><span data-stu-id="82d30-262">`az sql db ltr-policy/ltr-backup`: update/show long term retention policy, show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-263">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-263">Storage</span></span>

* <span data-ttu-id="82d30-264">Исправлена проблема с проверкой подлинности для включения поддержки получения токена для параметра --subscription.</span><span class="sxs-lookup"><span data-stu-id="82d30-264">Fix authentication issue to support get token for --subscription</span></span>
* <span data-ttu-id="82d30-265">`az storage remove`: исправлена ошибка № 13459 с возникновением исключения при сбое операции.</span><span class="sxs-lookup"><span data-stu-id="82d30-265">`az storage remove`: Fix issue #13459 to raise exception for operation failure</span></span>
* <span data-ttu-id="82d30-266">Устранены ошибки № 13012, 13632 и 13657 для удаления неиспользуемых аргументов для команд, связанных с generate-sas.</span><span class="sxs-lookup"><span data-stu-id="82d30-266">Fix issues #13012, #13632 and #13657 to remove unused arguments for generate-sas related commands</span></span>
* <span data-ttu-id="82d30-267">`az storage logging update`: добавлена проверка версии ведения журнала.</span><span class="sxs-lookup"><span data-stu-id="82d30-267">`az storage logging update`: Add check for logging version</span></span>
* <span data-ttu-id="82d30-268">`az storage blob show`: добавлены дополнительные свойства для большого двоичного объекта с использованием пакета SDK для Track 2.</span><span class="sxs-lookup"><span data-stu-id="82d30-268">`az storage blob show`: Add more properties for blob with track 2 SDK</span></span>
* <span data-ttu-id="82d30-269">Исправление № 13708: уточнены предупреждающие сообщения об учетных данных.</span><span class="sxs-lookup"><span data-stu-id="82d30-269">Fix #13708: Refine warning message for credential</span></span>
* <span data-ttu-id="82d30-270">`az storage share-rm create/update`: включена поддержка протокола NFS и корневого сжатия.</span><span class="sxs-lookup"><span data-stu-id="82d30-270">`az storage share-rm create/update`: Add NFS protocol and root squash support</span></span>
* <span data-ttu-id="82d30-271">`az storage account create`: включена поддержка двойного шифрования.</span><span class="sxs-lookup"><span data-stu-id="82d30-271">`az storage account create`: Add support for double encryption</span></span>
* <span data-ttu-id="82d30-272">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.]  `az storage blob/container/file/share/table/queue generate-sas`: параметры --expiry и --permissions являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="82d30-272">[BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: make --expiry and --permissions required</span></span>
* <span data-ttu-id="82d30-273">`az storage blob set-tier`: миграция на Track 2 для включения поддержки настройки приоритета восстановления.</span><span class="sxs-lookup"><span data-stu-id="82d30-273">`az storage blob set-tier`: Migrate to Track 2 to support setting rehydrate priority</span></span>

## <a name="june-02-2020"></a><span data-ttu-id="82d30-274">02 июня 2020 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-274">June 02, 2020</span></span>

<span data-ttu-id="82d30-275">Версия 2.7.0</span><span class="sxs-lookup"><span data-stu-id="82d30-275">Version 2.7.0</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-276">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-276">ACR</span></span>

* <span data-ttu-id="82d30-277">Исправлена опечатка в сообщении об ошибке, возникающем при создании токена.</span><span class="sxs-lookup"><span data-stu-id="82d30-277">Fix a typo in an error message of token creation</span></span>

### <a name="aks"></a><span data-ttu-id="82d30-278">AKS</span><span class="sxs-lookup"><span data-stu-id="82d30-278">AKS</span></span>

* <span data-ttu-id="82d30-279">Номер SKU виртуальной машины по умолчанию изменен на Standard_D2s_v3.</span><span class="sxs-lookup"><span data-stu-id="82d30-279">Change default vm sku to Standard_D2s_v3</span></span>
* <span data-ttu-id="82d30-280">Исправлен процесс создания назначения ролей для кластера MSI и настраиваемой подсети.</span><span class="sxs-lookup"><span data-stu-id="82d30-280">Fix creating role assignment for MSI clsuter plus custom subnet</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-281">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-281">AppService</span></span>

* <span data-ttu-id="82d30-282">Исправлена ошибка 12739, из-за которой команда az appservice list-locations возвращает недопустимые расположения.</span><span class="sxs-lookup"><span data-stu-id="82d30-282">Fix #12739 az appservice list-locations returns some invalid locations</span></span>

### <a name="arm"></a><span data-ttu-id="82d30-283">ARM</span><span class="sxs-lookup"><span data-stu-id="82d30-283">ARM</span></span>

* <span data-ttu-id="82d30-284">`az deployment`: Исправлена ошибка 13159, из-за которой отображается неправильное сообщение JSON после удаления комментариев и сжатия.</span><span class="sxs-lookup"><span data-stu-id="82d30-284">`az deployment`: Fix issue #13159 of incorrect message of JSON after removing comments and compressing</span></span>
* <span data-ttu-id="82d30-285">`az resource tag`: Исправлена ошибка 13255, связанная с добавлением тегов к ресурсам с помощью типа ресурса `Microsoft.ContainerRegistry/registries/webhooks`.</span><span class="sxs-lookup"><span data-stu-id="82d30-285">`az resource tag`: Fix issue #13255 of tagging resources with resource type `Microsoft.ContainerRegistry/registries/webhooks`</span></span>
* <span data-ttu-id="82d30-286">Улучшены примеры для модуля ресурсов.</span><span class="sxs-lookup"><span data-stu-id="82d30-286">Improve the examples for the resource module</span></span>

### <a name="aro"></a><span data-ttu-id="82d30-287">ARO</span><span class="sxs-lookup"><span data-stu-id="82d30-287">ARO</span></span>

* <span data-ttu-id="82d30-288">Исправлена ошибка CLIError, связанная с неправильным флагом для --worker-vm-disk-size-gb.</span><span class="sxs-lookup"><span data-stu-id="82d30-288">Change CLIError to correct flag for --worker-vm-disk-size-gb</span></span>

### <a name="eventhub"></a><span data-ttu-id="82d30-289">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="82d30-289">EventHub</span></span>

* <span data-ttu-id="82d30-290">Исправлена ошибка 12406, из-за которой аргумент --capture-interval не обновляет intervalInSeconds.</span><span class="sxs-lookup"><span data-stu-id="82d30-290">Fix for issue #12406 Argument --capture-interval does not update the "intervalInSeconds"</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82d30-291">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82d30-291">HDInsight</span></span>

* <span data-ttu-id="82d30-292">Объект get_json_object изменен на shell_safe_json_parse.</span><span class="sxs-lookup"><span data-stu-id="82d30-292">Change get_json_object to shell_safe_json_parse</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-293">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-293">Monitor</span></span>

* <span data-ttu-id="82d30-294">`az monitor metrics alert`: уточнены нескольких справочных сообщений.</span><span class="sxs-lookup"><span data-stu-id="82d30-294">`az monitor metrics alert`: refine several help messages</span></span>
* <span data-ttu-id="82d30-295">`az monitor diagnostic-settings create`: включена поддержка аргумента --export-to-resource-specific.</span><span class="sxs-lookup"><span data-stu-id="82d30-295">`az monitor diagnostic-settings create`: support --export-to-resource-specific argument</span></span>
* <span data-ttu-id="82d30-296">Включена поддержка восстановления рабочей области LA.</span><span class="sxs-lookup"><span data-stu-id="82d30-296">Support LA workspace recover</span></span>

### <a name="network"></a><span data-ttu-id="82d30-297">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-297">Network</span></span>

* <span data-ttu-id="82d30-298">`az network dns zone`: включена поддержка символа -.</span><span class="sxs-lookup"><span data-stu-id="82d30-298">`az network dns zone`: support - character</span></span>
* <span data-ttu-id="82d30-299">`az network vpn-connection ipsec-policy`: изменены значения --sa-lifetime и --sa-max-size на более крупные в примере.</span><span class="sxs-lookup"><span data-stu-id="82d30-299">`az network vpn-connection ipsec-policy`: change the --sa-lifetime and --sa-max-size to larger values in example</span></span>
* <span data-ttu-id="82d30-300">Обновление сети до версии 2020-04-01</span><span class="sxs-lookup"><span data-stu-id="82d30-300">Bump network to 2020-04-01</span></span>
* <span data-ttu-id="82d30-301">`az network private-endpoint-connection`: включена поддержка Сетки событий.</span><span class="sxs-lookup"><span data-stu-id="82d30-301">`az network private-endpoint-connection`: support event grid</span></span>
* <span data-ttu-id="82d30-302">`az network express-route list-route-tables`: исправлена ошибка, из-за которой нельзя было перечислять маршруты в виде таблицы.</span><span class="sxs-lookup"><span data-stu-id="82d30-302">`az network express-route list-route-tables`: fix bug that cannot list routes as table</span></span>

### <a name="packaging"></a><span data-ttu-id="82d30-303">Упаковка</span><span class="sxs-lookup"><span data-stu-id="82d30-303">Packaging</span></span>

* <span data-ttu-id="82d30-304">Добавлен пакет Ubuntu Focal.</span><span class="sxs-lookup"><span data-stu-id="82d30-304">Add Ubuntu Focal Package</span></span>

### <a name="rbac"></a><span data-ttu-id="82d30-305">RBAC</span><span class="sxs-lookup"><span data-stu-id="82d30-305">RBAC</span></span>

* <span data-ttu-id="82d30-306">`az ad sp credential reset`: изменен процесс создания учетных данных, чтобы не использовать проблемные специальные символы.</span><span class="sxs-lookup"><span data-stu-id="82d30-306">`az ad sp credential reset`: modify credential generation to avoid troublesome special characters</span></span>

### <a name="redis"></a><span data-ttu-id="82d30-307">Redis</span><span class="sxs-lookup"><span data-stu-id="82d30-307">Redis</span></span>

* <span data-ttu-id="82d30-308">Исправление 13529: изменена документация по параметру enable_non_ssl_port.</span><span class="sxs-lookup"><span data-stu-id="82d30-308">Fix #13529: Change documentation of parameter enable_non_ssl_port</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-309">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-309">Storage</span></span>

* <span data-ttu-id="82d30-310">`az storage copy`: Добавлен параметр `--follow-symlinks` для включения поддержки символических ссылок.</span><span class="sxs-lookup"><span data-stu-id="82d30-310">`az storage copy`: Add parameter `--follow-symlinks` to support symlinks</span></span>
* <span data-ttu-id="82d30-311">Включен локальный контекст для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="82d30-311">Enable local context for storage account</span></span>
* <span data-ttu-id="82d30-312">`az storage logging`: Исправление 11969: уточнено сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="82d30-312">`az storage logging`: Fix issue #11969 to refine error message</span></span>

## <a name="may-19-2020"></a><span data-ttu-id="82d30-313">19 мая 2020 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-313">May 19, 2020</span></span>

<span data-ttu-id="82d30-314">Версия 2.6.0</span><span class="sxs-lookup"><span data-stu-id="82d30-314">Version 2.6.0</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-315">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-315">ACR</span></span>

* <span data-ttu-id="82d30-316">Добавлено время ожидания по умолчанию (5 минут) для любых запросов ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-316">Add default timeout of 5 minutes for any requests to ACR</span></span>
* <span data-ttu-id="82d30-317">Добавлена поддержка отключения доступа к общедоступной сети</span><span class="sxs-lookup"><span data-stu-id="82d30-317">Support disable public network access</span></span>
* <span data-ttu-id="82d30-318">`az acr token create`: предоставляет аргумент --days</span><span class="sxs-lookup"><span data-stu-id="82d30-318">`az acr token create`: expose --days argument</span></span>
* <span data-ttu-id="82d30-319">`az acr import`: принимает значения аргумента --source, которые содержат имя для входа в имени сервера, добавленное путем исправления на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="82d30-319">`az acr import`: accept --source argument values which contain login in server name through client end correction</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-320">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-320">ACS</span></span>

* <span data-ttu-id="82d30-321">Исправление ошибки: удаление больше не существующих полей</span><span class="sxs-lookup"><span data-stu-id="82d30-321">Bug fix: remove fields cleanup for fields that no longer exist</span></span>

### <a name="aks"></a><span data-ttu-id="82d30-322">AKS</span><span class="sxs-lookup"><span data-stu-id="82d30-322">AKS</span></span>

* <span data-ttu-id="82d30-323">Обновлен контекст справки команды uptime-sla</span><span class="sxs-lookup"><span data-stu-id="82d30-323">Update uptime-sla command help context</span></span>
* <span data-ttu-id="82d30-324">Удалена проверка диапазона для обновления числа минут для автомасштабирования</span><span class="sxs-lookup"><span data-stu-id="82d30-324">Remove range check for updating min count for autoscaler</span></span>
* <span data-ttu-id="82d30-325">Исправлена ошибка, из-за которой CLI не выдает ошибку, когда пользователь указывает только пароль Windows</span><span class="sxs-lookup"><span data-stu-id="82d30-325">Fix that cli doe not fail when user only specifies Windows password</span></span>

### <a name="ams"></a><span data-ttu-id="82d30-326">AMS</span><span class="sxs-lookup"><span data-stu-id="82d30-326">AMS</span></span>

* <span data-ttu-id="82d30-327">`az ams transform create`: добавлена возможность создания преобразования с предустановкой FaceDetector</span><span class="sxs-lookup"><span data-stu-id="82d30-327">`az ams transform create`: Add ability to create a transform with a FaceDetector preset</span></span>
* <span data-ttu-id="82d30-328">`az ams content-key-policy create` : добавлена возможность создания политики ключа содержимого FairPlay с конфигурацией автономной аренды</span><span class="sxs-lookup"><span data-stu-id="82d30-328">`az ams content-key-policy create` : Add ability to create a FairPlay content key policy with an offline rental configuration</span></span>

### <a name="appconfig"></a><span data-ttu-id="82d30-329">AppConfig</span><span class="sxs-lookup"><span data-stu-id="82d30-329">AppConfig</span></span>

* <span data-ttu-id="82d30-330">Исправлена ошибка при отображении значений ключей с полями</span><span class="sxs-lookup"><span data-stu-id="82d30-330">Bug fix for list key values with fields</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-331">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-331">AppService</span></span>

* <span data-ttu-id="82d30-332">`az functionapp create`: параметр AzureWebJobsDashboard будет задан только в случае отключения AppInsights</span><span class="sxs-lookup"><span data-stu-id="82d30-332">`az functionapp create`: AzureWebJobsDashboard will only be set if AppInsights is disabled</span></span>
* <span data-ttu-id="82d30-333">Исправление № 10664 — интеграция виртуальной сети — проблема проверки расположения и исправление № 13257 — сбой веб-приложения az в случае необходимости создания группы ресурсов</span><span class="sxs-lookup"><span data-stu-id="82d30-333">Fix #10664- VNet Integration - Location Check Issue & fix #13257- az webapp up failing when RG needs to be created</span></span>
* <span data-ttu-id="82d30-334">`az webapp|functionapp config ssl import`: добавлен поиск хранилища ключей в группах ресурсов в подписке и улучшены справка и примеры.</span><span class="sxs-lookup"><span data-stu-id="82d30-334">`az webapp|functionapp config ssl import`: Lookup key vault across resources groups in subscription and improve help and examples.</span></span>
* <span data-ttu-id="82d30-335">Подключен локальный контекст для службы приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-335">Onboard local context for app service</span></span>

### <a name="arm"></a><span data-ttu-id="82d30-336">ARM</span><span class="sxs-lookup"><span data-stu-id="82d30-336">ARM</span></span>

* <span data-ttu-id="82d30-337">`az deployment`: устранена проблема, из-за которой templateLink не возвращается при развертывании или проверке template-uri</span><span class="sxs-lookup"><span data-stu-id="82d30-337">`az deployment`: Fix the problem that the templateLink will not be returned when deploying or validating template-uri</span></span>
* <span data-ttu-id="82d30-338">`az deployment`: устранена проблема, из-за которой развертывание или проверка не поддерживает специально закодированный символ</span><span class="sxs-lookup"><span data-stu-id="82d30-338">`az deployment`: Fix the problem that deployment/validate does not support specially encoded character</span></span>
* <span data-ttu-id="82d30-339">`az deployment sub/group what-if`: исправлены выравнивание массива и обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="82d30-339">`az deployment sub/group what-if`: Fix array alignment and error handling</span></span>
* <span data-ttu-id="82d30-340">`az deployment operation`: изменение сведений об устаревании</span><span class="sxs-lookup"><span data-stu-id="82d30-340">`az deployment operation`: Modify the deprecate information</span></span>

### <a name="aro"></a><span data-ttu-id="82d30-341">ARO</span><span class="sxs-lookup"><span data-stu-id="82d30-341">ARO</span></span>

* <span data-ttu-id="82d30-342">Добавлены примеры в az aro create, list, list-credentials, show, delete</span><span class="sxs-lookup"><span data-stu-id="82d30-342">Add examples to az aro create, list, list-credentials, show, delete</span></span>
* <span data-ttu-id="82d30-343">Добавлена функция generate_random_id</span><span class="sxs-lookup"><span data-stu-id="82d30-343">Add generate_random_id function</span></span>

### <a name="backup"></a><span data-ttu-id="82d30-344">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="82d30-344">Backup</span></span>

* <span data-ttu-id="82d30-345">Разрешен параметр FriendlyName при включении защиты для команды AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="82d30-345">Allow FriendlyName in enable protection for AzureFileShare command</span></span>
* <span data-ttu-id="82d30-346">Исправлена restore-disks в IaasVM</span><span class="sxs-lookup"><span data-stu-id="82d30-346">Fix in IaasVM restore-disks Command</span></span>
* <span data-ttu-id="82d30-347">Добавлен тип BackupManagementType "MAB" в команду item list</span><span class="sxs-lookup"><span data-stu-id="82d30-347">Add "MAB" BackupManagementType to item list command</span></span>
* <span data-ttu-id="82d30-348">Добавлена поддержка повторного обновления политики для элементов с ошибками.</span><span class="sxs-lookup"><span data-stu-id="82d30-348">Add support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="82d30-349">Добавлена функция защиты от возобновления для виртуальной машины Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-349">Add Resume Protection functionality for Azure Virtual Machine</span></span>
* <span data-ttu-id="82d30-350">Добавлена поддержка возможности указывать группу ресурсов для хранения instantRP во время создания или изменения политики</span><span class="sxs-lookup"><span data-stu-id="82d30-350">Add support to specify ResourceGroup for storing instantRP during Create or Modify Policy</span></span>

### <a name="ci"></a><span data-ttu-id="82d30-351">CI</span><span class="sxs-lookup"><span data-stu-id="82d30-351">CI</span></span>

* <span data-ttu-id="82d30-352">Поддержка flake8 3.8.0</span><span class="sxs-lookup"><span data-stu-id="82d30-352">Support flake8 3.8.0</span></span>

### <a name="compute"></a><span data-ttu-id="82d30-353">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="82d30-353">Compute</span></span>

* <span data-ttu-id="82d30-354">Новая команда az vm auto-shutdown</span><span class="sxs-lookup"><span data-stu-id="82d30-354">New command az vm auto-shutdown</span></span>
* <span data-ttu-id="82d30-355">`az vm list-skus`: обновлено поведение для параметра --zone — теперь он возвращает все номера SKU типов</span><span class="sxs-lookup"><span data-stu-id="82d30-355">`az vm list-skus`: Update --zone behavior, return all type skus now</span></span>

### <a name="core"></a><span data-ttu-id="82d30-356">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-356">Core</span></span>

* <span data-ttu-id="82d30-357">Обновлено состояние включения и выключения локального контекста на уровне глобального пользователя</span><span class="sxs-lookup"><span data-stu-id="82d30-357">Update local context on/off status to global user level</span></span>

### <a name="extension"></a><span data-ttu-id="82d30-358">Расширение</span><span class="sxs-lookup"><span data-stu-id="82d30-358">Extension</span></span>

* <span data-ttu-id="82d30-359">`az extension add`: добавлен параметр --system для включения установки расширений по системному пути</span><span class="sxs-lookup"><span data-stu-id="82d30-359">`az extension add`: Add --system to enable installing extensions in a system path</span></span>
* <span data-ttu-id="82d30-360">Реализована поддержка .egg-info для хранения метаданных расширения типа wheel</span><span class="sxs-lookup"><span data-stu-id="82d30-360">Support .egg-info to store wheel type extension metadata</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-361">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-361">IoT</span></span>

* <span data-ttu-id="82d30-362">`az iot`: теперь в сообщении для информирования о первом запуске модуля команд Интернета вещей используется точный и современный идентификатор `azure-iot`, который не считается нерекомендуемым.</span><span class="sxs-lookup"><span data-stu-id="82d30-362">`az iot`: Update the IoT command module first run extension awareness message to the accurate, non-deprecated modern Id `azure-iot`.</span></span>

### <a name="iot-hub"></a><span data-ttu-id="82d30-363">Центр Интернета вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-363">IoT Hub</span></span>

* <span data-ttu-id="82d30-364">Добавлена поддержка API 2020-03-01 и команд сетевой изоляции</span><span class="sxs-lookup"><span data-stu-id="82d30-364">Support for 2020-03-01 API and Network Isolation commands</span></span>

### <a name="netappfiles"></a><span data-ttu-id="82d30-365">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="82d30-365">NetAppFiles</span></span>

* <span data-ttu-id="82d30-366">`az volume create`: добавлен параметр snapshot-id для создания тома. Это позволит пользователям создавать тома из существующего моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="82d30-366">`az volume create`: Adds snapshot-id as a parameter to create volume this will allow users to create a volume from existing snapshot.</span></span>

### <a name="network"></a><span data-ttu-id="82d30-367">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-367">Network</span></span>

* <span data-ttu-id="82d30-368">Исправлена ошибка, из-за которой значение ttl изменялось непредвиденным образом для add-record для dns</span><span class="sxs-lookup"><span data-stu-id="82d30-368">Fix ttl value changed unintended for dns add-record</span></span>
* <span data-ttu-id="82d30-369">`az network public-ip create`: информирование клиентов о выпуске критического изменения</span><span class="sxs-lookup"><span data-stu-id="82d30-369">`az network public-ip create`: Inform customers of a coming breaking change</span></span>
* <span data-ttu-id="82d30-370">Поддержка универсальных команд для сценария Приватного канала</span><span class="sxs-lookup"><span data-stu-id="82d30-370">Support generic commands for private link scenario</span></span>
* <span data-ttu-id="82d30-371">`az network private-endpoint-connection`: поддержка типов mysql, postgre и mariadb</span><span class="sxs-lookup"><span data-stu-id="82d30-371">`az network private-endpoint-connection`: Support mysql, postgre and mariadb types</span></span>
* <span data-ttu-id="82d30-372">`az network private-endpoint-connection`: поддержка типов cosmosdb</span><span class="sxs-lookup"><span data-stu-id="82d30-372">`az network private-endpoint-connection`: Support cosmosdb types</span></span>
* <span data-ttu-id="82d30-373">`az network private-endpoint`: параметр --group-ids теперь является нерекомендуемым и перенаправляется на --group-id</span><span class="sxs-lookup"><span data-stu-id="82d30-373">`az network private-endpoint`: deprecate --group-ids and redirect to --group-id</span></span>

### <a name="output"></a><span data-ttu-id="82d30-374">Выходные данные</span><span class="sxs-lookup"><span data-stu-id="82d30-374">Output</span></span>

* <span data-ttu-id="82d30-375">Отображение обновленной инструкции для find, feedback и --help</span><span class="sxs-lookup"><span data-stu-id="82d30-375">Show update instruction in find, feedback and --help</span></span>

### <a name="packaging"></a><span data-ttu-id="82d30-376">Упаковка</span><span class="sxs-lookup"><span data-stu-id="82d30-376">Packaging</span></span>

* <span data-ttu-id="82d30-377">Создание пакетов MSI/Homebrew с зависимостями, разрешенным из requirements.txt</span><span class="sxs-lookup"><span data-stu-id="82d30-377">Build MSI/Homebrew packages with dependecies resolved from requirements.txt</span></span>

### <a name="rbac"></a><span data-ttu-id="82d30-378">RBAC</span><span class="sxs-lookup"><span data-stu-id="82d30-378">RBAC</span></span>

* <span data-ttu-id="82d30-379">`az ad sp credential reset`: устранена возможность создания слабых учетных данных</span><span class="sxs-lookup"><span data-stu-id="82d30-379">`az ad sp credential reset`: fix weak credential generation</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-380">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-380">Storage</span></span>

* <span data-ttu-id="82d30-381">`az storage account file-service-properties update/show`: добавлена поддержка свойств файлов для учетной записи хранения</span><span class="sxs-lookup"><span data-stu-id="82d30-381">`az storage account file-service-properties update/show`: Add File Properties Support for Storage Account</span></span>
* <span data-ttu-id="82d30-382">`az storage container create`: исправление № 13373 путем добавления проверяющего элемента управления для общего доступа</span><span class="sxs-lookup"><span data-stu-id="82d30-382">`az storage container create`: Fix #13373 by adding validator for public access</span></span>
* <span data-ttu-id="82d30-383">Добавлена поддержка track2 для ADLS 2-го поколения</span><span class="sxs-lookup"><span data-stu-id="82d30-383">Add ADLS Gen2 track2 support</span></span>
* <span data-ttu-id="82d30-384">`az storage blob sync`: Включена поддержка `--connection-string`.</span><span class="sxs-lookup"><span data-stu-id="82d30-384">`az storage blob sync`: Support `--connection-string`</span></span>
* <span data-ttu-id="82d30-385">`az storage blob sync`: исправлено неверное сообщение об ошибке, которое отображается, когда azcopy не удается найти расположение установки</span><span class="sxs-lookup"><span data-stu-id="82d30-385">`az storage blob sync`: Fix the incorrect error message when azcopy cannot find the installation location</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="82d30-386">30 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-386">April 30, 2020</span></span>

<span data-ttu-id="82d30-387">Версия 2.5.1</span><span class="sxs-lookup"><span data-stu-id="82d30-387">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-388">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-388">ACR</span></span>

* <span data-ttu-id="82d30-389">`az acr check-health`: исправлена ошибка DOCKER_PULL_ERROR в Windows.</span><span class="sxs-lookup"><span data-stu-id="82d30-389">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="82d30-390">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="82d30-390">Compute</span></span>

* <span data-ttu-id="82d30-391">`az vm list-ip-addresses`: Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="82d30-391">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="82d30-392">Исправлена ошибка создания виртуальной машины, которая возникает, если в профиле облака не задано значение endpoint_vm_image_alias_doc.</span><span class="sxs-lookup"><span data-stu-id="82d30-392">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="82d30-393">`az vmss create`: добавлен параметр --os-disk-size-gb.</span><span class="sxs-lookup"><span data-stu-id="82d30-393">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="82d30-394">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-394">Cosmos DB</span></span>

* <span data-ttu-id="82d30-395">`az cosmosdb create/update`: добавлена поддержка --enable-public-network.</span><span class="sxs-lookup"><span data-stu-id="82d30-395">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="82d30-396">Расширение</span><span class="sxs-lookup"><span data-stu-id="82d30-396">Extension</span></span>

* <span data-ttu-id="82d30-397">Исправлена загрузка неправильных метаданных для расширения типа колеса.</span><span class="sxs-lookup"><span data-stu-id="82d30-397">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="82d30-398">Упаковка</span><span class="sxs-lookup"><span data-stu-id="82d30-398">Packaging</span></span>

* <span data-ttu-id="82d30-399">Добавлен скрипт az для Git Bash/Cygwin в Windows.</span><span class="sxs-lookup"><span data-stu-id="82d30-399">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-400">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-400">SQL</span></span>

* <span data-ttu-id="82d30-401">`az sql instance-pool`: добавлена группа команд для пулов экземпляров.</span><span class="sxs-lookup"><span data-stu-id="82d30-401">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-402">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-402">Storage</span></span>

* <span data-ttu-id="82d30-403">Пакет azure-multiapi-storage обновлен до версии 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="82d30-403">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="82d30-404">Добавлена поддержка GZRS при создании и обновлении учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="82d30-404">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="82d30-405">`az storage account failover`: добавлена поддержка отработки отказа учетной записи хранения GRS или GZRS.</span><span class="sxs-lookup"><span data-stu-id="82d30-405">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="82d30-406">`az storage blob upload`: добавлен параметр --encryption-scope для указания сведений об области шифрования.</span><span class="sxs-lookup"><span data-stu-id="82d30-406">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="82d30-407">28 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-407">April 28, 2020</span></span>

<span data-ttu-id="82d30-408">Версия 2.5.0</span><span class="sxs-lookup"><span data-stu-id="82d30-408">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-409">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-409">ACS</span></span>

* <span data-ttu-id="82d30-410">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az openshift create: удален параметр --vnet-peer.</span><span class="sxs-lookup"><span data-stu-id="82d30-410">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="82d30-411">`az openshift create`: добавлены флаги для поддержки частного кластера.</span><span class="sxs-lookup"><span data-stu-id="82d30-411">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="82d30-412">`az openshift`: обновление до версии API `2019-10-27-preview`.</span><span class="sxs-lookup"><span data-stu-id="82d30-412">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="82d30-413">`az openshift`: добавлена команда `update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-413">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="82d30-414">AKS</span><span class="sxs-lookup"><span data-stu-id="82d30-414">AKS</span></span>

* <span data-ttu-id="82d30-415">`az aks create`: включена поддержка Windows.</span><span class="sxs-lookup"><span data-stu-id="82d30-415">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-416">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-416">AppService</span></span>

* <span data-ttu-id="82d30-417">`az webapp deployment source config-zip`: удалена функция перевода в спящий режим после выполнения request.get().</span><span class="sxs-lookup"><span data-stu-id="82d30-417">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="82d30-418">ARM</span><span class="sxs-lookup"><span data-stu-id="82d30-418">ARM</span></span>

* <span data-ttu-id="82d30-419">Добавлены команды What-If развертывания шаблона.</span><span class="sxs-lookup"><span data-stu-id="82d30-419">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="82d30-420">ARO</span><span class="sxs-lookup"><span data-stu-id="82d30-420">ARO</span></span>

* <span data-ttu-id="82d30-421">`az aro`: исправлены выходные данные таблицы.</span><span class="sxs-lookup"><span data-stu-id="82d30-421">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="82d30-422">CI</span><span class="sxs-lookup"><span data-stu-id="82d30-422">CI</span></span>

* <span data-ttu-id="82d30-423">Включена поддержка PyTest и прекращена поддержка Nose для автотестов.</span><span class="sxs-lookup"><span data-stu-id="82d30-423">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="82d30-424">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="82d30-424">Compute</span></span>

* <span data-ttu-id="82d30-425">`az vmss disk detach`: устранена проблема с NoneType для диска данных.</span><span class="sxs-lookup"><span data-stu-id="82d30-425">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="82d30-426">`az vm availability-set list`: включена поддержка отображения списка виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="82d30-426">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="82d30-427">`az vm list-skus`: исправлена проблема с отображением формата таблицы.</span><span class="sxs-lookup"><span data-stu-id="82d30-427">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="82d30-428">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="82d30-428">KeyVault</span></span>

* <span data-ttu-id="82d30-429">Добавлен новый параметр `--enable-rbac-authorization` для использования во время создания или обновления.</span><span class="sxs-lookup"><span data-stu-id="82d30-429">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-430">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-430">Monitor</span></span>

* <span data-ttu-id="82d30-431">Включена поддержка компонентов CMK в кластере LA.</span><span class="sxs-lookup"><span data-stu-id="82d30-431">Support LA cluster CMK features</span></span>
* <span data-ttu-id="82d30-432">`az monitor log-analytics workspace linked-storage`: включена поддержка функций BYOS.</span><span class="sxs-lookup"><span data-stu-id="82d30-432">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="82d30-433">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-433">Network</span></span>

* <span data-ttu-id="82d30-434">`az network security-partner`: включена поддержка поставщика партнера по безопасности.</span><span class="sxs-lookup"><span data-stu-id="82d30-434">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="82d30-435">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="82d30-435">Privatedns</span></span>

* <span data-ttu-id="82d30-436">Добавлена функция в частной зоне DNS для импорта и экспорта файла зоны.</span><span class="sxs-lookup"><span data-stu-id="82d30-436">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="82d30-437">21 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-437">April 21, 2020</span></span>

<span data-ttu-id="82d30-438">Версия 2.4.0</span><span class="sxs-lookup"><span data-stu-id="82d30-438">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-439">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-439">ACR</span></span>

* <span data-ttu-id="82d30-440">`az acr run --cmd`: отключает переопределение рабочего каталога.</span><span class="sxs-lookup"><span data-stu-id="82d30-440">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="82d30-441">Включена поддержка выделенной конечной точки данных.</span><span class="sxs-lookup"><span data-stu-id="82d30-441">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="82d30-442">AKS</span><span class="sxs-lookup"><span data-stu-id="82d30-442">AKS</span></span>

* <span data-ttu-id="82d30-443">`az aks list -o table` теперь показывает privateFqdn как FQDN для частных кластеров.</span><span class="sxs-lookup"><span data-stu-id="82d30-443">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="82d30-444">Добавлен параметр --uptime-sla.</span><span class="sxs-lookup"><span data-stu-id="82d30-444">Add --uptime-sla</span></span>
* <span data-ttu-id="82d30-445">Обновлен пакет containerservice.</span><span class="sxs-lookup"><span data-stu-id="82d30-445">Update containerservice package</span></span>
* <span data-ttu-id="82d30-446">Включена поддержка общедоступных IP-адресов узлов.</span><span class="sxs-lookup"><span data-stu-id="82d30-446">Add node public IP support</span></span>
* <span data-ttu-id="82d30-447">Исправлена опечатка в команде справки.</span><span class="sxs-lookup"><span data-stu-id="82d30-447">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="82d30-448">AppConfig</span><span class="sxs-lookup"><span data-stu-id="82d30-448">AppConfig</span></span>

* <span data-ttu-id="82d30-449">Разрешена ссылка на хранилище ключей для команд kv list и export.</span><span class="sxs-lookup"><span data-stu-id="82d30-449">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="82d30-450">Исправлена ошибка при отображении значений ключей.</span><span class="sxs-lookup"><span data-stu-id="82d30-450">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-451">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-451">AppService</span></span>

* <span data-ttu-id="82d30-452">`az functionapp create`: изменен способ настройки linuxFxVersion для приложений-функций dotnet в Linux.</span><span class="sxs-lookup"><span data-stu-id="82d30-452">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="82d30-453">Это должно исправить ошибку, препятствующую созданию приложений dotnet для использования в Linux.</span><span class="sxs-lookup"><span data-stu-id="82d30-453">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="82d30-454">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az webapp create` Исправлена ошибка для сохранения существующих параметров AppSettings с помощью az webapp create.</span><span class="sxs-lookup"><span data-stu-id="82d30-454">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="82d30-455">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az webapp up` Исправлена ошибка для создания группы ресурсов для команды az webapp up при использовании флага -g.</span><span class="sxs-lookup"><span data-stu-id="82d30-455">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="82d30-456">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az webapp config` Исправлена ошибка для отображения значений для выходных данных не в формате JSON с помощью команды az webapp config connection-string list.</span><span class="sxs-lookup"><span data-stu-id="82d30-456">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="82d30-457">ARM</span><span class="sxs-lookup"><span data-stu-id="82d30-457">ARM</span></span>

* <span data-ttu-id="82d30-458">`az deployment create/validate`: добавлен параметр `--no-prompt` для пропуска запроса отсутствующих параметров для шаблона ARM.</span><span class="sxs-lookup"><span data-stu-id="82d30-458">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="82d30-459">`az deployment group/mg/sub/tenant validate`: включена поддержка комментариев в файле параметров развертывания.</span><span class="sxs-lookup"><span data-stu-id="82d30-459">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="82d30-460">`az deployment`: удалено значение `is_preview` для параметра `--handle-extended-json-format`.</span><span class="sxs-lookup"><span data-stu-id="82d30-460">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="82d30-461">`az deployment group/mg/sub/tenant cancel`: включена поддержка отмены развертывания для шаблона ARM.</span><span class="sxs-lookup"><span data-stu-id="82d30-461">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="82d30-462">`az deployment group/mg/sub/tenant validate`: улучшено отображение сообщения об ошибке при сбое проверки развертывания.</span><span class="sxs-lookup"><span data-stu-id="82d30-462">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="82d30-463">`az deployment-scripts`: добавлена новая команда для DeploymentScripts.</span><span class="sxs-lookup"><span data-stu-id="82d30-463">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="82d30-464">`az resource tag`: добавлен параметр `--is-incremental` для инкрементного добавления тегов к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="82d30-464">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="82d30-465">ARO</span><span class="sxs-lookup"><span data-stu-id="82d30-465">ARO</span></span>

* <span data-ttu-id="82d30-466">`az aro`:  добавлен модуль команды aro Azure RedHat OpenShift версии 4.</span><span class="sxs-lookup"><span data-stu-id="82d30-466">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="82d30-467">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-467">Batch</span></span>

* <span data-ttu-id="82d30-468">Обновлен API пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="82d30-468">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="82d30-469">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="82d30-469">Compute</span></span>

* <span data-ttu-id="82d30-470">`az sig image-version create`: добавлен тип учетной записи хранения Premium_LRS.</span><span class="sxs-lookup"><span data-stu-id="82d30-470">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="82d30-471">`az vmss update`: устранена проблема с обновлением уведомления о завершении.</span><span class="sxs-lookup"><span data-stu-id="82d30-471">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="82d30-472">`az vm/vmss create`: включена поддержка версии специализированного образа.</span><span class="sxs-lookup"><span data-stu-id="82d30-472">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="82d30-473">API SIG версии 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="82d30-473">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="82d30-474">`az sig image-version create`: добавлен параметр --target-region-encryption.</span><span class="sxs-lookup"><span data-stu-id="82d30-474">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="82d30-475">Исправлена ошибка, из-за которой тесты завершались сбоем при последовательном выполнении из-за дублирования имени хранилища ключей в глобальном кэше в памяти.</span><span class="sxs-lookup"><span data-stu-id="82d30-475">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82d30-476">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-476">CosmosDB</span></span>

* <span data-ttu-id="82d30-477">Включена поддержка `az cosmosdb private-link-resource/private-endpoint-connection`.</span><span class="sxs-lookup"><span data-stu-id="82d30-477">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="82d30-478">IoT Central</span><span class="sxs-lookup"><span data-stu-id="82d30-478">IoT Central</span></span>

* <span data-ttu-id="82d30-479">Прекращена поддержка `az iotcentral`.</span><span class="sxs-lookup"><span data-stu-id="82d30-479">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="82d30-480">Добавлен модуль команды `az iot central`.</span><span class="sxs-lookup"><span data-stu-id="82d30-480">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-481">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-481">Monitor</span></span>

* <span data-ttu-id="82d30-482">Включена поддержка сценария приватного канала для монитора.</span><span class="sxs-lookup"><span data-stu-id="82d30-482">Support private link scenario for monitor</span></span>
* <span data-ttu-id="82d30-483">Исправлен неправильный способ имитации в test_monitor_general_operations.py.</span><span class="sxs-lookup"><span data-stu-id="82d30-483">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="82d30-484">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-484">Network</span></span>

* <span data-ttu-id="82d30-485">Прекращена поддержка SKU для команды public ip update.</span><span class="sxs-lookup"><span data-stu-id="82d30-485">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="82d30-486">`az network private-endpoint`: включена поддержка закрытой группы зон DNS.</span><span class="sxs-lookup"><span data-stu-id="82d30-486">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="82d30-487">Включена функция локального контекста для параметра vnet/subnet.</span><span class="sxs-lookup"><span data-stu-id="82d30-487">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="82d30-488">Исправлен неправильный пример использования в test_nw_flow_log_delete.</span><span class="sxs-lookup"><span data-stu-id="82d30-488">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="82d30-489">Упаковка</span><span class="sxs-lookup"><span data-stu-id="82d30-489">Packaging</span></span>

* <span data-ttu-id="82d30-490">Прекращена поддержка пакета Ubuntu/Disco.</span><span class="sxs-lookup"><span data-stu-id="82d30-490">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="82d30-491">RBAC</span><span class="sxs-lookup"><span data-stu-id="82d30-491">RBAC</span></span>

* <span data-ttu-id="82d30-492">`az ad app create/update`: включена поддержка параметра --optional-claims.</span><span class="sxs-lookup"><span data-stu-id="82d30-492">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="82d30-493">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="82d30-493">RDBMS</span></span>

* <span data-ttu-id="82d30-494">Добавлены команды администратора Azure Active Directory для PostgreSQL и MySQL.</span><span class="sxs-lookup"><span data-stu-id="82d30-494">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="82d30-495">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="82d30-495">Service Fabric</span></span>

* <span data-ttu-id="82d30-496">Исправление 12891: `az sf application update --application-parameters` удаляет старые параметры, отсутствующие в запросе.</span><span class="sxs-lookup"><span data-stu-id="82d30-496">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="82d30-497">Исправление 12470: включена поддержка az sf create cluster, исправлены ошибки, связанные с устойчивостью и надежностью обновления, поиск VMSS выполняется корректно в коде при указании имени типа узла.</span><span class="sxs-lookup"><span data-stu-id="82d30-497">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-498">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-498">SQL</span></span>

* <span data-ttu-id="82d30-499">Добавлены команды `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`.</span><span class="sxs-lookup"><span data-stu-id="82d30-499">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="82d30-500">`az sql midb`: обновление и отображение политик долгосрочного хранения, отображение и удаление долгосрочных резервных копий, восстановление долгосрочных резервных копий.</span><span class="sxs-lookup"><span data-stu-id="82d30-500">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-501">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-501">Storage</span></span>

* <span data-ttu-id="82d30-502">Обновлена версия azure-mgmt-storage до 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="82d30-502">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="82d30-503">`az storage logging off`: включено отключение ведения журналов для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="82d30-503">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="82d30-504">`az storage account update`: включена автоматическая смена ключа для CMK.</span><span class="sxs-lookup"><span data-stu-id="82d30-504">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="82d30-505">`az storage account encryption-scope create/update/list/show`: включена настройка области шифрования.</span><span class="sxs-lookup"><span data-stu-id="82d30-505">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="82d30-506">`az storage container create`: добавлены параметры --default-encryption-scope и --deny-encryption-scope-override для настройки области шифрования на уровне контейнера.</span><span class="sxs-lookup"><span data-stu-id="82d30-506">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="82d30-507">Опрос</span><span class="sxs-lookup"><span data-stu-id="82d30-507">Survey</span></span>

* <span data-ttu-id="82d30-508">Добавлен параметр для отключения ссылки опроса.</span><span class="sxs-lookup"><span data-stu-id="82d30-508">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="82d30-509">01 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-509">April 01, 2020</span></span>

<span data-ttu-id="82d30-510">Версия 2.3.1</span><span class="sxs-lookup"><span data-stu-id="82d30-510">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-511">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-511">ACR</span></span>

* <span data-ttu-id="82d30-512">Исправлена неправильная версия azure-mgmt-containerregistry для Linux.</span><span class="sxs-lookup"><span data-stu-id="82d30-512">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-513">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-513">Profile</span></span>

* <span data-ttu-id="82d30-514">az login: Исправлена ошибка входа в облачных профилях, отличающихся от `latest`.</span><span class="sxs-lookup"><span data-stu-id="82d30-514">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="82d30-515">31 марта 2020 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-515">March 31, 2020</span></span>

<span data-ttu-id="82d30-516">Версия 2.3.0</span><span class="sxs-lookup"><span data-stu-id="82d30-516">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-517">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-517">ACR</span></span>

* <span data-ttu-id="82d30-518">az acr task update: исключение пустого указателя.</span><span class="sxs-lookup"><span data-stu-id="82d30-518">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="82d30-519">`az acr import`: Отредактировано справочное сообщение и сообщение об ошибке для уточнения того, как использовать параметры --source и --registry.</span><span class="sxs-lookup"><span data-stu-id="82d30-519">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="82d30-520">Добавлено средство проверки для аргумента registry_name.</span><span class="sxs-lookup"><span data-stu-id="82d30-520">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="82d30-521">`az acr login`: удален флаг предпросмотра для --expose-token.</span><span class="sxs-lookup"><span data-stu-id="82d30-521">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="82d30-522">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр ветви az acr task create/update.</span><span class="sxs-lookup"><span data-stu-id="82d30-522">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="82d30-523">Клиент az acr task update теперь может независимо обновлять контекст, токен GitHub и триггеры.</span><span class="sxs-lookup"><span data-stu-id="82d30-523">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="82d30-524">az acr agentpool: новая функция.</span><span class="sxs-lookup"><span data-stu-id="82d30-524">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="82d30-525">AKS</span><span class="sxs-lookup"><span data-stu-id="82d30-525">AKS</span></span>

* <span data-ttu-id="82d30-526">Исправлена ошибка с apiServerAccessProfile при обновлении --api-server-authorized-ip-ranges.</span><span class="sxs-lookup"><span data-stu-id="82d30-526">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="82d30-527">Обновление AKS: при обновлении исходящие IP-адреса переопределяются с помощью входных значений.</span><span class="sxs-lookup"><span data-stu-id="82d30-527">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="82d30-528">Не создаются имена субъектов-служб для кластеров MSI и реализована поддержка присоединение ACR к кластерам MSI.</span><span class="sxs-lookup"><span data-stu-id="82d30-528">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="82d30-529">AMS</span><span class="sxs-lookup"><span data-stu-id="82d30-529">AMS</span></span>

* <span data-ttu-id="82d30-530">Исправление 12469: не удается добавить content-key-policy для FairPlay из-за проблем с параметром ask.</span><span class="sxs-lookup"><span data-stu-id="82d30-530">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="82d30-531">AppConfig</span><span class="sxs-lookup"><span data-stu-id="82d30-531">AppConfig</span></span>

* <span data-ttu-id="82d30-532">Добавлен параметр --skip-keyvault для экспорта kv.</span><span class="sxs-lookup"><span data-stu-id="82d30-532">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-533">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-533">AppService</span></span>

* <span data-ttu-id="82d30-534">Исправление 12509: удален тег, добавлявшийся по умолчанию при создании приложения с помощью az webapp up.</span><span class="sxs-lookup"><span data-stu-id="82d30-534">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="82d30-535">az functionapp create: обновлено меню справки для --runtime-version и добавлено предупреждение, когда пользователь указывает параметр --runtime-version для DotNet.</span><span class="sxs-lookup"><span data-stu-id="82d30-535">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="82d30-536">az functionapp create: изменен способ установки JavaVersion для приложений-функций Windows.</span><span class="sxs-lookup"><span data-stu-id="82d30-536">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="82d30-537">ARM</span><span class="sxs-lookup"><span data-stu-id="82d30-537">ARM</span></span>

* <span data-ttu-id="82d30-538">az deployment create/validate: по умолчанию используется параметр --handle-extended-json-format.</span><span class="sxs-lookup"><span data-stu-id="82d30-538">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="82d30-539">az lock create: в справочную документацию добавлены примеры создания подресурсов.</span><span class="sxs-lookup"><span data-stu-id="82d30-539">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="82d30-540">Список az deployment {group/mg/sub/tenant}: реализована поддержка фильтрации ProvisioningState.</span><span class="sxs-lookup"><span data-stu-id="82d30-540">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="82d30-541">az deployment: исправлена ошибка синтаксического анализа комментария в последнем аргументе.</span><span class="sxs-lookup"><span data-stu-id="82d30-541">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="82d30-542">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="82d30-542">Backup</span></span>

* <span data-ttu-id="82d30-543">Добавлена возможность восстановления нескольких файлов.</span><span class="sxs-lookup"><span data-stu-id="82d30-543">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="82d30-544">Добавлена возможность резервного копирования только дисков с ОС.</span><span class="sxs-lookup"><span data-stu-id="82d30-544">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="82d30-545">Добавлен параметр restore-as-unmanaged-disk, позволяющий задать неуправляемое восстановление.</span><span class="sxs-lookup"><span data-stu-id="82d30-545">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="82d30-546">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="82d30-546">Compute</span></span>

* <span data-ttu-id="82d30-547">az vm create: для --nsg-rule добавлен вариант NONE.</span><span class="sxs-lookup"><span data-stu-id="82d30-547">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="82d30-548">az vmss create/update: удален тег предпросмотра для автоматического восстановления VMSS.</span><span class="sxs-lookup"><span data-stu-id="82d30-548">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="82d30-549">az vm update: реализована поддержка --workspace.</span><span class="sxs-lookup"><span data-stu-id="82d30-549">az vm update: Support --workspace</span></span>
* <span data-ttu-id="82d30-550">Исправлена ошибка в коде инициализации VirtualMachineScaleSetExtension.</span><span class="sxs-lookup"><span data-stu-id="82d30-550">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="82d30-551">Версия VMAccessAgent обновлена до 2.4.</span><span class="sxs-lookup"><span data-stu-id="82d30-551">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="82d30-552">az vmss set-orchestration-service-state: реализована поддержка состояния службы оркестрации наборов VMSS.</span><span class="sxs-lookup"><span data-stu-id="82d30-552">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="82d30-553">Версия API диска обновлена до 2019-11-01.</span><span class="sxs-lookup"><span data-stu-id="82d30-553">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="82d30-554">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun.</span><span class="sxs-lookup"><span data-stu-id="82d30-554">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="82d30-555">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-555">Cosmos DB</span></span>

* <span data-ttu-id="82d30-556">Добавлен отсутствовавший параметр --type для перенаправления в связи с устареванием.</span><span class="sxs-lookup"><span data-stu-id="82d30-556">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="82d30-557">Docker</span><span class="sxs-lookup"><span data-stu-id="82d30-557">Docker</span></span>

* <span data-ttu-id="82d30-558">Обновление до Alpine 3.11 и Python 3.6.10.</span><span class="sxs-lookup"><span data-stu-id="82d30-558">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="82d30-559">Расширение</span><span class="sxs-lookup"><span data-stu-id="82d30-559">Extension</span></span>

* <span data-ttu-id="82d30-560">Добавлена возможность загрузки расширений в системный путь через пакеты.</span><span class="sxs-lookup"><span data-stu-id="82d30-560">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82d30-561">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82d30-561">HDInsight</span></span>

* <span data-ttu-id="82d30-562">(az hdinsight create:) Добавлена возможность указания клиентами минимальной поддерживаемой версии TLS с помощью параметра `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="82d30-562">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="82d30-563">Допустимые значения: 1.0,1.1,1.2.</span><span class="sxs-lookup"><span data-stu-id="82d30-563">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-564">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-564">IoT</span></span>

* <span data-ttu-id="82d30-565">Добавлен параметр codeowner.</span><span class="sxs-lookup"><span data-stu-id="82d30-565">Add codeowner</span></span>
* <span data-ttu-id="82d30-566">az iot hub create: номер SKU по умолчанию изменен с F1 на S1.</span><span class="sxs-lookup"><span data-stu-id="82d30-566">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="82d30-567">iot hub: реализована поддержка IotHub в профиле 2019-03-01-hybrid.</span><span class="sxs-lookup"><span data-stu-id="82d30-567">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="82d30-568">IoT Central</span><span class="sxs-lookup"><span data-stu-id="82d30-568">IoTCentral</span></span>

* <span data-ttu-id="82d30-569">Обновлены сведения об ошибках, шаблон приложения по умолчанию и сообщение с подсказкой.</span><span class="sxs-lookup"><span data-stu-id="82d30-569">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="82d30-570">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="82d30-570">KeyVault</span></span>

* <span data-ttu-id="82d30-571">Реализована поддержка резервного копирования и восстановления сертификатов.</span><span class="sxs-lookup"><span data-stu-id="82d30-571">Support certificate backup/restore</span></span>
* <span data-ttu-id="82d30-572">keyvault create/update: добавлена поддержка параметра --retention-days.</span><span class="sxs-lookup"><span data-stu-id="82d30-572">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="82d30-573">При перечислении больше не показываются управляемые ключи и секреты.</span><span class="sxs-lookup"><span data-stu-id="82d30-573">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="82d30-574">az keyvault create: реализована поддержка `--network-acls`, `--network-acls-ips` и `--network-acls-vnets` для указания сетевых правил при создании хранилища.</span><span class="sxs-lookup"><span data-stu-id="82d30-574">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="82d30-575">Блокировка</span><span class="sxs-lookup"><span data-stu-id="82d30-575">Lock</span></span>

* <span data-ttu-id="82d30-576">Исправлена ошибка с командой az lock delete, не работавшей с Microsoft.DocumentDB.</span><span class="sxs-lookup"><span data-stu-id="82d30-576">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-577">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-577">Monitor</span></span>

* <span data-ttu-id="82d30-578">az monitor clone: добавлена возможность клонирования правил метрики из одного ресурса в другой.</span><span class="sxs-lookup"><span data-stu-id="82d30-578">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="82d30-579">Исправлена ошибка IcM179210086: не удается создать настраиваемое оповещение для метрики Application Insights.</span><span class="sxs-lookup"><span data-stu-id="82d30-579">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="82d30-580">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="82d30-580">NetAppFiles</span></span>

* <span data-ttu-id="82d30-581">az volume create: для томов защиты данных добавлены операции репликации (approve, suspend, resume, status, remove).</span><span class="sxs-lookup"><span data-stu-id="82d30-581">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="82d30-582">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-582">Network</span></span>

* <span data-ttu-id="82d30-583">az network application-gateway waf-policy managed-rule rule-set add: добавлена поддержка Microsoft_BotManagerRuleSet.</span><span class="sxs-lookup"><span data-stu-id="82d30-583">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="82d30-584">Журнал потоков наблюдателя за сетями: исправлены неправильные сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="82d30-584">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="82d30-585">Добавлена поддержка имен узлов в прослушивателе шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="82d30-585">support host names in application gateway listener</span></span>
* <span data-ttu-id="82d30-586">az network nat gateway: добавлена возможность создания пустого ресурса без общедоступного IP-адреса или общедоступного IP-префикса.</span><span class="sxs-lookup"><span data-stu-id="82d30-586">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="82d30-587">Добавлена возможность создания VPN-шлюза.</span><span class="sxs-lookup"><span data-stu-id="82d30-587">Support vpn gateway generation</span></span>
* <span data-ttu-id="82d30-588">Реализована поддержка `--if-none-match` для `az network dns record-set {} add-record`.</span><span class="sxs-lookup"><span data-stu-id="82d30-588">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="82d30-589">Упаковка</span><span class="sxs-lookup"><span data-stu-id="82d30-589">Packaging</span></span>

* <span data-ttu-id="82d30-590">Прекращена поддержка Python 3.5.</span><span class="sxs-lookup"><span data-stu-id="82d30-590">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-591">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-591">Profile</span></span>

* <span data-ttu-id="82d30-592">az login: добавлен показ предупреждений об ошибках MFA.</span><span class="sxs-lookup"><span data-stu-id="82d30-592">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="82d30-593">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="82d30-593">RDBMS</span></span>

* <span data-ttu-id="82d30-594">Добавлены команды управления ключами шифрования данных сервера для PostgreSQL и MySQL.</span><span class="sxs-lookup"><span data-stu-id="82d30-594">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="82d30-595">10 марта 2020 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-595">March 10, 2020</span></span>

<span data-ttu-id="82d30-596">Версия 2.2.0</span><span class="sxs-lookup"><span data-stu-id="82d30-596">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-597">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-597">ACR</span></span>

* <span data-ttu-id="82d30-598">Исправлена команда `az acr login`, которая неправильно вызывала ошибку.</span><span class="sxs-lookup"><span data-stu-id="82d30-598">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="82d30-599">Добавлена новая команда `az acr helm install-cli`.</span><span class="sxs-lookup"><span data-stu-id="82d30-599">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="82d30-600">Добавлена частная ссылка и включена поддержка CMK.</span><span class="sxs-lookup"><span data-stu-id="82d30-600">Add private link and CMK support</span></span>
* <span data-ttu-id="82d30-601">Добавлена команда private-link-resource list.</span><span class="sxs-lookup"><span data-stu-id="82d30-601">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="82d30-602">AKS</span><span class="sxs-lookup"><span data-stu-id="82d30-602">AKS</span></span>

* <span data-ttu-id="82d30-603">Исправлена функция поиска AKS в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="82d30-603">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="82d30-604">az aks: устранены ошибки NoneType при мониторинге надстроек и пула агентов.</span><span class="sxs-lookup"><span data-stu-id="82d30-604">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="82d30-605">Добавлен параметр --nodepool-tags в пуле узлов при создании кластера Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="82d30-605">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="82d30-606">Добавлен параметр --tags при добавлении пула узлов в кластер или его обновлении.</span><span class="sxs-lookup"><span data-stu-id="82d30-606">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="82d30-607">aks create: добавлен параметр `--enable-private-cluster`.</span><span class="sxs-lookup"><span data-stu-id="82d30-607">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="82d30-608">Добавлен параметр --nodepool-labels в пуле узлов при создании кластера Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="82d30-608">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="82d30-609">Добавлен параметр --labels при добавлении нового пула узлов в кластер Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="82d30-609">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="82d30-610">Добавлен отсутствующий символ / в URL-адрес панели мониторинга.</span><span class="sxs-lookup"><span data-stu-id="82d30-610">add missing / in the dashboard url</span></span>
* <span data-ttu-id="82d30-611">Включена поддержка создания кластеров AKS для управляемых удостоверений</span><span class="sxs-lookup"><span data-stu-id="82d30-611">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="82d30-612">az aks: включена проверка состояния сетевого подключаемого модуля: Azure или Kubenet.</span><span class="sxs-lookup"><span data-stu-id="82d30-612">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="82d30-613">az aks: включена поддержка ключа сеанса AAD.</span><span class="sxs-lookup"><span data-stu-id="82d30-613">az aks: Add aad session key support</span></span>
* <span data-ttu-id="82d30-614">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az aks: включена поддержка изменений MSI для GF и BF для omsagent (мониторинг контейнеров) (1)</span><span class="sxs-lookup"><span data-stu-id="82d30-614">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="82d30-615">az aks use-dev-spaces: добавлен параметр типа конечной точки в команду use-dev-spaces для настройки конечной точки, созданной в контроллере Azure Dev Spaces.</span><span class="sxs-lookup"><span data-stu-id="82d30-615">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="82d30-616">AppConfig</span><span class="sxs-lookup"><span data-stu-id="82d30-616">AppConfig</span></span>

* <span data-ttu-id="82d30-617">Включена разблокировка с использованием kv set для добавления функции и ссылки на хранилище ключей.</span><span class="sxs-lookup"><span data-stu-id="82d30-617">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-618">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-618">AppService</span></span>

* <span data-ttu-id="82d30-619">az webapp create: устранена проблема с выполнением команды с параметром --runtime.</span><span class="sxs-lookup"><span data-stu-id="82d30-619">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="82d30-620">az functionapp deployment source config-zip: добавлено сообщение об ошибке, если группа ресурсов или имя функции недействительны или не существуют.</span><span class="sxs-lookup"><span data-stu-id="82d30-620">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="82d30-621">functionapp create: исправлено сообщение с предупреждением, которое появляется с `functionapp create` и в котором указан флаг `--functions_version`, но в имени флага ошибочно используется `_` вместо `-`.</span><span class="sxs-lookup"><span data-stu-id="82d30-621">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="82d30-622">az functionapp create: обновлен способ настройки linuxFxVersion и имени образа контейнера для приложений с функциями Linux.</span><span class="sxs-lookup"><span data-stu-id="82d30-622">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="82d30-623">az functionapp deployment source config-zip: устранена проблема, вызванная изменением параметров приложения во время развертывания ZIP, что приводит к ошибкам 5xx во время развертывания.</span><span class="sxs-lookup"><span data-stu-id="82d30-623">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="82d30-624">Исправление 5720946: не удается задать имя с помощью az webapp backup.</span><span class="sxs-lookup"><span data-stu-id="82d30-624">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="82d30-625">ARM</span><span class="sxs-lookup"><span data-stu-id="82d30-625">ARM</span></span>

* <span data-ttu-id="82d30-626">az resource: улучшены примеры для модуля ресурсов.</span><span class="sxs-lookup"><span data-stu-id="82d30-626">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="82d30-627">az policy assignment list: Включена поддержка списков назначений политик в области группы управления.</span><span class="sxs-lookup"><span data-stu-id="82d30-627">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="82d30-628">Добавлены команды `az deployment group` и `az deployment operation group` для развертывания шаблонов в группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="82d30-628">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="82d30-629">Это дубликат `az group deployment` и `az group deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="82d30-629">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="82d30-630">Добавлены команды `az deployment sub` и `az deployment operation sub` для развертывания шаблонов в области подписки.</span><span class="sxs-lookup"><span data-stu-id="82d30-630">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="82d30-631">Это дубликат `az deployment` и `az deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="82d30-631">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="82d30-632">Добавлены команды `az deployment mg` и `az deployment operation mg` для развертывания шаблонов в группах управления.</span><span class="sxs-lookup"><span data-stu-id="82d30-632">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="82d30-633">Добавлены команды `az deployment tenant` и `az deployment operation tenant` для развертывания шаблонов в области арендатора.</span><span class="sxs-lookup"><span data-stu-id="82d30-633">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="82d30-634">az policy assignment create: добавлено описание параметра `--location`.</span><span class="sxs-lookup"><span data-stu-id="82d30-634">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="82d30-635">az group deployment create: добавлен параметр `--aux-tenants` для включения поддержки перекрестных арендаторов.</span><span class="sxs-lookup"><span data-stu-id="82d30-635">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="82d30-636">CDN</span><span class="sxs-lookup"><span data-stu-id="82d30-636">CDN</span></span>

* <span data-ttu-id="82d30-637">Добавлены команды WAF CDN.</span><span class="sxs-lookup"><span data-stu-id="82d30-637">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="82d30-638">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="82d30-638">Compute</span></span>

* <span data-ttu-id="82d30-639">az sig image-version: добавлен параметр --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="82d30-639">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="82d30-640">az ppg show: добавлен параметр --colocation-status, чтобы включить выборку состояния совместного размещения всех ресурсов в группе размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="82d30-640">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="82d30-641">az vmss create/update: включена поддержка автоматического исправления.</span><span class="sxs-lookup"><span data-stu-id="82d30-641">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="82d30-642">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az image template: шаблон переименован в построитель.</span><span class="sxs-lookup"><span data-stu-id="82d30-642">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="82d30-643">az image builder create: добавлен параметр --image-template.</span><span class="sxs-lookup"><span data-stu-id="82d30-643">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="82d30-644">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-644">Cosmos DB</span></span>

* <span data-ttu-id="82d30-645">Добавлены командлеты хранимой процедуры SQL, определяемых пользователем функций и триггеров.</span><span class="sxs-lookup"><span data-stu-id="82d30-645">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="82d30-646">az cosmosdb create: добавлен параметр --key-uri для добавления сведений о шифровании хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="82d30-646">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="82d30-647">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="82d30-647">KeyVault</span></span>

* <span data-ttu-id="82d30-648">keyvault create: включена функция обратимого удаления по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-648">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-649">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-649">Monitor</span></span>

* <span data-ttu-id="82d30-650">az monitor metrics alert create: включена поддержка `~` в `--condition`.</span><span class="sxs-lookup"><span data-stu-id="82d30-650">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="82d30-651">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-651">Network</span></span>

* <span data-ttu-id="82d30-652">az network application-gateway rewrite-rule create: включена поддержка конфигурации URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="82d30-652">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="82d30-653">az network dns zone import: для параметра --zone-name в будущем можно будет не учитывать регистр.</span><span class="sxs-lookup"><span data-stu-id="82d30-653">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="82d30-654">az network private-endpoint/private-link-service: удалена метка предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="82d30-654">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="82d30-655">az network bastion: включена поддержка бастиона.</span><span class="sxs-lookup"><span data-stu-id="82d30-655">az network bastion: support bastion</span></span>
* <span data-ttu-id="82d30-656">az network vnet list-available-ips: включена поддержка списка доступных IP-адресов в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="82d30-656">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="82d30-657">az network watcher flow-log create/list/delete/update: добавлены новые команды для управления журналами потоков Наблюдателя и предоставлен параметр --location для явного определения Наблюдателя.</span><span class="sxs-lookup"><span data-stu-id="82d30-657">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="82d30-658">az network watcher flow-log configure: поддержка прекращена.</span><span class="sxs-lookup"><span data-stu-id="82d30-658">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="82d30-659">az network watcher flow-log show: включена поддержка параметров --location и --name для получения результатов в формате ARM; поддержка предыдущего форматированного вывода прекращена.</span><span class="sxs-lookup"><span data-stu-id="82d30-659">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="82d30-660">Политика</span><span class="sxs-lookup"><span data-stu-id="82d30-660">Policy</span></span>

* <span data-ttu-id="82d30-661">az policy assignment create: исправлена ошибка, из-за которой автоматически генерируемое имя назначения политики превышало предельное значение.</span><span class="sxs-lookup"><span data-stu-id="82d30-661">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="82d30-662">RBAC</span><span class="sxs-lookup"><span data-stu-id="82d30-662">RBAC</span></span>

* <span data-ttu-id="82d30-663">az ad group show: исправлено значение --group, обрабатываемое как проблема с регулярными выражениями.</span><span class="sxs-lookup"><span data-stu-id="82d30-663">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="82d30-664">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="82d30-664">RDBMS</span></span>

* <span data-ttu-id="82d30-665">Обновлена версия пакета SDK azure-mgmt-rdbms до 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="82d30-665">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="82d30-666">az postgres private-endpoint-connection: включено управление подключениями частных конечных точек Postgres.</span><span class="sxs-lookup"><span data-stu-id="82d30-666">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="82d30-667">az postgres private-link-resource: включено управление ресурсами частных ссылок Postgres.</span><span class="sxs-lookup"><span data-stu-id="82d30-667">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="82d30-668">az mysql private-endpoint-connection: включено управление подключениями частных конечных точек MySQL.</span><span class="sxs-lookup"><span data-stu-id="82d30-668">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="82d30-669">az mysql private-link-resource: включено управление ресурсами частных ссылок MySQL.</span><span class="sxs-lookup"><span data-stu-id="82d30-669">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="82d30-670">az mariadb private-endpoint-connection: включено управление подключениями частных конечных точек MariaDB.</span><span class="sxs-lookup"><span data-stu-id="82d30-670">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="82d30-671">az mariadb private-link-resource: включено управление ресурсами частных ссылок MariaDB.</span><span class="sxs-lookup"><span data-stu-id="82d30-671">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="82d30-672">Обновление тестов частной конечной точки RDBMS</span><span class="sxs-lookup"><span data-stu-id="82d30-672">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-673">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-673">SQL</span></span>

* <span data-ttu-id="82d30-674">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention.</span><span class="sxs-lookup"><span data-stu-id="82d30-674">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="82d30-675">(sql server create:) добавлен необязательный флаг включения и отключения доступа к общедоступным сетям в команду создания SQL Server.</span><span class="sxs-lookup"><span data-stu-id="82d30-675">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="82d30-676">(sql server update:) внесены некоторые изменения для клиентов.</span><span class="sxs-lookup"><span data-stu-id="82d30-676">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="82d30-677">Добавлено свойство minimal_tls_version для MI и SQL DB.</span><span class="sxs-lookup"><span data-stu-id="82d30-677">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-678">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-678">Storage</span></span>

* <span data-ttu-id="82d30-679">az storage blob delete-batch: исправлено неправильное поведение флага `--dryrun`.</span><span class="sxs-lookup"><span data-stu-id="82d30-679">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="82d30-680">az storage account network-rule add (исправление): добавлено требование того, чтобы операция была идемпотентной.</span><span class="sxs-lookup"><span data-stu-id="82d30-680">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="82d30-681">az storage account create/update: включена поддержка предпочтения маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="82d30-681">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="82d30-682">Обновлена версия azure-mgmt-storage до 8.0.0.</span><span class="sxs-lookup"><span data-stu-id="82d30-682">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="82d30-683">az storage container immutability create: добавлен параметр --allow-protected-append-write.</span><span class="sxs-lookup"><span data-stu-id="82d30-683">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="82d30-684">az storage account private-link-resource list: включена поддержка вывода списка ресурсов частной ссылки для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="82d30-684">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="82d30-685">az storage account private-endpoint-connection approve/reject/show/delete: включена поддержка управления подключениями к частным конечным точкам.</span><span class="sxs-lookup"><span data-stu-id="82d30-685">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="82d30-686">az storage account blob-service-properties update: добавлены параметры --enable-restore-policy и --restore-days.</span><span class="sxs-lookup"><span data-stu-id="82d30-686">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="82d30-687">az storage blob restore: включена поддержка восстановления диапазонов BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="82d30-687">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="82d30-688">18 февраля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-688">February 18, 2020</span></span>

<span data-ttu-id="82d30-689">Версия 2.1.0</span><span class="sxs-lookup"><span data-stu-id="82d30-689">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-690">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-690">ACR</span></span>

* <span data-ttu-id="82d30-691">Добавлен новый аргумент `--expose-token` для `az acr login`.</span><span class="sxs-lookup"><span data-stu-id="82d30-691">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="82d30-692">Исправлены неправильные выходные данные `az acr task identity show -n Name -r Registry -o table`.</span><span class="sxs-lookup"><span data-stu-id="82d30-692">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="82d30-693">az acr login: отображение CLIError при наличии ошибок, возвращаемых командой docker.</span><span class="sxs-lookup"><span data-stu-id="82d30-693">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-694">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-694">ACS</span></span>

* <span data-ttu-id="82d30-695">aks create/update: добавление проверки `--vnet-subnet-id`.</span><span class="sxs-lookup"><span data-stu-id="82d30-695">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="82d30-696">Aladdin</span><span class="sxs-lookup"><span data-stu-id="82d30-696">Aladdin</span></span>

* <span data-ttu-id="82d30-697">Выполнение синтаксического анализа созданных примеров в _help.py для команд.</span><span class="sxs-lookup"><span data-stu-id="82d30-697">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="82d30-698">AMS</span><span class="sxs-lookup"><span data-stu-id="82d30-698">AMS</span></span>

* <span data-ttu-id="82d30-699">az ams теперь предоставляется в общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="82d30-699">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="82d30-700">AppConfig</span><span class="sxs-lookup"><span data-stu-id="82d30-700">AppConfig</span></span>

* <span data-ttu-id="82d30-701">Исправлено справочное сообщение, чтобы исключить неподдерживаемый фильтр ключей или меток.</span><span class="sxs-lookup"><span data-stu-id="82d30-701">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="82d30-702">Удален тег preview для большинства команд, кроме управляемого удостоверения и флагов функций.</span><span class="sxs-lookup"><span data-stu-id="82d30-702">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="82d30-703">Добавлен управляемый ключ клиента при обновлении магазинов.</span><span class="sxs-lookup"><span data-stu-id="82d30-703">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-704">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-704">AppService</span></span>

* <span data-ttu-id="82d30-705">az webapp list-runtimes: исправлена ошибка для list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="82d30-705">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="82d30-706">Добавлена команда az webapp|functionapp config ssl create.</span><span class="sxs-lookup"><span data-stu-id="82d30-706">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="82d30-707">Включена поддержка приложений-функций версии 3 и Node 12.</span><span class="sxs-lookup"><span data-stu-id="82d30-707">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="82d30-708">ARM</span><span class="sxs-lookup"><span data-stu-id="82d30-708">ARM</span></span>

* <span data-ttu-id="82d30-709">az policy assignment create: исправлено сообщение об ошибке, если параметр `--policy` является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="82d30-709">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="82d30-710">az group deployment create: Устранена ошибка stat: path too long for Windows при использовании большого файла parameters.json.</span><span class="sxs-lookup"><span data-stu-id="82d30-710">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="82d30-711">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="82d30-711">Backup</span></span>

* <span data-ttu-id="82d30-712">Исправлен поток восстановления на уровне элемента в OLR.</span><span class="sxs-lookup"><span data-stu-id="82d30-712">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="82d30-713">Включена поддержка восстановления в виде файлов для баз данных SQL и SAP.</span><span class="sxs-lookup"><span data-stu-id="82d30-713">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="82d30-714">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="82d30-714">Compute</span></span>

* <span data-ttu-id="82d30-715">vm/vmss/availability-set update: add --ppg: разрешено обновление ProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="82d30-715">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="82d30-716">vmss create: add --data-disk-iops and --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="82d30-716">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="82d30-717">az vm host: удален тег preview для `vm host` и `vm host group`.</span><span class="sxs-lookup"><span data-stu-id="82d30-717">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="82d30-718">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправление 10728. `az vm create`: автоматическое создание подсети, если указанные виртуальная сеть и подсеть не существуют.</span><span class="sxs-lookup"><span data-stu-id="82d30-718">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="82d30-719">Повышена надежность списка образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="82d30-719">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="82d30-720">Eventhub</span><span class="sxs-lookup"><span data-stu-id="82d30-720">Eventhub</span></span>

* <span data-ttu-id="82d30-721">Включена поддержка Azure Stack для профиля 2019-03-01-hybrid.</span><span class="sxs-lookup"><span data-stu-id="82d30-721">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="82d30-722">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="82d30-722">KeyVault</span></span>

* <span data-ttu-id="82d30-723">az keyvault key create: добавлено новое значение `import` для параметра `--ops`.</span><span class="sxs-lookup"><span data-stu-id="82d30-723">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="82d30-724">az keyvault key list-versions: включена поддержка параметров `--id` для определения ключей.</span><span class="sxs-lookup"><span data-stu-id="82d30-724">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="82d30-725">Включена поддержка подключений к частным конечным точкам.</span><span class="sxs-lookup"><span data-stu-id="82d30-725">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="82d30-726">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-726">Network</span></span>

* <span data-ttu-id="82d30-727">Выполнена активация azure-mgmt-network 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="82d30-727">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="82d30-728">az network private-link-service update/create: включена поддержка --enable-proxy-protocol.</span><span class="sxs-lookup"><span data-stu-id="82d30-728">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="82d30-729">Добавлена функция монитора подключения версии 2.</span><span class="sxs-lookup"><span data-stu-id="82d30-729">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="82d30-730">Упаковка</span><span class="sxs-lookup"><span data-stu-id="82d30-730">Packaging</span></span>

* <span data-ttu-id="82d30-731">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка Python 2.7.</span><span class="sxs-lookup"><span data-stu-id="82d30-731">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-732">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-732">Profile</span></span>

* <span data-ttu-id="82d30-733">Предварительный просмотр: В учетные записи подписок добавлены новые атрибуты `homeTenantId` и `managedByTenants`.</span><span class="sxs-lookup"><span data-stu-id="82d30-733">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="82d30-734">Чтобы изменения вступили в силу, повторно выполните команду `az login`.</span><span class="sxs-lookup"><span data-stu-id="82d30-734">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="82d30-735">az login: отображение предупреждения, если подписка связана с несколькими клиентами, но по умолчанию используется с первым из них</span><span class="sxs-lookup"><span data-stu-id="82d30-735">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="82d30-736">(чтобы выбрать определенный клиент при доступе к этой подписке, включите `--tenant` в `az login`).</span><span class="sxs-lookup"><span data-stu-id="82d30-736">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="82d30-737">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-737">Role</span></span>

* <span data-ttu-id="82d30-738">az role assignment create: исправлена ошибка с кодом HTTP 400, возникающая при присвоении роли субъекту-службе по отображаемому имени.</span><span class="sxs-lookup"><span data-stu-id="82d30-738">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-739">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-739">SQL</span></span>

* <span data-ttu-id="82d30-740">Обновлен командлет `az sql mi update` Управляемого экземпляра SQL (добавлены два новых параметра: tier и family).</span><span class="sxs-lookup"><span data-stu-id="82d30-740">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-741">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-741">Storage</span></span>

* <span data-ttu-id="82d30-742">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az storage account create`: Тип учетной записи хранения по умолчанию изменен на StorageV2.</span><span class="sxs-lookup"><span data-stu-id="82d30-742">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="82d30-743">4 февраля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-743">February 04, 2020</span></span>

<span data-ttu-id="82d30-744">Версия 2.0.81</span><span class="sxs-lookup"><span data-stu-id="82d30-744">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-745">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-745">ACS</span></span>

* <span data-ttu-id="82d30-746">Добавлена возможность задания выделенных исходящих портов и времени ожидания подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="82d30-746">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="82d30-747">Выполнено обновление до API версии 2019-11-01.</span><span class="sxs-lookup"><span data-stu-id="82d30-747">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-748">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-748">ACR</span></span>

* <span data-ttu-id="82d30-749">[Критическое изменение] `az acr delete` будет выводить запрос.</span><span class="sxs-lookup"><span data-stu-id="82d30-749">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="82d30-750">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда az acr task delete будет выводить запрос.</span><span class="sxs-lookup"><span data-stu-id="82d30-750">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="82d30-751">Добавлена новая группа команд az acr taskrun show/list/delete для управления выполнением задач.</span><span class="sxs-lookup"><span data-stu-id="82d30-751">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="82d30-752">AKS</span><span class="sxs-lookup"><span data-stu-id="82d30-752">AKS</span></span>

* <span data-ttu-id="82d30-753">Каждый кластер получает отдельный субъект-службу для улучшения изоляции.</span><span class="sxs-lookup"><span data-stu-id="82d30-753">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="82d30-754">AppConfig</span><span class="sxs-lookup"><span data-stu-id="82d30-754">AppConfig</span></span>

* <span data-ttu-id="82d30-755">Поддержка импорта ссылок на хранилище ключей из службы приложений и их экспорта в нее.</span><span class="sxs-lookup"><span data-stu-id="82d30-755">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="82d30-756">Поддержка импорта и экспорта всех меток между файлами appconfig.</span><span class="sxs-lookup"><span data-stu-id="82d30-756">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="82d30-757">Проверка имен ключей и функций перед настройкой и импортом.</span><span class="sxs-lookup"><span data-stu-id="82d30-757">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="82d30-758">Предоставление изменений номера SKU в хранилище конфигураций.</span><span class="sxs-lookup"><span data-stu-id="82d30-758">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="82d30-759">Новая группа команд для управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="82d30-759">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-760">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-760">AppService</span></span>

* <span data-ttu-id="82d30-761">Azure Stack: команды поверхности в профиле 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="82d30-761">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="82d30-762">functionapp: добавлена возможность создавать приложения-функции Java в Linux.</span><span class="sxs-lookup"><span data-stu-id="82d30-762">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="82d30-763">ARM</span><span class="sxs-lookup"><span data-stu-id="82d30-763">ARM</span></span>

* <span data-ttu-id="82d30-764">Исправление ошибки 10246: аварийное завершение `az resource tag` в случае, если переданный параметр `--ids` являлся идентификатором группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="82d30-764">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="82d30-765">Исправление ошибки 11658: команда `az group export` не поддерживала параметры `--query` и `--output`.</span><span class="sxs-lookup"><span data-stu-id="82d30-765">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="82d30-766">Исправление ошибки 10279: код выхода `az group deployment validate` был равен 0, если проверка не пройдена.</span><span class="sxs-lookup"><span data-stu-id="82d30-766">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="82d30-767">Исправление ошибки 9916: улучшено сообщение об ошибке из-за конфликта между тегом и другими условиями фильтра для команды `az resource list`.</span><span class="sxs-lookup"><span data-stu-id="82d30-767">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="82d30-768">Добавлен новый параметр `--managed-by` для добавления данных managedBy для команды `az group create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-768">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="82d30-769">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="82d30-769">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="82d30-770">Добавлена подгруппа `monitor` для управления мониторингом Log Analytics в кластере Azure Red Hat OpensShift.</span><span class="sxs-lookup"><span data-stu-id="82d30-770">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="82d30-771">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="82d30-771">BotService</span></span>

* <span data-ttu-id="82d30-772">Исправление ошибки 11697: команда `az bot create` не являлась идемпотентной.</span><span class="sxs-lookup"><span data-stu-id="82d30-772">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="82d30-773">Проверки исправления имен изменены для выполнения только в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="82d30-773">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="82d30-774">CDN</span><span class="sxs-lookup"><span data-stu-id="82d30-774">CDN</span></span>

* <span data-ttu-id="82d30-775">Добавлена поддержка функции rulesEngine.</span><span class="sxs-lookup"><span data-stu-id="82d30-775">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="82d30-776">Добавлена новая группа команд cdn endpoint rule для управления правилами.</span><span class="sxs-lookup"><span data-stu-id="82d30-776">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="82d30-777">Пакет azure-mgmt-cdn обновлен до версии 4.0.0 для использования API версии 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="82d30-777">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="82d30-778">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="82d30-778">Deployment Manager</span></span>

* <span data-ttu-id="82d30-779">Добавлена операция вывода списка всех ресурсов.</span><span class="sxs-lookup"><span data-stu-id="82d30-779">Add list operation for all resources.</span></span>
* <span data-ttu-id="82d30-780">Улучшен ресурс шага для нового типа шага.</span><span class="sxs-lookup"><span data-stu-id="82d30-780">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="82d30-781">Пакет azure-mgmt-deploymentmanager обновлен для использования версии 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="82d30-781">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-782">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-782">IoT</span></span>

* <span data-ttu-id="82d30-783">Команды IoT hub Job объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="82d30-783">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="82d30-784">IoT Central</span><span class="sxs-lookup"><span data-stu-id="82d30-784">IoT Central</span></span>

* <span data-ttu-id="82d30-785">Добавлена поддержка создания и обновления приложений с новыми SKU: ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="82d30-785">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="82d30-786">Key Vault</span><span class="sxs-lookup"><span data-stu-id="82d30-786">Key Vault</span></span>

* <span data-ttu-id="82d30-787">Добавлена новая команда `az keyvault key download` для скачивания ключей.</span><span class="sxs-lookup"><span data-stu-id="82d30-787">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="82d30-788">Разное</span><span class="sxs-lookup"><span data-stu-id="82d30-788">Misc</span></span>

* <span data-ttu-id="82d30-789">Исправление ошибки 6371: поддержка завершения имен файлов и переменных среды в Bash.</span><span class="sxs-lookup"><span data-stu-id="82d30-789">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="82d30-790">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-790">Network</span></span>

* <span data-ttu-id="82d30-791">Исправление ошибки 2092: для команды az network dns record-set add/remove добавлено предупреждение, отображаемое, если набор записей не найден.</span><span class="sxs-lookup"><span data-stu-id="82d30-791">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="82d30-792">В будущем для подтверждения этого автоматического создания будет добавлен дополнительный аргумент.</span><span class="sxs-lookup"><span data-stu-id="82d30-792">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="82d30-793">Политика</span><span class="sxs-lookup"><span data-stu-id="82d30-793">Policy</span></span>

* <span data-ttu-id="82d30-794">Добавлена новая команда `az policy metadata` для получения ресурсов метаданных расширенной политики.</span><span class="sxs-lookup"><span data-stu-id="82d30-794">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="82d30-795">`az policy remediation create`: С помощью параметра `--resource-discovery-mode` можно указать, следует ли повторно оценить соответствие перед исправлением.</span><span class="sxs-lookup"><span data-stu-id="82d30-795">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-796">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-796">Profile</span></span>

* <span data-ttu-id="82d30-797">`az account get-access-token`: Добавлен параметр `--tenant` для получения маркера для арендатора напрямую, без необходимости указывать подписку.</span><span class="sxs-lookup"><span data-stu-id="82d30-797">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="82d30-798">RBAC</span><span class="sxs-lookup"><span data-stu-id="82d30-798">RBAC</span></span>

* <span data-ttu-id="82d30-799">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправление ошибки 11883: `az role assignment create`: пустая область приведет к ошибке.</span><span class="sxs-lookup"><span data-stu-id="82d30-799">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="82d30-800">Безопасность</span><span class="sxs-lookup"><span data-stu-id="82d30-800">Security</span></span>

* <span data-ttu-id="82d30-801">Добавлены новые команды `az atp show` и `az atp update` для просмотра и настройки дополнительных параметров защиты от угроз для учетных записей хранения.</span><span class="sxs-lookup"><span data-stu-id="82d30-801">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-802">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-802">SQL</span></span>

* <span data-ttu-id="82d30-803">`sql dw create`: параметры `--zone-redundant` и `--read-replica-count` объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="82d30-803">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="82d30-804">Эти параметры не применяются к хранилищу данных.</span><span class="sxs-lookup"><span data-stu-id="82d30-804">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="82d30-805">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql db create`: Значения WideWorldImportersStd и WideWorldImportersFull больше не являются задокументированным допустимыми значениями для команды az sql db create --sample-name.</span><span class="sxs-lookup"><span data-stu-id="82d30-805">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="82d30-806">Эти примеры базы данных всегда будут приводить к сбою создания.</span><span class="sxs-lookup"><span data-stu-id="82d30-806">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="82d30-807">Добавлены новые команды `sql db classification show/list/update/delete` и `sql db classification recommendation list/enable/disable` для управления классификациями конфиденциальности баз данных SQL.</span><span class="sxs-lookup"><span data-stu-id="82d30-807">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="82d30-808">`az sql db audit-policy`: устранены пустые действия аудита и группы.</span><span class="sxs-lookup"><span data-stu-id="82d30-808">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-809">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-809">Storage</span></span>

* <span data-ttu-id="82d30-810">Добавлена новая группа команд `az storage share-rm` для использования поставщика ресурсов Microsoft.Storage в операциях управления файловыми ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="82d30-810">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="82d30-811">Исправление ошибки 11415: ошибка разрешения для `az storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-811">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="82d30-812">Добавлены интеграция AzCopy 10.3.3 и поддержка Win32.</span><span class="sxs-lookup"><span data-stu-id="82d30-812">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="82d30-813">`az storage copy`: добавлены параметры `--include-path`, `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="82d30-813">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="82d30-814">`az storage remove`: параметры `--inlcude` и `--exclude` заменены параметрами `--include-path`, `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="82d30-814">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="82d30-815">`az storage sync`: добавлены параметры `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="82d30-815">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="82d30-816">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="82d30-816">ServiceFabric</span></span>

* <span data-ttu-id="82d30-817">Добавлены новые команды для управления приложениями и службами.</span><span class="sxs-lookup"><span data-stu-id="82d30-817">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="82d30-818">13 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-818">January 13, 2020</span></span>

<span data-ttu-id="82d30-819">Версия 2.0.80</span><span class="sxs-lookup"><span data-stu-id="82d30-819">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="82d30-820">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="82d30-820">Compute</span></span>

* <span data-ttu-id="82d30-821">Обновление диска: добавлены параметры --disk-encryption-set и --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="82d30-821">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="82d30-822">Создание и обновление моментального снимка: добавлены параметры --disk-encryption-set и --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="82d30-822">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-823">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-823">Storage</span></span>

* <span data-ttu-id="82d30-824">Обновление azure-mgmt-storage до версии 7.1.0</span><span class="sxs-lookup"><span data-stu-id="82d30-824">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="82d30-825">`az storage account create`: добавлены параметры `--encryption-key-type-for-table` и `--encryption-key-type-for-queue` для включения поддержки службы шифрования таблиц и очередей.</span><span class="sxs-lookup"><span data-stu-id="82d30-825">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="82d30-826">7 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-826">January 07, 2020</span></span>

<span data-ttu-id="82d30-827">Версия 2.0.79</span><span class="sxs-lookup"><span data-stu-id="82d30-827">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-828">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-828">ACR</span></span>

* <span data-ttu-id="82d30-829">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --os для команд acr build, acr task create/update, acr run и acr pack.</span><span class="sxs-lookup"><span data-stu-id="82d30-829">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="82d30-830">Вместо этого используется параметр --platform.</span><span class="sxs-lookup"><span data-stu-id="82d30-830">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="82d30-831">AppConfig</span><span class="sxs-lookup"><span data-stu-id="82d30-831">AppConfig</span></span>

* <span data-ttu-id="82d30-832">Добавлена поддержка импорта и экспорта флагов функций.</span><span class="sxs-lookup"><span data-stu-id="82d30-832">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="82d30-833">Добавлена новая команда az appconfig kv set-keyvault для создания ссылки на хранилище ключей.</span><span class="sxs-lookup"><span data-stu-id="82d30-833">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="82d30-834">Добавлена поддержка различных соглашений об именовании при экспорте флагов функций в файл.</span><span class="sxs-lookup"><span data-stu-id="82d30-834">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-835">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-835">AppService</span></span>

* <span data-ttu-id="82d30-836">Устранена проблема № 7154: обновлена документация по команде <> — теперь в ней используются обратные, а не одинарные кавычки.</span><span class="sxs-lookup"><span data-stu-id="82d30-836">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="82d30-837">Устранена проблема № 11287 (webapp up): по умолчанию для приложения, созданного с использованием этого флага, должен быть включен SSL.</span><span class="sxs-lookup"><span data-stu-id="82d30-837">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="82d30-838">Устранена проблема № 11592: добавлен флаг az webapp up для статических сайтов HTML.</span><span class="sxs-lookup"><span data-stu-id="82d30-838">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="82d30-839">ARM</span><span class="sxs-lookup"><span data-stu-id="82d30-839">ARM</span></span>

* <span data-ttu-id="82d30-840">Исправлена ошибка с командой `az resource tag`: невозможно было обновить теги хранилища Служб восстановления.</span><span class="sxs-lookup"><span data-stu-id="82d30-840">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="82d30-841">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="82d30-841">Backup</span></span>

* <span data-ttu-id="82d30-842">Добавлена новая команда backup protection undelete для включения функции обратимого удаления рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="82d30-842">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="82d30-843">Добавлен новый параметр --soft-delete-feature-state для команды set backup-properties.</span><span class="sxs-lookup"><span data-stu-id="82d30-843">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="82d30-844">Добавлена поддержка исключения диска для рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="82d30-844">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="82d30-845">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="82d30-845">Compute</span></span>

* <span data-ttu-id="82d30-846">Исправлен сбой `vm create` в профиле Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="82d30-846">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="82d30-847">Добавлена поддержка определений списков и метрик запросов для виртуальной машины (vm monitor metrics tail/list-definitions).</span><span class="sxs-lookup"><span data-stu-id="82d30-847">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="82d30-848">Добавлено новое действия повторного применения команды az vm</span><span class="sxs-lookup"><span data-stu-id="82d30-848">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82d30-849">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82d30-849">HDInsight</span></span>

* <span data-ttu-id="82d30-850">Включена поддержка создания кластера Kafka с помощью прокси-сервера Kafka RESTful.</span><span class="sxs-lookup"><span data-stu-id="82d30-850">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="82d30-851">Обновление azure-mgmt-hdinsight до версии 1.3.0</span><span class="sxs-lookup"><span data-stu-id="82d30-851">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="82d30-852">Прочее</span><span class="sxs-lookup"><span data-stu-id="82d30-852">Misc.</span></span>

* <span data-ttu-id="82d30-853">Добавлена команда `az version show` предварительного просмотра для отображения версий модулей и расширений Azure CLI в формате JSON по умолчанию или в формате, настроенном с помощью параметра --output</span><span class="sxs-lookup"><span data-stu-id="82d30-853">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="82d30-854">Центры событий</span><span class="sxs-lookup"><span data-stu-id="82d30-854">Event Hubs</span></span>

* <span data-ttu-id="82d30-855">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az eventhubs eventhub update и az eventhubs eventhub create.</span><span class="sxs-lookup"><span data-stu-id="82d30-855">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="82d30-856">Данный параметр недопустим для сущностей концентратора событий.</span><span class="sxs-lookup"><span data-stu-id="82d30-856">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="82d30-857">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="82d30-857">Service Bus</span></span>

* <span data-ttu-id="82d30-858">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az servicebus topic create, az servicebus topic update, az servicebus queue create и az servicebus queue update.</span><span class="sxs-lookup"><span data-stu-id="82d30-858">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="82d30-859">Этот параметр является недопустимым для разделов и очередей служебной шины.</span><span class="sxs-lookup"><span data-stu-id="82d30-859">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="82d30-860">RBAC</span><span class="sxs-lookup"><span data-stu-id="82d30-860">RBAC</span></span>

* <span data-ttu-id="82d30-861">Устранена проблема № 11712: команда `az ad app/sp show` не возвращала код выхода 3, если приложение или субъект-служба не существует.</span><span class="sxs-lookup"><span data-stu-id="82d30-861">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-862">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-862">Storage</span></span>

* <span data-ttu-id="82d30-863">`az storage account create`: удален флаг предварительного просмотра для параметра --enable-hierarchical-namespace.</span><span class="sxs-lookup"><span data-stu-id="82d30-863">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="82d30-864">Хранилище azure-mgmt-storage обновлено до версии 7.0.0 для использования API версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="82d30-864">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="82d30-865">Добавлены новые параметры (`--enable-delete-retention` и `--delete-retention-days`) для поддержки управления политикой хранения удаленных свойств службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="82d30-865">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="82d30-866">17 декабря 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-866">December 17, 2019</span></span>

<span data-ttu-id="82d30-867">2.0.78</span><span class="sxs-lookup"><span data-stu-id="82d30-867">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-868">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-868">ACR</span></span>

* <span data-ttu-id="82d30-869">Добавлена поддержка локального контекста во время выполнения задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="82d30-869">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-870">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-870">ACS</span></span>

* <span data-ttu-id="82d30-871">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде az openshift create параметр `--workspace-resource-id` переименован на `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="82d30-871">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="82d30-872">AMS</span><span class="sxs-lookup"><span data-stu-id="82d30-872">AMS</span></span>

* <span data-ttu-id="82d30-873">Команды show обновлены для возвращения ответа 3, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="82d30-873">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="82d30-874">AppConfig</span><span class="sxs-lookup"><span data-stu-id="82d30-874">AppConfig</span></span>

* <span data-ttu-id="82d30-875">Исправлена ошибка, возникающая при добавлении api-version в URL-адрес запроса.</span><span class="sxs-lookup"><span data-stu-id="82d30-875">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="82d30-876">Имеющееся решение не работает с разбивкой на страницы.</span><span class="sxs-lookup"><span data-stu-id="82d30-876">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="82d30-877">Добавлена поддержка отображения языков, кроме английского, так как наша внутренняя служба поддерживает Юникод для глобализации.</span><span class="sxs-lookup"><span data-stu-id="82d30-877">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-878">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-878">AppService</span></span>

* <span data-ttu-id="82d30-879">Устранена проблема № 11217 (webapp): теперь команда az webapp config ssl upload поддерживает параметр слота.</span><span class="sxs-lookup"><span data-stu-id="82d30-879">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="82d30-880">Устранена проблема № 10965. Ошибка: Имя не может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="82d30-880">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="82d30-881">Разрешено удаление по IP-адресу и подсети.</span><span class="sxs-lookup"><span data-stu-id="82d30-881">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="82d30-882">Добавлена поддержка импорта сертификатов из хранилища ключей: `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="82d30-882">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="82d30-883">ARM</span><span class="sxs-lookup"><span data-stu-id="82d30-883">ARM</span></span>

* <span data-ttu-id="82d30-884">Обновлен пакет ресурсов azure-mgmt-resource для использования версии 6.0.0</span><span class="sxs-lookup"><span data-stu-id="82d30-884">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="82d30-885">Добавлена межклиентская поддержка команды `az group deployment create` путем добавления нового параметра `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="82d30-885">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="82d30-886">Добавлен новый параметр `--metadata` для поддержки добавления метаданных определений наборов политик.</span><span class="sxs-lookup"><span data-stu-id="82d30-886">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="82d30-887">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="82d30-887">Backup</span></span>

* <span data-ttu-id="82d30-888">Добавлена поддержка резервного копирования для рабочей нагрузки SQL и SAP HANA.</span><span class="sxs-lookup"><span data-stu-id="82d30-888">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="82d30-889">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="82d30-889">BotService</span></span>

* <span data-ttu-id="82d30-890">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг --version из предварительной версии команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="82d30-890">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="82d30-891">Поддерживаются только боты пакетов SDK версии 4.</span><span class="sxs-lookup"><span data-stu-id="82d30-891">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="82d30-892">Добавлена проверка доступности имени для команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="82d30-892">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="82d30-893">Добавлена поддержка обновления URL-адреса значка для бота с помощью команды az bot update.</span><span class="sxs-lookup"><span data-stu-id="82d30-893">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="82d30-894">Добавлена поддержка обновления канала Direct Line с помощью команды az bot directline update.</span><span class="sxs-lookup"><span data-stu-id="82d30-894">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="82d30-895">Добавлена поддержка флага --enable-enhanced-auth в команде az bot directline create.</span><span class="sxs-lookup"><span data-stu-id="82d30-895">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="82d30-896">Следующие группы команд предоставляются в общедоступной, а не в предварительной версии: az bot authsetting.</span><span class="sxs-lookup"><span data-stu-id="82d30-896">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="82d30-897">Следующие команды в az bot предоставляются в общедоступной, а не в предварительной версии: create, prepare-deploy, show, delete и update.</span><span class="sxs-lookup"><span data-stu-id="82d30-897">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="82d30-898">Устранена проблема с командой az bot prepare-deploy, которая изменяла значение параметра --proj-file-path на нижний регистр (например, с Test.csproj на test.csproj).</span><span class="sxs-lookup"><span data-stu-id="82d30-898">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="82d30-899">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="82d30-899">Compute</span></span>

* <span data-ttu-id="82d30-900">vmss create/update: добавлен параметр --scale-on-policy, который определяет, какие виртуальные машины выбираются для удаления при масштабировании VMSS.</span><span class="sxs-lookup"><span data-stu-id="82d30-900">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="82d30-901">vm/vmss update: добавлен параметр --priority.</span><span class="sxs-lookup"><span data-stu-id="82d30-901">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="82d30-902">vm/vmss update: добавлен параметр --max-price.</span><span class="sxs-lookup"><span data-stu-id="82d30-902">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="82d30-903">Добавлена группа команд для шифрования дисков (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="82d30-903">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="82d30-904">disk create: добавлены параметры --encryption-type и --disk-encryption-set.</span><span class="sxs-lookup"><span data-stu-id="82d30-904">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="82d30-905">vm/vmss create. Добавлены параметры --os-disk-encryption-set и --data-disk-encryption-sets.</span><span class="sxs-lookup"><span data-stu-id="82d30-905">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="82d30-906">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-906">Core</span></span>

* <span data-ttu-id="82d30-907">Удалена поддержка Python версии 3.4.</span><span class="sxs-lookup"><span data-stu-id="82d30-907">Removed support for Python 3.4</span></span>
* <span data-ttu-id="82d30-908">Подключение к опросу HaTS в нескольких командах.</span><span class="sxs-lookup"><span data-stu-id="82d30-908">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="82d30-909">DLS</span><span class="sxs-lookup"><span data-stu-id="82d30-909">DLS</span></span>

* <span data-ttu-id="82d30-910">Обновлена версия пакета SDK для ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="82d30-910">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="82d30-911">Установка</span><span class="sxs-lookup"><span data-stu-id="82d30-911">Install</span></span>

* <span data-ttu-id="82d30-912">Добавлена поддержка установки скриптов Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="82d30-912">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-913">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-913">IOT</span></span>

* <span data-ttu-id="82d30-914">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --failover-region из команды manual-failover.</span><span class="sxs-lookup"><span data-stu-id="82d30-914">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="82d30-915">Теперь она будет выполнять отработку отказа в назначенный геопарный дополнительный регион.</span><span class="sxs-lookup"><span data-stu-id="82d30-915">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="82d30-916">Key Vault</span><span class="sxs-lookup"><span data-stu-id="82d30-916">Key Vault</span></span>

* <span data-ttu-id="82d30-917">Устранена проблема № 8095: (`az keyvault storage remove`): улучшено справочное сообщение.</span><span class="sxs-lookup"><span data-stu-id="82d30-917">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="82d30-918">Устранена проблема № 8921 (`az keyvault key/secret/certificate list/list-deleted/list-versions`): исправлена ошибка проверки в параметре `--maxresults`.</span><span class="sxs-lookup"><span data-stu-id="82d30-918">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="82d30-919">Устранена проблема № 10512 (`az keyvault set-policy`): улучшено сообщение об ошибке, возвращаемое, если не указан ни один из параметров `--object-id`, `--spn` или `--upn`.</span><span class="sxs-lookup"><span data-stu-id="82d30-919">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="82d30-920">Устранена проблема № 10846 (`az keyvault secret show-deleted`): при указании значения `--id` значение `--name/-n` не требовалось.</span><span class="sxs-lookup"><span data-stu-id="82d30-920">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="82d30-921">Устранена проблема № 11084: (`az keyvault secret download`): улучшено справочное сообщение параметра `--encoding`.</span><span class="sxs-lookup"><span data-stu-id="82d30-921">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="82d30-922">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-922">Network</span></span>

* <span data-ttu-id="82d30-923">az network application-gateway probe: добавлена поддержка параметра --port, позволяющего указать порт, который используется для проверки внутренних серверов при создании и обновлении.</span><span class="sxs-lookup"><span data-stu-id="82d30-923">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="82d30-924">az network application-gateway url-path-map create/update: исправлена ошибка с `--waf-policy`.</span><span class="sxs-lookup"><span data-stu-id="82d30-924">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="82d30-925">az network application-gateway: добавлена поддержка параметра `--rewrite-rule-set`.</span><span class="sxs-lookup"><span data-stu-id="82d30-925">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="82d30-926">az network list-service-aliases: добавлена поддержка перечисления псевдонимов служб, которые можно использовать для политик конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="82d30-926">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="82d30-927">az network dns zone import: добавлена поддержка символа .@ в имени записи.</span><span class="sxs-lookup"><span data-stu-id="82d30-927">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="82d30-928">Упаковка</span><span class="sxs-lookup"><span data-stu-id="82d30-928">Packaging</span></span>

* <span data-ttu-id="82d30-929">Снова добавлены сборки Edge для установки PIP.</span><span class="sxs-lookup"><span data-stu-id="82d30-929">Added back edge builds for pip install</span></span>
* <span data-ttu-id="82d30-930">Добавлен пакет Ubuntu eoan.</span><span class="sxs-lookup"><span data-stu-id="82d30-930">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="82d30-931">Политика</span><span class="sxs-lookup"><span data-stu-id="82d30-931">Policy</span></span>

* <span data-ttu-id="82d30-932">Добавлена поддержка API Политики версии 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="82d30-932">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="82d30-933">az policy set-definition: добавлена поддержка группирования в определениях наборов политик с помощью параметра `--definition-groups`.</span><span class="sxs-lookup"><span data-stu-id="82d30-933">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="82d30-934">Redis</span><span class="sxs-lookup"><span data-stu-id="82d30-934">Redis</span></span>

* <span data-ttu-id="82d30-935">В команду `az redis create` добавлена предварительная версия параметра `--replicas-per-master`.</span><span class="sxs-lookup"><span data-stu-id="82d30-935">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="82d30-936">Обновлена версия azure-mgmt-redis с 6.0.0 на 7.0.0 RC1.</span><span class="sxs-lookup"><span data-stu-id="82d30-936">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="82d30-937">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="82d30-937">ServiceFabric</span></span>

* <span data-ttu-id="82d30-938">Исправлена логика добавления типа узла, а также устранена проблема № 10963: при добавлении нового типа узла с уровнем устойчивости Gold возникала ошибка CLI.</span><span class="sxs-lookup"><span data-stu-id="82d30-938">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="82d30-939">Обновлена версия параметра ServiceFabricNodeVmExt до 1.1 в шаблоне создания.</span><span class="sxs-lookup"><span data-stu-id="82d30-939">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-940">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-940">SQL</span></span>

* <span data-ttu-id="82d30-941">В команды create и update базы данных SQL добавлены параметры --read-scale и --read-replicas для поддержки управления масштабированием операций чтения.</span><span class="sxs-lookup"><span data-stu-id="82d30-941">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-942">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-942">Storage</span></span>

* <span data-ttu-id="82d30-943">Выпущена общедоступная версия больших файловых ресурсов для команды создания и обновления учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="82d30-943">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="82d30-944">Выпущена общедоступная версия поддержки маркера SAS для делегирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="82d30-944">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="82d30-945">Добавлены новые команды (`az storage account blob-service-properties show` и `az storage account blob-service-properties update --enable-change-feed`) для управления свойствами службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="82d30-945">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="82d30-946">[ОЖИДАЕТСЯ КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] `az storage copy`: символ `*` больше не поддерживается в качестве подстановочного знака в URL-адресе. Тем не менее новые параметры--include-pattern и--exclude-pattern будут добавлены с поддержкой подстановочных знаков `*`.</span><span class="sxs-lookup"><span data-stu-id="82d30-946">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="82d30-947">Устранена проблема № 11043: добавлена поддержка удаления всего контейнера или общего ресурса в команде `az storage remove`.</span><span class="sxs-lookup"><span data-stu-id="82d30-947">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="82d30-948">26 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-948">November 26, 2019</span></span>

<span data-ttu-id="82d30-949">Версия 2.0.77</span><span class="sxs-lookup"><span data-stu-id="82d30-949">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-950">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-950">ACR</span></span>

* <span data-ttu-id="82d30-951">Параметр `--branch`, используемый при обновлении или создании задачи ACR, объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="82d30-951">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="82d30-952">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="82d30-952">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="82d30-953">Добавлен флаг `--workspace-resource-id` для создания кластера Azure Red Hat Openshift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="82d30-953">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="82d30-954">Добавлен флаг `monitor_profile` для создания кластера Azure Red Hat OpenShift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="82d30-954">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="82d30-955">AKS</span><span class="sxs-lookup"><span data-stu-id="82d30-955">AKS</span></span>

* <span data-ttu-id="82d30-956">Включена поддержка операции смены сертификата кластера с использованием команды az aks rotate-certs.</span><span class="sxs-lookup"><span data-stu-id="82d30-956">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="82d30-957">AppConfig</span><span class="sxs-lookup"><span data-stu-id="82d30-957">AppConfig</span></span>

* <span data-ttu-id="82d30-958">Включена поддержка использования символа ":" для разделителя `as az appconfig kv import`.</span><span class="sxs-lookup"><span data-stu-id="82d30-958">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="82d30-959">Исправлена проблема с перечислением значений ключей с несколькими метками, включая метку NULL.</span><span class="sxs-lookup"><span data-stu-id="82d30-959">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="82d30-960">Обновлен пакет SDK для плоскости управления, azure-mgmt-appconfiguration, до версии 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="82d30-960">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="82d30-961">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-961">AppService</span></span>

* <span data-ttu-id="82d30-962">Исправлена ошибка № 11100. Использование AttributeError для az webapp up при создании плана службы.</span><span class="sxs-lookup"><span data-stu-id="82d30-962">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="82d30-963">az webapp up. При принудительном создании или развертывании сайта для поддерживаемых языков значения по умолчанию не используются.</span><span class="sxs-lookup"><span data-stu-id="82d30-963">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="82d30-964">Включена поддержка Среды службы приложений: az appservice ase show | list | list-addresses | list-plans | create | update | delete.</span><span class="sxs-lookup"><span data-stu-id="82d30-964">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="82d30-965">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="82d30-965">Backup</span></span>

* <span data-ttu-id="82d30-966">Исправлена проблема в команде az backup policy list-associated-items.</span><span class="sxs-lookup"><span data-stu-id="82d30-966">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="82d30-967">Добавлен необязательный параметр BackupManagementType.</span><span class="sxs-lookup"><span data-stu-id="82d30-967">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="82d30-968">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="82d30-968">Compute</span></span>

* <span data-ttu-id="82d30-969">Обновлена версия API вычислений, дисков, моментальных снимков до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="82d30-969">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="82d30-970">vmss create. Улучшение для --orchestration-mode.</span><span class="sxs-lookup"><span data-stu-id="82d30-970">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="82d30-971">sig image-definition create. Добавлен параметр --os-state для указания того, являются ли виртуальные машины, созданные в этом образе, универсальными или специализированными.</span><span class="sxs-lookup"><span data-stu-id="82d30-971">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="82d30-972">sig image-definition create. Добавлен параметр --hyper-v-generation для указания создания гипервизора.</span><span class="sxs-lookup"><span data-stu-id="82d30-972">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="82d30-973">sig image-version create. Включена поддержка параметров --os-snapshot и --data-snapshots.</span><span class="sxs-lookup"><span data-stu-id="82d30-973">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="82d30-974">image create. Включена поддержка параметра --data-disk-caching для указания параметра кэширования для дисков данных.</span><span class="sxs-lookup"><span data-stu-id="82d30-974">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="82d30-975">Обновлена версия пакета SDK для вычислений Python до 10.0.0.</span><span class="sxs-lookup"><span data-stu-id="82d30-975">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="82d30-976">vm/vmss create. Добавлен фрагмент Spot в свойство перечисления Priority.</span><span class="sxs-lookup"><span data-stu-id="82d30-976">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="82d30-977">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименование параметра --max-billing в --max-price для виртуальных машин и Масштабируемых наборов виртуальных машин в соответствии с командлетами Swagger и PowerShell.</span><span class="sxs-lookup"><span data-stu-id="82d30-977">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="82d30-978">vm monitor log show. Включена поддержка запроса журналов в связанной рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="82d30-978">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-979">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-979">IOT</span></span>

* <span data-ttu-id="82d30-980">Исправление № 2531. Добавлены вспомогательные аргументы для обновления концентратора.</span><span class="sxs-lookup"><span data-stu-id="82d30-980">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="82d30-981">Исправление № 8323. Добавлены недостающие параметры для создания пользовательской конечной точки хранилища.</span><span class="sxs-lookup"><span data-stu-id="82d30-981">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="82d30-982">Исправлена ошибка регрессии. Отменены изменения, переопределяющие конечную точку хранилища по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-982">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="82d30-983">Key Vault</span><span class="sxs-lookup"><span data-stu-id="82d30-983">Key Vault</span></span>

* <span data-ttu-id="82d30-984">Исправление № 11121. При использовании `az keyvault certificate list` для передачи `--include-pending` теперь не требуется значение `true` или `false`.</span><span class="sxs-lookup"><span data-stu-id="82d30-984">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="82d30-985">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="82d30-985">NetAppFiles</span></span>

* <span data-ttu-id="82d30-986">Обновлена версия azure-mgmt-netapp до 0.7.0, которая включает некоторые дополнительные свойства тома, связанные с предстоящими операциями репликации.</span><span class="sxs-lookup"><span data-stu-id="82d30-986">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="82d30-987">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-987">Network</span></span>

* <span data-ttu-id="82d30-988">application-gateway waf-config. Не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="82d30-988">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="82d30-989">application-gateway waf-policy. Добавлены управляемые правила подгрупп для контроля управляемых наборов правил и правил исключения.</span><span class="sxs-lookup"><span data-stu-id="82d30-989">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="82d30-990">application-gateway waf-policy. Добавлен параметр политики подгруппы для управления глобальной конфигурацией политики WAF.</span><span class="sxs-lookup"><span data-stu-id="82d30-990">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="82d30-991">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] application-gateway waf-policy. Переименовано правило подгруппы в пользовательское правило.</span><span class="sxs-lookup"><span data-stu-id="82d30-991">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="82d30-992">application-gateway http-listener. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="82d30-992">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="82d30-993">application-gateway url-path-map rule. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="82d30-993">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="82d30-994">Упаковка</span><span class="sxs-lookup"><span data-stu-id="82d30-994">Packaging</span></span>

* <span data-ttu-id="82d30-995">Удалена команда az wrapper в Python.</span><span class="sxs-lookup"><span data-stu-id="82d30-995">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="82d30-996">Включена поддержка Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="82d30-996">Added support for Python 3.8</span></span>
* <span data-ttu-id="82d30-997">Изменена версия на Python 3 для пакета RPM.</span><span class="sxs-lookup"><span data-stu-id="82d30-997">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-998">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-998">Profile</span></span>

* <span data-ttu-id="82d30-999">Исправлена ошибка при выполнении `az login -u {} -p {}` с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="82d30-999">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="82d30-1000">Исправлена ошибка с `SSLError` при выполнении `az login` за прокси-сервером с самозаверяющим корневым сертификатом.</span><span class="sxs-lookup"><span data-stu-id="82d30-1000">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="82d30-1001">Исправлена ошибка № 10578. `az login` зависает при одновременном запуске нескольких экземпляров в Windows или WSL.</span><span class="sxs-lookup"><span data-stu-id="82d30-1001">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="82d30-1002">Исправлена ошибка № 11059. Сбой выполнения `az login --allow-no-subscriptions`, если в клиенте есть подписки.</span><span class="sxs-lookup"><span data-stu-id="82d30-1002">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="82d30-1003">Исправлена ошибка № 11238. После переименования подписки вход с помощью MSI приведет к тому, что одна и та же подписка появится дважды.</span><span class="sxs-lookup"><span data-stu-id="82d30-1003">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="82d30-1004">RBAC</span><span class="sxs-lookup"><span data-stu-id="82d30-1004">RBAC</span></span>

* <span data-ttu-id="82d30-1005">Исправлена ошибка № 10996. Исправлена ошибка с `--force-change-password-next-login` в `az ad user update`, если `--password` не указывается.</span><span class="sxs-lookup"><span data-stu-id="82d30-1005">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="82d30-1006">Redis</span><span class="sxs-lookup"><span data-stu-id="82d30-1006">Redis</span></span>

* <span data-ttu-id="82d30-1007">Исправлена ошибка № 2902. Предотвращена настройка конфигураций памяти при обновлении кэша с номером SKU "Базовый".</span><span class="sxs-lookup"><span data-stu-id="82d30-1007">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="82d30-1008">Резервирование</span><span class="sxs-lookup"><span data-stu-id="82d30-1008">Reservations</span></span>

* <span data-ttu-id="82d30-1009">Обновлена версия пакета SDK до 0.6.0</span><span class="sxs-lookup"><span data-stu-id="82d30-1009">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="82d30-1010">Добавлены сведения о плане выставления счетов после вызова Get-Catalogs.</span><span class="sxs-lookup"><span data-stu-id="82d30-1010">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="82d30-1011">Добавлена новая команда `az reservations reservation-order calculate` для вычисления стоимости резервирования.</span><span class="sxs-lookup"><span data-stu-id="82d30-1011">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="82d30-1012">Добавлена новая команда `az reservations reservation-order purchase` для приобретения нового резервирования.</span><span class="sxs-lookup"><span data-stu-id="82d30-1012">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="82d30-1013">Rest</span><span class="sxs-lookup"><span data-stu-id="82d30-1013">Rest</span></span>
* <span data-ttu-id="82d30-1014">Изменена версия `az rest` на общедоступную.</span><span class="sxs-lookup"><span data-stu-id="82d30-1014">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-1015">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-1015">SQL</span></span>

* <span data-ttu-id="82d30-1016">Обновлена версия azure-mgmt-sql до 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="82d30-1016">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-1017">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-1017">Storage</span></span>

* <span data-ttu-id="82d30-1018">storage account create. Добавлен параметр --enable-hierarchical-namespace для включения поддержки семантики файловой системы в службе больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1018">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="82d30-1019">Удалено несвязанное исключение из сообщения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="82d30-1019">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="82d30-1020">Исправлены проблемы, из-за которых появлялось неверное сообщение об отсутствии нужных разрешений на выполнение требуемой операции</span><span class="sxs-lookup"><span data-stu-id="82d30-1020">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="82d30-1021">при блокировке правилами сети (AuthenticationFailed).</span><span class="sxs-lookup"><span data-stu-id="82d30-1021">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="82d30-1022">4 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1022">November 4, 2019</span></span>

<span data-ttu-id="82d30-1023">Версия 2.0.76</span><span class="sxs-lookup"><span data-stu-id="82d30-1023">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-1024">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-1024">ACR</span></span>

* <span data-ttu-id="82d30-1025">В команду `az acr pack build` добавлен параметр предварительной версии `--pack-image-tag`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1025">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="82d30-1026">Добавлена поддержка включения аудита при создании реестра.</span><span class="sxs-lookup"><span data-stu-id="82d30-1026">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="82d30-1027">Включена поддержка функции RBAC, распространяющаяся на репозиторий.</span><span class="sxs-lookup"><span data-stu-id="82d30-1027">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="82d30-1028">AKS</span><span class="sxs-lookup"><span data-stu-id="82d30-1028">AKS</span></span>

* <span data-ttu-id="82d30-1029">В команду `az aks create` добавлены `--enable-cluster-autoscaler`, `--min-count` и `--max-count`, что позволяет автоматически масштабировать кластер для пула узлов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1029">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="82d30-1030">Добавлены указанные выше флаги, а также `--update-cluster-autoscaler` и `--disable-cluster-autoscaler` в команду `az aks update`, что позволяет обновлять средство автоматического масштабирования кластера.</span><span class="sxs-lookup"><span data-stu-id="82d30-1030">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="82d30-1031">AppConfig</span><span class="sxs-lookup"><span data-stu-id="82d30-1031">AppConfig</span></span>

* <span data-ttu-id="82d30-1032">Добавлена группа команд функции appconfig для управления флагами функций, хранимыми в Конфигурации приложений.</span><span class="sxs-lookup"><span data-stu-id="82d30-1032">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="82d30-1033">Исправлена незначительная ошибка команды экспорта в файл appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="82d30-1033">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="82d30-1034">Прерывание чтения содержимого конечного файла во время экспорта.</span><span class="sxs-lookup"><span data-stu-id="82d30-1034">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-1035">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-1035">AppService</span></span>

* <span data-ttu-id="82d30-1036">`az appservice plan create`: Добавлена поддержка определения persitescaling при создании плана appservice.</span><span class="sxs-lookup"><span data-stu-id="82d30-1036">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="82d30-1037">Исправлена проблема, из-за которой операция webapp config ssl bind удаляла существующие теги из ресурса.</span><span class="sxs-lookup"><span data-stu-id="82d30-1037">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="82d30-1038">Добавлен флаг `--build-remote` для `az functionapp deployment source config-zip` для включения поддержки действия удаленной сборки во время развертывания приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="82d30-1038">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="82d30-1039">Изменена версия узла по умолчанию для приложений-функций на ~10 для Windows</span><span class="sxs-lookup"><span data-stu-id="82d30-1039">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="82d30-1040">В `az functionapp create` добавлено свойство `--runtime-version`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1040">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="82d30-1041">ARM</span><span class="sxs-lookup"><span data-stu-id="82d30-1041">ARM</span></span>

* <span data-ttu-id="82d30-1042">`az deployment/group deployment validate`: В `--handle-extended-json-format` добавлен параметр для включения поддержки многострочности и комментариев в шаблоне JSON при развертывании.</span><span class="sxs-lookup"><span data-stu-id="82d30-1042">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="82d30-1043">Версия azure-mgmt-resource обновлена до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="82d30-1043">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="82d30-1044">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="82d30-1044">Backup</span></span>

* <span data-ttu-id="82d30-1045">Добавлена поддержка резервного копирования AzureFiles.</span><span class="sxs-lookup"><span data-stu-id="82d30-1045">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="82d30-1046">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="82d30-1046">Compute</span></span>

* <span data-ttu-id="82d30-1047">`az vm create`: Добавлено предупреждение при одновременном определении ускоренной сети и существующей сетевой карты.</span><span class="sxs-lookup"><span data-stu-id="82d30-1047">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="82d30-1048">`az vm create`: Добавлен параметр `--vmss` для определения существующего масштабируемого набора виртуальных машин, которому должна быть назначена виртуальная машина.</span><span class="sxs-lookup"><span data-stu-id="82d30-1048">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="82d30-1049">`az vm/vmss create`: Добавлена локальная копия файла псевдонима изображения, к которой можно получить доступ в ограниченной сетевой среде.</span><span class="sxs-lookup"><span data-stu-id="82d30-1049">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="82d30-1050">`az vmss create`: Добавлен параметр `--orchestration-mode` для определения того, как виртуальные машины управляются масштабируемым набором.</span><span class="sxs-lookup"><span data-stu-id="82d30-1050">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="82d30-1051">`az vm/vmss update`: Добавлен параметр `--ultra-ssd-enabled`, чтобы разрешить обновление параметра Ultra SSD.</span><span class="sxs-lookup"><span data-stu-id="82d30-1051">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="82d30-1052">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az vm extension set`: Исправлена ошибка, из-за которой пользователям не удавалось определять расширение на виртуальной машине с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1052">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="82d30-1053">Добавлены новые команды `az vm image terms accept/cancel/show` для управления условиями использования образов Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="82d30-1053">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="82d30-1054">Расширение VMAccessForLinux обновлено до версии 1.5.</span><span class="sxs-lookup"><span data-stu-id="82d30-1054">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82d30-1055">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-1055">CosmosDB</span></span>

* <span data-ttu-id="82d30-1056">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql container create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="82d30-1056">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="82d30-1057">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az gremlin graph create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="82d30-1057">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="82d30-1058">`az sql container create`: Добавлены команды `--unique-key-policy` и `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1058">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="82d30-1059">`az sql container create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-1059">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="82d30-1060">`gremlin graph create`: Добавлена команда `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1060">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="82d30-1061">`gremlin graph create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-1061">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="82d30-1062">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="82d30-1062">Fixed typo in help message</span></span>
* <span data-ttu-id="82d30-1063">База данных: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="82d30-1063">database: Added deprecation information</span></span>
* <span data-ttu-id="82d30-1064">Коллекция: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="82d30-1064">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-1065">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-1065">IoT</span></span>

* <span data-ttu-id="82d30-1066">Добавлен новый тип источника маршрутизации: DigitalTwinChangeEvents.</span><span class="sxs-lookup"><span data-stu-id="82d30-1066">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="82d30-1067">Добавлены отсутствующие компоненты в `az iot hub create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1067">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="82d30-1068">Key Vault</span><span class="sxs-lookup"><span data-stu-id="82d30-1068">Key Vault</span></span>

* <span data-ttu-id="82d30-1069">Исправлена непредвиденная ошибка с отсутствием файла сертификата.</span><span class="sxs-lookup"><span data-stu-id="82d30-1069">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="82d30-1070">Исправлена ошибка с неработающей командой `az keyvault recover/purge`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1070">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="82d30-1071">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="82d30-1071">NetAppFiles</span></span>

* <span data-ttu-id="82d30-1072">Пакет azure-mgmt-netapp обновлен до версии 0.6.0 для включения поддержки API версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="82d30-1072">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="82d30-1073">Эта новая версия API включает:</span><span class="sxs-lookup"><span data-stu-id="82d30-1073">This new API version includes:</span></span>

    - <span data-ttu-id="82d30-1074">При создании тома с использованием `--protocol-types` допускается NFSv4.1 вместо NFSv4.</span><span class="sxs-lookup"><span data-stu-id="82d30-1074">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="82d30-1075">Свойство политики экспорта томов теперь называется nfsv41, а не nfsv4.</span><span class="sxs-lookup"><span data-stu-id="82d30-1075">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="82d30-1076">Параметр `--creation-token` для тома переименован в `--file-path`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1076">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="82d30-1077">Дата создания моментального снимка теперь имеет значение Created.</span><span class="sxs-lookup"><span data-stu-id="82d30-1077">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="82d30-1078">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-1078">Network</span></span>

* <span data-ttu-id="82d30-1079">`az network private-dns link vnet create/update`: Добавлена поддержка связывания виртуальных сетей между клиентами.</span><span class="sxs-lookup"><span data-stu-id="82d30-1079">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="82d30-1080">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az network vnet subnet list`: Параметры `--resource-group` и `--vnet-name` теперь являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="82d30-1080">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="82d30-1081">`az network public-ip prefix create`: Включена поддержка определения версии IP-адреса (IPv4, IPv6) при создании.</span><span class="sxs-lookup"><span data-stu-id="82d30-1081">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="82d30-1082">Версия azure-mgmt-network обновлена до 7.0.0 и версия api-version до 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="82d30-1082">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="82d30-1083">`az network vrouter`: Включена поддержка нового виртуального маршрутизатора службы и пиринга виртуальных маршрутизаторов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1083">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="82d30-1084">`az network express-route gateway connection`: Добавлена поддержка параметра `--internet-security`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1084">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-1085">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-1085">Profile</span></span>

* <span data-ttu-id="82d30-1086">Исправлена ошибка с неработающей командой `az account get-access-token --resource-type ms-graph`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1086">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="82d30-1087">Удалено предупреждение из `az login`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1087">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="82d30-1088">RBAC</span><span class="sxs-lookup"><span data-stu-id="82d30-1088">RBAC</span></span>

* <span data-ttu-id="82d30-1089">Исправление `az ad app update --id {} --display-name {}` не работает.</span><span class="sxs-lookup"><span data-stu-id="82d30-1089">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="82d30-1090">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="82d30-1090">ServiceFabric</span></span>

* <span data-ttu-id="82d30-1091">`az sf cluster create`: Исправлена проблема путем изменения VMSS для вычислений с использованием файла template.json для Service Fabric Linux и Windows со стандартных дисков на управляемые.</span><span class="sxs-lookup"><span data-stu-id="82d30-1091">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-1092">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-1092">SQL</span></span>

* <span data-ttu-id="82d30-1093">Добавлены параметры `--compute-model`, `--auto-pause-delay` и `--min-capacity` для включения поддержки операций CRUD для нового предложения Базы данных SQL: Модель бессерверных вычислений.</span><span class="sxs-lookup"><span data-stu-id="82d30-1093">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-1094">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-1094">Storage</span></span>

* <span data-ttu-id="82d30-1095">`az storage account create/update`: Добавлен параметр --enable-files-adds и группа аргументов свойств Azure Active Directory для включения поддержки аутентификации доменных служб Azure Active Directory для Файлов Azure.</span><span class="sxs-lookup"><span data-stu-id="82d30-1095">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="82d30-1096">Расширена команда `az storage account keys list/renew` для включения поддержки перечисления или повторного создания ключей Kerberos для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="82d30-1096">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="82d30-1097">15 октября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1097">October 15, 2019</span></span>

<span data-ttu-id="82d30-1098">Версия 2.0.75</span><span class="sxs-lookup"><span data-stu-id="82d30-1098">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="82d30-1099">AKS</span><span class="sxs-lookup"><span data-stu-id="82d30-1099">AKS</span></span>

* <span data-ttu-id="82d30-1100">Для параметра `--load-balancer-sku` изменено значение по умолчанию на `standard`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="82d30-1100">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="82d30-1101">Для параметра `--vm-set-type` изменено значение по умолчанию на `virtualmachinescalesets`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="82d30-1101">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="82d30-1102">AMS</span><span class="sxs-lookup"><span data-stu-id="82d30-1102">AMS</span></span>

* <span data-ttu-id="82d30-1103">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя `job start` изменено на `job create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1103">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="82d30-1104">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В параметре `--ask` команды `content-key-policy create` вместо кодировки UTF8 теперь используется шестнадцатеричная строка из 32 символов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1104">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-1105">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-1105">AppService</span></span>

* <span data-ttu-id="82d30-1106">Добавлены команды `webapp config access-restriction show|set|add|remove`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1106">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="82d30-1107">Улучшена обработка ошибок в `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1107">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="82d30-1108">Для `appservice plan update` добавлена поддержка номера SKU `Isolated`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1108">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="82d30-1109">ARM</span><span class="sxs-lookup"><span data-stu-id="82d30-1109">ARM</span></span>

* <span data-ttu-id="82d30-1110">В `deployment create` добавлен параметр `--handle-extended-json-format` для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="82d30-1110">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="82d30-1111">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="82d30-1111">Compute</span></span>

* <span data-ttu-id="82d30-1112">Добавлен параметр `--enable-agent` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1112">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="82d30-1113">Внесены изменения в `vm create`, позволяющие автоматически использовать номер SKU "Стандартный" для общедоступных IP-адресов при использовании зон.</span><span class="sxs-lookup"><span data-stu-id="82d30-1113">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="82d30-1114">Внесены изменения в `vm create`, позволяющие автоматически создавать допустимое имя для виртуальной машины, если оно не задано.</span><span class="sxs-lookup"><span data-stu-id="82d30-1114">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="82d30-1115">В `vmss create` добавлен параметр `--computer-name-prefix` для поддержки пользовательского префикса имени для виртуальных машин в VMSS.</span><span class="sxs-lookup"><span data-stu-id="82d30-1115">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="82d30-1116">В `vm create` добавлен параметр `--workspace` для автоматического включения рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="82d30-1116">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="82d30-1117">API коллекций обновлен до версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="82d30-1117">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="82d30-1118">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-1118">Core</span></span>

* <span data-ttu-id="82d30-1119">Добавлена проверка синтаксиса для параметра `--set` в универсальной команде обновления.</span><span class="sxs-lookup"><span data-stu-id="82d30-1119">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-1120">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-1120">IoT</span></span>

* <span data-ttu-id="82d30-1121">Исправлена проблема, при которой `iot hub show` неправильно выдавал ошибку "Ресурс не найден".</span><span class="sxs-lookup"><span data-stu-id="82d30-1121">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-1122">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-1122">Monitor</span></span>

* <span data-ttu-id="82d30-1123">В `monitor log-analytics workspace` добавлена поддержка CRUD.</span><span class="sxs-lookup"><span data-stu-id="82d30-1123">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="82d30-1124">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-1124">Network</span></span>

* <span data-ttu-id="82d30-1125">В `network private-dns link vnet [create|update]` добавлена поддержка виртуального канала для клиентов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1125">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="82d30-1126">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для `network vnet subnet list` теперь требуются параметры `--resource-group` и `--vnet-name`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1126">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-1127">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-1127">SQL</span></span>

* <span data-ttu-id="82d30-1128">В `sql mi ad-admin` добавлены команды, которые поддерживают назначение администратора AAD в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="82d30-1128">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-1129">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-1129">Storage</span></span>

* <span data-ttu-id="82d30-1130">В `storage copy` добавлен параметр `--preserve-s2s-access-tier`, позволяющий сохранить уровень доступа во время копирования между службами.</span><span class="sxs-lookup"><span data-stu-id="82d30-1130">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="82d30-1131">В `storage account [create|update]` добавлен параметр `--enable-large-file-share` для поддержки общих папок большого размера в учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="82d30-1131">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="82d30-1132">24 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1132">September 24, 2019</span></span>

<span data-ttu-id="82d30-1133">Версия 2.0.74</span><span class="sxs-lookup"><span data-stu-id="82d30-1133">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-1134">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-1134">ACR</span></span>

* <span data-ttu-id="82d30-1135">В `acr config retention update` добавлен обязательный параметр `--type`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1135">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="82d30-1136">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованный параметр `--name -n` изменен на `--registry -r ` для группы команд `acr config`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1136">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="82d30-1137">AKS</span><span class="sxs-lookup"><span data-stu-id="82d30-1137">AKS</span></span>

* <span data-ttu-id="82d30-1138">В команду `aks create` добавлен параметр `--load-balancer-sku`, позволяющий создать кластер AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="82d30-1138">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="82d30-1139">В команды `aks [create|update]` добавлены параметры `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` и `--load-balancer-outbound-ip-prefixes`, позволяющие обновлять профиль подсистемы балансировки нагрузки у кластера AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="82d30-1139">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="82d30-1140">В команду `aks create` добавлен параметр `--vm-set-type`, позволяющий указывать типы виртуальных машин в кластере AKS.</span><span class="sxs-lookup"><span data-stu-id="82d30-1140">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="82d30-1141">ARM</span><span class="sxs-lookup"><span data-stu-id="82d30-1141">ARM</span></span>

* <span data-ttu-id="82d30-1142">В команду `group deployment create` добавлен параметр `--handle-extended-json-format`, для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="82d30-1142">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="82d30-1143">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="82d30-1143">Compute</span></span>

* <span data-ttu-id="82d30-1144">В команды `vmss [create|update]` добавлен параметр `--terminate-notification-time`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="82d30-1144">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="82d30-1145">В команду `vmss update` добавлен параметр `--enable-terminate-notification`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="82d30-1145">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="82d30-1146">В команды `[vm|vmss] create` добавлены параметры `--priority,`, `--eviction-policy,` и `--max-billing`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1146">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="82d30-1147">Изменена команда `disk create`, которая теперь позволяет указать точный размер отправки на диск.</span><span class="sxs-lookup"><span data-stu-id="82d30-1147">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="82d30-1148">В `snapshot create` добавлена поддержка добавочных моментальных снимков для управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="82d30-1148">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="82d30-1149">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-1149">Cosmos DB</span></span>

* <span data-ttu-id="82d30-1150">В команду `cosmosdb keys list` добавлен параметр `--type <key-type>` для отображения ключей, ключей только для чтения или строк подключения.</span><span class="sxs-lookup"><span data-stu-id="82d30-1150">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="82d30-1151">Добавлена команда `cosmosdb keys regenerate`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1151">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="82d30-1152">[УСТАРЕЛО] Команды `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` и `cosmosdb list-read-only-keys` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="82d30-1152">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="82d30-1153">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="82d30-1153">EventGrid</span></span>

* <span data-ttu-id="82d30-1154">Исправлен текст справки по конечной точке — дана ссылка на правильный параметр.</span><span class="sxs-lookup"><span data-stu-id="82d30-1154">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="82d30-1155">Key Vault</span><span class="sxs-lookup"><span data-stu-id="82d30-1155">Key Vault</span></span>

* <span data-ttu-id="82d30-1156">Исправлена проблема, из-за которой вход с помощью клиента (`login -t`) мог приводить к сбою `keyvault create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1156">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-1157">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-1157">Monitor</span></span>

* <span data-ttu-id="82d30-1158">Исправлена проблема с тем, что символ `:` являлся недопустимым в аргументе `--condition` для `monitor metrics alert create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1158">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="82d30-1159">Политика</span><span class="sxs-lookup"><span data-stu-id="82d30-1159">Policy</span></span>

* <span data-ttu-id="82d30-1160">Добавлена поддержка API Политики версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="82d30-1160">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="82d30-1161">В команду `policy assignment create` добавлен параметр `--enforcement-mode`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1161">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-1162">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-1162">Storage</span></span>

* <span data-ttu-id="82d30-1163">В команду `az storage copy` добавлен параметр `--blob-type`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1163">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="82d30-1164">10 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1164">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-1165">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-1165">ACR</span></span>

* <span data-ttu-id="82d30-1166">Добавлена группа команд `acr config retention` для настройки политики хранения.</span><span class="sxs-lookup"><span data-stu-id="82d30-1166">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="82d30-1167">AKS</span><span class="sxs-lookup"><span data-stu-id="82d30-1167">AKS</span></span>

* <span data-ttu-id="82d30-1168">Добавлена возможность интеграции ACR с помощью следующих команд:</span><span class="sxs-lookup"><span data-stu-id="82d30-1168">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="82d30-1169">В `aks [create|update]` добавлен параметр `--attach-acr` для подключения ACR к кластеру AKS.</span><span class="sxs-lookup"><span data-stu-id="82d30-1169">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="82d30-1170">В `aks update` добавлен параметр `--detach-acr` для отключения ACR от кластера AKS.</span><span class="sxs-lookup"><span data-stu-id="82d30-1170">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="82d30-1171">ARM</span><span class="sxs-lookup"><span data-stu-id="82d30-1171">ARM</span></span>

* <span data-ttu-id="82d30-1172">Добавлена возможность использования API версии 2019-05-10.</span><span class="sxs-lookup"><span data-stu-id="82d30-1172">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="82d30-1173">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-1173">Batch</span></span>

* <span data-ttu-id="82d30-1174">Добавлены новые параметры конфигурации JSON в `--json-file` для `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="82d30-1174">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="82d30-1175">Добавлен параметр `MountConfigurations` для подключений файловой системы (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="82d30-1175">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="82d30-1176">Добавлено необязательное свойство `publicIPs` в `NetworkConfiguration` для общедоступных IP-адресов в пулах (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="82d30-1176">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="82d30-1177">В `--image` добавлена поддержка коллекций общих образов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1177">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="82d30-1178">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `--start-task-wait-for-success` в `batch pool create` изменено на `true`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1178">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="82d30-1179">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `Scope` в `AutoUserSpecification` задано как Pool (ранее `Task` на узлах Windows и `Pool` на узлах Linux).</span><span class="sxs-lookup"><span data-stu-id="82d30-1179">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="82d30-1180">Этот аргумент можно задать только в конфигурации JSON с помощью `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1180">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82d30-1181">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82d30-1181">HDInsight</span></span>

* <span data-ttu-id="82d30-1182">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="82d30-1182">GA release</span></span>
* <span data-ttu-id="82d30-1183">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--workernode-count/-c` в `az hdinsight resize` теперь является обязательным.</span><span class="sxs-lookup"><span data-stu-id="82d30-1183">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="82d30-1184">Key Vault</span><span class="sxs-lookup"><span data-stu-id="82d30-1184">Key Vault</span></span>

* <span data-ttu-id="82d30-1185">Исправлена проблема, когда подсети не удавалось удалить из сетевых правил.</span><span class="sxs-lookup"><span data-stu-id="82d30-1185">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="82d30-1186">Исправлена проблема, когда дублированные подсети и IP-адреса могли быть добавлены к сетевым правилам.</span><span class="sxs-lookup"><span data-stu-id="82d30-1186">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="82d30-1187">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-1187">Network</span></span>

* <span data-ttu-id="82d30-1188">Добавлен параметр `--interval` в `network watcher flow-log` для выбора значения интервала анализа трафика.</span><span class="sxs-lookup"><span data-stu-id="82d30-1188">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="82d30-1189">Добавлена команда `network application-gateway identity` для управления удостоверением шлюза.</span><span class="sxs-lookup"><span data-stu-id="82d30-1189">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="82d30-1190">Добавлена возможность указать идентификатор Key Vault в команде `network application-gateway ssl-cert`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1190">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="82d30-1191">Добавлена команда `network express-route peering peer-connection [show|list]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1191">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="82d30-1192">Политика</span><span class="sxs-lookup"><span data-stu-id="82d30-1192">Policy</span></span>

* <span data-ttu-id="82d30-1193">Добавлена возможность использования API версии 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="82d30-1193">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="82d30-1194">27 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1194">August 27, 2019</span></span>

<span data-ttu-id="82d30-1195">Версия 2.0.72</span><span class="sxs-lookup"><span data-stu-id="82d30-1195">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-1196">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-1196">ACR</span></span>

* <span data-ttu-id="82d30-1197">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка SKU `classic`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1197">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="82d30-1198">Управление API</span><span class="sxs-lookup"><span data-stu-id="82d30-1198">API Management</span></span>

* <span data-ttu-id="82d30-1199">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена группа команд `apim`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1199">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-1200">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-1200">AppService</span></span>

* <span data-ttu-id="82d30-1201">Исправлена проблема с командой `webapp webjob continuous start` при указании слота.</span><span class="sxs-lookup"><span data-stu-id="82d30-1201">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="82d30-1202">Изменена команда `webapp up` для обнаружения и удаления папки `env` из файла, используемого для развертывания.</span><span class="sxs-lookup"><span data-stu-id="82d30-1202">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="82d30-1203">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="82d30-1203">Keyvault</span></span>

* <span data-ttu-id="82d30-1204">Исправлена ошибка в команде `keyvault secret set`, которая игнорировала аргумент `--expires`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1204">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="82d30-1205">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-1205">Network</span></span>

* <span data-ttu-id="82d30-1206">Добавлена поддержка IPv6-адресов для аргументов `--private-ip-address-version`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1206">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="82d30-1207">Добавлены новые команды `network private-endpoint [create|update|list-types]` для управления закрытыми конечными точками.</span><span class="sxs-lookup"><span data-stu-id="82d30-1207">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="82d30-1208">Добавлена группа команд для `network private-link-service`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1208">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="82d30-1209">Добавлены аргументы `--private-endpoint-network-policies` и `--private-link-service-network-policies` для команды `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="82d30-1209">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="82d30-1210">RBAC</span><span class="sxs-lookup"><span data-stu-id="82d30-1210">RBAC</span></span>

* <span data-ttu-id="82d30-1211">Исправлена проблема с `ad app update --homepage`, когда домашнюю страницу нельзя было обновить.</span><span class="sxs-lookup"><span data-stu-id="82d30-1211">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="82d30-1212">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="82d30-1212">ServiceFabric</span></span>

* <span data-ttu-id="82d30-1213">Добавлена поддержка имен Key Vault в смешанном регистре.</span><span class="sxs-lookup"><span data-stu-id="82d30-1213">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="82d30-1214">Исправлена проблема с использованием сертификатов в Key Vault.</span><span class="sxs-lookup"><span data-stu-id="82d30-1214">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="82d30-1215">Исправлена проблема с использованием файлов сертификатов PFX.</span><span class="sxs-lookup"><span data-stu-id="82d30-1215">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="82d30-1216">Исправлена проблема с `sf cluster certificate add`, когда группа ресурсов Key Vault не была указана.</span><span class="sxs-lookup"><span data-stu-id="82d30-1216">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="82d30-1217">Исправлена проблема с неработающей командой `sf cluster set`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1217">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="82d30-1218">SignalR</span><span class="sxs-lookup"><span data-stu-id="82d30-1218">SignalR</span></span>

* <span data-ttu-id="82d30-1219">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="82d30-1219">Added new commands:</span></span>
  * <span data-ttu-id="82d30-1220">`signalr cors`: Управление CORS SignalR</span><span class="sxs-lookup"><span data-stu-id="82d30-1220">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="82d30-1221">`signalr restart`: Перезапуск службы SignalR</span><span class="sxs-lookup"><span data-stu-id="82d30-1221">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="82d30-1222">`signalr update`: Обновление службы SignalR</span><span class="sxs-lookup"><span data-stu-id="82d30-1222">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="82d30-1223">Добавлен аргумент `--service-mode` для команды `signalr create`</span><span class="sxs-lookup"><span data-stu-id="82d30-1223">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-1224">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-1224">Storage</span></span>

* <span data-ttu-id="82d30-1225">Добавлена команда `storage account revoke-delegation-keys`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1225">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="82d30-1226">13 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1226">August 13, 2019</span></span>

<span data-ttu-id="82d30-1227">Версия 2.0.71</span><span class="sxs-lookup"><span data-stu-id="82d30-1227">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-1228">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-1228">AppService</span></span>

* <span data-ttu-id="82d30-1229">Исправлена проблема, из-за которой выполнение команд `webapp webjob continuous` для слотов завершалось сбоем.</span><span class="sxs-lookup"><span data-stu-id="82d30-1229">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="82d30-1230">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="82d30-1230">BotService</span></span>

* <span data-ttu-id="82d30-1231">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка создания ботов на основе пакета SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="82d30-1231">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="82d30-1232">Cognitive Services:</span><span class="sxs-lookup"><span data-stu-id="82d30-1232">CognitiveServices</span></span>

* <span data-ttu-id="82d30-1233">Добавлены команды `cognitiveservices account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1233">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="82d30-1234">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-1234">Cosmos DB</span></span>

* <span data-ttu-id="82d30-1235">Удалено предупреждение при обновлении нескольких расположений для записи.</span><span class="sxs-lookup"><span data-stu-id="82d30-1235">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="82d30-1236">Добавлены команды CRUD для ресурсов CosmosDB SQL, MongoDB, Cassandra, Gremlin и ресурсов таблиц, а также пропускной способности ресурсов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1236">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82d30-1237">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82d30-1237">HDInsight</span></span>

<span data-ttu-id="82d30-1238">Этот выпуск содержит большое число критических изменений.</span><span class="sxs-lookup"><span data-stu-id="82d30-1238">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="82d30-1239">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="82d30-1239">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="82d30-1240">Переименование `--storage-default-container` в `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="82d30-1240">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="82d30-1241">Переименование `--storage-default-filesystem` в `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="82d30-1241">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="82d30-1242">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--name` для `application create`, чтобы представлять имя приложения вместо имени кластера.</span><span class="sxs-lookup"><span data-stu-id="82d30-1242">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="82d30-1243">Добавлен аргумент `--cluster-name` для `application create`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1243">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="82d30-1244">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="82d30-1244">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="82d30-1245">Переименование `--application-type` в `--type`</span><span class="sxs-lookup"><span data-stu-id="82d30-1245">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="82d30-1246">Переименование `--marketplace-identifier` в `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="82d30-1246">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="82d30-1247">Переименование `--https-endpoint-access-mode` в `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="82d30-1247">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="82d30-1248">Переименован аргумент `--https-endpoint-destination-port` на `--destination-port`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1248">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="82d30-1249">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="82d30-1249">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="82d30-1250">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Переименован аргумент `--target-instance-count` на `--workernode-count` для `hdinsight resize`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1250">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="82d30-1251">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены все команды в группе `hdinsight script-action`, чтобы использовать параметр `--name` в качестве имени действия скрипта.</span><span class="sxs-lookup"><span data-stu-id="82d30-1251">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="82d30-1252">Добавлен аргумент `--cluster-name` для всех команд `hdinsight script-action`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1252">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="82d30-1253">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименован аргумент `--script-execution-id` на `--execution-id`для всех команд `hdinsight script-action`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1253">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="82d30-1254">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `hdinsight script-action show` переименована в `hdinsight script-action show-execution-details`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1254">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="82d30-1255">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Изменены параметры для `hdinsight script-action execute --roles`, чтобы они разделялись пробелами, а не запятыми.</span><span class="sxs-lookup"><span data-stu-id="82d30-1255">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="82d30-1256">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--persisted` для `hdinsight script-action list`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1256">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="82d30-1257">Изменен параметр `hdinsight create --cluster-configurations`, чтобы принимать путь к локальному файлу JSON или строке JSON.</span><span class="sxs-lookup"><span data-stu-id="82d30-1257">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="82d30-1258">Добавлена команда `hdinsight script-action list-execution-history`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1258">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="82d30-1259">Изменен параметр `hdinsight monitor enable --workspace`, чтобы принимать идентификатор или имя рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="82d30-1259">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="82d30-1260">Добавлен аргумент `hdinsight monitor enable --primary-key`, который требуется, если в качестве параметра указан идентификатор рабочей области.</span><span class="sxs-lookup"><span data-stu-id="82d30-1260">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="82d30-1261">Добавлены дополнительные примеры и обновленные описания для справочных сообщений.</span><span class="sxs-lookup"><span data-stu-id="82d30-1261">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="82d30-1262">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="82d30-1262">Interactive</span></span>

* <span data-ttu-id="82d30-1263">Исправлена ошибка загрузки.</span><span class="sxs-lookup"><span data-stu-id="82d30-1263">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="82d30-1264">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="82d30-1264">Kubernetes</span></span>

* <span data-ttu-id="82d30-1265">Теперь используется `https`, если порт контейнера панели мониторинга использует `https`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1265">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="82d30-1266">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-1266">Network</span></span>

* <span data-ttu-id="82d30-1267">Добавлен аргумент `--yes` для `network dns record-set cname delete`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1267">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-1268">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-1268">Profile</span></span>

* <span data-ttu-id="82d30-1269">Добавлен аргумент `--resource-type` для `account get-access-token`, чтобы получать маркеры доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="82d30-1269">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="82d30-1270">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="82d30-1270">ServiceFabric</span></span>

* <span data-ttu-id="82d30-1271">Добавлены все поддерживаемые версии ОС для команды sf cluster create.</span><span class="sxs-lookup"><span data-stu-id="82d30-1271">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="82d30-1272">Исправлена ошибка проверки основного сертификата.</span><span class="sxs-lookup"><span data-stu-id="82d30-1272">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-1273">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-1273">Storage</span></span>

* <span data-ttu-id="82d30-1274">Добавлена команда `storage copy`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1274">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="82d30-1275">30 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1275">July 30, 2019</span></span>

<span data-ttu-id="82d30-1276">Версия 2.0.70</span><span class="sxs-lookup"><span data-stu-id="82d30-1276">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-1277">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-1277">ACR</span></span>

* <span data-ttu-id="82d30-1278">Исправлена проблема № 9952 (регрессия в команде `acr pack build`).</span><span class="sxs-lookup"><span data-stu-id="82d30-1278">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="82d30-1279">Удалено имя образа построителя по умолчанию в `acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1279">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-1280">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-1280">Appservice</span></span>

* <span data-ttu-id="82d30-1281">Команда `webapp config ssl` изменена для отображения сообщения, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="82d30-1281">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="82d30-1282">Исправлена проблема, когда команда `functionapp create` не принимала тип учетной записи хранения `Standard_RAGRS`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1282">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="82d30-1283">Исправлена проблема, когда команда `webapp up` завершала работу со сбоем в случае выполнения со старой версией Python.</span><span class="sxs-lookup"><span data-stu-id="82d30-1283">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="82d30-1284">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-1284">Network</span></span>

* <span data-ttu-id="82d30-1285">Удален недопустимый параметр `--ids` из `network nic ip-config add` (исправление проблемы № 9861).</span><span class="sxs-lookup"><span data-stu-id="82d30-1285">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="82d30-1286">Исправлена проблема № 9604.</span><span class="sxs-lookup"><span data-stu-id="82d30-1286">Fixes #9604.</span></span> <span data-ttu-id="82d30-1287">Добавлен параметр `--root-certs` в `network application-gateway http-settings [create|update]` для поддержки связанных с пользователем доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1287">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="82d30-1288">Исправлен аргумент `--subscription` для `network dns record-set ns create` (проблема № 9965).</span><span class="sxs-lookup"><span data-stu-id="82d30-1288">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="82d30-1289">RBAC</span><span class="sxs-lookup"><span data-stu-id="82d30-1289">RBAC</span></span>

* <span data-ttu-id="82d30-1290">Добавлена команда `user update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1290">Added `user update` command</span></span>
* <span data-ttu-id="82d30-1291">[УСТАРЕЛО]`--upn-or-object-id` не рекомендуется использовать в связанных с пользователями командах.</span><span class="sxs-lookup"><span data-stu-id="82d30-1291">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="82d30-1292">Вместо этого применяйте аргумент `--id`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1292">Use replacement argument `--id`</span></span>
* <span data-ttu-id="82d30-1293">Добавлен аргумент `--id` в связанные с пользователями команды.</span><span class="sxs-lookup"><span data-stu-id="82d30-1293">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-1294">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-1294">SQL</span></span>

* <span data-ttu-id="82d30-1295">Добавлены команды управления для ключей и предохранителя TDE управляемого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="82d30-1295">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-1296">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-1296">Storage</span></span>

* <span data-ttu-id="82d30-1297">Добавлена команда `storage remove`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1297">Added `storage remove` command</span></span>
* <span data-ttu-id="82d30-1298">Исправлена проблема с `storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1298">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-1299">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-1299">VM</span></span>

* <span data-ttu-id="82d30-1300">Изменена команда `list-skus` для использования новой версии API для вывода сведений о зонах.</span><span class="sxs-lookup"><span data-stu-id="82d30-1300">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="82d30-1301">Изменено значение по умолчанию параметра `--single-placement-group` на `false` для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1301">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="82d30-1302">Добавлена возможность выбирать номера SKU хранилища ZRS для `[snapshot|disk] create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1302">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="82d30-1303">Добавлена новая группа команд `vm host` для поддержки выделенных узлов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1303">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="82d30-1304">Добавлены параметры `--host` и `--host-group` в команде `vm create` для указания выделенного узла виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="82d30-1304">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="82d30-1305">16 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1305">July 16, 2019</span></span>

<span data-ttu-id="82d30-1306">Версия 2.0.69</span><span class="sxs-lookup"><span data-stu-id="82d30-1306">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-1307">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-1307">Appservice</span></span>

* <span data-ttu-id="82d30-1308">Изменены команды `webapp identity`. Теперь они возвращают правильное сообщение об ошибке, если параметр ResourceGroupName или имя приложения недопустимы.</span><span class="sxs-lookup"><span data-stu-id="82d30-1308">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="82d30-1309">Исправлена команда `webapp list`. Теперь она возвращает правильное значение для параметра numberOfSites, если не указан параметр ResourceGroup.</span><span class="sxs-lookup"><span data-stu-id="82d30-1309">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="82d30-1310">Исправлены побочные эффекты для команд `appservice plan create` и `webapp create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1310">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="82d30-1311">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-1311">Core</span></span>

* <span data-ttu-id="82d30-1312">Исправлена ошибка, при которой отображался параметр `--subscription`, хотя он был неприменим.</span><span class="sxs-lookup"><span data-stu-id="82d30-1312">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="82d30-1313">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-1313">Batch</span></span>

* <span data-ttu-id="82d30-1314">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `batch pool node-agent-skus list` заменена на `batch pool supported-images list`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1314">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="82d30-1315">Добавлена поддержка правил безопасности, которые блокируют сетевой доступ к пулу на основе исходного порта трафика при использовании параметра `--json-file` команды `batch pool create network`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1315">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="82d30-1316">Добавлена поддержка выполнения задачи в рабочей папке контейнера или рабочей папке задачи пакета при использовании параметра `--json-file` команды `batch task create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1316">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="82d30-1317">Исправлена ошибка в параметре `--application-package-references` команды `batch pool create`, которая позволяла работать только со значениями по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-1317">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="82d30-1318">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="82d30-1318">Eventhubs</span></span>

* <span data-ttu-id="82d30-1319">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1319">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="82d30-1320">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="82d30-1320">RDBMS</span></span>

* <span data-ttu-id="82d30-1321">Добавлен необязательный параметр для указания номера SKU реплики в команде создания реплики.</span><span class="sxs-lookup"><span data-stu-id="82d30-1321">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="82d30-1322">Исправлена ошибка теста CI при создании реплики MySQL.</span><span class="sxs-lookup"><span data-stu-id="82d30-1322">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="82d30-1323">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="82d30-1323">Relay</span></span>

* <span data-ttu-id="82d30-1324">Исправлена проблема с гибридным подключением при выключенной авторизации клиента ([8775](https://github.com/azure/azure-cli/issues/8775)).</span><span class="sxs-lookup"><span data-stu-id="82d30-1324">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="82d30-1325">Добавлен параметр `--requires-transport-security` для команды `relay wcfrelay create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1325">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="82d30-1326">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="82d30-1326">Servicebus</span></span>

* <span data-ttu-id="82d30-1327">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1327">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-1328">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-1328">Storage</span></span>

* <span data-ttu-id="82d30-1329">Добавлена возможность обновления учетной записи хранения для AADDS в службе "Файлы".</span><span class="sxs-lookup"><span data-stu-id="82d30-1329">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="82d30-1330">Устранена проблема, описанная здесь: `storage blob service-properties update --set`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1330">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="82d30-1331">2 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1331">July 2, 2019</span></span>

<span data-ttu-id="82d30-1332">Версия 2.0.68</span><span class="sxs-lookup"><span data-stu-id="82d30-1332">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="82d30-1333">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-1333">Core</span></span>

* <span data-ttu-id="82d30-1334">Командные модули теперь объединены в один распространяемый пакет Python.</span><span class="sxs-lookup"><span data-stu-id="82d30-1334">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="82d30-1335">В результате этого прекращается непосредственное использование множества пакетов `azure-cli-` в PyPI.</span><span class="sxs-lookup"><span data-stu-id="82d30-1335">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="82d30-1336">Это также должно уменьшить размер установки и повлияет только на пользователей, которые выполняли установку непосредственно через `pip`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1336">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-1337">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-1337">ACR</span></span>

* <span data-ttu-id="82d30-1338">В заданиях добавлена поддержка триггеров таймера.</span><span class="sxs-lookup"><span data-stu-id="82d30-1338">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-1339">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-1339">Appservice</span></span>

* <span data-ttu-id="82d30-1340">Внесены изменения в `functionapp create` для включения Application Insights по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-1340">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="82d30-1341">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена устаревшая команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1341">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="82d30-1342">Вместо нее используйте новую команду `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1342">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="82d30-1343">В `functionapp deployment config-zip` добавлена поддержка плана потребления приложения-функции Linux.</span><span class="sxs-lookup"><span data-stu-id="82d30-1343">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="82d30-1344">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-1344">Cosmos DB</span></span>

* <span data-ttu-id="82d30-1345">Добавлена возможность отключения TTL.</span><span class="sxs-lookup"><span data-stu-id="82d30-1345">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="82d30-1346">DLS</span><span class="sxs-lookup"><span data-stu-id="82d30-1346">DLS</span></span>

* <span data-ttu-id="82d30-1347">Обновленная версия ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="82d30-1347">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="82d30-1348">Отзывы</span><span class="sxs-lookup"><span data-stu-id="82d30-1348">Feedback</span></span>

* <span data-ttu-id="82d30-1349">При сообщении о сбое при выполнении команды расширения `az feedback` теперь пытается открыть браузер по URL-адресу репозитория или проекта расширения из индекса.</span><span class="sxs-lookup"><span data-stu-id="82d30-1349">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82d30-1350">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82d30-1350">HDInsight</span></span>

* <span data-ttu-id="82d30-1351">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя группы команд `oms` изменилось на `monitor`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1351">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="82d30-1352">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--http-password/-p` стал обязательным.</span><span class="sxs-lookup"><span data-stu-id="82d30-1352">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="82d30-1353">Добавлены средства заполнения для `--cluster-admin-account` и средство заполнения для параметров `cluster-users-group-dns`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1353">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="82d30-1354">Параметр `cluster-users-group-dns` стал обязательным, если присутствует `—esp`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1354">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="82d30-1355">Добавлено время ожидания для всех существующих средств автоматического заполнения аргументов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1355">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="82d30-1356">Добавлено время ожидания для преобразования имени ресурса в идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="82d30-1356">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="82d30-1357">Внесены изменения в средства автоматического заполнения для выбора ресурсов из любой группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1357">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="82d30-1358">Это может быть группа ресурсов, отличная от той, которая указана с помощью `-g`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1358">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="82d30-1359">Добавлена поддержка параметров `--sub-domain-suffix` и `--disable_gateway_auth` в команде `hdinsight application create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1359">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="82d30-1360">Управляемые службы</span><span class="sxs-lookup"><span data-stu-id="82d30-1360">Managed Services</span></span>

* <span data-ttu-id="82d30-1361">Командный модуль управляемых служб выпущен в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="82d30-1361">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-1362">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-1362">Profile</span></span>
* <span data-ttu-id="82d30-1363">Аргумент `--subscription` подавляется для команды выхода.</span><span class="sxs-lookup"><span data-stu-id="82d30-1363">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="82d30-1364">RBAC</span><span class="sxs-lookup"><span data-stu-id="82d30-1364">RBAC</span></span>

* <span data-ttu-id="82d30-1365">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален аргумент `--password` для `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1365">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="82d30-1366">В команду `create` добавлен параметр `--assignee-principal-type` для устранения периодических сбоев из-за задержки репликации сервера AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="82d30-1366">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="82d30-1367">Исправлен сбой в `ad signed-in-user` при перечислении собственных объектов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1367">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="82d30-1368">Исправлена проблема, при которой `ad sp` не удавалось найти нужное приложение в субъекте-службе.</span><span class="sxs-lookup"><span data-stu-id="82d30-1368">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="82d30-1369">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="82d30-1369">RDBMS</span></span>

* <span data-ttu-id="82d30-1370">Добавлена поддержка репликации MariaDB.</span><span class="sxs-lookup"><span data-stu-id="82d30-1370">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-1371">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-1371">SQL</span></span>

* <span data-ttu-id="82d30-1372">Описаны допустимые значения для `sql db create --sample-name`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1372">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-1373">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-1373">Storage</span></span>

* <span data-ttu-id="82d30-1374">В `storage blob generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1374">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="82d30-1375">В `storage container generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1375">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="82d30-1376">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-1376">VM</span></span>

* <span data-ttu-id="82d30-1377">Исправлена ошибка, при которой команда `vmss create` возвращала сообщение об ошибке при выполнении с `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1377">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="82d30-1378">Прекращена проверка `vmss create --single-placement-group` на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="82d30-1378">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="82d30-1379">Команда не завершается сбоем, если для `--single-placement-group` задано значение `true`, а значение `--instance-count` больше 100 или указаны зоны доступности. Сама проверка теперь выполняется службой вычислений.</span><span class="sxs-lookup"><span data-stu-id="82d30-1379">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="82d30-1380">Исправлена ошибка, при которой команда `[vm|vmss] extension image list` завершалась сбоем при указании `--latest`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1380">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="82d30-1381">18 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1381">June 18, 2019</span></span>

<span data-ttu-id="82d30-1382">Версия 2.0.67</span><span class="sxs-lookup"><span data-stu-id="82d30-1382">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="82d30-1383">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-1383">Core</span></span>

<span data-ttu-id="82d30-1384">В этом выпуске добавлен новый тег [Предварительная версия], который яснее дает понять, что группа команд, команда или аргумент находятся в состоянии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="82d30-1384">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="82d30-1385">Ранее это указывалось в тексте справки или подразумевалось в номере версии командного модуля.</span><span class="sxs-lookup"><span data-stu-id="82d30-1385">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="82d30-1386">В будущем в интерфейсе командной строки номера версий отдельных пакетов не будут указываться.</span><span class="sxs-lookup"><span data-stu-id="82d30-1386">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="82d30-1387">Если команда доступна в предварительной версии, это также касается и всех ее аргументов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1387">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="82d30-1388">Если группа команд помечается как находящаяся в предварительной версии, значит все команды и аргументы также считаются доступными в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="82d30-1388">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="82d30-1389">В результате этого изменения несколько групп команд могут "внезапно" оказаться в состоянии предварительной версии в этом выпуске.</span><span class="sxs-lookup"><span data-stu-id="82d30-1389">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="82d30-1390">В действительности большинство пакетов, которые находились в состоянии предварительной версии, в этом выпуске будут считаться общедоступными.</span><span class="sxs-lookup"><span data-stu-id="82d30-1390">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-1391">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-1391">ACR</span></span>
* <span data-ttu-id="82d30-1392">Добавлена команда acr check-health.</span><span class="sxs-lookup"><span data-stu-id="82d30-1392">Added 'acr check-health' command</span></span>
* <span data-ttu-id="82d30-1393">Улучшена обработка ошибок с маркерами безопасности AAD и ошибок при получении внешних команд.</span><span class="sxs-lookup"><span data-stu-id="82d30-1393">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-1394">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-1394">ACS</span></span>
* <span data-ttu-id="82d30-1395">Устаревшие команды ACS теперь скрыты в тексте справки.</span><span class="sxs-lookup"><span data-stu-id="82d30-1395">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="82d30-1396">AMS</span><span class="sxs-lookup"><span data-stu-id="82d30-1396">AMS</span></span>
* <span data-ttu-id="82d30-1397">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в возврате строк времени ISO 8601 для archive-window-length и key-frame-interval-duration.</span><span class="sxs-lookup"><span data-stu-id="82d30-1397">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-1398">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-1398">AppService</span></span>
* <span data-ttu-id="82d30-1399">Добавлена маршрутизация на основе расположение для `webapp deleted list` и `webapp deleted restore`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1399">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="82d30-1400">Исправлена проблема, при которой целевой URL-адрес веб-приложения ("Вы можете запустить приложение в...") не был активным в Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="82d30-1400">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="82d30-1401">Устранена проблема, при которой создание приложений в некоторых SKU завершалось сбоем с ошибкой AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="82d30-1401">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="82d30-1402">Добавлена предварительная проверка в `[appservice|webapp] create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1402">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="82d30-1403">Исправлено `[webapp|functionapp] traffic-routing` для использования правильного actionHostName.</span><span class="sxs-lookup"><span data-stu-id="82d30-1403">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="82d30-1404">Добавлена поддержка слотов для команд `functionapp`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1404">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="82d30-1405">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-1405">Batch</span></span>
* <span data-ttu-id="82d30-1406">Исправлена регрессия проверки подлинности AAD, которую вызывал чрезмерный поток уведомлений об авторизации с помощью общего ключа.</span><span class="sxs-lookup"><span data-stu-id="82d30-1406">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="82d30-1407">Batch AI</span><span class="sxs-lookup"><span data-stu-id="82d30-1407">BatchAI</span></span>
* <span data-ttu-id="82d30-1408">Команды BatchAI теперь признаны устаревшими и скрыты.</span><span class="sxs-lookup"><span data-stu-id="82d30-1408">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="82d30-1409">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="82d30-1409">BotService</span></span>
* <span data-ttu-id="82d30-1410">Добавлены предупреждающие сообщения о прекращении поддержки и режиме обслуживания для команд, которые поддерживают пакет SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="82d30-1410">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82d30-1411">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-1411">CosmosDB</span></span>
* <span data-ttu-id="82d30-1412">[УСТАРЕЛО] использовать команду `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1412">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="82d30-1413">Добавлена команда `cosmosdb keys list`, заменяющая `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1413">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="82d30-1414">`cosmsodb create/update`: Добавлен новый формат для --location, который позволяет задавать свойство isZoneRedundant.</span><span class="sxs-lookup"><span data-stu-id="82d30-1414">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="82d30-1415">Нерекомендуемый старый формат.</span><span class="sxs-lookup"><span data-stu-id="82d30-1415">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="82d30-1416">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="82d30-1416">EventGrid</span></span>
* <span data-ttu-id="82d30-1417">Добавлены команды `eventgrid domain` для операций CRUD домена.</span><span class="sxs-lookup"><span data-stu-id="82d30-1417">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="82d30-1418">Добавлены команды `eventgrid domain topic` для операций CRUD разделов домена.</span><span class="sxs-lookup"><span data-stu-id="82d30-1418">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="82d30-1419">В `eventgrid [topic|event-subscription] list` добавлен аргумент `--odata-query` для фильтрации результатов с использованием синтаксиса OData.</span><span class="sxs-lookup"><span data-stu-id="82d30-1419">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="82d30-1420">`event-subscription create/update`: Добавлена ServiceBusQueue в качестве новых значений для параметра `--endpoint-type`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1420">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="82d30-1421">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в прекращении поддержки `--included-event-types All` с `eventgrid event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1421">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82d30-1422">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82d30-1422">HDInsight</span></span>
* <span data-ttu-id="82d30-1423">Добавлена поддержка параметра `--ssh-public-key` в команде `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1423">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-1424">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-1424">IoT</span></span>
* <span data-ttu-id="82d30-1425">Добавлена поддержка для повторного создания ключей политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="82d30-1425">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="82d30-1426">Добавлен пакет SDK и поддержка для службы подготовки репозитория DigitalTwin.</span><span class="sxs-lookup"><span data-stu-id="82d30-1426">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="82d30-1427">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-1427">Network</span></span>
* <span data-ttu-id="82d30-1428">Добавлена поддержка зон для Шлюза NAT.</span><span class="sxs-lookup"><span data-stu-id="82d30-1428">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="82d30-1429">Добавлена команда `network list-service-tags`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1429">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="82d30-1430">Исправлена проблема с `dns zone import`, при которой пользователям не удавалось импортировать записи А с подстановочным знаком.</span><span class="sxs-lookup"><span data-stu-id="82d30-1430">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="82d30-1431">Исправлена проблема с `watcher flow-log configure`, при которой не удавалось включить ведение журнала потоков в определенных регионах.</span><span class="sxs-lookup"><span data-stu-id="82d30-1431">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-1432">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-1432">Resource</span></span>
* <span data-ttu-id="82d30-1433">Добавлена команда `az rest` для вызовов REST.</span><span class="sxs-lookup"><span data-stu-id="82d30-1433">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="82d30-1434">Исправлена ошибка, возникавшая при использовании `policy assignment list` с группой ресурсов или уровнем подписки `--scope`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1434">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="82d30-1435">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="82d30-1435">ServiceBus</span></span>
* <span data-ttu-id="82d30-1436">Устранена проблема № [9319](https://github.com/azure/azure-cli/issues/9319) с `servicebus topic create --max-size`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1436">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-1437">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-1437">SQL</span></span>
* <span data-ttu-id="82d30-1438">Параметр `--location` стал необязательным для `sql [server|mi] create`. Если он не указан, используется расположение группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1438">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="82d30-1439">Исправлена ошибка "Объект NoneType не подлежит итерации" с `sql db list-editions --available`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1439">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="82d30-1440">SQLVm</span><span class="sxs-lookup"><span data-stu-id="82d30-1440">SQLVm</span></span>
* <span data-ttu-id="82d30-1441">Критическое изменение. Для `sql vm create` теперь требуется параметр `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1441">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="82d30-1442">Внесены изменения, позволяющие задавать SKU образа SQL при создании или обновлении виртуальной машины SQL.</span><span class="sxs-lookup"><span data-stu-id="82d30-1442">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-1443">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-1443">Storage</span></span>
* <span data-ttu-id="82d30-1444">Исправлена проблема с отсутствующим ключом учетной записи для `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1444">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="82d30-1445">Исправлена проблема с `storage blob sync` на платформе Linux.</span><span class="sxs-lookup"><span data-stu-id="82d30-1445">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-1446">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-1446">VM</span></span>
* <span data-ttu-id="82d30-1447">[Предварительная версия] Добавлены команды `vm image template` для создания образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="82d30-1447">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="82d30-1448">4 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1448">June 4, 2019</span></span>

<span data-ttu-id="82d30-1449">Версия 2.0.66</span><span class="sxs-lookup"><span data-stu-id="82d30-1449">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="82d30-1450">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-1450">Core</span></span>
* <span data-ttu-id="82d30-1451">Исправлена ошибка, из-за которой выполнение команды завершалось со сбоем, если параметр `--output yaml` использовался с параметром `--query`</span><span class="sxs-lookup"><span data-stu-id="82d30-1451">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-1452">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-1452">ACR</span></span>
* <span data-ttu-id="82d30-1453">Добавлена группа команд acr pack для создания заданий быстрой сборки с помощью пакетов сборок.</span><span class="sxs-lookup"><span data-stu-id="82d30-1453">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-1454">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-1454">ACS</span></span>
* <span data-ttu-id="82d30-1455">Разрешено включение и отключение надстройки панели мониторинга Kubernetes для AKS.</span><span class="sxs-lookup"><span data-stu-id="82d30-1455">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="82d30-1456">Если подписку нельзя использовать с Azure Red Hat OpenShift, будет отображаться соответствующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="82d30-1456">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="82d30-1457">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-1457">Batch</span></span>
* <span data-ttu-id="82d30-1458">Улучшена обработка ошибок, если не выполнен вход в учетную запись \[[№ 9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[№ 8978](https://github.com/Azure/azure-cli/issues/8978)\].</span><span class="sxs-lookup"><span data-stu-id="82d30-1458">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-1459">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-1459">IoT</span></span>
* <span data-ttu-id="82d30-1460">Добавлена поддержка для перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="82d30-1460">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="82d30-1461">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-1461">Network</span></span>
* <span data-ttu-id="82d30-1462">Добавлены команды `network application-gateway waf-policy` для поддержки настраиваемых правил WAF.</span><span class="sxs-lookup"><span data-stu-id="82d30-1462">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="82d30-1463">Добавлены аргументы `--waf-policy` и `--max-capacity` для команды `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82d30-1463">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="82d30-1464">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-1464">Resource</span></span>
* <span data-ttu-id="82d30-1465">Улучшен вывод сообщения команды `deployment create` при отсутствии TTY.</span><span class="sxs-lookup"><span data-stu-id="82d30-1465">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="82d30-1466">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-1466">Role</span></span>
* <span data-ttu-id="82d30-1467">Обновлен текст справки.</span><span class="sxs-lookup"><span data-stu-id="82d30-1467">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="82d30-1468">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="82d30-1468">Compute</span></span>
* <span data-ttu-id="82d30-1469">Добавлена поддержка команды `vm create` для создания виртуальных машин из управляемого образа с номерами LUN дисков данных, которые не начинаются с 0 или для которых пропущены номера.</span><span class="sxs-lookup"><span data-stu-id="82d30-1469">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="82d30-1470">21 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1470">May 21, 2019</span></span>

<span data-ttu-id="82d30-1471">Версия 2.0.65</span><span class="sxs-lookup"><span data-stu-id="82d30-1471">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="82d30-1472">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-1472">Core</span></span>
* <span data-ttu-id="82d30-1473">Улучшена функция обратной связи при ошибках аутентификации.</span><span class="sxs-lookup"><span data-stu-id="82d30-1473">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="82d30-1474">Исправлена проблема, из-за которой интерфейс командной строки загружал расширения, которые не были совместимы с его базовой версией.</span><span class="sxs-lookup"><span data-stu-id="82d30-1474">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="82d30-1475">Исправлена проблема с запуском и неисправностью `clouds.config`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1475">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-1476">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-1476">ACR</span></span>
* <span data-ttu-id="82d30-1477">Добавлена поддержка управляемых удостоверений в Задачи.</span><span class="sxs-lookup"><span data-stu-id="82d30-1477">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-1478">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-1478">ACS</span></span>
* <span data-ttu-id="82d30-1479">Исправлена команда `openshift create`, используемая с пользовательским клиентом AAD.</span><span class="sxs-lookup"><span data-stu-id="82d30-1479">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-1480">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-1480">AppService</span></span>
* <span data-ttu-id="82d30-1481">[УСТАРЕЛО] Команда `functionapp devops-build` устарела и будет удалена в следующем выпуске.</span><span class="sxs-lookup"><span data-stu-id="82d30-1481">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="82d30-1482">Внесено изменение в `functionapp devops-pipeline` для получения журнала сборки из Azure DevOps в режиме подробного протоколирования.</span><span class="sxs-lookup"><span data-stu-id="82d30-1482">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="82d30-1483">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален неподдерживаемый флаг `--use_local_settings` из команды `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1483">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="82d30-1484">Внесено изменение в `webapp up` для возврата выходных данных JSON, если `--logs` не используется.</span><span class="sxs-lookup"><span data-stu-id="82d30-1484">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="82d30-1485">Добавлена поддержка записи ресурсов по умолчанию в локальную конфигурацию для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1485">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="82d30-1486">Добавлена поддержка `webapp up` для повторного развертывания приложения без использования аргумента `--location`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1486">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="82d30-1487">Устранена проблема, из-за которой нельзя было создать для Linux номер SKU с планом службы приложений "Бесплатный".</span><span class="sxs-lookup"><span data-stu-id="82d30-1487">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="82d30-1488">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="82d30-1488">BotService</span></span>
* <span data-ttu-id="82d30-1489">Внесено изменение для включения поддержки всех регистров в параметрах `--lang` для команд.</span><span class="sxs-lookup"><span data-stu-id="82d30-1489">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="82d30-1490">Обновлено описание модуля команды.</span><span class="sxs-lookup"><span data-stu-id="82d30-1490">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="82d30-1491">Потребление</span><span class="sxs-lookup"><span data-stu-id="82d30-1491">Consumption</span></span>
* <span data-ttu-id="82d30-1492">Добавлен отсутствующий обязательный параметр при выполнении `consumption usage list --billing-period-name`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1492">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-1493">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-1493">IoT</span></span>
* <span data-ttu-id="82d30-1494">Добавлена поддержка перечисления всех ключей.</span><span class="sxs-lookup"><span data-stu-id="82d30-1494">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="82d30-1495">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-1495">Network</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="82d30-1497">Добавлен аргумент `--nat-gateway` для `network vnet subnet [create|update]` для подключения к шлюзу NAT.</span><span class="sxs-lookup"><span data-stu-id="82d30-1497">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="82d30-1498">Исправлена проблема с `dns zone import`, из-за которой имена записей не сопоставлялись с типом записей.</span><span class="sxs-lookup"><span data-stu-id="82d30-1498">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="82d30-1499">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="82d30-1499">RDBMS</span></span>
* <span data-ttu-id="82d30-1500">Добавлена поддержка Postgres и MySQL для георепликации.</span><span class="sxs-lookup"><span data-stu-id="82d30-1500">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="82d30-1501">RBAC</span><span class="sxs-lookup"><span data-stu-id="82d30-1501">RBAC</span></span>
* <span data-ttu-id="82d30-1502">Добавлена поддержка области группы управления для `role assignment`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1502">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-1503">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-1503">Storage</span></span>
* <span data-ttu-id="82d30-1504">`storage blob sync`: добавьте команду синхронизации для хранилища BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1504">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="82d30-1505">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="82d30-1505">Compute</span></span>
* <span data-ttu-id="82d30-1506">Добавлен параметр `--computer-name` для `vm create` для установки имени виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="82d30-1506">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="82d30-1507">Переименован параметр `--ssh-key-value` в `--ssh-key-values` для `[vm|vmss] create` для приема нескольких значений пути или открытого ключа SSH.</span><span class="sxs-lookup"><span data-stu-id="82d30-1507">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="82d30-1508">__Примечание.__ Это **не** критическое изменение, благодаря которому `--ssh-key-value` будет правильно анализироваться, так как соответствует только `--ssh-key-values`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1508">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="82d30-1509">Внесено изменение в аргумент `ppg create` для `--type` — теперь он необязательный.</span><span class="sxs-lookup"><span data-stu-id="82d30-1509">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="82d30-1510">6 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1510">May 6, 2019</span></span>

<span data-ttu-id="82d30-1511">Версия 2.0.64</span><span class="sxs-lookup"><span data-stu-id="82d30-1511">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-1512">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-1512">ACS</span></span>
* <span data-ttu-id="82d30-1513">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--fqdn` из команд `openshift`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1513">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="82d30-1514">Внесено изменение для использования общедоступной версии API для Azure Red Hat Openshift.</span><span class="sxs-lookup"><span data-stu-id="82d30-1514">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="82d30-1515">Добавлен флаг `customer-admin-group-id` в `openshift create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1515">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="82d30-1516">[Общедоступная версия.] `(PREVIEW)` больше не используется для `aks create` в параметре `--network-policy`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1516">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-1517">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-1517">Appservice</span></span>
* <span data-ttu-id="82d30-1518">[УСТАРЕЛО] Команда `functionapp devops-build` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="82d30-1518">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="82d30-1519">Команда переименована в `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1519">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="82d30-1520">Исправлен процесс получения правильного имени пользователя для Cloud Shell, приводивший к ошибке выполнения `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1520">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="82d30-1521">Обновлена документация по `appservice plan --sku` в соответствии с поддерживаемыми планами службы приложений.</span><span class="sxs-lookup"><span data-stu-id="82d30-1521">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="82d30-1522">Добавлены необязательные аргументы для группы ресурсов и план для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1522">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="82d30-1523">Добавлена поддержка `webapp ssh` в соответствии с переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1523">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="82d30-1524">Добавлена поддержка `appserviceplan create` для ценовой категории "Бесплатный" в Linux.</span><span class="sxs-lookup"><span data-stu-id="82d30-1524">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="82d30-1525">Внесено изменение в `webapp up` для перевода в спящий режим на 30 с после установки параметра приложения `SCM_DO_BUILD_DURING_DEPLOYMENT=true` для обработки холодного запуска Kudu.</span><span class="sxs-lookup"><span data-stu-id="82d30-1525">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="82d30-1526">Добавлена поддержка среды выполнения `powershell` для `functionapp create` в Windows.</span><span class="sxs-lookup"><span data-stu-id="82d30-1526">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="82d30-1527">Добавлена команда `create-remote-connection`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1527">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="82d30-1528">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-1528">Batch</span></span>
* <span data-ttu-id="82d30-1529">Исправлена ошибка в проверяющем элементе управления для параметров `--application-package-references`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1529">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="82d30-1530">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="82d30-1530">Botservice</span></span>
* <span data-ttu-id="82d30-1531">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` для создания пустого бота веб-приложения по умолчанию (т. е. бот не развертывается в Службе приложений).</span><span class="sxs-lookup"><span data-stu-id="82d30-1531">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="82d30-1532">Добавлен флаг `--echo` в `bot create` для использования старого поведения с `-v v4`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1532">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="82d30-1533">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено значение по умолчанию `--version` на `v4`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1533">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="82d30-1534">__ПРИМЕЧАНИЕ.__ `bot prepare-publish` по-прежнему использует старое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-1534">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="82d30-1535">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `--lang` — значение `Csharp` больше не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-1535">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="82d30-1536">Если команда требует `--lang`, который не указан, команда завершит работу с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="82d30-1536">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="82d30-1537">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в аргументы `--appid` и `--password` для `bot create` — теперь они являются обязательными и их можно создать с помощью `ad app create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1537">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="82d30-1538">Добавлена проверка `--appid` и `--password`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1538">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="82d30-1539">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4`, чтобы не создавать или не использовать учетную запись хранения или Application Insights.</span><span class="sxs-lookup"><span data-stu-id="82d30-1539">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="82d30-1540">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v3`, чтобы требовать регион, где доступна служба Application Insights.</span><span class="sxs-lookup"><span data-stu-id="82d30-1540">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="82d30-1541">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot update`, чтобы влиять только на определенные свойства бота.</span><span class="sxs-lookup"><span data-stu-id="82d30-1541">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="82d30-1542">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в флаг `--lang` для принятия `Javascript` вместо `Node`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1542">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="82d30-1543">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`Node` больше не используется как допустимое значение `--lang`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1543">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="82d30-1544">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` — значение `SCM_DO_BUILD_DURING_DEPLOYMENT` больше не равно true.</span><span class="sxs-lookup"><span data-stu-id="82d30-1544">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="82d30-1545">Все развертывания через Kudu будут работать в соответствии с поведением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-1545">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="82d30-1546">Внесено изменение в `bot download` для ботов без файлов `.bot`, чтобы создавать файл конфигурации для определенного языка со значениями из параметров приложения для бота.</span><span class="sxs-lookup"><span data-stu-id="82d30-1546">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="82d30-1547">В команду `bot prepare-deploy` добавлена поддержка параметра `Typescript`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1547">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="82d30-1548">Добавлено предупреждающее сообщение в `bot prepare-deploy` для ботов `Javascript` и `Typescript`, когда `--code-dir` не содержит `package.json`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1548">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="82d30-1549">Внесено изменение в `bot prepare-deploy` для возврата `true` при успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="82d30-1549">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="82d30-1550">Включено ведение подробного журнала для `bot prepare-deploy`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1550">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="82d30-1551">Добавлены более доступные регионы Application Insights для `az bot create -v v3`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1551">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="82d30-1552">Configure</span><span class="sxs-lookup"><span data-stu-id="82d30-1552">Configure</span></span>
* <span data-ttu-id="82d30-1553">Добавлена поддержка конфигурации по умолчанию для аргумента на основе папки.</span><span class="sxs-lookup"><span data-stu-id="82d30-1553">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="82d30-1554">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="82d30-1554">Eventhubs</span></span>
* <span data-ttu-id="82d30-1555">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1555">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="82d30-1556">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1556">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="82d30-1557">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-1557">Network</span></span>
* <span data-ttu-id="82d30-1558">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--cache` на `--defer` для `vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1558">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="82d30-1559">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="82d30-1559">Policy Insights</span></span>
* <span data-ttu-id="82d30-1560">Добавлена поддержка `--expand PolicyEvaluationDetails` для результатов оценки политики запросов для ресурса.</span><span class="sxs-lookup"><span data-stu-id="82d30-1560">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="82d30-1561">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-1561">Role</span></span>
* <span data-ttu-id="82d30-1562">[УСТАРЕЛО] Внесено изменение в `create-for-rbac` для скрытия аргумента --password (поддержка прекращается в мае 2019 г.).</span><span class="sxs-lookup"><span data-stu-id="82d30-1562">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="82d30-1563">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="82d30-1563">Service Bus</span></span>
* <span data-ttu-id="82d30-1564">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1564">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="82d30-1565">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1565">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="82d30-1566">Внесено исправление в `topic [create|update]` — теперь `--max-size` поддерживает значения 10, 20, 40 и 80 ГБ для номера SKU ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="82d30-1566">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-1567">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-1567">SQL</span></span>
* <span data-ttu-id="82d30-1568">Добавлены команды `sql virtual-cluster [list|show|delete]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1568">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-1569">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-1569">VM</span></span>
* <span data-ttu-id="82d30-1570">Добавлены параметры `--protect-from-scale-in` и `--protect-from-scale-set-actions` для `vmss update`, чтобы включать обновления политики защиты для экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="82d30-1570">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="82d30-1571">Добавлены параметры `--instance-id` для `vmss update` для включения общего обновления экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="82d30-1571">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="82d30-1572">Добавлен параметр `--instance-id` для команды `vmss wait`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1572">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="82d30-1573">Добавлена новая группа команд `ppg` для управления группами размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="82d30-1573">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="82d30-1574">Добавлен параметр `--ppg` для `[vm|vmss] create` и `vm availability-set create` для управления PPG.</span><span class="sxs-lookup"><span data-stu-id="82d30-1574">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="82d30-1575">Добавлен параметр `--hyper-v-generation` для команды `image create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1575">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="82d30-1576">23 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1576">April 23, 2019</span></span>

<span data-ttu-id="82d30-1577">Версия 2.0.63</span><span class="sxs-lookup"><span data-stu-id="82d30-1577">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-1578">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-1578">ACS</span></span>
* <span data-ttu-id="82d30-1579">Внесено изменение в `aks get-credentials` для запроса на перезапись повторяющихся значений.</span><span class="sxs-lookup"><span data-stu-id="82d30-1579">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="82d30-1580">Удалено описание `(PREVIEW)` из команд Dev Spaces aks use-dev-spaces и aks remove-dev-spaces.</span><span class="sxs-lookup"><span data-stu-id="82d30-1580">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="82d30-1581">AMS</span><span class="sxs-lookup"><span data-stu-id="82d30-1581">AMS</span></span>
* <span data-ttu-id="82d30-1582">Исправлена ошибка с обновлением фильтров ресурсов и учетных записей.</span><span class="sxs-lookup"><span data-stu-id="82d30-1582">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-1583">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-1583">AppService</span></span>
* <span data-ttu-id="82d30-1584">Добавлена поддержка ASE и времени ожидания для `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1584">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="82d30-1585">Добавлена возможность настройки непрерывной интеграции и развертывания в конвейере Azure DevOps из репозитория Github для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="82d30-1585">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="82d30-1586">Добавлен аргумент `--github-pat` для `functionapp devops-build create` для получения личного маркера доступа Github.</span><span class="sxs-lookup"><span data-stu-id="82d30-1586">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="82d30-1587">Добавлен аргумент `--github-repository` для `functionapp devops-build create` для подключения репозитория Github, который содержит исходный код приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="82d30-1587">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="82d30-1588">Исправлена проблема со сбоем `az webapp up --logs` и обновлением .Net Core до версии 2.1 по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-1588">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="82d30-1589">Удалены ненужные параметры приложения-функции при создании приложения-функции с помощью плана потребления.</span><span class="sxs-lookup"><span data-stu-id="82d30-1589">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="82d30-1590">Внесены изменения в `webapp up`, чтобы строка ASP по умолчанию добавляла номера в конец для создания плана службы приложений на основе параметров SKU.</span><span class="sxs-lookup"><span data-stu-id="82d30-1590">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="82d30-1591">Добавлен параметр `-b` для `webapp up` для запуска приложения в браузере.</span><span class="sxs-lookup"><span data-stu-id="82d30-1591">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="82d30-1592">Внесены изменения в `webapp deployment source config zip` для обработки переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1592">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="82d30-1593">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="82d30-1593">Deployment Manager</span></span>
* <span data-ttu-id="82d30-1594">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Создание и администрирование артефактов, которые поддерживают развертывания</span><span class="sxs-lookup"><span data-stu-id="82d30-1594">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="82d30-1595">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="82d30-1595">Lab</span></span>
* <span data-ttu-id="82d30-1596">Исправлена ошибка, которая приводила к неожиданному завершению работы.</span><span class="sxs-lookup"><span data-stu-id="82d30-1596">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="82d30-1597">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-1597">Network</span></span>
* <span data-ttu-id="82d30-1598">Добавлено автоматическое делегирование сервера имен для `dns zone create` в родительском объекте во время создания дочерней зоны.</span><span class="sxs-lookup"><span data-stu-id="82d30-1598">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-1599">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-1599">Resource</span></span>
* <span data-ttu-id="82d30-1600">[УСТАРЕЛО] Не рекомендуются к использованию аргументы `--link-id`, `--target-id` и `--filter-string` для `resource link`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1600">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="82d30-1601">Используйте вместо них аргументы `--link`, `--target` и `--filter`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1601">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="82d30-1602">Исправлена проблема, из-за которой команды `resource link [create|update]` не работали.</span><span class="sxs-lookup"><span data-stu-id="82d30-1602">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="82d30-1603">Исправлена проблема, из-за которой удаление с помощью идентификатора ресурса приводило к сбою или ошибке.</span><span class="sxs-lookup"><span data-stu-id="82d30-1603">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-1604">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-1604">SQL</span></span>
* <span data-ttu-id="82d30-1605">Добавлена поддержка пользовательского часового пояса в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="82d30-1605">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="82d30-1606">Внесено изменение, чтобы разрешить использовать имя эластичного пула с `sql db update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1606">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="82d30-1607">В команду `sql server [create|update]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1607">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="82d30-1608">Добавлена команда `sql server wait`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1608">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-1609">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-1609">Storage</span></span>
* <span data-ttu-id="82d30-1610">Устранена проблема с двойной кодировкой маркеров SAS в `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1610">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-1611">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-1611">VM</span></span>
* <span data-ttu-id="82d30-1612">Добавлен флаг `--skip-shutdown` для `vm|vmss stop` для выключения виртуальных машин без завершения работы.</span><span class="sxs-lookup"><span data-stu-id="82d30-1612">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="82d30-1613">Добавлен аргумент `--storage-account-type` для `sig image-version create` настройки типа учетной записи профиля публикации.</span><span class="sxs-lookup"><span data-stu-id="82d30-1613">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="82d30-1614">Добавлен аргумент `--target-regions` для `sig image-version create` для указания типов учетных записей хранения, связанных с регионами.</span><span class="sxs-lookup"><span data-stu-id="82d30-1614">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="82d30-1615">9 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1615">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="82d30-1616">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-1616">Core</span></span>
* <span data-ttu-id="82d30-1617">Исправлена проблема, из-за которой для некоторых расширений отображалась версия `Unknown` и ее невозможно было обновить.</span><span class="sxs-lookup"><span data-stu-id="82d30-1617">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-1618">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-1618">ACR</span></span>
* <span data-ttu-id="82d30-1619">Добавлена поддержка запуска образа без контекста.</span><span class="sxs-lookup"><span data-stu-id="82d30-1619">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="82d30-1620">AMS</span><span class="sxs-lookup"><span data-stu-id="82d30-1620">AMS</span></span>
* [УСТАРЕЛО]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="82d30-1623">Добавлена поддержка новых параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1623">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="82d30-1624">Добавлен новый параметр `--filters` для `ams streaming-locator create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1624">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-1625">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-1625">AppService</span></span>
* <span data-ttu-id="82d30-1626">В команду `webapp up` добавлена поддержка параметра `--logs`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1626">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="82d30-1627">Исправлены ошибки в команде `functionapp devops-build create` при создании файла `azure-pipelines.yml`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1627">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="82d30-1628">Улучшена обработка и индикаторы ошибок с `unctionapp devops-build create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1628">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="82d30-1629">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--local-git` для команды `devops-build`. Обнаружение и обработка локального репозитория Git являются обязательными для создания конвейеров DevOps в Azure.</span><span class="sxs-lookup"><span data-stu-id="82d30-1629">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="82d30-1630">Добавлена поддержка создания плана функций Linux.</span><span class="sxs-lookup"><span data-stu-id="82d30-1630">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="82d30-1631">Добавлена возможность менять план для приложения-функции с помощью `functionapp update --plan`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1631">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="82d30-1632">Добавлена поддержка параметров горизонтального увеличения масштаба плана "Премиум" для Функций Azure.</span><span class="sxs-lookup"><span data-stu-id="82d30-1632">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="82d30-1633">CDN</span><span class="sxs-lookup"><span data-stu-id="82d30-1633">CDN</span></span>
* <span data-ttu-id="82d30-1634">Добавлена поддержка `Microsoft_Standard` и `Standard_ChinaCdn`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1634">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="82d30-1635">Отзывы</span><span class="sxs-lookup"><span data-stu-id="82d30-1635">Feedback</span></span>
* <span data-ttu-id="82d30-1636">Внесены изменения в `feedback` для отображения метаданных недавно выполненных команд.</span><span class="sxs-lookup"><span data-stu-id="82d30-1636">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="82d30-1637">Внесены изменения в `feedback`. Теперь при регистрации проблемы отображается запрос, в соответствии с которым пользователь должен открыть браузер и воспользоваться шаблоном проблемы.</span><span class="sxs-lookup"><span data-stu-id="82d30-1637">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="82d30-1638">Внесены изменения в `feedback`. Теперь текст проблемы выводится при запуске с параметром --verbose.</span><span class="sxs-lookup"><span data-stu-id="82d30-1638">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-1639">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-1639">Monitor</span></span>
* <span data-ttu-id="82d30-1640">Исправлена проблема, из-за которой у параметра count было недопустимое значение в `metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1640">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="82d30-1641">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-1641">Network</span></span>
* <span data-ttu-id="82d30-1642">Исправлен формат таблицы, которая не отображалась с помощью `vnet-gateway list-bgp-peer-status`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1642">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="82d30-1643">Добавлены команды `list-request-headers` и `list-response-headers` для `application-gateway rewrite-rule`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1643">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="82d30-1644">Добавлена команда `list-server-variables` для `application-gateway rewrite-rule condition`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1644">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="82d30-1645">Исправлена проблема, из-за которой обновление состояния соединения на порту ExpressRoute вызывало неизвестное исключение атрибута `express-route port update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1645">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="82d30-1646">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="82d30-1646">PrivateDNS</span></span>
* <span data-ttu-id="82d30-1647">Добавлена команда `network private-dns` для частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="82d30-1647">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-1648">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-1648">Resource</span></span>
* <span data-ttu-id="82d30-1649">Исправлена проблема с `deployment create` и `group deployment create`, из-за которой файл параметров с пустым набором параметров не работал.</span><span class="sxs-lookup"><span data-stu-id="82d30-1649">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="82d30-1650">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-1650">Role</span></span>
* <span data-ttu-id="82d30-1651">Внесены исправления в `create-for-rbac`. Теперь `--years` обрабатывается правильно.</span><span class="sxs-lookup"><span data-stu-id="82d30-1651">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="82d30-1652">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `role assignment delete`. Теперь появляется запрос при удалении всех назначений в рамках подписки без дополнительных условий.</span><span class="sxs-lookup"><span data-stu-id="82d30-1652">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-1653">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-1653">SQL</span></span>
* <span data-ttu-id="82d30-1654">Команда `sql mi [create|update]` обновлена с помощью свойств proxyOverride и publicDataEndpointEnabled.</span><span class="sxs-lookup"><span data-stu-id="82d30-1654">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-1655">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-1655">Storage</span></span>
* <span data-ttu-id="82d30-1656">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален результат выполнения `storage blob delete`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1656">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="82d30-1657">В команду `storage blob generate-sas` добавлен параметр `--full-uri` для создания полного URI большого двоичного объекта с помощью SAS.</span><span class="sxs-lookup"><span data-stu-id="82d30-1657">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="82d30-1658">В команду `storage file copy start` добавлен параметр `--file-snapshot` для копирования файла из моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="82d30-1658">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="82d30-1659">Внесены изменения в `storage blob copy cancel`. Теперь вместо исключения для NoPendingCopyOperation отображается только сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="82d30-1659">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="82d30-1660">26 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1660">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="82d30-1661">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-1661">Core</span></span>
* <span data-ttu-id="82d30-1662">Устранены проблемы с несовместимостью расширений для разработки.</span><span class="sxs-lookup"><span data-stu-id="82d30-1662">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="82d30-1663">Функция обработки ошибок теперь указывает клиентам на страницу проблем.</span><span class="sxs-lookup"><span data-stu-id="82d30-1663">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="82d30-1664">Cloud</span><span class="sxs-lookup"><span data-stu-id="82d30-1664">Cloud</span></span>
* <span data-ttu-id="82d30-1665">Исправлена ошибка с сообщением о не найденной подписке в `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1665">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-1666">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-1666">ACR</span></span>
* <span data-ttu-id="82d30-1667">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="82d30-1667">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="82d30-1668">Добавлено `--auth-mode` в команды `acr build`, `acr run`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1668">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="82d30-1669">Добавлена команда acr task credential для управления учетными данными для задачи.</span><span class="sxs-lookup"><span data-stu-id="82d30-1669">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="82d30-1670">Добавлено --no-wait в команду `acr build`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1670">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-1671">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-1671">AppService</span></span>
* <span data-ttu-id="82d30-1672">Исправлена ошибка с `webapp up`, из-за которой нельзя было правильно выполнить запуск из пустого каталога или скрипта неизвестного кода.</span><span class="sxs-lookup"><span data-stu-id="82d30-1672">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="82d30-1673">Исправлена ошибка, из-за которой не работали слоты для `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1673">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="82d30-1674">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="82d30-1674">BOT Service</span></span>
* <span data-ttu-id="82d30-1675">Добавлено `bot prepare-deploy` для подготовки к развертыванию ботов с помощью `webapp`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1675">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="82d30-1676">Изменено `bot create --kind registration` для отображения пароля, если пароль не указан.</span><span class="sxs-lookup"><span data-stu-id="82d30-1676">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="82d30-1677">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--endpoint` в `bot create --kind registration` на пустую строку (по умолчанию) вместо запрашиваемой.</span><span class="sxs-lookup"><span data-stu-id="82d30-1677">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="82d30-1678">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="82d30-1678">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="82d30-1679">CDN</span><span class="sxs-lookup"><span data-stu-id="82d30-1679">CDN</span></span>
* <span data-ttu-id="82d30-1680">Добавлена поддержка параметра `--no-wait` в команде `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1680">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="82d30-1681">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено поведение кэширования строки запроса `cdn endpoint create` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-1681">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="82d30-1682">IgnoreQueryString больше не используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-1682">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="82d30-1683">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="82d30-1683">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82d30-1684">Сosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-1684">Cosmosdb</span></span>
* <span data-ttu-id="82d30-1685">Добавлена поддержка `--enable-multiple-write-locations` для обновления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="82d30-1685">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="82d30-1686">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="82d30-1686">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="82d30-1687">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="82d30-1687">Interactive</span></span>
* <span data-ttu-id="82d30-1688">Исправлена несовместимость с интерактивным расширением, установленным с помощью azdev.</span><span class="sxs-lookup"><span data-stu-id="82d30-1688">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-1689">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-1689">Monitor</span></span>
* <span data-ttu-id="82d30-1690">Внесено изменение, разрешающее использовать значение измерения `*` для `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1690">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="82d30-1691">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-1691">Network</span></span>
* <span data-ttu-id="82d30-1692">Добавлена группа команд `rewrite-rule` для `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1692">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-1693">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-1693">Profile</span></span>
* <span data-ttu-id="82d30-1694">Включена поддержка учетной записи уровня клиентов для управляемого удостоверения службы для `login`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1694">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="82d30-1695">Postgres</span><span class="sxs-lookup"><span data-stu-id="82d30-1695">Postgres</span></span> 
* <span data-ttu-id="82d30-1696">Добавлены команды postgresql `replica` и команда `restart server`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1696">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="82d30-1697">Внесены изменения для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="82d30-1697">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-1698">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-1698">Resource</span></span>
* <span data-ttu-id="82d30-1699">Улучшены табличные выходные данные для `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1699">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="82d30-1700">Исправлена проблема с `deployment [create|validate]`, из-за которой secureObject типа не распознавался.</span><span class="sxs-lookup"><span data-stu-id="82d30-1700">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="82d30-1701">График</span><span class="sxs-lookup"><span data-stu-id="82d30-1701">Graph</span></span>
* <span data-ttu-id="82d30-1702">Добавлена поддержка параметра `--end-date` в команде `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1702">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="82d30-1703">Добавлена поддержка разрешений для `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1703">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="82d30-1704">Исправлена проблема с `ad app permission list`, из-за которой отсутствовали разрешения.</span><span class="sxs-lookup"><span data-stu-id="82d30-1704">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="82d30-1705">Изменено `ad sp delete` для пропуска удаления назначения роли, если текущая учетная запись не содержит подписок.</span><span class="sxs-lookup"><span data-stu-id="82d30-1705">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="82d30-1706">Изменено `ad app create` для использования `--identifier-uris` пустого списка (по умолчанию), если список не указан.</span><span class="sxs-lookup"><span data-stu-id="82d30-1706">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-1707">носителей.</span><span class="sxs-lookup"><span data-stu-id="82d30-1707">storage</span></span>
* <span data-ttu-id="82d30-1708">Добавлено `--snapshot` для `storage file download-batch` для скачивания из моментального снимка общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="82d30-1708">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="82d30-1709">Изменен индикатор выполнения `storage blob [download-batch|upload-batch]`, чтобы обобщить сведения и указать текущий большой двоичный объект.</span><span class="sxs-lookup"><span data-stu-id="82d30-1709">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="82d30-1710">Исправлена проблема с `storage account update` при обновлении параметров шифрования.</span><span class="sxs-lookup"><span data-stu-id="82d30-1710">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="82d30-1711">Исправлена проблема со сбоем `storage blob show` при использовании OAuth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="82d30-1711">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-1712">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-1712">VM</span></span>
* <span data-ttu-id="82d30-1713">Добавлена команда `image update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1713">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="82d30-1714">12 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1714">March 12, 2019</span></span>

<span data-ttu-id="82d30-1715">Версия 2.0.60</span><span class="sxs-lookup"><span data-stu-id="82d30-1715">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="82d30-1716">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-1716">Core</span></span>

* <span data-ttu-id="82d30-1717">Исправлена недопустимая ошибка в `cloud set` о том, что подписка не найдена.</span><span class="sxs-lookup"><span data-stu-id="82d30-1717">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-1718">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-1718">ACR</span></span>

* <span data-ttu-id="82d30-1719">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="82d30-1719">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-1720">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-1720">ACS</span></span>

* <span data-ttu-id="82d30-1721">Внесены изменения, в соответствии с которыми параметр `--listen-address` для `aks browse` игнорируется, если он не поддерживается kubectl.</span><span class="sxs-lookup"><span data-stu-id="82d30-1721">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="82d30-1722">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-1722">AppService</span></span>

* <span data-ttu-id="82d30-1723">Добавлено `[webapp|functionapp] deployment list-publishing-credentials` для получения URL-адреса публикации Kudu и связанных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="82d30-1723">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="82d30-1724">Удалена ошибочная инструкция печати для `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1724">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="82d30-1725">Исправлено `functionapp` для настройки правильного образа для среды выполнения в планах службы приложений Linux.</span><span class="sxs-lookup"><span data-stu-id="82d30-1725">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="82d30-1726">Удален тег предварительной версии для `webapp up` и добавлены усовершенствования в команду.</span><span class="sxs-lookup"><span data-stu-id="82d30-1726">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="82d30-1727">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="82d30-1727">Botservice</span></span>

* <span data-ttu-id="82d30-1728">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="82d30-1728">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="82d30-1729">Добавлено `Microsoft-BotFramework-AppId` и `Microsoft-BotFramework-AppPassword` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="82d30-1729">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="82d30-1730">Удалены одинарные кавычки из выходных данных команды `bot publish` в конце `bot create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1730">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="82d30-1731">Изменено `bot publish` для включения поддержки асинхронных операций.</span><span class="sxs-lookup"><span data-stu-id="82d30-1731">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="82d30-1732">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-1732">Container</span></span>

* <span data-ttu-id="82d30-1733">Добавлен аргумент `--no-wait` для команды `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="82d30-1733">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="82d30-1734">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="82d30-1734">EventHub</span></span>

* <span data-ttu-id="82d30-1735">Добавлен флаг `--skip-empty-archives` для `eventhub create|update` для включения поддержки пустых архивов при записи.</span><span class="sxs-lookup"><span data-stu-id="82d30-1735">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="82d30-1736">Поиск</span><span class="sxs-lookup"><span data-stu-id="82d30-1736">Find</span></span>

* <span data-ttu-id="82d30-1737">Основные обновления функций</span><span class="sxs-lookup"><span data-stu-id="82d30-1737">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82d30-1738">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82d30-1738">HDInsight</span></span>

* <span data-ttu-id="82d30-1739">Добавлен параметр `--storage-account-managed-identity` для `hdinsight create` для включения поддержки MSI ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="82d30-1739">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="82d30-1740">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-1740">Network</span></span>

* <span data-ttu-id="82d30-1741">Исправлена проблема с `vpn-connection update`, когда обновление VPN-подключения между шлюзами в разных подписках завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="82d30-1741">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="82d30-1742">Rdbms</span><span class="sxs-lookup"><span data-stu-id="82d30-1742">Rdbms</span></span>

* <span data-ttu-id="82d30-1743">Незначительные исправления для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="82d30-1743">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="82d30-1744">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-1744">Role</span></span>

* <span data-ttu-id="82d30-1745">Исправлено `role definition update` для использования идентификатора для правильного разрешения определения.</span><span class="sxs-lookup"><span data-stu-id="82d30-1745">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="82d30-1746">Изменено `ad app credential reset` для исключения предположения о том, что субъект-служба приложения всегда существует.</span><span class="sxs-lookup"><span data-stu-id="82d30-1746">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="82d30-1747">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="82d30-1747">Service Fabric</span></span>

* <span data-ttu-id="82d30-1748">Исправлена проблема с `sf cluster list` и невозможностью итерации.</span><span class="sxs-lookup"><span data-stu-id="82d30-1748">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="82d30-1749">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1749">February 26, 2019</span></span>

<span data-ttu-id="82d30-1750">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="82d30-1750">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="82d30-1751">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-1751">Core</span></span>

* <span data-ttu-id="82d30-1752">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="82d30-1752">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-1753">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-1753">ACR</span></span>

* <span data-ttu-id="82d30-1754">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1754">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="82d30-1755">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="82d30-1755">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-1756">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-1756">ACS</span></span>

* <span data-ttu-id="82d30-1757">Добавлен параметр `--listen-address` для команды `aks port-forward`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1757">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-1758">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-1758">AppService</span></span>

* <span data-ttu-id="82d30-1759">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1759">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="82d30-1760">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-1760">Batch</span></span>
* <span data-ttu-id="82d30-1761">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1761">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="82d30-1762">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1762">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="82d30-1763">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="82d30-1763">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="82d30-1764">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1764">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="82d30-1765">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="82d30-1765">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="82d30-1766">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="82d30-1766">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82d30-1767">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-1767">CosmosDB</span></span>

* <span data-ttu-id="82d30-1768">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="82d30-1768">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="82d30-1769">Kusto</span><span class="sxs-lookup"><span data-stu-id="82d30-1769">Kusto</span></span>

* <span data-ttu-id="82d30-1770">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="82d30-1770">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="82d30-1771">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-1771">Network</span></span>

* <span data-ttu-id="82d30-1772">Добавлен аргумент `--express-route-gateway-bypass` для команды `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82d30-1772">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="82d30-1773">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1773">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="82d30-1774">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1774">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="82d30-1775">Добавлен аргумент `--legacy-mode` в команду `express-route peering [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1775">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="82d30-1776">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1776">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="82d30-1777">Добавлен аргумент `--gateway-default-site` для команды `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82d30-1777">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="82d30-1778">Добавлены команды `ipsec-policy` для `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1778">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-1779">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-1779">Resource</span></span>

* <span data-ttu-id="82d30-1780">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="82d30-1780">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="82d30-1781">Добавлена поддержка файла параметров на основе URI для `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1781">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="82d30-1782">Добавлена поддержка определений и параметров на основе URI для `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1782">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="82d30-1783">Исправлена обработка параметров и правил для `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1783">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="82d30-1784">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="82d30-1784">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="82d30-1785">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-1785">Role</span></span>

* <span data-ttu-id="82d30-1786">Добавлена поддержка ролей приложений для `ad app [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1786">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-1787">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-1787">VM</span></span>

* <span data-ttu-id="82d30-1788">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="82d30-1788">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="82d30-1789">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1789">February 12, 2019</span></span>

<span data-ttu-id="82d30-1790">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="82d30-1790">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="82d30-1791">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-1791">Core</span></span>

* <span data-ttu-id="82d30-1792">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="82d30-1792">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="82d30-1793">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="82d30-1793">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-1794">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-1794">ACR</span></span>
* <span data-ttu-id="82d30-1795">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1795">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="82d30-1796">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1796">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-1797">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-1797">ACS</span></span>
* <span data-ttu-id="82d30-1798">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="82d30-1798">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="82d30-1799">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1799">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="82d30-1800">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="82d30-1800">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="82d30-1801">AMS</span><span class="sxs-lookup"><span data-stu-id="82d30-1801">AMS</span></span>
* <span data-ttu-id="82d30-1802">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1802">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="82d30-1803">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1803">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-1804">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-1804">Appservice</span></span>
* <span data-ttu-id="82d30-1805">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="82d30-1805">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="82d30-1806">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="82d30-1806">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="82d30-1807">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1807">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="82d30-1808">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="82d30-1808">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="82d30-1809">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="82d30-1809">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="82d30-1810">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="82d30-1810">Botservice</span></span>
* <span data-ttu-id="82d30-1811">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1811">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="82d30-1812">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1812">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="82d30-1813">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1813">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="82d30-1814">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="82d30-1814">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="82d30-1815">[УСТАРЕЛО] Аргумент `--proj-name` не рекомендуется к использованию. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1815">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="82d30-1816">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="82d30-1816">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="82d30-1817">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="82d30-1817">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="82d30-1818">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="82d30-1818">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="82d30-1819">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="82d30-1819">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="82d30-1820">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="82d30-1820">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="82d30-1821">Key Vault</span><span class="sxs-lookup"><span data-stu-id="82d30-1821">Key Vault</span></span>
* <span data-ttu-id="82d30-1822">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1822">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-1823">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-1823">Monitor</span></span>
* <span data-ttu-id="82d30-1824">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1824">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="82d30-1825">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-1825">Network</span></span>
* <span data-ttu-id="82d30-1826">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="82d30-1826">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="82d30-1827">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="82d30-1827">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="82d30-1828">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="82d30-1828">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="82d30-1829">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1829">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="82d30-1830">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="82d30-1830">Policy Insights</span></span>
* <span data-ttu-id="82d30-1831">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1831">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="82d30-1832">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="82d30-1832">RDBMS</span></span>
* <span data-ttu-id="82d30-1833">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="82d30-1833">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="82d30-1834">Redis</span><span class="sxs-lookup"><span data-stu-id="82d30-1834">Redis</span></span>
* <span data-ttu-id="82d30-1835">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="82d30-1835">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="82d30-1836">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="82d30-1836">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="82d30-1837">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="82d30-1837">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="82d30-1838">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="82d30-1838">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="82d30-1839">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1839">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="82d30-1840">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="82d30-1840">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="82d30-1841">[УСТАРЕЛО] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82d30-1841">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="82d30-1842">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-1842">Role</span></span>
* <span data-ttu-id="82d30-1843">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1843">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="82d30-1844">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-1844">SQL VM</span></span>
* <span data-ttu-id="82d30-1845">[УСТАРЕЛО] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="82d30-1845">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-1846">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-1846">VM</span></span>
* <span data-ttu-id="82d30-1847">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1847">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="82d30-1848">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1848">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="82d30-1849">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="82d30-1849">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="82d30-1850">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1850">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="82d30-1851">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1851">January 31, 2019</span></span>

<span data-ttu-id="82d30-1852">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="82d30-1852">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="82d30-1853">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-1853">Core</span></span>

* <span data-ttu-id="82d30-1854">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="82d30-1854">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="82d30-1855">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1855">January 28, 2019</span></span>

<span data-ttu-id="82d30-1856">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="82d30-1856">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-1857">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-1857">ACR</span></span>
* <span data-ttu-id="82d30-1858">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1858">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-1859">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-1859">ACS</span></span>
* <span data-ttu-id="82d30-1860">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1860">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="82d30-1861">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="82d30-1861">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="82d30-1862">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1862">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="82d30-1863">AMS</span><span class="sxs-lookup"><span data-stu-id="82d30-1863">AMS</span></span>
* <span data-ttu-id="82d30-1864">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1864">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="82d30-1865">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1865">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-1866">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-1866">Appservice</span></span>
* <span data-ttu-id="82d30-1867">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1867">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="82d30-1868">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="82d30-1868">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="82d30-1869">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="82d30-1869">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="82d30-1870">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-1870">Container</span></span>
* <span data-ttu-id="82d30-1871">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1871">Added `container start` command</span></span>
* <span data-ttu-id="82d30-1872">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="82d30-1872">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="82d30-1873">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="82d30-1873">EventGrid</span></span>
* <span data-ttu-id="82d30-1874">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1874">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="82d30-1875">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1875">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="82d30-1876">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="82d30-1876">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="82d30-1877">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="82d30-1877">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="82d30-1878">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="82d30-1878">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82d30-1879">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82d30-1879">HDInsight</span></span>
* <span data-ttu-id="82d30-1880">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1880">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="82d30-1881">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1881">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="82d30-1882">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1882">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="82d30-1883">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="82d30-1883">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="82d30-1884">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1884">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="82d30-1885">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1885">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-1886">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-1886">IoT</span></span>
* <span data-ttu-id="82d30-1887">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="82d30-1887">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="82d30-1888">Kusto</span><span class="sxs-lookup"><span data-stu-id="82d30-1888">Kusto</span></span>
* <span data-ttu-id="82d30-1889">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="82d30-1889">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-1890">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-1890">Monitor</span></span>
* <span data-ttu-id="82d30-1891">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="82d30-1891">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-1892">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-1892">Profile</span></span>
* <span data-ttu-id="82d30-1893">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="82d30-1893">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="82d30-1894">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-1894">Network</span></span>
* <span data-ttu-id="82d30-1895">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1895">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="82d30-1896">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="82d30-1896">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-1897">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-1897">Resource</span></span>
* <span data-ttu-id="82d30-1898">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1898">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="82d30-1899">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1899">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="82d30-1900">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-1900">SQL Virtual Machine</span></span>
* <span data-ttu-id="82d30-1901">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="82d30-1901">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-1902">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-1902">Storage</span></span>
* <span data-ttu-id="82d30-1903">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="82d30-1903">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="82d30-1904">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="82d30-1904">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-1905">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-1905">VM</span></span>
* <span data-ttu-id="82d30-1906">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="82d30-1906">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="82d30-1907">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1907">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="82d30-1908">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1908">January 15, 2019</span></span>

<span data-ttu-id="82d30-1909">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="82d30-1909">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-1910">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-1910">ACR</span></span>
* <span data-ttu-id="82d30-1911">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="82d30-1911">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="82d30-1912">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="82d30-1912">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="82d30-1913">[УСТАРЕЛО] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="82d30-1913">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="82d30-1914">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-1914">ACS</span></span>
* <span data-ttu-id="82d30-1915">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="82d30-1915">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-1916">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-1916">Appservice</span></span>
* <span data-ttu-id="82d30-1917">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="82d30-1917">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="82d30-1918">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="82d30-1918">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="82d30-1919">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="82d30-1919">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="82d30-1920">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1920">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="82d30-1921">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="82d30-1921">Botservice</span></span>
* <span data-ttu-id="82d30-1922">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1922">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="82d30-1923">Configure</span><span class="sxs-lookup"><span data-stu-id="82d30-1923">Configure</span></span>
* <span data-ttu-id="82d30-1924">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1924">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82d30-1925">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-1925">CosmosDB</span></span>
* <span data-ttu-id="82d30-1926">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="82d30-1926">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82d30-1927">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82d30-1927">HDInsight</span></span>
* <span data-ttu-id="82d30-1928">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="82d30-1928">Added commands for managing applications</span></span>
* <span data-ttu-id="82d30-1929">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1929">Added commands for managing script actions</span></span>
* <span data-ttu-id="82d30-1930">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="82d30-1930">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="82d30-1931">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1931">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="82d30-1932">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-1932">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="82d30-1933">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-1933">Network</span></span>
* <span data-ttu-id="82d30-1934">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82d30-1934">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="82d30-1935">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="82d30-1935">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="82d30-1936">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82d30-1936">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="82d30-1937">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1937">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="82d30-1938">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-1938">Role</span></span>
* <span data-ttu-id="82d30-1939">[УСТАРЕЛО] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82d30-1939">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="82d30-1940">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="82d30-1940">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="82d30-1941">Безопасность</span><span class="sxs-lookup"><span data-stu-id="82d30-1941">Security</span></span>
* <span data-ttu-id="82d30-1942">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="82d30-1942">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-1943">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-1943">Storage</span></span>
* <span data-ttu-id="82d30-1944">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="82d30-1944">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="82d30-1945">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1945">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="82d30-1946">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1946">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="82d30-1947">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1947">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="82d30-1948">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1948">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-1949">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-1949">VM</span></span>
* <span data-ttu-id="82d30-1950">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="82d30-1950">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="82d30-1951">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1951">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="82d30-1952">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1952">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="82d30-1953">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="82d30-1953">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="82d30-1954">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-1954">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="82d30-1955">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="82d30-1955">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="82d30-1956">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1956">December 20, 2018</span></span>

<span data-ttu-id="82d30-1957">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="82d30-1957">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="82d30-1958">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-1958">Appservice</span></span>
* <span data-ttu-id="82d30-1959">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="82d30-1959">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="82d30-1960">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="82d30-1960">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="82d30-1961">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="82d30-1961">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="82d30-1962">IoT Central</span><span class="sxs-lookup"><span data-stu-id="82d30-1962">IoTCentral</span></span>
* <span data-ttu-id="82d30-1963">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="82d30-1963">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="82d30-1964">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-1964">Role</span></span>
* <span data-ttu-id="82d30-1965">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1965">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-1966">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-1966">SQL</span></span>
* <span data-ttu-id="82d30-1967">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="82d30-1967">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-1968">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-1968">VM</span></span>
* <span data-ttu-id="82d30-1969">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1969">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="82d30-1970">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1970">December 18, 2018</span></span>

<span data-ttu-id="82d30-1971">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="82d30-1971">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="82d30-1972">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-1972">ACR</span></span>
* <span data-ttu-id="82d30-1973">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="82d30-1973">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="82d30-1974">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="82d30-1974">Condensed the table layout for task list</span></span>
* <span data-ttu-id="82d30-1975">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="82d30-1975">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-1976">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-1976">ACS</span></span>
* <span data-ttu-id="82d30-1977">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1977">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="82d30-1978">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="82d30-1978">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="82d30-1979">[УСТАРЕЛО] Команды `az acs` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="82d30-1979">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="82d30-1980">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-1980">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="82d30-1981">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="82d30-1981">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="82d30-1982">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="82d30-1982">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-1983">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-1983">Appservice</span></span>
* <span data-ttu-id="82d30-1984">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1984">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="82d30-1985">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="82d30-1985">Botservice</span></span>
* <span data-ttu-id="82d30-1986">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1986">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="82d30-1987">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="82d30-1987">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="82d30-1988">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="82d30-1988">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="82d30-1989">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="82d30-1989">Reduced Kudu network calls</span></span>
* <span data-ttu-id="82d30-1990">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="82d30-1990">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="82d30-1991">Потребление</span><span class="sxs-lookup"><span data-stu-id="82d30-1991">Consumption</span></span>
* <span data-ttu-id="82d30-1992">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="82d30-1992">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82d30-1993">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-1993">CosmosDB</span></span>
* <span data-ttu-id="82d30-1994">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="82d30-1994">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="82d30-1995">Maps</span><span class="sxs-lookup"><span data-stu-id="82d30-1995">Maps</span></span>
* <span data-ttu-id="82d30-1996">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="82d30-1996">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="82d30-1997">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-1997">Network</span></span>
* <span data-ttu-id="82d30-1998">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="82d30-1998">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="82d30-1999">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="82d30-1999">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-2000">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-2000">Resource</span></span>
* <span data-ttu-id="82d30-2001">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2001">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="82d30-2002">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2002">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-2003">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-2003">Storage</span></span>
*  <span data-ttu-id="82d30-2004">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="82d30-2004">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2005">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2005">VM</span></span>
* <span data-ttu-id="82d30-2006">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="82d30-2006">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="82d30-2007">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2007">December 4, 2018</span></span>

<span data-ttu-id="82d30-2008">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="82d30-2008">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="82d30-2009">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-2009">Core</span></span>
* <span data-ttu-id="82d30-2010">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="82d30-2010">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="82d30-2011">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="82d30-2011">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-2012">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-2012">Appservice</span></span>
* <span data-ttu-id="82d30-2013">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="82d30-2013">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="82d30-2014">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="82d30-2014">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="82d30-2015">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-2015">Network</span></span>
* <span data-ttu-id="82d30-2016">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="82d30-2016">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="82d30-2017">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-2017">Role</span></span>
* <span data-ttu-id="82d30-2018">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="82d30-2018">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="82d30-2019">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2019">VM</span></span>
* <span data-ttu-id="82d30-2020">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82d30-2020">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="82d30-2021">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="82d30-2021">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="82d30-2022">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="82d30-2022">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="82d30-2023">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="82d30-2023">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="82d30-2024">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2024">November 20, 2018</span></span>

<span data-ttu-id="82d30-2025">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="82d30-2025">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="82d30-2026">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-2026">Core</span></span>
* <span data-ttu-id="82d30-2027">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="82d30-2027">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-2028">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-2028">ACR</span></span>
* <span data-ttu-id="82d30-2029">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="82d30-2029">Added context token to task step</span></span>
* <span data-ttu-id="82d30-2030">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="82d30-2030">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="82d30-2031">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2031">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-2032">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-2032">Appservice</span></span>
* <span data-ttu-id="82d30-2033">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="82d30-2033">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="82d30-2034">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-2034">Updated the default `node_version`.</span></span> <span data-ttu-id="82d30-2035">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="82d30-2035">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="82d30-2036">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="82d30-2036">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="82d30-2037">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="82d30-2037">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="82d30-2038">IotCentral</span><span class="sxs-lookup"><span data-stu-id="82d30-2038">IotCentral</span></span>
* <span data-ttu-id="82d30-2039">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="82d30-2039">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="82d30-2040">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="82d30-2040">KeyVault</span></span>
* <span data-ttu-id="82d30-2041">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="82d30-2041">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="82d30-2042">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-2042">Network</span></span>
* <span data-ttu-id="82d30-2043">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2043">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="82d30-2044">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2044">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="82d30-2045">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="82d30-2045">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="82d30-2046">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2046">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="82d30-2047">Rdbms</span><span class="sxs-lookup"><span data-stu-id="82d30-2047">Rdbms</span></span>
* <span data-ttu-id="82d30-2048">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="82d30-2048">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="82d30-2049">RBAC:</span><span class="sxs-lookup"><span data-stu-id="82d30-2049">Rbac</span></span>
* <span data-ttu-id="82d30-2050">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2050">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="82d30-2051">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="82d30-2051">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="82d30-2052">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-2052">Storage</span></span>
* <span data-ttu-id="82d30-2053">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="82d30-2053">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="82d30-2054">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2054">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="82d30-2055">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="82d30-2055">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="82d30-2056">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2056">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2057">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2057">VM</span></span>
* <span data-ttu-id="82d30-2058">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="82d30-2058">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="82d30-2059">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2059">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="82d30-2060">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2060">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="82d30-2061">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="82d30-2061">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="82d30-2062">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2062">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="82d30-2063">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2063">Added `snapshot wait` command</span></span>
* <span data-ttu-id="82d30-2064">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2064">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="82d30-2065">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2065">November 6, 2018</span></span>

<span data-ttu-id="82d30-2066">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="82d30-2066">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="82d30-2067">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-2067">Core</span></span>
* <span data-ttu-id="82d30-2068">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="82d30-2068">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-2069">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-2069">ACR</span></span>
* <span data-ttu-id="82d30-2070">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="82d30-2070">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="82d30-2071">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="82d30-2071">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-2072">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-2072">ACS</span></span>
* <span data-ttu-id="82d30-2073">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-2073">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="82d30-2074">Помощник</span><span class="sxs-lookup"><span data-stu-id="82d30-2074">Advisor</span></span>
* <span data-ttu-id="82d30-2075">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="82d30-2075">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="82d30-2076">AMS</span><span class="sxs-lookup"><span data-stu-id="82d30-2076">AMS</span></span>
* <span data-ttu-id="82d30-2077">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="82d30-2077">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="82d30-2078">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="82d30-2078">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="82d30-2079">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2079">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="82d30-2080">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="82d30-2080">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="82d30-2081">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2081">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="82d30-2082">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2082">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="82d30-2083">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2083">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="82d30-2084">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2084">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="82d30-2085">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2085">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="82d30-2086">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2086">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="82d30-2087">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2087">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="82d30-2088">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2088">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="82d30-2089">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="82d30-2089">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="82d30-2090">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="82d30-2090">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="82d30-2091">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2091">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="82d30-2092">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="82d30-2092">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="82d30-2093">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="82d30-2093">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-2094">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-2094">AppService</span></span>
* <span data-ttu-id="82d30-2095">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="82d30-2095">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="82d30-2096">Configure</span><span class="sxs-lookup"><span data-stu-id="82d30-2096">Configure</span></span>
* <span data-ttu-id="82d30-2097">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="82d30-2097">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="82d30-2098">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-2098">Container</span></span>
* <span data-ttu-id="82d30-2099">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="82d30-2099">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="82d30-2100">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="82d30-2100">EventHub</span></span>
* <span data-ttu-id="82d30-2101">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2101">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="82d30-2102">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="82d30-2102">Interactive</span></span>
* <span data-ttu-id="82d30-2103">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="82d30-2103">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-2104">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-2104">Monitor</span></span>
* <span data-ttu-id="82d30-2105">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2105">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="82d30-2106">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-2106">Network</span></span>
* <span data-ttu-id="82d30-2107">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2107">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="82d30-2108">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="82d30-2108">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="82d30-2109">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2109">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="82d30-2110">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-2110">Profile</span></span>
* <span data-ttu-id="82d30-2111">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2111">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="82d30-2112">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="82d30-2112">RDBMS</span></span>
* <span data-ttu-id="82d30-2113">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="82d30-2113">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-2114">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-2114">Resource</span></span>
* <span data-ttu-id="82d30-2115">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2115">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="82d30-2116">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-2116">Role</span></span>
* <span data-ttu-id="82d30-2117">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="82d30-2117">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="82d30-2118">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="82d30-2118">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="82d30-2119">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="82d30-2119">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-2120">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-2120">Storage</span></span>
* <span data-ttu-id="82d30-2121">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2121">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2122">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2122">VM</span></span>
* <span data-ttu-id="82d30-2123">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="82d30-2123">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="82d30-2124">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="82d30-2124">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="82d30-2125">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="82d30-2125">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="82d30-2126">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="82d30-2126">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="82d30-2127">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="82d30-2127">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="82d30-2128">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2128">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="82d30-2129">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2129">October 23, 2018</span></span>

<span data-ttu-id="82d30-2130">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="82d30-2130">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="82d30-2131">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-2131">Core</span></span>
* <span data-ttu-id="82d30-2132">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2132">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="82d30-2133">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2133">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-2134">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-2134">ACR</span></span>
* <span data-ttu-id="82d30-2135">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="82d30-2135">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="82d30-2136">CDN</span><span class="sxs-lookup"><span data-stu-id="82d30-2136">CDN</span></span>
* <span data-ttu-id="82d30-2137">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-2137">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="82d30-2138">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="82d30-2138">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="82d30-2139">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-2139">Container</span></span>
* <span data-ttu-id="82d30-2140">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="82d30-2140">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="82d30-2141">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="82d30-2141">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="82d30-2142">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2142">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="82d30-2143">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="82d30-2143">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="82d30-2144">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="82d30-2144">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="82d30-2145">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="82d30-2145">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="82d30-2146">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2146">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82d30-2147">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-2147">CosmosDB</span></span>
* <span data-ttu-id="82d30-2148">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2148">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="82d30-2149">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="82d30-2149">Interactive</span></span>
* <span data-ttu-id="82d30-2150">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="82d30-2150">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="82d30-2151">IoT Central</span><span class="sxs-lookup"><span data-stu-id="82d30-2151">IoT Central</span></span>
* <span data-ttu-id="82d30-2152">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="82d30-2152">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="82d30-2153">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="82d30-2153">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-2154">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-2154">Monitor</span></span>
* <span data-ttu-id="82d30-2155">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="82d30-2155">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="82d30-2156">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="82d30-2156">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="82d30-2157">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="82d30-2157">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="82d30-2158">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="82d30-2158">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="82d30-2159">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2159">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="82d30-2160">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="82d30-2160">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="82d30-2161">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="82d30-2161">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="82d30-2162">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="82d30-2162">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="82d30-2163">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="82d30-2163">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="82d30-2164">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2164">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="82d30-2165">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-2165">Network</span></span>
* <span data-ttu-id="82d30-2166">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="82d30-2166">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="82d30-2167">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="82d30-2167">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="82d30-2168">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="82d30-2168">ServiceBus</span></span>
* <span data-ttu-id="82d30-2169">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="82d30-2169">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-2170">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-2170">SQL</span></span>
* <span data-ttu-id="82d30-2171">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="82d30-2171">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-2172">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-2172">Storage</span></span>
* <span data-ttu-id="82d30-2173">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="82d30-2173">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="82d30-2174">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="82d30-2174">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2175">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2175">VM</span></span>
* <span data-ttu-id="82d30-2176">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="82d30-2176">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="82d30-2177">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="82d30-2177">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="82d30-2178">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="82d30-2178">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="82d30-2179">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2179">October 16, 2018</span></span>

<span data-ttu-id="82d30-2180">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="82d30-2180">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2181">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2181">VM</span></span>
* <span data-ttu-id="82d30-2182">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="82d30-2182">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="82d30-2183">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2183">October 9, 2018</span></span>

<span data-ttu-id="82d30-2184">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="82d30-2184">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="82d30-2185">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-2185">Core</span></span>
* <span data-ttu-id="82d30-2186">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="82d30-2186">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-2187">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-2187">ACR</span></span>
* <span data-ttu-id="82d30-2188">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="82d30-2188">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-2189">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-2189">ACS</span></span>
* <span data-ttu-id="82d30-2190">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="82d30-2190">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="82d30-2191">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="82d30-2191">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="82d30-2192">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2192">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="82d30-2193">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="82d30-2193">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="82d30-2194">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-2194">Container</span></span>
* <span data-ttu-id="82d30-2195">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="82d30-2195">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="82d30-2196">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="82d30-2196">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="82d30-2197">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="82d30-2197">Event Hub</span></span>
* <span data-ttu-id="82d30-2198">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2198">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="82d30-2199">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="82d30-2199">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="82d30-2200">Модули</span><span class="sxs-lookup"><span data-stu-id="82d30-2200">Extensions</span></span>
* <span data-ttu-id="82d30-2201">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="82d30-2201">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="82d30-2202">HDInsight</span><span class="sxs-lookup"><span data-stu-id="82d30-2202">HDInsight</span></span>
* <span data-ttu-id="82d30-2203">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="82d30-2203">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-2204">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-2204">IoT</span></span>
* <span data-ttu-id="82d30-2205">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="82d30-2205">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="82d30-2206">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="82d30-2206">KeyVault</span></span>
* <span data-ttu-id="82d30-2207">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="82d30-2207">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="82d30-2208">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-2208">Network</span></span>
* <span data-ttu-id="82d30-2209">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-2209">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="82d30-2210">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="82d30-2210">See #6052</span></span>
* <span data-ttu-id="82d30-2211">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2211">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="82d30-2212">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="82d30-2212">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="82d30-2213">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2213">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="82d30-2214">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2214">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="82d30-2215">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2215">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="82d30-2216">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2216">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="82d30-2217">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-2217">Role</span></span>
* <span data-ttu-id="82d30-2218">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2218">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="82d30-2219">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2219">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="82d30-2220">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="82d30-2220">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="82d30-2221">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="82d30-2221">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="82d30-2222">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="82d30-2222">Service Bus</span></span>
* <span data-ttu-id="82d30-2223">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="82d30-2223">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2224">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2224">VM</span></span>
* <span data-ttu-id="82d30-2225">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2225">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="82d30-2226">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="82d30-2226">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="82d30-2227">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2227">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="82d30-2228">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2228">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="82d30-2229">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="82d30-2229">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="82d30-2230">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="82d30-2230">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="82d30-2231">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2231">September 21, 2018</span></span>

<span data-ttu-id="82d30-2232">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="82d30-2232">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-2233">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-2233">ACR</span></span>
* <span data-ttu-id="82d30-2234">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="82d30-2234">Added ACR Task commands</span></span>
* <span data-ttu-id="82d30-2235">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="82d30-2235">Added quick run command</span></span>
* <span data-ttu-id="82d30-2236">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="82d30-2236">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="82d30-2237">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="82d30-2237">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="82d30-2238">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="82d30-2238">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="82d30-2239">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="82d30-2239">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-2240">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-2240">ACS</span></span>
* <span data-ttu-id="82d30-2241">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="82d30-2241">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="82d30-2242">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="82d30-2242">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-2243">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-2243">AppService</span></span>

* <span data-ttu-id="82d30-2244">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="82d30-2244">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="82d30-2245">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="82d30-2245">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="82d30-2246">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="82d30-2246">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="82d30-2247">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="82d30-2247">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="82d30-2248">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-2248">Batch</span></span>
* <span data-ttu-id="82d30-2249">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="82d30-2249">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="82d30-2250">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2250">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="82d30-2251">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2251">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="82d30-2252">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="82d30-2252">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="82d30-2253">Batch AI</span><span class="sxs-lookup"><span data-stu-id="82d30-2253">Batch AI</span></span> 
* <span data-ttu-id="82d30-2254">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2254">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="82d30-2255">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="82d30-2255">Cognitive Services</span></span>
* <span data-ttu-id="82d30-2256">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2256">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="82d30-2257">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2257">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="82d30-2258">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2258">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="82d30-2259">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2259">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="82d30-2260">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="82d30-2260">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="82d30-2261">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2261">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="82d30-2262">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-2262">Container</span></span>
* <span data-ttu-id="82d30-2263">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="82d30-2263">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="82d30-2264">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="82d30-2264">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="82d30-2265">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="82d30-2265">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="82d30-2266">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="82d30-2266">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="82d30-2267">Data Lake</span><span class="sxs-lookup"><span data-stu-id="82d30-2267">Datalake</span></span>
* <span data-ttu-id="82d30-2268">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="82d30-2268">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="82d30-2269">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="82d30-2269">Interactive Shell</span></span>
* <span data-ttu-id="82d30-2270">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="82d30-2270">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="82d30-2271">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2271">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-2272">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-2272">IoT</span></span>
* <span data-ttu-id="82d30-2273">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="82d30-2273">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="82d30-2274">Key Vault</span><span class="sxs-lookup"><span data-stu-id="82d30-2274">Key Vault</span></span>
* <span data-ttu-id="82d30-2275">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="82d30-2275">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="82d30-2276">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-2276">Network</span></span>
* <span data-ttu-id="82d30-2277">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2277">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="82d30-2278">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="82d30-2278">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="82d30-2279">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="82d30-2279">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="82d30-2280">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2280">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="82d30-2281">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2281">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="82d30-2282">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2282">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="82d30-2283">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="82d30-2283">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="82d30-2284">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2284">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="82d30-2285">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2285">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="82d30-2286">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2286">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="82d30-2287">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2287">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="82d30-2288">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2288">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="82d30-2289">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2289">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="82d30-2290">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="82d30-2290">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="82d30-2291">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2291">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="82d30-2292">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="82d30-2292">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="82d30-2293">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="82d30-2293">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="82d30-2294">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="82d30-2294">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="82d30-2295">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="82d30-2295">RDBMS</span></span>
* <span data-ttu-id="82d30-2296">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="82d30-2296">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="82d30-2297">резервирование.</span><span class="sxs-lookup"><span data-stu-id="82d30-2297">Reservation</span></span>
* <span data-ttu-id="82d30-2298">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2298">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="82d30-2299">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="82d30-2299">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="82d30-2300">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="82d30-2300">Manage App</span></span>
* <span data-ttu-id="82d30-2301">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="82d30-2301">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="82d30-2302">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="82d30-2302">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="82d30-2303">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-2303">Role</span></span>
* <span data-ttu-id="82d30-2304">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="82d30-2304">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="82d30-2305">SignalR</span><span class="sxs-lookup"><span data-stu-id="82d30-2305">SignalR</span></span>
* <span data-ttu-id="82d30-2306">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="82d30-2306">First release</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-2307">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-2307">Storage</span></span>
* <span data-ttu-id="82d30-2308">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="82d30-2308">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="82d30-2309">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="82d30-2309">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2310">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2310">VM</span></span>
* <span data-ttu-id="82d30-2311">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="82d30-2311">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="82d30-2312">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2312">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="82d30-2313">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2313">August 28, 2018</span></span>

<span data-ttu-id="82d30-2314">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="82d30-2314">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="82d30-2315">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-2315">Core</span></span>

* <span data-ttu-id="82d30-2316">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="82d30-2316">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="82d30-2317">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="82d30-2317">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-2318">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-2318">ACR</span></span>

* <span data-ttu-id="82d30-2319">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="82d30-2319">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="82d30-2320">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2320">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-2321">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-2321">ACS</span></span>

* <span data-ttu-id="82d30-2322">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2322">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="82d30-2323">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="82d30-2323">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-2324">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-2324">AppService</span></span>

* <span data-ttu-id="82d30-2325">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="82d30-2325">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="82d30-2326">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="82d30-2326">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="82d30-2327">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="82d30-2327">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="82d30-2328">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="82d30-2328">Backup</span></span>

* <span data-ttu-id="82d30-2329">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="82d30-2329">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="82d30-2330">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="82d30-2330">Bot Service</span></span>

* <span data-ttu-id="82d30-2331">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="82d30-2331">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="82d30-2332">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="82d30-2332">Cognitive Services</span></span>

* <span data-ttu-id="82d30-2333">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="82d30-2333">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-2334">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-2334">IoT</span></span>

* <span data-ttu-id="82d30-2335">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="82d30-2335">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-2336">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-2336">Monitor</span></span>

* <span data-ttu-id="82d30-2337">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="82d30-2337">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="82d30-2338">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="82d30-2338">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="82d30-2339">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-2339">Network</span></span>

* <span data-ttu-id="82d30-2340">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="82d30-2340">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-2341">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-2341">Resource</span></span>

* <span data-ttu-id="82d30-2342">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="82d30-2342">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-2343">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-2343">Storage</span></span>

* <span data-ttu-id="82d30-2344">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="82d30-2344">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2345">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2345">VM</span></span>

* <span data-ttu-id="82d30-2346">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="82d30-2346">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="82d30-2347">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2347">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="82d30-2348">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2348">Auguest 14, 2018</span></span>

<span data-ttu-id="82d30-2349">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="82d30-2349">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="82d30-2350">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-2350">Core</span></span>

* <span data-ttu-id="82d30-2351">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2351">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="82d30-2352">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="82d30-2352">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="82d30-2353">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="82d30-2353">Telemetry</span></span>

* <span data-ttu-id="82d30-2354">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="82d30-2354">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-2355">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-2355">ACR</span></span>

* <span data-ttu-id="82d30-2356">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2356">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="82d30-2357">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2357">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-2358">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-2358">ACS</span></span>

* <span data-ttu-id="82d30-2359">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="82d30-2359">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="82d30-2360">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="82d30-2360">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="82d30-2361">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="82d30-2361">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="82d30-2362">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="82d30-2362">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="82d30-2363">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="82d30-2363">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="82d30-2364">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-2364">AppService</span></span>

* <span data-ttu-id="82d30-2365">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2365">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="82d30-2366">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="82d30-2366">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="82d30-2367">Batch AI</span><span class="sxs-lookup"><span data-stu-id="82d30-2367">BatchAI</span></span>

* <span data-ttu-id="82d30-2368">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="82d30-2368">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="82d30-2369">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-2369">Container</span></span>

* <span data-ttu-id="82d30-2370">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="82d30-2370">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="82d30-2371">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-2371">IoT</span></span>

* <span data-ttu-id="82d30-2372">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="82d30-2372">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="82d30-2373">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2373">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="82d30-2374">IoT Central</span><span class="sxs-lookup"><span data-stu-id="82d30-2374">Iot Central</span></span>

* <span data-ttu-id="82d30-2375">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="82d30-2375">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="82d30-2376">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="82d30-2376">KeyVault</span></span>


* <span data-ttu-id="82d30-2377">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="82d30-2377">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="82d30-2378">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="82d30-2378">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="82d30-2379">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="82d30-2379">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="82d30-2380">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="82d30-2380">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="82d30-2381">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="82d30-2381">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="82d30-2382">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="82d30-2382">Relay</span></span>

* <span data-ttu-id="82d30-2383">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="82d30-2383">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-2384">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-2384">Sql</span></span>

* <span data-ttu-id="82d30-2385">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2385">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-2386">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-2386">Storage</span></span>

* <span data-ttu-id="82d30-2387">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="82d30-2387">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="82d30-2388">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="82d30-2388">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="82d30-2389">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="82d30-2389">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="82d30-2390">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="82d30-2390">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="82d30-2391">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="82d30-2391">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2392">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2392">VM</span></span>

* <span data-ttu-id="82d30-2393">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="82d30-2393">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="82d30-2394">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2394">July 31, 2018</span></span>

<span data-ttu-id="82d30-2395">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="82d30-2395">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-2396">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-2396">ACR</span></span>

* <span data-ttu-id="82d30-2397">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2397">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="82d30-2398">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2398">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-2399">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-2399">ACS</span></span>

* <span data-ttu-id="82d30-2400">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="82d30-2400">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="82d30-2401">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-2401">Batch</span></span>

* <span data-ttu-id="82d30-2402">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="82d30-2402">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="82d30-2403">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-2403">Container</span></span>

* <span data-ttu-id="82d30-2404">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="82d30-2404">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="82d30-2405">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-2405">Network</span></span>

* <span data-ttu-id="82d30-2406">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="82d30-2406">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="82d30-2407">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-2407">Resource</span></span>

* <span data-ttu-id="82d30-2408">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="82d30-2408">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="82d30-2409">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="82d30-2409">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="82d30-2410">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-2410">Role</span></span>

* <span data-ttu-id="82d30-2411">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="82d30-2411">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="82d30-2412">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="82d30-2412">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="82d30-2413">Поиск</span><span class="sxs-lookup"><span data-stu-id="82d30-2413">Search</span></span>

* <span data-ttu-id="82d30-2414">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="82d30-2414">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="82d30-2415">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="82d30-2415">Service Bus</span></span>

* <span data-ttu-id="82d30-2416">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="82d30-2416">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="82d30-2417">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="82d30-2417">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="82d30-2418">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="82d30-2418">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="82d30-2419">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2419">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-2420">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-2420">Storage</span></span>

* <span data-ttu-id="82d30-2421">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="82d30-2421">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="82d30-2422">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="82d30-2422">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2423">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2423">VM</span></span>

* <span data-ttu-id="82d30-2424">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="82d30-2424">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="82d30-2425">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2425">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="82d30-2426">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="82d30-2426">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="82d30-2427">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="82d30-2427">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="82d30-2428">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2428">July 18, 2018</span></span>

<span data-ttu-id="82d30-2429">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="82d30-2429">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="82d30-2430">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-2430">Core</span></span>

* <span data-ttu-id="82d30-2431">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="82d30-2431">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="82d30-2432">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="82d30-2432">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="82d30-2433">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="82d30-2433">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-2434">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-2434">ACR</span></span>

* <span data-ttu-id="82d30-2435">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="82d30-2435">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="82d30-2436">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2436">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="82d30-2437">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="82d30-2437">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="82d30-2438">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="82d30-2438">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-2439">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-2439">ACS</span></span>

* <span data-ttu-id="82d30-2440">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="82d30-2440">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-2441">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-2441">AppService</span></span>

* <span data-ttu-id="82d30-2442">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="82d30-2442">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="82d30-2443">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-2443">Batch</span></span>

* <span data-ttu-id="82d30-2444">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="82d30-2444">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="82d30-2445">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="82d30-2445">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="82d30-2446">Batch AI</span><span class="sxs-lookup"><span data-stu-id="82d30-2446">Batch AI</span></span>

* <span data-ttu-id="82d30-2447">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2447">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="82d30-2448">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-2448">Container</span></span>

* <span data-ttu-id="82d30-2449">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="82d30-2449">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="82d30-2450">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="82d30-2450">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="82d30-2451">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-2451">Network</span></span>

* <span data-ttu-id="82d30-2452">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2452">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="82d30-2453">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2453">Added `network nic wait`</span></span>
* <span data-ttu-id="82d30-2454">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="82d30-2454">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="82d30-2455">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="82d30-2455">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="82d30-2456">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-2456">Resource</span></span>

* <span data-ttu-id="82d30-2457">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2457">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="82d30-2458">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2458">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="82d30-2459">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2459">Added `deployment wait` command</span></span>
* <span data-ttu-id="82d30-2460">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="82d30-2460">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-2461">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-2461">SQL</span></span>

* <span data-ttu-id="82d30-2462">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2462">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="82d30-2463">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2463">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="82d30-2464">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2464">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-2465">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-2465">Storage</span></span>

* <span data-ttu-id="82d30-2466">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2466">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2467">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2467">VM</span></span>

* <span data-ttu-id="82d30-2468">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-2468">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="82d30-2469">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2469">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="82d30-2470">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2470">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="82d30-2471">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2471">July 3, 2018</span></span>

<span data-ttu-id="82d30-2472">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="82d30-2472">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="82d30-2473">AKS</span><span class="sxs-lookup"><span data-stu-id="82d30-2473">AKS</span></span>

* <span data-ttu-id="82d30-2474">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="82d30-2474">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="82d30-2475">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2475">July 3, 2018</span></span>

<span data-ttu-id="82d30-2476">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="82d30-2476">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="82d30-2477">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-2477">Core</span></span>

* <span data-ttu-id="82d30-2478">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="82d30-2478">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-2479">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-2479">ACR</span></span>

* <span data-ttu-id="82d30-2480">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="82d30-2480">Added polling build status</span></span>
* <span data-ttu-id="82d30-2481">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="82d30-2481">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="82d30-2482">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2482">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-2483">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-2483">ACS</span></span>

* <span data-ttu-id="82d30-2484">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-2484">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="82d30-2485">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-2485">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="82d30-2486">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2486">Updated options for `aks browse` command.</span></span> <span data-ttu-id="82d30-2487">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2487">Added `--listen-port` support</span></span>
* <span data-ttu-id="82d30-2488">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2488">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="82d30-2489">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="82d30-2489">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="82d30-2490">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2490">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-2491">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-2491">AppService</span></span>

* <span data-ttu-id="82d30-2492">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2492">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="82d30-2493">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="82d30-2493">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="82d30-2494">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="82d30-2494">Backup</span></span>

* <span data-ttu-id="82d30-2495">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="82d30-2495">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="82d30-2496">Batch AI</span><span class="sxs-lookup"><span data-stu-id="82d30-2496">BatchAI</span></span>

* <span data-ttu-id="82d30-2497">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2497">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="82d30-2498">Cloud</span><span class="sxs-lookup"><span data-stu-id="82d30-2498">Cloud</span></span>

* <span data-ttu-id="82d30-2499">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2499">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="82d30-2500">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-2500">Container</span></span>

* <span data-ttu-id="82d30-2501">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="82d30-2501">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="82d30-2502">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2502">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="82d30-2503">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="82d30-2503">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="82d30-2504">Расширение</span><span class="sxs-lookup"><span data-stu-id="82d30-2504">Extension</span></span>

* <span data-ttu-id="82d30-2505">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="82d30-2505">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="82d30-2506">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-2506">Network</span></span>

* <span data-ttu-id="82d30-2507">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="82d30-2507">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="82d30-2508">Rdbms</span><span class="sxs-lookup"><span data-stu-id="82d30-2508">Rdbms</span></span>

* <span data-ttu-id="82d30-2509">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2509">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-2510">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-2510">Resource</span></span>

* <span data-ttu-id="82d30-2511">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2511">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2512">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2512">VM</span></span>

* <span data-ttu-id="82d30-2513">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="82d30-2513">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="82d30-2514">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2514">June 25, 2018</span></span>

<span data-ttu-id="82d30-2515">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="82d30-2515">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="82d30-2516">CLI</span><span class="sxs-lookup"><span data-stu-id="82d30-2516">CLI</span></span>

* <span data-ttu-id="82d30-2517">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="82d30-2517">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="82d30-2518">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2518">June 19, 2018</span></span>

<span data-ttu-id="82d30-2519">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="82d30-2519">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="82d30-2520">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-2520">Core</span></span>

* <span data-ttu-id="82d30-2521">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="82d30-2521">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-2522">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-2522">ACR</span></span>

* <span data-ttu-id="82d30-2523">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2523">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="82d30-2524">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="82d30-2524">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-2525">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-2525">ACS</span></span>

* <span data-ttu-id="82d30-2526">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2526">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="82d30-2527">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2527">Added `--update` support</span></span>
* <span data-ttu-id="82d30-2528">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2528">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="82d30-2529">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2529">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="82d30-2530">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2530">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="82d30-2531">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2531">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="82d30-2532">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2532">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="82d30-2533">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2533">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-2534">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-2534">AppService</span></span>

* <span data-ttu-id="82d30-2535">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="82d30-2535">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="82d30-2536">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2536">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="82d30-2537">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-2537">Batch</span></span>

* <span data-ttu-id="82d30-2538">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2538">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="82d30-2539">Batch AI</span><span class="sxs-lookup"><span data-stu-id="82d30-2539">Batch AI</span></span>

* <span data-ttu-id="82d30-2540">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="82d30-2540">Added support for workspaces.</span></span> <span data-ttu-id="82d30-2541">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2541">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="82d30-2542">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2542">Added support for experiments.</span></span> <span data-ttu-id="82d30-2543">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="82d30-2543">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="82d30-2544">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="82d30-2544">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="82d30-2545">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2545">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="82d30-2546">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2546">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="82d30-2547">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2547">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="82d30-2548">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="82d30-2548">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="82d30-2549">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2549">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="82d30-2550">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2550">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="82d30-2551">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2551">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="82d30-2552">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2552">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="82d30-2553">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2553">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="82d30-2554">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2554">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="82d30-2555">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="82d30-2555">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="82d30-2556">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2556">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="82d30-2557">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="82d30-2557">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="82d30-2558">[`--config`, `-c`] переименовано в [`--config-file`, `-f`].</span><span class="sxs-lookup"><span data-stu-id="82d30-2558">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="82d30-2559">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="82d30-2559">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="82d30-2560">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="82d30-2560">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="82d30-2561">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="82d30-2561">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="82d30-2562">Maps</span><span class="sxs-lookup"><span data-stu-id="82d30-2562">Maps</span></span>

* <span data-ttu-id="82d30-2563">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2563">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="82d30-2564">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-2564">Network</span></span>

* <span data-ttu-id="82d30-2565">Добавлена поддержка `https` в `network lb probe create` ([№ 6571](https://github.com/Azure/azure-cli/issues/6571)).</span><span class="sxs-lookup"><span data-stu-id="82d30-2565">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="82d30-2566">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="82d30-2566">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="82d30-2567">#6502</span><span class="sxs-lookup"><span data-stu-id="82d30-2567">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="82d30-2568">Резервирование</span><span class="sxs-lookup"><span data-stu-id="82d30-2568">Reservations</span></span>

* <span data-ttu-id="82d30-2569">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2569">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="82d30-2570">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2570">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="82d30-2571">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2571">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="82d30-2572">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2572">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="82d30-2573">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2573">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="82d30-2574">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2574">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="82d30-2575">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-2575">Role</span></span>

* <span data-ttu-id="82d30-2576">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="82d30-2576">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-2577">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-2577">SQL</span></span>

* <span data-ttu-id="82d30-2578">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="82d30-2578">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-2579">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-2579">Storage</span></span>

* <span data-ttu-id="82d30-2580">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="82d30-2580">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2581">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2581">VM</span></span>

* <span data-ttu-id="82d30-2582">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2582">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="82d30-2583">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2583">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="82d30-2584">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="82d30-2584">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="82d30-2585">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2585">June 13, 2018</span></span>

<span data-ttu-id="82d30-2586">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="82d30-2586">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="82d30-2587">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-2587">Core</span></span>

* <span data-ttu-id="82d30-2588">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="82d30-2588">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="82d30-2589">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2589">June 13, 2018</span></span>

<span data-ttu-id="82d30-2590">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="82d30-2590">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="82d30-2591">AKS</span><span class="sxs-lookup"><span data-stu-id="82d30-2591">AKS</span></span>

* <span data-ttu-id="82d30-2592">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="82d30-2592">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="82d30-2593">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="82d30-2593">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="82d30-2594">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="82d30-2594">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="82d30-2595">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="82d30-2595">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="82d30-2596">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="82d30-2596">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-2597">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-2597">AppService</span></span>

* <span data-ttu-id="82d30-2598">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="82d30-2598">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="82d30-2599">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2599">June 5, 2018</span></span>

<span data-ttu-id="82d30-2600">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="82d30-2600">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="82d30-2601">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="82d30-2601">Interactive</span></span>

* <span data-ttu-id="82d30-2602">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="82d30-2602">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="82d30-2603">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2603">June 5, 2018</span></span>

<span data-ttu-id="82d30-2604">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="82d30-2604">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="82d30-2605">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-2605">Core</span></span>

* <span data-ttu-id="82d30-2606">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="82d30-2606">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="82d30-2607">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="82d30-2607">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-2608">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-2608">ACR</span></span>

* <span data-ttu-id="82d30-2609">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="82d30-2609">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="82d30-2610">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2610">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="82d30-2611">AKS</span><span class="sxs-lookup"><span data-stu-id="82d30-2611">AKS</span></span>

* <span data-ttu-id="82d30-2612">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="82d30-2612">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="82d30-2613">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-2613">Batch</span></span>

* <span data-ttu-id="82d30-2614">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="82d30-2614">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-2615">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-2615">IOT</span></span>

* <span data-ttu-id="82d30-2616">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="82d30-2616">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="82d30-2617">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-2617">Network</span></span>

* <span data-ttu-id="82d30-2618">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2618">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="82d30-2619">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="82d30-2619">Policy Insights</span></span>

* <span data-ttu-id="82d30-2620">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="82d30-2620">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="82d30-2621">ARM</span><span class="sxs-lookup"><span data-stu-id="82d30-2621">ARM</span></span>

* <span data-ttu-id="82d30-2622">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2622">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-2623">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-2623">SQL</span></span>

* <span data-ttu-id="82d30-2624">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="82d30-2624">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="82d30-2625">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="82d30-2625">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="82d30-2626">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-2626">Storage</span></span>

* <span data-ttu-id="82d30-2627">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2627">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2628">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2628">VM</span></span>

* <span data-ttu-id="82d30-2629">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2629">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="82d30-2630">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2630">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="82d30-2631">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2631">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="82d30-2632">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2632">May 22, 2018</span></span>

<span data-ttu-id="82d30-2633">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="82d30-2633">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="82d30-2634">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-2634">Core</span></span>

* <span data-ttu-id="82d30-2635">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2635">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-2636">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-2636">ACS</span></span>

* <span data-ttu-id="82d30-2637">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2637">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="82d30-2638">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="82d30-2638">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-2639">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-2639">AppService</span></span>

* <span data-ttu-id="82d30-2640">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="82d30-2640">Improved generic update commands</span></span>
* <span data-ttu-id="82d30-2641">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2641">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="82d30-2642">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-2642">Container</span></span>

* <span data-ttu-id="82d30-2643">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="82d30-2643">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="82d30-2644">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="82d30-2644">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="82d30-2645">Расширение</span><span class="sxs-lookup"><span data-stu-id="82d30-2645">Extension</span></span>

* <span data-ttu-id="82d30-2646">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="82d30-2646">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="82d30-2647">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="82d30-2647">Interactive</span></span>

* <span data-ttu-id="82d30-2648">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="82d30-2648">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="82d30-2649">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="82d30-2649">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="82d30-2650">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="82d30-2650">KeyVault</span></span>

* <span data-ttu-id="82d30-2651">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="82d30-2651">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="82d30-2652">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-2652">Network</span></span>

* <span data-ttu-id="82d30-2653">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="82d30-2653">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="82d30-2654">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="82d30-2654">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-2655">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-2655">SQL</span></span>

* <span data-ttu-id="82d30-2656">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="82d30-2656">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="82d30-2657">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2657">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="82d30-2658">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2658">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="82d30-2659">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="82d30-2659">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="82d30-2660">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="82d30-2660">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="82d30-2661">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2661">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="82d30-2662">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2662">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="82d30-2663">`edition`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2663">`edition`.</span></span> <span data-ttu-id="82d30-2664">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2664">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="82d30-2665">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2665">`elasticPoolName`.</span></span> <span data-ttu-id="82d30-2666">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2666">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="82d30-2667">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="82d30-2667">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="82d30-2668">`edition`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2668">`edition`.</span></span> <span data-ttu-id="82d30-2669">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2669">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="82d30-2670">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2670">`dtu`.</span></span> <span data-ttu-id="82d30-2671">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2671">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="82d30-2672">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2672">`databaseDtuMin`.</span></span> <span data-ttu-id="82d30-2673">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2673">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="82d30-2674">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2674">`databaseDtuMax`.</span></span> <span data-ttu-id="82d30-2675">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2675">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="82d30-2676">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2676">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="82d30-2677">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2677">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-2678">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-2678">Storage</span></span>

* <span data-ttu-id="82d30-2679">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2679">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="82d30-2680">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2680">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2681">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2681">VM</span></span>

* <span data-ttu-id="82d30-2682">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2682">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="82d30-2683">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2683">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="82d30-2684">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2684">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="82d30-2685">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="82d30-2685">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="82d30-2686">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2686">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="82d30-2687">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2687">May 7, 2018</span></span>

<span data-ttu-id="82d30-2688">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="82d30-2688">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="82d30-2689">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-2689">Core</span></span>

* <span data-ttu-id="82d30-2690">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="82d30-2690">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="82d30-2691">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2691">Added limited support for positional arguments</span></span>
* <span data-ttu-id="82d30-2692">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2692">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="82d30-2693">#5591</span><span class="sxs-lookup"><span data-stu-id="82d30-2693">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="82d30-2694">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2694">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="82d30-2695">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="82d30-2695">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="82d30-2696">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="82d30-2696">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="82d30-2697">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2697">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="82d30-2698">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="82d30-2698">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-2699">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-2699">ACR</span></span>

* <span data-ttu-id="82d30-2700">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="82d30-2700">Added ACR Build commands</span></span>
* <span data-ttu-id="82d30-2701">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="82d30-2701">Improved resource not found error messages</span></span>
* <span data-ttu-id="82d30-2702">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="82d30-2702">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="82d30-2703">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="82d30-2703">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="82d30-2704">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="82d30-2704">Improved repository commands error messages</span></span>
* <span data-ttu-id="82d30-2705">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="82d30-2705">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-2706">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-2706">ACS</span></span>

* <span data-ttu-id="82d30-2707">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="82d30-2707">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="82d30-2708">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="82d30-2708">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="82d30-2709">AMS</span><span class="sxs-lookup"><span data-stu-id="82d30-2709">AMS</span></span>

* <span data-ttu-id="82d30-2710">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="82d30-2710">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-2711">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-2711">Appservice</span></span>

* <span data-ttu-id="82d30-2712">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="82d30-2712">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="82d30-2713">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2713">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="82d30-2714">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="82d30-2714">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="82d30-2715">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="82d30-2715">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="82d30-2716">Batch AI</span><span class="sxs-lookup"><span data-stu-id="82d30-2716">Batch AI</span></span>

* <span data-ttu-id="82d30-2717">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="82d30-2717">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="82d30-2718">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="82d30-2718">Cognitive Services</span></span>

* <span data-ttu-id="82d30-2719">Исправлена опечатка в примере для `cognitiveservices account create` ([№ 5603](https://github.com/Azure/azure-cli/issues/5603)).</span><span class="sxs-lookup"><span data-stu-id="82d30-2719">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="82d30-2720">Потребление</span><span class="sxs-lookup"><span data-stu-id="82d30-2720">Consumption</span></span>

* <span data-ttu-id="82d30-2721">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="82d30-2721">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="82d30-2722">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-2722">Container</span></span>

* <span data-ttu-id="82d30-2723">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="82d30-2723">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="82d30-2724">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-2724">Cosmos DB</span></span>

* <span data-ttu-id="82d30-2725">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-2725">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="82d30-2726">DMS</span><span class="sxs-lookup"><span data-stu-id="82d30-2726">DMS</span></span>

* <span data-ttu-id="82d30-2727">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="82d30-2727">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="82d30-2728">Расширение</span><span class="sxs-lookup"><span data-stu-id="82d30-2728">Extension</span></span>

* <span data-ttu-id="82d30-2729">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="82d30-2729">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="82d30-2730">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="82d30-2730">Interactive</span></span>

* <span data-ttu-id="82d30-2731">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="82d30-2731">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="82d30-2732">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="82d30-2732">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="82d30-2733">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="82d30-2733">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="82d30-2734">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="82d30-2734">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="82d30-2735">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="82d30-2735">Lab</span></span>

* <span data-ttu-id="82d30-2736">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="82d30-2736">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="82d30-2737">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-2737">Network</span></span>

* <span data-ttu-id="82d30-2738">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="82d30-2738">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="82d30-2739">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-2739">Profile</span></span>

* <span data-ttu-id="82d30-2740">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2740">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="82d30-2741">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="82d30-2741">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="82d30-2742">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2742">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="82d30-2743">Redis</span><span class="sxs-lookup"><span data-stu-id="82d30-2743">Redis</span></span>

* <span data-ttu-id="82d30-2744">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2744">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="82d30-2745">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="82d30-2745">Deprecated `redis list-all`.</span></span> <span data-ttu-id="82d30-2746">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2746">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="82d30-2747">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2747">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="82d30-2748">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="82d30-2748">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="82d30-2749">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-2749">Role</span></span>

* <span data-ttu-id="82d30-2750">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="82d30-2750">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-2751">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-2751">Storage</span></span>

* <span data-ttu-id="82d30-2752">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="82d30-2752">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="82d30-2753">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="82d30-2753">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="82d30-2754">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="82d30-2754">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="82d30-2755">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="82d30-2755">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="82d30-2756">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="82d30-2756">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2757">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2757">VM</span></span>

* <span data-ttu-id="82d30-2758">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="82d30-2758">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="82d30-2759">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="82d30-2759">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="82d30-2760">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="82d30-2760">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="82d30-2761">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2761">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="82d30-2762">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="82d30-2762">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="82d30-2763">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="82d30-2763">Added write accelerator support</span></span>
* <span data-ttu-id="82d30-2764">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2764">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="82d30-2765">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="82d30-2765">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="82d30-2766">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="82d30-2766">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="82d30-2767">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2767">April 10, 2018</span></span>

<span data-ttu-id="82d30-2768">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="82d30-2768">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-2769">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-2769">ACR</span></span>

* <span data-ttu-id="82d30-2770">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="82d30-2770">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-2771">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-2771">ACS</span></span>

* <span data-ttu-id="82d30-2772">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="82d30-2772">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-2773">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-2773">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="82d30-2775">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="82d30-2775">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="82d30-2776">Batch AI</span><span class="sxs-lookup"><span data-stu-id="82d30-2776">BatchAI</span></span>

* <span data-ttu-id="82d30-2777">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="82d30-2777">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="82d30-2778">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="82d30-2778">Job level mounting</span></span>
  - <span data-ttu-id="82d30-2779">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2779">Environment variables with secret values</span></span>
  - <span data-ttu-id="82d30-2780">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="82d30-2780">Performance counters settings</span></span>
  - <span data-ttu-id="82d30-2781">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="82d30-2781">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="82d30-2782">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2782">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="82d30-2783">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="82d30-2783">Usage and limits reporting</span></span>
  - <span data-ttu-id="82d30-2784">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2784">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="82d30-2785">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2785">Support for custom images</span></span>
  - <span data-ttu-id="82d30-2786">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="82d30-2786">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="82d30-2787">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="82d30-2787">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="82d30-2788">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2788">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="82d30-2789">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="82d30-2789">National clouds are supported</span></span>
* <span data-ttu-id="82d30-2790">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="82d30-2790">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="82d30-2791">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="82d30-2791">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="82d30-2792">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="82d30-2792">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="82d30-2793">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="82d30-2793">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="82d30-2794">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="82d30-2794">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="82d30-2795">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="82d30-2795">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="82d30-2796">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2796">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="82d30-2797">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="82d30-2797">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="82d30-2798">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="82d30-2798">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="82d30-2799">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2799">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="82d30-2800">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="82d30-2800">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="82d30-2801">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2801">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="82d30-2802">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2802">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="82d30-2803">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="82d30-2803">Billing</span></span>

* <span data-ttu-id="82d30-2804">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="82d30-2804">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="82d30-2805">Потребление</span><span class="sxs-lookup"><span data-stu-id="82d30-2805">Consumption</span></span>

* <span data-ttu-id="82d30-2806">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2806">Added `marketplace` commands</span></span>
* <span data-ttu-id="82d30-2807">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2807">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="82d30-2808">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2808">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="82d30-2809">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2809">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="82d30-2810">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2810">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="82d30-2811">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2811">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="82d30-2812">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-2812">Container</span></span>

* <span data-ttu-id="82d30-2813">Добавлены параметры подключения тома репозитория Git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2813">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="82d30-2814">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="82d30-2814">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="82d30-2815">Расширение</span><span class="sxs-lookup"><span data-stu-id="82d30-2815">Extension</span></span>

* <span data-ttu-id="82d30-2816">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="82d30-2816">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="82d30-2817">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="82d30-2817">Interactive</span></span>

* <span data-ttu-id="82d30-2818">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="82d30-2818">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="82d30-2819">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="82d30-2819">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="82d30-2820">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2820">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="82d30-2821">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-2821">Network</span></span>

* <span data-ttu-id="82d30-2822">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2822">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="82d30-2823">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2823">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="82d30-2824">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="82d30-2824">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="82d30-2825">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="82d30-2825">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="82d30-2826">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="82d30-2826">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="82d30-2827">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2827">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="82d30-2828">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2828">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="82d30-2829">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="82d30-2829">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-2830">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-2830">Profile</span></span>

* <span data-ttu-id="82d30-2831">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2831">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="82d30-2832">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi` & `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2832">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="82d30-2833">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="82d30-2833">RDBMS</span></span>

* <span data-ttu-id="82d30-2834">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2834">Added `georestore` command</span></span>
* <span data-ttu-id="82d30-2835">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="82d30-2835">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-2836">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-2836">Resource</span></span>

* <span data-ttu-id="82d30-2837">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2837">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="82d30-2838">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2838">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-2839">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-2839">SQL</span></span>

* <span data-ttu-id="82d30-2840">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2840">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-2841">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-2841">Storage</span></span>

* <span data-ttu-id="82d30-2842">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="82d30-2842">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2843">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2843">VM</span></span>

* <span data-ttu-id="82d30-2844">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="82d30-2844">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="82d30-2845">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="82d30-2845">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="82d30-2847">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2847">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="82d30-2848">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="82d30-2848">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="82d30-2849">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="82d30-2849">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="82d30-2850">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="82d30-2850">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="82d30-2851">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2851">March 27, 2018</span></span>

<span data-ttu-id="82d30-2852">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="82d30-2852">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="82d30-2853">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-2853">Core</span></span>

* <span data-ttu-id="82d30-2854">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="82d30-2854">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-2855">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-2855">ACS</span></span>

* <span data-ttu-id="82d30-2856">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="82d30-2856">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-2857">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-2857">Appservice</span></span>

* <span data-ttu-id="82d30-2858">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2858">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="82d30-2859">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2859">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="82d30-2860">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="82d30-2860">Backup</span></span>

* <span data-ttu-id="82d30-2861">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2861">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="82d30-2862">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="82d30-2862">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="82d30-2863">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="82d30-2863">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="82d30-2864">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2864">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="82d30-2865">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-2865">Container</span></span>

* <span data-ttu-id="82d30-2866">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2866">Added `container exec` command.</span></span> <span data-ttu-id="82d30-2867">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="82d30-2867">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="82d30-2868">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="82d30-2868">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="82d30-2869">Расширение</span><span class="sxs-lookup"><span data-stu-id="82d30-2869">Extension</span></span>

* <span data-ttu-id="82d30-2870">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="82d30-2870">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="82d30-2871">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2871">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="82d30-2872">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-2872">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="82d30-2873">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="82d30-2873">Interactive</span></span>

* <span data-ttu-id="82d30-2874">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="82d30-2874">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="82d30-2875">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2875">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="82d30-2876">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="82d30-2876">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="82d30-2877">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="82d30-2877">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="82d30-2878">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="82d30-2878">Lab</span></span>

* <span data-ttu-id="82d30-2879">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2879">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-2880">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-2880">Monitor</span></span>

* <span data-ttu-id="82d30-2881">Добавлена поддержка аргументов `--top`, `--orderby` и `--namespace` для `metrics list` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="82d30-2881">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="82d30-2882">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="82d30-2882">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="82d30-2883">Добавлена поддержка `--namespace` для `metrics list-definitions` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="82d30-2883">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="82d30-2884">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-2884">Network</span></span>

* <span data-ttu-id="82d30-2885">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="82d30-2885">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-2886">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-2886">Profile</span></span>

* <span data-ttu-id="82d30-2887">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2887">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="82d30-2888">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="82d30-2888">RDBMS</span></span>

* <span data-ttu-id="82d30-2889">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="82d30-2889">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-2890">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-2890">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="82d30-2892">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-2892">Role</span></span>

* <span data-ttu-id="82d30-2893">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2893">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="82d30-2894">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="82d30-2894">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="82d30-2895">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="82d30-2895">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="82d30-2896">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2896">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="82d30-2897">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2897">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-2898">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-2898">Storage</span></span>

* <span data-ttu-id="82d30-2899">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="82d30-2899">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="82d30-2900">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="82d30-2900">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2901">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2901">VM</span></span>

* <span data-ttu-id="82d30-2902">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="82d30-2902">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="82d30-2903">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2903">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="82d30-2904">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="82d30-2904">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="82d30-2905">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="82d30-2905">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="82d30-2906">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2906">March 13, 2018</span></span>

<span data-ttu-id="82d30-2907">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="82d30-2907">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-2908">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-2908">ACR</span></span>

* <span data-ttu-id="82d30-2909">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2909">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="82d30-2910">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="82d30-2910">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="82d30-2911">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="82d30-2911">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-2912">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-2912">ACS</span></span>

* <span data-ttu-id="82d30-2913">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="82d30-2913">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="82d30-2914">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="82d30-2914">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="82d30-2915">Помощник</span><span class="sxs-lookup"><span data-stu-id="82d30-2915">Advisor</span></span>

* <span data-ttu-id="82d30-2916">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2916">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="82d30-2917">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2917">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="82d30-2918">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2918">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="82d30-2919">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2919">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="82d30-2920">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2920">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-2921">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-2921">Appservice</span></span>

* <span data-ttu-id="82d30-2922">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="82d30-2922">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="82d30-2923">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2923">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="82d30-2924">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="82d30-2924">Eventhubs</span></span>

* <span data-ttu-id="82d30-2925">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="82d30-2925">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="82d30-2926">Расширение</span><span class="sxs-lookup"><span data-stu-id="82d30-2926">Extension</span></span>

* <span data-ttu-id="82d30-2927">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="82d30-2927">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="82d30-2928">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="82d30-2928">Interactive</span></span>

* <span data-ttu-id="82d30-2929">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="82d30-2929">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="82d30-2930">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="82d30-2930">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="82d30-2931">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="82d30-2931">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="82d30-2932">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="82d30-2932">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-2933">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-2933">Monitor</span></span>

* <span data-ttu-id="82d30-2934">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="82d30-2934">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="82d30-2935">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2935">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="82d30-2936">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2936">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="82d30-2937">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2937">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="82d30-2938">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-2938">Network</span></span>

* <span data-ttu-id="82d30-2939">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2939">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="82d30-2940">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="82d30-2940">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="82d30-2941">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2941">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="82d30-2942">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2942">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-2943">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-2943">Profile</span></span>

* <span data-ttu-id="82d30-2944">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="82d30-2944">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="82d30-2945">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2945">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="82d30-2946">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="82d30-2946">RDBMS</span></span>

* <span data-ttu-id="82d30-2947">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="82d30-2947">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="82d30-2948">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="82d30-2948">Service Bus</span></span>

* <span data-ttu-id="82d30-2949">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="82d30-2949">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-2950">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-2950">Storage</span></span>

* <span data-ttu-id="82d30-2951">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="82d30-2951">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="82d30-2952">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="82d30-2952">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2953">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2953">VM</span></span>

* <span data-ttu-id="82d30-2954">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="82d30-2954">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="82d30-2955">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="82d30-2955">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="82d30-2956">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2956">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="82d30-2957">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="82d30-2957">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="82d30-2958">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="82d30-2958">February 27, 2018</span></span>

<span data-ttu-id="82d30-2959">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="82d30-2959">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="82d30-2960">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-2960">Core</span></span>

* <span data-ttu-id="82d30-2961">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="82d30-2961">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="82d30-2962">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="82d30-2962">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="82d30-2963">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2963">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-2964">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-2964">ACS</span></span>

* <span data-ttu-id="82d30-2965">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-2965">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="82d30-2966">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="82d30-2966">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="82d30-2967">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2967">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="82d30-2968">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2968">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-2969">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-2969">Appservice</span></span>

* <span data-ttu-id="82d30-2970">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="82d30-2970">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="82d30-2971">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="82d30-2971">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="82d30-2972">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="82d30-2972">Cognitive Services</span></span>

* <span data-ttu-id="82d30-2973">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="82d30-2973">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="82d30-2974">Потребление</span><span class="sxs-lookup"><span data-stu-id="82d30-2974">Consumption</span></span>

* <span data-ttu-id="82d30-2975">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="82d30-2975">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="82d30-2976">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="82d30-2976">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="82d30-2977">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-2977">Container</span></span>

* <span data-ttu-id="82d30-2978">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="82d30-2978">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="82d30-2979">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-2979">Network</span></span>

* <span data-ttu-id="82d30-2980">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2980">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-2981">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-2981">Resource</span></span>

* <span data-ttu-id="82d30-2982">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="82d30-2982">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="82d30-2983">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-2983">Role</span></span>

* <span data-ttu-id="82d30-2984">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="82d30-2984">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-2985">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-2985">SQL</span></span>

* <span data-ttu-id="82d30-2986">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="82d30-2986">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-2987">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-2987">Storage</span></span>

* <span data-ttu-id="82d30-2988">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2988">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-2989">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-2989">VM</span></span>

* <span data-ttu-id="82d30-2990">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="82d30-2990">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="82d30-2991">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-2991">February 13, 2018</span></span>

<span data-ttu-id="82d30-2992">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="82d30-2992">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="82d30-2993">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-2993">Core</span></span>

* <span data-ttu-id="82d30-2994">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="82d30-2994">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-2995">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-2995">ACS</span></span>

* <span data-ttu-id="82d30-2996">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="82d30-2996">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="82d30-2997">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-2997">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="82d30-2998">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="82d30-2998">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="82d30-2999">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="82d30-2999">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="82d30-3000">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="82d30-3000">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="82d30-3001">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3001">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="82d30-3002">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="82d30-3002">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="82d30-3003">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3003">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-3004">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-3004">Appservice</span></span>

* <span data-ttu-id="82d30-3005">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="82d30-3005">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="82d30-3006">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3006">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="82d30-3007">CDN</span><span class="sxs-lookup"><span data-stu-id="82d30-3007">CDN</span></span>

* <span data-ttu-id="82d30-3008">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3008">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="82d30-3009">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-3009">Container</span></span>

* <span data-ttu-id="82d30-3010">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="82d30-3010">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="82d30-3011">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="82d30-3011">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82d30-3012">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-3012">CosmosDB</span></span>

* <span data-ttu-id="82d30-3013">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="82d30-3013">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="82d30-3014">Расширение</span><span class="sxs-lookup"><span data-stu-id="82d30-3014">Extension</span></span>

* <span data-ttu-id="82d30-3015">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3015">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="82d30-3016">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3016">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="82d30-3017">Отзывы</span><span class="sxs-lookup"><span data-stu-id="82d30-3017">Feedback</span></span>

* <span data-ttu-id="82d30-3018">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="82d30-3018">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="82d30-3019">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="82d30-3019">Interactive</span></span>

* <span data-ttu-id="82d30-3020">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="82d30-3020">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="82d30-3021">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="82d30-3021">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-3022">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-3022">IoT</span></span>

* <span data-ttu-id="82d30-3023">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="82d30-3023">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="82d30-3024">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="82d30-3024">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="82d30-3025">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3025">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="82d30-3026">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="82d30-3026">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-3027">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-3027">Monitor</span></span>

* <span data-ttu-id="82d30-3028">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3028">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="82d30-3029">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-3029">Network</span></span>

* <span data-ttu-id="82d30-3030">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="82d30-3030">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="82d30-3031">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-3031">Profile</span></span>

* <span data-ttu-id="82d30-3032">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="82d30-3032">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-3033">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-3033">Resource</span></span>

* <span data-ttu-id="82d30-3034">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3034">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="82d30-3035">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-3035">Role</span></span>

* <span data-ttu-id="82d30-3036">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="82d30-3036">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-3037">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-3037">SQL</span></span>

* <span data-ttu-id="82d30-3038">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3038">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="82d30-3039">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3039">Added `sql db rename`</span></span>
* <span data-ttu-id="82d30-3040">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="82d30-3040">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-3041">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-3041">Storage</span></span>

* <span data-ttu-id="82d30-3042">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="82d30-3042">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-3043">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-3043">VM</span></span>

* <span data-ttu-id="82d30-3044">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="82d30-3044">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="82d30-3045">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="82d30-3045">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="82d30-3046">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="82d30-3046">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="82d30-3047">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-3047">January 31, 2018</span></span>

<span data-ttu-id="82d30-3048">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="82d30-3048">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="82d30-3049">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-3049">Core</span></span>

* <span data-ttu-id="82d30-3050">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="82d30-3050">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="82d30-3051">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="82d30-3051">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="82d30-3052">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="82d30-3052">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="82d30-3053">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="82d30-3053">Use `--verbose` to see</span></span>
* <span data-ttu-id="82d30-3054">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="82d30-3054">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-3055">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-3055">ACS</span></span>

* <span data-ttu-id="82d30-3056">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3056">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="82d30-3057">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3057">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-3058">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-3058">Appservice</span></span>

* <span data-ttu-id="82d30-3059">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="82d30-3059">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="82d30-3060">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="82d30-3060">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="82d30-3061">CDN</span><span class="sxs-lookup"><span data-stu-id="82d30-3061">CDN</span></span>

* <span data-ttu-id="82d30-3062">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3062">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82d30-3063">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-3063">CosmosDB</span></span>

* <span data-ttu-id="82d30-3064">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="82d30-3064">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="82d30-3065">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="82d30-3065">Interactive</span></span>

* <span data-ttu-id="82d30-3066">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="82d30-3066">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="82d30-3067">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-3067">Network</span></span>

* <span data-ttu-id="82d30-3068">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3068">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="82d30-3069">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-3069">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="82d30-3070">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3070">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="82d30-3071">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3071">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="82d30-3072">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3072">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="82d30-3073">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="82d30-3073">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="82d30-3074">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="82d30-3074">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="82d30-3075">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="82d30-3075">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="82d30-3076">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3076">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="82d30-3077">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3077">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-3078">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-3078">Profile</span></span>

* <span data-ttu-id="82d30-3079">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="82d30-3079">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-3080">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-3080">Resource</span></span>

* <span data-ttu-id="82d30-3081">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="82d30-3081">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-3082">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-3082">Storage</span></span>

* <span data-ttu-id="82d30-3083">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="82d30-3083">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="82d30-3084">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="82d30-3084">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="82d30-3085">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3085">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="82d30-3086">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3086">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="82d30-3087">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="82d30-3087">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-3088">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-3088">VM</span></span>

* <span data-ttu-id="82d30-3089">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="82d30-3089">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="82d30-3090">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="82d30-3090">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="82d30-3091">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="82d30-3091">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="82d30-3092">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3092">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="82d30-3093">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-3093">January 17, 2018</span></span>

<span data-ttu-id="82d30-3094">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="82d30-3094">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-3095">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-3095">ACR</span></span>

* <span data-ttu-id="82d30-3096">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="82d30-3096">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="82d30-3097">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="82d30-3097">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-3098">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-3098">ACS</span></span>

* <span data-ttu-id="82d30-3099">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3099">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="82d30-3100">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="82d30-3100">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-3101">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-3101">Appservice</span></span>

* <span data-ttu-id="82d30-3102">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="82d30-3102">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="82d30-3103">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="82d30-3103">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="82d30-3104">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3104">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="82d30-3105">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="82d30-3105">Backup</span></span>

* <span data-ttu-id="82d30-3106">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="82d30-3106">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="82d30-3107">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="82d30-3107">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="82d30-3108">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="82d30-3108">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="82d30-3109">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="82d30-3109">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="82d30-3110">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="82d30-3110">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="82d30-3111">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-3111">Batch</span></span>

* <span data-ttu-id="82d30-3112">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="82d30-3112">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="82d30-3113">Cloud</span><span class="sxs-lookup"><span data-stu-id="82d30-3113">Cloud</span></span>

* <span data-ttu-id="82d30-3114">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="82d30-3114">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="82d30-3115">Потребление</span><span class="sxs-lookup"><span data-stu-id="82d30-3115">Consumption</span></span>

* <span data-ttu-id="82d30-3116">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3116">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="82d30-3117">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-3117">Event Grid</span></span>

* <span data-ttu-id="82d30-3118">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3118">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="82d30-3119">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3119">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="82d30-3120">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3120">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="82d30-3121">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3121">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="82d30-3122">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3122">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="82d30-3123">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3123">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="82d30-3124">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3124">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="82d30-3125">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="82d30-3125">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="82d30-3126">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="82d30-3126">Interactive</span></span>

* <span data-ttu-id="82d30-3127">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="82d30-3127">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="82d30-3128">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="82d30-3128">Fixed errors on startup</span></span>
* <span data-ttu-id="82d30-3129">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="82d30-3129">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-3130">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-3130">IoT</span></span>

* <span data-ttu-id="82d30-3131">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="82d30-3131">Added support for device provisioning service</span></span>
* <span data-ttu-id="82d30-3132">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="82d30-3132">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="82d30-3133">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="82d30-3133">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-3134">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-3134">Monitor</span></span>

* <span data-ttu-id="82d30-3135">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="82d30-3135">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="82d30-3136">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3136">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="82d30-3137">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="82d30-3137">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="82d30-3138">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-3138">Network</span></span>

* <span data-ttu-id="82d30-3139">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="82d30-3139">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="82d30-3140">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="82d30-3140">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-3141">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-3141">Profile</span></span>

* <span data-ttu-id="82d30-3142">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="82d30-3142">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="82d30-3143">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-3143">Role</span></span>

* <span data-ttu-id="82d30-3144">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="82d30-3144">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="82d30-3145">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="82d30-3145">Service Fabric</span></span>

* <span data-ttu-id="82d30-3146">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="82d30-3146">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="82d30-3147">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="82d30-3147">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-3148">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-3148">VM</span></span>

* <span data-ttu-id="82d30-3149">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3149">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="82d30-3150">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="82d30-3150">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="82d30-3151">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3151">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="82d30-3152">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="82d30-3152">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="82d30-3153">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="82d30-3153">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="82d30-3154">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3154">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="82d30-3155">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3155">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="82d30-3156">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3156">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="82d30-3157">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-3157">December 19, 2017</span></span>

<span data-ttu-id="82d30-3158">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="82d30-3158">Version 2.0.23</span></span>

* <span data-ttu-id="82d30-3159">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="82d30-3159">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="82d30-3160">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-3160">Container</span></span>

* <span data-ttu-id="82d30-3161">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="82d30-3161">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="82d30-3162">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-3162">Network</span></span>

* <span data-ttu-id="82d30-3163">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82d30-3163">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="82d30-3164">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82d30-3164">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-3165">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-3165">Storage</span></span>

* <span data-ttu-id="82d30-3166">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="82d30-3166">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-3167">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-3167">VM</span></span>

* <span data-ttu-id="82d30-3168">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="82d30-3168">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="82d30-3169">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-3169">December 5, 2017</span></span>

<span data-ttu-id="82d30-3170">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="82d30-3170">Version 2.0.22</span></span>

* <span data-ttu-id="82d30-3171">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3171">Removed `az component` commands.</span></span> <span data-ttu-id="82d30-3172">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3172">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="82d30-3173">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-3173">Core</span></span>
* <span data-ttu-id="82d30-3174">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="82d30-3174">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="82d30-3175">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="82d30-3175">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-3176">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-3176">ACS</span></span>

* <span data-ttu-id="82d30-3177">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3177">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="82d30-3178">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3178">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="82d30-3179">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="82d30-3179">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="82d30-3180">Помощник</span><span class="sxs-lookup"><span data-stu-id="82d30-3180">Advisor</span></span>

* <span data-ttu-id="82d30-3181">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="82d30-3181">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-3182">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-3182">Appservice</span></span>

* <span data-ttu-id="82d30-3183">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3183">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="82d30-3184">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="82d30-3184">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="82d30-3185">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3185">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="82d30-3186">Потребление</span><span class="sxs-lookup"><span data-stu-id="82d30-3186">Consumption</span></span>

* <span data-ttu-id="82d30-3187">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="82d30-3187">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="82d30-3188">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-3188">Container</span></span>

* <span data-ttu-id="82d30-3189">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="82d30-3189">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-3190">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-3190">Monitor</span></span>

* <span data-ttu-id="82d30-3191">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="82d30-3191">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-3192">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-3192">Resource</span></span>

* <span data-ttu-id="82d30-3193">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="82d30-3193">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="82d30-3194">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-3194">Role</span></span>

* <span data-ttu-id="82d30-3195">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3195">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="82d30-3196">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="82d30-3196">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="82d30-3197">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3197">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-3198">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-3198">SQL</span></span>

* <span data-ttu-id="82d30-3199">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3199">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="82d30-3200">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3200">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-3201">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-3201">VM</span></span>

* <span data-ttu-id="82d30-3202">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3202">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="82d30-3203">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-3203">November 14, 2017</span></span>

<span data-ttu-id="82d30-3204">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="82d30-3204">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-3205">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-3205">ACR</span></span>

* <span data-ttu-id="82d30-3206">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="82d30-3206">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="82d30-3207">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-3207">ACS</span></span>

* <span data-ttu-id="82d30-3208">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="82d30-3208">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="82d30-3209">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="82d30-3209">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="82d30-3210">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3210">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="82d30-3211">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="82d30-3211">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="82d30-3212">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="82d30-3212">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-3213">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-3213">Appservice</span></span>

* <span data-ttu-id="82d30-3214">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="82d30-3214">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="82d30-3215">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3215">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="82d30-3216">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3216">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="82d30-3217">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3217">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="82d30-3218">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="82d30-3218">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="82d30-3219">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="82d30-3219">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="82d30-3220">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-3220">Batch</span></span>

* <span data-ttu-id="82d30-3221">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3221">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="82d30-3222">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="82d30-3222">Batchai</span></span>

* <span data-ttu-id="82d30-3223">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3223">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="82d30-3224">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3224">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="82d30-3225">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3225">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="82d30-3226">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3226">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="82d30-3227">Cloud</span><span class="sxs-lookup"><span data-stu-id="82d30-3227">Cloud</span></span>

* <span data-ttu-id="82d30-3228">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="82d30-3228">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="82d30-3229">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-3229">Container</span></span>

* <span data-ttu-id="82d30-3230">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="82d30-3230">Added support to open multiple ports</span></span>
* <span data-ttu-id="82d30-3231">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="82d30-3231">Added container group restart policy</span></span>
* <span data-ttu-id="82d30-3232">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="82d30-3232">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="82d30-3233">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="82d30-3233">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="82d30-3234">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="82d30-3234">Data Lake Analytics</span></span>

* <span data-ttu-id="82d30-3235">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="82d30-3235">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="82d30-3236">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="82d30-3236">Data Lake Store</span></span>

* <span data-ttu-id="82d30-3237">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="82d30-3237">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="82d30-3238">Расширение</span><span class="sxs-lookup"><span data-stu-id="82d30-3238">Extension</span></span>

* <span data-ttu-id="82d30-3239">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="82d30-3239">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="82d30-3240">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="82d30-3240">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-3241">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-3241">IoT</span></span>

* <span data-ttu-id="82d30-3242">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="82d30-3242">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-3243">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-3243">Monitor</span></span>

* <span data-ttu-id="82d30-3244">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3244">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="82d30-3245">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-3245">Network</span></span>

* <span data-ttu-id="82d30-3246">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="82d30-3246">Added support for CAA DNS records</span></span>
* <span data-ttu-id="82d30-3247">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3247">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="82d30-3248">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="82d30-3248">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="82d30-3249">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3249">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="82d30-3250">Резервирование</span><span class="sxs-lookup"><span data-stu-id="82d30-3250">Reservations</span></span>

* <span data-ttu-id="82d30-3251">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="82d30-3251">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-3252">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-3252">Resource</span></span>

* <span data-ttu-id="82d30-3253">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3253">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-3254">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-3254">SQL</span></span>

* <span data-ttu-id="82d30-3255">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3255">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-3256">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-3256">Storage</span></span>

* <span data-ttu-id="82d30-3257">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-3257">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="82d30-3258">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="82d30-3258">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="82d30-3259">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3259">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="82d30-3260">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3260">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="82d30-3261">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3261">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="82d30-3262">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3262">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="82d30-3263">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3263">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-3264">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-3264">VM</span></span>

* <span data-ttu-id="82d30-3265">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3265">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="82d30-3266">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="82d30-3266">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="82d30-3267">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3267">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="82d30-3268">Переименование `vm format-secret` в `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="82d30-3268">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="82d30-3269">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="82d30-3269">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="82d30-3270">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-3270">October 24, 2017</span></span>

<span data-ttu-id="82d30-3271">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="82d30-3271">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="82d30-3272">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-3272">Core</span></span>

* <span data-ttu-id="82d30-3273">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="82d30-3273">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-3274">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-3274">ACR</span></span>

* <span data-ttu-id="82d30-3275">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="82d30-3275">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="82d30-3276">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="82d30-3276">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="82d30-3277">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="82d30-3277">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-3278">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-3278">ACS</span></span>

* <span data-ttu-id="82d30-3279">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="82d30-3279">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="82d30-3280">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="82d30-3280">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-3281">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-3281">Appservice</span></span>

* <span data-ttu-id="82d30-3282">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="82d30-3282">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="82d30-3283">Компонент</span><span class="sxs-lookup"><span data-stu-id="82d30-3283">Component</span></span>

* <span data-ttu-id="82d30-3284">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="82d30-3284">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-3285">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-3285">Monitor</span></span>

* <span data-ttu-id="82d30-3286">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3286">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-3287">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-3287">Resource</span></span>

* <span data-ttu-id="82d30-3288">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="82d30-3288">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="82d30-3289">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="82d30-3289">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-3290">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-3290">VM</span></span>

* <span data-ttu-id="82d30-3291">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="82d30-3291">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="82d30-3292">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-3292">October 9, 2017</span></span>

<span data-ttu-id="82d30-3293">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="82d30-3293">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="82d30-3294">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-3294">Core</span></span>

* <span data-ttu-id="82d30-3295">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="82d30-3295">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-3296">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-3296">Appservice</span></span>

* <span data-ttu-id="82d30-3297">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3297">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="82d30-3298">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-3298">Batch</span></span>

* <span data-ttu-id="82d30-3299">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="82d30-3299">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="82d30-3300">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="82d30-3300">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="82d30-3301">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="82d30-3301">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="82d30-3302">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="82d30-3302">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="82d30-3303">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="82d30-3303">Batchai</span></span>

* <span data-ttu-id="82d30-3304">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="82d30-3304">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="82d30-3305">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="82d30-3305">Keyvault</span></span>

* <span data-ttu-id="82d30-3306">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="82d30-3306">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="82d30-3307">(#4448)</span><span class="sxs-lookup"><span data-stu-id="82d30-3307">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="82d30-3308">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-3308">Network</span></span>

* <span data-ttu-id="82d30-3309">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="82d30-3309">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="82d30-3310">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="82d30-3310">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-3311">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-3311">Resource</span></span>

* <span data-ttu-id="82d30-3312">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3312">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="82d30-3313">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="82d30-3313">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="82d30-3314">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="82d30-3314">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="82d30-3315">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="82d30-3315">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-3316">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-3316">Sql</span></span>

* <span data-ttu-id="82d30-3317">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="82d30-3317">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="82d30-3318">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="82d30-3318">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="82d30-3319">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="82d30-3319">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-3320">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-3320">Storage</span></span>

* <span data-ttu-id="82d30-3321">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="82d30-3321">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-3322">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="82d30-3322">Vm</span></span>

* <span data-ttu-id="82d30-3323">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="82d30-3323">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="82d30-3324">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3324">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="82d30-3325">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3325">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="82d30-3326">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3326">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="82d30-3327">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="82d30-3327">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="82d30-3328">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-3328">September 22, 2017</span></span>

<span data-ttu-id="82d30-3329">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="82d30-3329">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-3330">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-3330">Resource</span></span>

* <span data-ttu-id="82d30-3331">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="82d30-3331">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="82d30-3332">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="82d30-3332">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="82d30-3333">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="82d30-3333">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="82d30-3334">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3334">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="82d30-3335">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-3335">Network</span></span>

* <span data-ttu-id="82d30-3336">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="82d30-3336">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="82d30-3337">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="82d30-3337">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="82d30-3338">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="82d30-3338">Added `asg` application security group commands</span></span>
* <span data-ttu-id="82d30-3339">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="82d30-3339">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="82d30-3340">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82d30-3340">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="82d30-3341">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82d30-3341">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="82d30-3342">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3342">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-3343">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-3343">Storage</span></span>

* <span data-ttu-id="82d30-3344">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="82d30-3344">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="82d30-3345">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="82d30-3345">Eventgrid</span></span>

* <span data-ttu-id="82d30-3346">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="82d30-3346">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-3347">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-3347">SQL</span></span>

* <span data-ttu-id="82d30-3348">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="82d30-3348">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="82d30-3349">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="82d30-3349">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="82d30-3350">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="82d30-3350">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="82d30-3351">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="82d30-3351">Keyvault</span></span>

* <span data-ttu-id="82d30-3352">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="82d30-3352">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-3353">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-3353">VM</span></span>

* <span data-ttu-id="82d30-3354">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="82d30-3354">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="82d30-3355">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="82d30-3355">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="82d30-3356">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="82d30-3356">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="82d30-3357">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="82d30-3357">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="82d30-3358">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="82d30-3358">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="82d30-3359">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="82d30-3359">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-3360">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-3360">ACS</span></span>

* <span data-ttu-id="82d30-3361">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="82d30-3361">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-3362">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-3362">Appservice</span></span>

* <span data-ttu-id="82d30-3363">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="82d30-3363">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="82d30-3364">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="82d30-3364">Backup</span></span>

* <span data-ttu-id="82d30-3365">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="82d30-3365">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="82d30-3366">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-3366">September 11, 2017</span></span>

<span data-ttu-id="82d30-3367">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="82d30-3367">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="82d30-3368">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-3368">Core</span></span>

* <span data-ttu-id="82d30-3369">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="82d30-3369">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="82d30-3370">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="82d30-3370">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-3371">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-3371">Acs</span></span>

* <span data-ttu-id="82d30-3372">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3372">Added `acs list-locations` command</span></span>
* <span data-ttu-id="82d30-3373">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-3373">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-3374">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-3374">Appservice</span></span>

* <span data-ttu-id="82d30-3375">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="82d30-3375">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="82d30-3376">CDN</span><span class="sxs-lookup"><span data-stu-id="82d30-3376">CDN</span></span>

* <span data-ttu-id="82d30-3377">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3377">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="82d30-3378">Расширение</span><span class="sxs-lookup"><span data-stu-id="82d30-3378">Extension</span></span>

* <span data-ttu-id="82d30-3379">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="82d30-3379">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="82d30-3380">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="82d30-3380">Keyvault</span></span>

* <span data-ttu-id="82d30-3381">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3381">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="82d30-3382">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-3382">Network</span></span>

* <span data-ttu-id="82d30-3383">Переименование `vnet list-private-access-services` в `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="82d30-3383">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="82d30-3384">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3384">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="82d30-3385">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3385">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="82d30-3386">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3386">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="82d30-3387">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3387">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-3388">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-3388">Resource</span></span>

* <span data-ttu-id="82d30-3389">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3389">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="82d30-3390">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3390">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="82d30-3391">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="82d30-3391">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="82d30-3392">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="82d30-3392">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-3393">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-3393">SQL</span></span>

* <span data-ttu-id="82d30-3394">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3394">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-3395">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-3395">VM</span></span>

* <span data-ttu-id="82d30-3396">Исправлено: Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="82d30-3396">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="82d30-3397">Исправлено: Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="82d30-3397">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="82d30-3398">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3398">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="82d30-3399">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="82d30-3399">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="82d30-3400">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="82d30-3400">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="82d30-3401">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-3401">August 31, 2017</span></span>

<span data-ttu-id="82d30-3402">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="82d30-3402">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="82d30-3403">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="82d30-3403">Keyvault</span></span>

* <span data-ttu-id="82d30-3404">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3404">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="82d30-3405">Sf</span><span class="sxs-lookup"><span data-stu-id="82d30-3405">Sf</span></span>

* <span data-ttu-id="82d30-3406">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="82d30-3406">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-3407">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-3407">Storage</span></span>

* <span data-ttu-id="82d30-3408">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="82d30-3408">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="82d30-3409">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="82d30-3409">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="82d30-3410">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-3410">August 28, 2017</span></span>

<span data-ttu-id="82d30-3411">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="82d30-3411">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="82d30-3412">CLI</span><span class="sxs-lookup"><span data-stu-id="82d30-3412">CLI</span></span>

* <span data-ttu-id="82d30-3413">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="82d30-3413">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-3414">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-3414">ACS</span></span>

* <span data-ttu-id="82d30-3415">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="82d30-3415">Corrected preview regions</span></span>
* <span data-ttu-id="82d30-3416">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3416">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="82d30-3417">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="82d30-3417">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-3418">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-3418">Appservice</span></span>

* <span data-ttu-id="82d30-3419">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3419">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="82d30-3420">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3420">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="82d30-3421">Предоставлен параметр `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3421">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="82d30-3422">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="82d30-3422">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="82d30-3423">Исправлено: Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="82d30-3423">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-3424">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-3424">IoT</span></span>

* <span data-ttu-id="82d30-3425">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="82d30-3425">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="82d30-3426">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-3426">Network</span></span>

* <span data-ttu-id="82d30-3427">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3427">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="82d30-3428">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3428">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="82d30-3429">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3429">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="82d30-3430">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3430">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="82d30-3431">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3431">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-3432">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-3432">Profile</span></span>

* <span data-ttu-id="82d30-3433">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="82d30-3433">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="82d30-3434">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="82d30-3434">Service Fabric</span></span>

* <span data-ttu-id="82d30-3435">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="82d30-3435">Preview release</span></span>
* <span data-ttu-id="82d30-3436">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="82d30-3436">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="82d30-3437">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="82d30-3437">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="82d30-3438">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3438">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-3439">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-3439">Storage</span></span>

* <span data-ttu-id="82d30-3440">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="82d30-3440">Enabled setting blob tier</span></span>
* <span data-ttu-id="82d30-3441">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="82d30-3441">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="82d30-3442">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3442">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="82d30-3443">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="82d30-3443">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="82d30-3444">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3444">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="82d30-3445">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3445">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-3446">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-3446">VM</span></span>

* <span data-ttu-id="82d30-3447">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3447">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="82d30-3448">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3448">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="82d30-3449">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="82d30-3449">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="82d30-3450">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="82d30-3450">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="82d30-3451">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="82d30-3451">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="82d30-3452">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3452">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="82d30-3453">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-3453">August 15, 2017</span></span>

<span data-ttu-id="82d30-3454">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="82d30-3454">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-3455">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-3455">ACS</span></span>

* <span data-ttu-id="82d30-3456">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="82d30-3456">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-3457">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-3457">Appservice</span></span>

* <span data-ttu-id="82d30-3458">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="82d30-3458">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="82d30-3459">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-3459">Event Grid</span></span>

* <span data-ttu-id="82d30-3460">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="82d30-3460">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="82d30-3461">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-3461">August 11, 2017</span></span>

<span data-ttu-id="82d30-3462">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="82d30-3462">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-3463">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-3463">ACS</span></span>

* <span data-ttu-id="82d30-3464">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="82d30-3464">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="82d30-3465">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-3465">Batch</span></span>

* <span data-ttu-id="82d30-3466">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="82d30-3466">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="82d30-3467">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="82d30-3467">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="82d30-3468">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="82d30-3468">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="82d30-3469">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="82d30-3469">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="82d30-3470">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="82d30-3470">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="82d30-3471">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="82d30-3471">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="82d30-3472">Компонент</span><span class="sxs-lookup"><span data-stu-id="82d30-3472">Component</span></span>

* <span data-ttu-id="82d30-3473">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="82d30-3473">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="82d30-3474">Контейнер</span><span class="sxs-lookup"><span data-stu-id="82d30-3474">Container</span></span>

* <span data-ttu-id="82d30-3475">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="82d30-3475">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="82d30-3476">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="82d30-3476">Data Lake Store</span></span>

* <span data-ttu-id="82d30-3477">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="82d30-3477">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="82d30-3478">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-3478">Event Grid</span></span>

* <span data-ttu-id="82d30-3479">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="82d30-3479">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="82d30-3480">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-3480">Network</span></span>

* <span data-ttu-id="82d30-3481">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="82d30-3481">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="82d30-3482">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3482">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="82d30-3483">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3483">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="82d30-3484">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3484">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-3485">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-3485">Profile</span></span>

* <span data-ttu-id="82d30-3486">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="82d30-3486">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-3487">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-3487">Storage</span></span>

* <span data-ttu-id="82d30-3488">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="82d30-3488">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-3489">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-3489">VM</span></span>

* <span data-ttu-id="82d30-3490">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="82d30-3490">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="82d30-3491">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3491">Exposed `list-skus` command</span></span>
* <span data-ttu-id="82d30-3492">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="82d30-3492">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="82d30-3493">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="82d30-3493">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="82d30-3494">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="82d30-3494">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="82d30-3495">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-3495">July 28, 2017</span></span>

<span data-ttu-id="82d30-3496">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="82d30-3496">Version 2.0.12</span></span>

* <span data-ttu-id="82d30-3497">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="82d30-3497">Added container commands</span></span>
* <span data-ttu-id="82d30-3498">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="82d30-3498">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="82d30-3499">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-3499">Core</span></span>

* <span data-ttu-id="82d30-3500">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="82d30-3500">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="82d30-3501">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="82d30-3501">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="82d30-3502">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="82d30-3502">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="82d30-3503">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="82d30-3503">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="82d30-3504">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="82d30-3504">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="82d30-3505">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="82d30-3505">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="82d30-3506">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="82d30-3506">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="82d30-3507">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="82d30-3507">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="82d30-3508">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="82d30-3508">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="82d30-3509">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="82d30-3509">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="82d30-3510">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="82d30-3510">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="82d30-3511">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="82d30-3511">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="82d30-3512">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="82d30-3512">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="82d30-3513">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="82d30-3513">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="82d30-3514">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="82d30-3514">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="82d30-3515">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="82d30-3515">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="82d30-3516">ACR</span><span class="sxs-lookup"><span data-stu-id="82d30-3516">ACR</span></span>

* <span data-ttu-id="82d30-3517">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="82d30-3517">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="82d30-3518">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="82d30-3518">Support SKU update for managed registries</span></span>
* <span data-ttu-id="82d30-3519">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="82d30-3519">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="82d30-3520">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="82d30-3520">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="82d30-3521">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="82d30-3521">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="82d30-3522">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="82d30-3522">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-3523">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-3523">ACS</span></span>

* <span data-ttu-id="82d30-3524">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="82d30-3524">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-3525">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="82d30-3525">Appservice</span></span>

* <span data-ttu-id="82d30-3526">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="82d30-3526">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="82d30-3527">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="82d30-3527">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="82d30-3528">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3528">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="82d30-3529">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="82d30-3529">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="82d30-3530">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="82d30-3530">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="82d30-3531">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="82d30-3531">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="82d30-3532">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="82d30-3532">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="82d30-3533">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="82d30-3533">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="82d30-3534">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="82d30-3534">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="82d30-3535">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3535">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="82d30-3536">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="82d30-3536">Batch</span></span>

* <span data-ttu-id="82d30-3537">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="82d30-3537">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="82d30-3538">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3538">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="82d30-3539">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3539">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="82d30-3540">CDN</span><span class="sxs-lookup"><span data-stu-id="82d30-3540">CDN</span></span>

* <span data-ttu-id="82d30-3541">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="82d30-3541">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="82d30-3542">Cloud</span><span class="sxs-lookup"><span data-stu-id="82d30-3542">Cloud</span></span>

* <span data-ttu-id="82d30-3543">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="82d30-3543">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="82d30-3544">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="82d30-3544">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="82d30-3545">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="82d30-3545">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="82d30-3546">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="82d30-3546">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="82d30-3547">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3547">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82d30-3548">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-3548">CosmosDB</span></span>

* <span data-ttu-id="82d30-3549">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="82d30-3549">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="82d30-3550">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="82d30-3550">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="82d30-3551">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="82d30-3551">Data Lake Analytics</span></span>

* <span data-ttu-id="82d30-3552">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3552">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="82d30-3553">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3553">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="82d30-3554">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3554">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="82d30-3555">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="82d30-3555">Data Lake Store</span></span>

* <span data-ttu-id="82d30-3556">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3556">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="82d30-3557">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="82d30-3557">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="82d30-3558">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3558">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="82d30-3559">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="82d30-3559">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="82d30-3560">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="82d30-3560">Interactive</span></span>

* <span data-ttu-id="82d30-3561">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="82d30-3561">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="82d30-3562">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="82d30-3562">Increased test coverage</span></span>
* <span data-ttu-id="82d30-3563">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="82d30-3563">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="82d30-3564">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="82d30-3564">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="82d30-3565">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="82d30-3565">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="82d30-3566">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="82d30-3566">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="82d30-3567">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="82d30-3567">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="82d30-3568">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3568">Added `--progress` flag</span></span>
* <span data-ttu-id="82d30-3569">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3569">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="82d30-3570">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="82d30-3570">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="82d30-3571">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="82d30-3571">IoT</span></span>

* <span data-ttu-id="82d30-3572">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="82d30-3572">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="82d30-3573">(3934).</span><span class="sxs-lookup"><span data-stu-id="82d30-3573">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="82d30-3574">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="82d30-3574">Key vault</span></span>

* <span data-ttu-id="82d30-3575">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="82d30-3575">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="82d30-3576">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3576">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="82d30-3577">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="82d30-3577">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="82d30-3578">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3578">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="82d30-3579">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3579">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="82d30-3580">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="82d30-3580">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="82d30-3581">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="82d30-3581">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="82d30-3582">(3307).</span><span class="sxs-lookup"><span data-stu-id="82d30-3582">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="82d30-3583">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="82d30-3583">Lab</span></span>

* <span data-ttu-id="82d30-3584">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3584">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="82d30-3585">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3585">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-3586">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-3586">Monitor</span></span>

* <span data-ttu-id="82d30-3587">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="82d30-3587">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="82d30-3588">Переименование `monitor alert-rule-incidents list` в `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="82d30-3588">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="82d30-3589">Переименование `monitor alert-rule-incidents show` в `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="82d30-3589">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="82d30-3590">Переименование `monitor metric-defintions list` в `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="82d30-3590">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="82d30-3591">Переименование `monitor alert-rules` в `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="82d30-3591">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="82d30-3592">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="82d30-3592">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="82d30-3593">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="82d30-3593">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="82d30-3594">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="82d30-3594">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="82d30-3595">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="82d30-3595">`location` no longer required</span></span>
  * <span data-ttu-id="82d30-3596">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="82d30-3596">Add name and ID support for target</span></span>
  * <span data-ttu-id="82d30-3597">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="82d30-3597">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="82d30-3598">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="82d30-3598">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="82d30-3599">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="82d30-3599">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="82d30-3600">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="82d30-3600">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="82d30-3601">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3601">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="82d30-3602">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3602">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="82d30-3603">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-3603">Network</span></span>

* <span data-ttu-id="82d30-3604">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3604">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="82d30-3605">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3605">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="82d30-3606">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="82d30-3606">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="82d30-3607">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3607">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="82d30-3608">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3608">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="82d30-3609">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3609">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="82d30-3610">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3610">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="82d30-3611">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3611">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="82d30-3612">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3612">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="82d30-3613">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3613">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="82d30-3614">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3614">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="82d30-3615">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3615">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="82d30-3616">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3616">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="82d30-3617">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3617">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="82d30-3618">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3618">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="82d30-3619">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3619">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="82d30-3620">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="82d30-3620">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="82d30-3621">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3621">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="82d30-3622">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3622">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="82d30-3623">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3623">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="82d30-3624">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3624">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="82d30-3625">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3625">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="82d30-3626">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3626">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="82d30-3627">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="82d30-3627">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="82d30-3628">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="82d30-3628">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="82d30-3629">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="82d30-3629">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="82d30-3630">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="82d30-3630">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-3631">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-3631">Profile</span></span>

* <span data-ttu-id="82d30-3632">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="82d30-3632">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="82d30-3633">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="82d30-3633">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="82d30-3634">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="82d30-3634">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="82d30-3635">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="82d30-3635">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="82d30-3636">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="82d30-3636">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="82d30-3637">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="82d30-3637">RDBMS</span></span>

* <span data-ttu-id="82d30-3638">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="82d30-3638">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="82d30-3639">Исправлена проблема с обработкой `%s` из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="82d30-3639">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="82d30-3640">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="82d30-3640">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="82d30-3641">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="82d30-3641">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-3642">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-3642">Resource</span></span>

* <span data-ttu-id="82d30-3643">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3643">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="82d30-3644">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3644">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="82d30-3645">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3645">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="82d30-3646">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3646">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="82d30-3647">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="82d30-3647">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="82d30-3648">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3648">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="82d30-3649">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="82d30-3649">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="82d30-3650">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3650">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="82d30-3651">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-3651">Role</span></span>

* <span data-ttu-id="82d30-3652">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="82d30-3652">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="82d30-3653">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="82d30-3653">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="82d30-3654">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="82d30-3654">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="82d30-3655">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="82d30-3655">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="82d30-3656">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3656">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="82d30-3657">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="82d30-3657">Service Fabric</span></span>
* <span data-ttu-id="82d30-3658">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="82d30-3658">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="82d30-3659">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="82d30-3659">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="82d30-3660">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="82d30-3660">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-3661">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-3661">SQL</span></span>

* <span data-ttu-id="82d30-3662">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3662">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="82d30-3663">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3663">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="82d30-3664">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3664">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-3665">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-3665">Storage</span></span>

* <span data-ttu-id="82d30-3666">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="82d30-3666">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="82d30-3667">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="82d30-3667">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="82d30-3668">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="82d30-3668">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="82d30-3669">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="82d30-3669">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="82d30-3670">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="82d30-3670">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="82d30-3671">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="82d30-3671">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-3672">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-3672">VM</span></span>

* <span data-ttu-id="82d30-3673">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="82d30-3673">Support configuring nsg</span></span>
* <span data-ttu-id="82d30-3674">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="82d30-3674">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="82d30-3675">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="82d30-3675">Support managed service identities</span></span>
* <span data-ttu-id="82d30-3676">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3676">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="82d30-3677">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="82d30-3677">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="82d30-3678">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-3678">May 10, 2017</span></span>

<span data-ttu-id="82d30-3679">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="82d30-3679">Version 2.0.6</span></span>

* <span data-ttu-id="82d30-3680">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="82d30-3680">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="82d30-3681">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="82d30-3681">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="82d30-3682">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="82d30-3682">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="82d30-3683">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="82d30-3683">Include Cognitive Services module</span></span>
* <span data-ttu-id="82d30-3684">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="82d30-3684">Include Service Fabric module</span></span>
* <span data-ttu-id="82d30-3685">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="82d30-3685">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="82d30-3686">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="82d30-3686">Add support for CDN commands</span></span>
* <span data-ttu-id="82d30-3687">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="82d30-3687">Remove Container module</span></span>
* <span data-ttu-id="82d30-3688">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3688">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="82d30-3689">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3689">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="82d30-3690">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-3690">Core</span></span>

* <span data-ttu-id="82d30-3691">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="82d30-3691">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="82d30-3692">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([#2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3692">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="82d30-3693">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3693">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="82d30-3694">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3694">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="82d30-3695">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3695">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="82d30-3696">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3696">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="82d30-3697">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3697">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="82d30-3698">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3698">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="82d30-3699">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3699">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="82d30-3700">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="82d30-3700">core: Improved performance</span></span>
* <span data-ttu-id="82d30-3701">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="82d30-3701">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="82d30-3702">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="82d30-3702">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-3703">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-3703">ACS</span></span>

* <span data-ttu-id="82d30-3704">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="82d30-3704">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="82d30-3705">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="82d30-3705">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="82d30-3706">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="82d30-3706">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="82d30-3707">Удален профиль Windows перед вызовом метода PUT для команды scale ([#2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3707">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-3708">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-3708">AppService</span></span>

* <span data-ttu-id="82d30-3709">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="82d30-3709">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="82d30-3710">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="82d30-3710">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="82d30-3711">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="82d30-3711">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="82d30-3712">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="82d30-3712">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="82d30-3713">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="82d30-3713">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="82d30-3714">Включена поддержка настройки строк подключения ([#2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3714">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="82d30-3715">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="82d30-3715">support slot swap with preview</span></span>
* <span data-ttu-id="82d30-3716">Устранены ошибки из команд службы приложений ([#2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3716">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="82d30-3717">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([#2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3717">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="82d30-3718">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82d30-3718">CosmosDB</span></span>

* <span data-ttu-id="82d30-3719">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="82d30-3719">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="82d30-3720">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="82d30-3720">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="82d30-3721">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="82d30-3721">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="82d30-3722">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="82d30-3722">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="82d30-3723">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="82d30-3723">Data Lake Analytics</span></span>

* <span data-ttu-id="82d30-3724">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="82d30-3724">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="82d30-3725">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="82d30-3725">Add support for new catalog item type: package.</span></span> <span data-ttu-id="82d30-3726">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3726">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="82d30-3727">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="82d30-3727">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="82d30-3728">Таблица</span><span class="sxs-lookup"><span data-stu-id="82d30-3728">Table</span></span>
  * <span data-ttu-id="82d30-3729">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="82d30-3729">Table valued function</span></span>
  * <span data-ttu-id="82d30-3730">Представление</span><span class="sxs-lookup"><span data-stu-id="82d30-3730">View</span></span>
  * <span data-ttu-id="82d30-3731">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="82d30-3731">Table Statistics.</span></span> <span data-ttu-id="82d30-3732">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="82d30-3732">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="82d30-3733">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="82d30-3733">Data Lake Store</span></span>

* <span data-ttu-id="82d30-3734">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="82d30-3734">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="82d30-3735">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3735">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="82d30-3736">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="82d30-3736">missed help for access show.</span></span> <span data-ttu-id="82d30-3737">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="82d30-3737">adding it.</span></span> <span data-ttu-id="82d30-3738">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="82d30-3738">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="82d30-3739">Поиск</span><span class="sxs-lookup"><span data-stu-id="82d30-3739">Find</span></span>

* <span data-ttu-id="82d30-3740">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="82d30-3740">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="82d30-3741">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="82d30-3741">KeyVault</span></span>

* <span data-ttu-id="82d30-3742">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="82d30-3742">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="82d30-3743">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="82d30-3743">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="82d30-3744">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="82d30-3744">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="82d30-3745">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="82d30-3745">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="82d30-3746">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3746">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="82d30-3747">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="82d30-3747">Lab</span></span>

* <span data-ttu-id="82d30-3748">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="82d30-3748">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="82d30-3749">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="82d30-3749">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="82d30-3750">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="82d30-3750">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="82d30-3751">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="82d30-3751">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="82d30-3752">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="82d30-3752">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="82d30-3753">Монитор</span><span class="sxs-lookup"><span data-stu-id="82d30-3753">Monitor</span></span>

* <span data-ttu-id="82d30-3754">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3754">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="82d30-3755">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3755">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="82d30-3756">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-3756">Network</span></span>

* <span data-ttu-id="82d30-3757">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3757">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="82d30-3758">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3758">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="82d30-3759">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="82d30-3759">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="82d30-3760">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="82d30-3760">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="82d30-3761">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="82d30-3761">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="82d30-3762">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="82d30-3762">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="82d30-3763">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="82d30-3763">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="82d30-3764">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="82d30-3764">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="82d30-3765">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3765">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="82d30-3766">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="82d30-3766">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="82d30-3767">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3767">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="82d30-3768">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3768">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="82d30-3769">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="82d30-3769">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="82d30-3770">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="82d30-3770">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="82d30-3771">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="82d30-3771">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="82d30-3772">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="82d30-3772">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="82d30-3773">Профиль</span><span class="sxs-lookup"><span data-stu-id="82d30-3773">Profile</span></span>

* <span data-ttu-id="82d30-3774">Включена поддержка входа при отсутствии подписок ([#2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3774">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="82d30-3775">Включена поддержка сокращенных имен параметров в команде az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3775">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="82d30-3776">Redis</span><span class="sxs-lookup"><span data-stu-id="82d30-3776">Redis</span></span>

* <span data-ttu-id="82d30-3777">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="82d30-3777">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="82d30-3778">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="82d30-3778">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="82d30-3779">Ресурс</span><span class="sxs-lookup"><span data-stu-id="82d30-3779">Resource</span></span>

* <span data-ttu-id="82d30-3780">Добавлены команды определения managedapp и managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3780">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="82d30-3781">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3781">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="82d30-3782">Включена поддержка создания универсального ресурса ([#2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3782">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="82d30-3783">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="82d30-3783">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="82d30-3784">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="82d30-3784">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="82d30-3785">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="82d30-3785">Add docs for az lock update.</span></span> <span data-ttu-id="82d30-3786">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="82d30-3786">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="82d30-3787">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="82d30-3787">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="82d30-3788">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="82d30-3788">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="82d30-3789">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="82d30-3789">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="82d30-3790">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="82d30-3790">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="82d30-3791">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([#2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3791">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="82d30-3792">Роль</span><span class="sxs-lookup"><span data-stu-id="82d30-3792">Role</span></span>

* <span data-ttu-id="82d30-3793">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([#2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3793">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="82d30-3794">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3794">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="82d30-3795">Роль: устранены проблемы при обновлении определения роли ([#2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3795">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="82d30-3796">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="82d30-3796">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="82d30-3797">SQL</span><span class="sxs-lookup"><span data-stu-id="82d30-3797">SQL</span></span>

* <span data-ttu-id="82d30-3798">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="82d30-3798">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="82d30-3799">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3799">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="82d30-3800">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-3800">Storage</span></span>

* <span data-ttu-id="82d30-3801">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3801">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="82d30-3802">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="82d30-3802">Add support for incremental blob copy</span></span>
* <span data-ttu-id="82d30-3803">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="82d30-3803">Add support for large block blob upload</span></span>
* <span data-ttu-id="82d30-3804">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="82d30-3804">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-3805">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-3805">VM</span></span>

* <span data-ttu-id="82d30-3806">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="82d30-3806">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="82d30-3807">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="82d30-3807">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="82d30-3808">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="82d30-3808">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="82d30-3809">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="82d30-3809">az vm/vmss disk</span></span>
  3. <span data-ttu-id="82d30-3810">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="82d30-3810">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="82d30-3811">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="82d30-3811">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="82d30-3812">vm/vmss: добавлена поддержка создания из образа Marketplace, для которого требуются сведения о плане ([#1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3812">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="82d30-3813">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-3813">April 3, 2017</span></span>

<span data-ttu-id="82d30-3814">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="82d30-3814">Version 2.0.2</span></span>

<span data-ttu-id="82d30-3815">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="82d30-3815">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="82d30-3816">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="82d30-3816">Core</span></span>

* <span data-ttu-id="82d30-3817">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-3817">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="82d30-3818">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3818">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="82d30-3819">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3819">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="82d30-3820">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3820">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="82d30-3821">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3821">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="82d30-3822">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="82d30-3822">Add prompting for missing template parameters.</span></span> <span data-ttu-id="82d30-3823">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3823">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="82d30-3824">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="82d30-3824">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="82d30-3825">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="82d30-3825">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="82d30-3826">ACS</span><span class="sxs-lookup"><span data-stu-id="82d30-3826">ACS</span></span>

* <span data-ttu-id="82d30-3827">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3827">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="82d30-3828">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="82d30-3828">Add support for ssh key password prompting.</span></span> <span data-ttu-id="82d30-3829">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3829">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="82d30-3830">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="82d30-3830">Add support for windows clusters.</span></span> <span data-ttu-id="82d30-3831">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3831">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="82d30-3832">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="82d30-3832">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="82d30-3833">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3833">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="82d30-3834">AppService</span><span class="sxs-lookup"><span data-stu-id="82d30-3834">AppService</span></span>

* <span data-ttu-id="82d30-3835">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3835">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="82d30-3836">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3836">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="82d30-3837">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3837">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="82d30-3838">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3838">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="82d30-3839">Data Lake</span><span class="sxs-lookup"><span data-stu-id="82d30-3839">DataLake</span></span>

* <span data-ttu-id="82d30-3840">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="82d30-3840">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="82d30-3841">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="82d30-3841">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="82d30-3842">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="82d30-3842">DocuemntDB</span></span>

* <span data-ttu-id="82d30-3843">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3843">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="82d30-3844">ВМ</span><span class="sxs-lookup"><span data-stu-id="82d30-3844">VM</span></span>

* <span data-ttu-id="82d30-3845">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3845">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="82d30-3846">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3846">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="82d30-3847">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3847">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="82d30-3848">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3848">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="82d30-3849">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3849">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="82d30-3850">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3850">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="82d30-3851">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="82d30-3851">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="82d30-3852">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="82d30-3852">February 27, 2017</span></span>

<span data-ttu-id="82d30-3853">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="82d30-3853">Version 2.0.0</span></span>

<span data-ttu-id="82d30-3854">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="82d30-3854">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="82d30-3855">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="82d30-3855">Container Service (acs)</span></span>
- <span data-ttu-id="82d30-3856">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="82d30-3856">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="82d30-3857">Сеть</span><span class="sxs-lookup"><span data-stu-id="82d30-3857">Networking</span></span>
- <span data-ttu-id="82d30-3858">Память</span><span class="sxs-lookup"><span data-stu-id="82d30-3858">Storage</span></span>

<span data-ttu-id="82d30-3859">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3859">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="82d30-3860">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="82d30-3860">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="82d30-3861">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="82d30-3861">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="82d30-3862">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="82d30-3862">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="82d30-3863">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="82d30-3863">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="82d30-3864">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="82d30-3864">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="82d30-3865">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="82d30-3865">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="82d30-3866">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="82d30-3866">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="82d30-3867">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="82d30-3867">Provide feedback from the command line with the `az feedback` command</span></span>

# <a name="beta-release-notes"></a>[<span data-ttu-id="82d30-3868">Заметки о выпуске бета-версии</span><span class="sxs-lookup"><span data-stu-id="82d30-3868">Beta release notes</span></span>](#tab/azure-cli-beta)

<span data-ttu-id="82d30-3869">Бета-версия Azure CLI позволяет перейти с метода аутентификации платформы AAD (версия 1.0) на [платформу удостоверений Майкрософт (версия 2.0)](/azure/active-directory/develop/v2-overview).</span><span class="sxs-lookup"><span data-stu-id="82d30-3869">The Azure CLI beta release is a migration from the authentican method of AAD platform (v1.0) to [Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview).</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="82d30-3870">23 июня 2020 года</span><span class="sxs-lookup"><span data-stu-id="82d30-3870">June 23, 2020</span></span>

### <a name="things-to-know-about-the-new-azure-cli-beta-release"></a><span data-ttu-id="82d30-3871">Сведения о новой бета-версии Azure CLI</span><span class="sxs-lookup"><span data-stu-id="82d30-3871">Things to know about the new Azure CLI beta release</span></span>

-   <span data-ttu-id="82d30-3872">Бета-версия Azure CLI поддерживает все команды интерфейса командной строки, которые включены в текущую выпущенную версию.</span><span class="sxs-lookup"><span data-stu-id="82d30-3872">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span>
-   <span data-ttu-id="82d30-3873">После установки бета-версии требуется выполнить повторный вход.</span><span class="sxs-lookup"><span data-stu-id="82d30-3873">Relogin is required after install the beta version.</span></span>
-   <span data-ttu-id="82d30-3874">Бета-версия поддерживает только платформу Windows.</span><span class="sxs-lookup"><span data-stu-id="82d30-3874">The beta release only supports the Windows platform.</span></span>
-   <span data-ttu-id="82d30-3875">Azure Stack не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82d30-3875">The Azure Stack is not supported.</span></span>
-   <span data-ttu-id="82d30-3876">Параметр `--use-cert-sn-issuer` не поддерживается, если для проверки подлинности используется ключ субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="82d30-3876">`--use-cert-sn-issuer` parameter is not supported when using service principal key to authenticate.</span></span>
-   <span data-ttu-id="82d30-3877">Пропуск проверки SSL с использованием `ADAL_PYTHON_SSL_NO_VERIFY` среды не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82d30-3877">Skip SSL verification via environment `ADAL_PYTHON_SSL_NO_VERIFY` is not supported.</span></span>

<span data-ttu-id="82d30-3878">Если у вас возникли проблемы с использованием бета-версии, вы можете обратиться к группе разработчиков Azure CLI на [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span><span class="sxs-lookup"><span data-stu-id="82d30-3878">If you find any issues in the beta release, the Azure CLI engineering team welcomes your comments on [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span></span>

---
