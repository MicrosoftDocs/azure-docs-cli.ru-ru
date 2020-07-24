---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 07/16/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: d8f134b28c3c2c288a0a0faa0fcb64c109cb1970
ms.sourcegitcommit: c473377d1c08ac4efd2480bf852c30dbf1044a57
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2020
ms.locfileid: "86415312"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="4a611-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="4a611-103">Azure CLI release notes</span></span>

# <a name="current-release-notes"></a>[<span data-ttu-id="4a611-104">Заметки о текущем выпуске</span><span class="sxs-lookup"><span data-stu-id="4a611-104">Current release notes</span></span>](#tab/azure-cli)

## <a name="july-16-2020"></a><span data-ttu-id="4a611-105">16 июля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-105">July 16, 2020</span></span>

<span data-ttu-id="4a611-106">Версия 2.9.1</span><span class="sxs-lookup"><span data-stu-id="4a611-106">Version 2.9.1</span></span>

### <a name="aks"></a><span data-ttu-id="4a611-107">AKS</span><span class="sxs-lookup"><span data-stu-id="4a611-107">AKS</span></span>

* <span data-ttu-id="4a611-108">Явный параметр VMSS в примере команды для Windows удален, так как он теперь используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-108">Remove explicit setting of VMSS in Windows example command since it is now default</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-109">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-109">IoT</span></span>

* <span data-ttu-id="4a611-110">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az iot pnp`: удаление предварительной версии команд IoT PNP из основной версии CLI.</span><span class="sxs-lookup"><span data-stu-id="4a611-110">[BREAKING CHANGE] `az iot pnp`: Remove IoT PNP preview commands from core CLI</span></span>

### <a name="rest"></a><span data-ttu-id="4a611-111">REST</span><span class="sxs-lookup"><span data-stu-id="4a611-111">REST</span></span>

* <span data-ttu-id="4a611-112">Исправлена ошибка № 14152. `az rest`: URL-адреса ARM принимаются без идентификатора подписки.</span><span class="sxs-lookup"><span data-stu-id="4a611-112">Fix #14152: `az rest`: Accept ARM URLs without subscription ID</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-113">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-113">Storage</span></span>

* <span data-ttu-id="4a611-114">Исправлена ошибка № 14138. Некоторые разрешения стали необязательными.</span><span class="sxs-lookup"><span data-stu-id="4a611-114">Fix #14138: Make some permissions optional</span></span>

## <a name="july-14-2020"></a><span data-ttu-id="4a611-115">14 июля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-115">July 14, 2020</span></span>

<span data-ttu-id="4a611-116">Версия 2.9.0</span><span class="sxs-lookup"><span data-stu-id="4a611-116">Version 2.9.0</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-117">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-117">ACR</span></span>

* <span data-ttu-id="4a611-118">Обработка ссылки на артефакт журнала из реестра для потоковой передачи журналов.</span><span class="sxs-lookup"><span data-stu-id="4a611-118">Handle log artifact link from Registry to stream logs</span></span>
* <span data-ttu-id="4a611-119">Устарели команды helm2.</span><span class="sxs-lookup"><span data-stu-id="4a611-119">Deprecate helm2 commands</span></span>

### <a name="aks"></a><span data-ttu-id="4a611-120">AKS</span><span class="sxs-lookup"><span data-stu-id="4a611-120">AKS</span></span>

* <span data-ttu-id="4a611-121">`az aks create`: добавлен аргумент --enable-aad.</span><span class="sxs-lookup"><span data-stu-id="4a611-121">`az aks create`: add --enable-aad argument</span></span>
* <span data-ttu-id="4a611-122">`az aks update`: добавлен аргумент --enable-aad.</span><span class="sxs-lookup"><span data-stu-id="4a611-122">`az aks update`: add --enable-aad argument</span></span>

### <a name="apim"></a><span data-ttu-id="4a611-123">APIM</span><span class="sxs-lookup"><span data-stu-id="4a611-123">APIM</span></span>

* <span data-ttu-id="4a611-124">Добавлены общие команды az apim api.</span><span class="sxs-lookup"><span data-stu-id="4a611-124">Added general az apim api commands</span></span>

### <a name="appconfig"></a><span data-ttu-id="4a611-125">AppConfig</span><span class="sxs-lookup"><span data-stu-id="4a611-125">AppConfig</span></span>

* <span data-ttu-id="4a611-126">Добавлен пример для использования --fields в appconfig revision.</span><span class="sxs-lookup"><span data-stu-id="4a611-126">Add example for using --fields in appconfig revision</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-127">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-127">AppService</span></span>

* <span data-ttu-id="4a611-128">`az functionapp create`: включена поддержка Java 11 и PowerShell 7.</span><span class="sxs-lookup"><span data-stu-id="4a611-128">`az functionapp create`: Added support for Java 11 and Powershell 7.</span></span> <span data-ttu-id="4a611-129">Включена поддержка API стеков.</span><span class="sxs-lookup"><span data-stu-id="4a611-129">Added Stacks API Support.</span></span>
* <span data-ttu-id="4a611-130">Исправлена ошибка № 14208, из-за которой создание многоконтейнерного приложения завершается сбоем.</span><span class="sxs-lookup"><span data-stu-id="4a611-130">Fix #14208 multi-container app creation fails</span></span>
* <span data-ttu-id="4a611-131">Исправлена ошибка с az webapp create, связанная с использованием вписанных в код стеков среды выполнения.</span><span class="sxs-lookup"><span data-stu-id="4a611-131">Fix az webapp create - use hardcoded runtime stacks</span></span>

### <a name="arm"></a><span data-ttu-id="4a611-132">ARM</span><span class="sxs-lookup"><span data-stu-id="4a611-132">ARM</span></span>

* <span data-ttu-id="4a611-133">`az resource tag`: исправлена ошибка, связанная с добавлением тегов к ресурсам с помощью типа ресурса `Microsoft.ContainerInstance/containerGroups`.</span><span class="sxs-lookup"><span data-stu-id="4a611-133">`az resource tag`: Fix the problem of tagging resources with resource type `Microsoft.ContainerInstance/containerGroups`</span></span>

### <a name="compute"></a><span data-ttu-id="4a611-134">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4a611-134">Compute</span></span>

* <span data-ttu-id="4a611-135">Выполнено обновление версии дисков до 2020-05-01 и вычислительных ресурсов до 2020-06-01.</span><span class="sxs-lookup"><span data-stu-id="4a611-135">Bump version disks 2020-05-01, compute 2020-06-01</span></span>
* <span data-ttu-id="4a611-136">Включено двойное шифрование набора шифрования диска.</span><span class="sxs-lookup"><span data-stu-id="4a611-136">Double encryption of disk encryption set</span></span>
* <span data-ttu-id="4a611-137">`az vmss update`: включена поддержка определения межклиентского образа.</span><span class="sxs-lookup"><span data-stu-id="4a611-137">`az vmss update`: support specify cross tenant image.</span></span>
* <span data-ttu-id="4a611-138">`az sig image-version create`: включена поддержка определения межклиентского образа.</span><span class="sxs-lookup"><span data-stu-id="4a611-138">`az sig image-version create`: support specify cross tenant image.</span></span>
* <span data-ttu-id="4a611-139">vm/vmss create. Включено шифрование кэша и передаваемых данных для дисков ОС и данных и временных дисков для виртуальных машин и Масштабируемых наборов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="4a611-139">vm/vmss create: Encryption of cache & data-in-transit for OS/Data disks and temp disks for VM & VMSS</span></span>
* <span data-ttu-id="4a611-140">Добавлена операция имитации удаления для виртуальных машин и Масштабируемых наборов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="4a611-140">Add simulate-eviction operation for VM and VMSS</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4a611-141">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-141">CosmosDB</span></span>

* <span data-ttu-id="4a611-142">Последние компоненты: Autoscale, IpRules, EnableFreeTier и EnableAnalyticalStorage.</span><span class="sxs-lookup"><span data-stu-id="4a611-142">Recent features: Autoscale, IpRules, EnableFreeTier and EnableAnalyticalStorage</span></span>

### <a name="eventgrid"></a><span data-ttu-id="4a611-143">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="4a611-143">EventGrid</span></span>

* <span data-ttu-id="4a611-144">Включена поддержка CLI для 2020-04-01-preview и отмечены предварительные версии функций как is_Preview=true.</span><span class="sxs-lookup"><span data-stu-id="4a611-144">Add CLI support for 2020-04-01-preview and mark preview features with is_Preview=True</span></span>

### <a name="find"></a><span data-ttu-id="4a611-145">Поиск</span><span class="sxs-lookup"><span data-stu-id="4a611-145">Find</span></span>

* <span data-ttu-id="4a611-146">Исправлена ошибка № 14094, связанная с az find. Исправлена ошибка, из-за которой не удается войти при отключенной телеметрии.</span><span class="sxs-lookup"><span data-stu-id="4a611-146">Fix #14094 az find Fix Queries failing when not logged in and when telemetry is disabled</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4a611-147">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4a611-147">HDInsight</span></span>

* <span data-ttu-id="4a611-148">Добавлены две команды для перезагрузки узла HDInsight.</span><span class="sxs-lookup"><span data-stu-id="4a611-148">Add two commands to support hdinsight node reboot feature</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-149">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-149">Monitor</span></span>

* <span data-ttu-id="4a611-150">Удален флаг предварительной версии для команд в рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="4a611-150">Remove preview flag for commands under Log Analytics workspace</span></span>
* <span data-ttu-id="4a611-151">`az monitor diagnostic-settings subscription`: включена поддержка параметров диагностики для подписки.</span><span class="sxs-lookup"><span data-stu-id="4a611-151">`az monitor diagnostic-settings subscription`: Support diagnositc settings for subscription</span></span>
* <span data-ttu-id="4a611-152">`az monitor metrics`: включена поддержка символов "," и "|" в именах метрик.</span><span class="sxs-lookup"><span data-stu-id="4a611-152">`az monitor metrics`: support ',' and '|' in metric name</span></span>
* <span data-ttu-id="4a611-153">`az monitor log-analytics workspace data-export`: включена поддержка экспорта данных аналитики журнала.</span><span class="sxs-lookup"><span data-stu-id="4a611-153">`az monitor log-analytics workspace data-export`: support log analytics data export</span></span>

### <a name="network"></a><span data-ttu-id="4a611-154">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-154">Network</span></span>

* <span data-ttu-id="4a611-155">`az network application-gateway frontend-ip update`: Устарел параметр --public-ip-address.</span><span class="sxs-lookup"><span data-stu-id="4a611-155">`az network application-gateway frontend-ip update`: Deprecating the --public-ip-address parameter</span></span>
* <span data-ttu-id="4a611-156">Выполнено обновление azure-mgmt-network до 11.0.0.</span><span class="sxs-lookup"><span data-stu-id="4a611-156">Bump azure-mgmt-network to 11.0.0</span></span>
* <span data-ttu-id="4a611-157">`az network express-route gateway connection`: включена конфигурация маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="4a611-157">`az network express-route gateway connection`: support routing configuration</span></span>
* <span data-ttu-id="4a611-158">`az network virtual-appliance`: Включена поддержка сетевого виртуального устройства Azure.</span><span class="sxs-lookup"><span data-stu-id="4a611-158">`az network virtual-appliance`: Support Azure network virtual appliance.</span></span>
* <span data-ttu-id="4a611-159">Включена поддержка компонента Приватного канала в Шлюзе приложений.</span><span class="sxs-lookup"><span data-stu-id="4a611-159">Application Gateway support private link feature</span></span>

### <a name="policyinsights"></a><span data-ttu-id="4a611-160">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="4a611-160">PolicyInsights</span></span>

* <span data-ttu-id="4a611-161">`az policy state`: добавлена команда trigger-scan для активации оценки соответствия политикам.</span><span class="sxs-lookup"><span data-stu-id="4a611-161">`az policy state`: add trigger-scan command to trigger policy compliance evaluations</span></span>
* <span data-ttu-id="4a611-162">`az policy state list`: предоставлены версии сущностей политики в каждой записи соответствия.</span><span class="sxs-lookup"><span data-stu-id="4a611-162">`az policy state list`: expose versions of policy entities in each compliance record</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-163">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-163">Profile</span></span>

* <span data-ttu-id="4a611-164">`az account get-access-token`: включено отображение expiresOn для управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4a611-164">`az account get-access-token`: Show expiresOn for Managed Identity</span></span>

### <a name="rdbms"></a><span data-ttu-id="4a611-165">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4a611-165">RDBMS</span></span>

* <span data-ttu-id="4a611-166">Включена поддержка минимальной версии TLS.</span><span class="sxs-lookup"><span data-stu-id="4a611-166">Support Minimum TLS version</span></span>
* <span data-ttu-id="4a611-167">Включено шифрование инфраструктуры для Azure Postgres и MySQL</span><span class="sxs-lookup"><span data-stu-id="4a611-167">Add Infrastructure Encryption for Azure Postgres and MySQL</span></span>

### <a name="security"></a><span data-ttu-id="4a611-168">Безопасность</span><span class="sxs-lookup"><span data-stu-id="4a611-168">Security</span></span>

* <span data-ttu-id="4a611-169">Добавлены команды allowed_connections.</span><span class="sxs-lookup"><span data-stu-id="4a611-169">Add allowed_connections commands</span></span>
* <span data-ttu-id="4a611-170">Добавлены команды адаптивного усиления защиты сети.</span><span class="sxs-lookup"><span data-stu-id="4a611-170">Add Adaptive network hardeningss commands</span></span>
* <span data-ttu-id="4a611-171">Добавлены команды adaptive_application_controls.</span><span class="sxs-lookup"><span data-stu-id="4a611-171">Add adaptive_application_controls commands</span></span>
* <span data-ttu-id="4a611-172">Добавлены команды REST az security iot-solution/iot-alerts/iot-recommendations/iot-analytics в Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="4a611-172">Addition of az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST to Azure CLI</span></span>
* <span data-ttu-id="4a611-173">Добавлен интерфейс командной строки для обеспечения соответствия нормативным требованиям.</span><span class="sxs-lookup"><span data-stu-id="4a611-173">Add regulatory compliance CLI</span></span>

### <a name="signalr"></a><span data-ttu-id="4a611-174">SignalR</span><span class="sxs-lookup"><span data-stu-id="4a611-174">SignalR</span></span>

* <span data-ttu-id="4a611-175">Добавлены возможности, включая управление подключениями к частным конечным точкам, сетевыми правилами и вышестоящими компонентами.</span><span class="sxs-lookup"><span data-stu-id="4a611-175">Add features including managing private endpoint connections, network rules and upstream</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-176">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-176">SQL</span></span>

* <span data-ttu-id="4a611-177">`az sql mi create`, `az sql mi update`: добавлен параметр `--tags` для поддержки тегов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a611-177">`az sql mi create`, `az sql mi update`: Add `--tags` parameter to support resource tagging</span></span>
* <span data-ttu-id="4a611-178">`az sql mi failover`: включена поддержка отработки отказа с основного сайта на дополнительный.</span><span class="sxs-lookup"><span data-stu-id="4a611-178">`az sql mi failover`: Support failover from primary or secondary point</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-179">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-179">Storage</span></span>

* <span data-ttu-id="4a611-180">`az storage account create/update`: добавлен параметр --allow-blob-public-access для включения и отключения общего доступа к большим двоичным объектам и контейнерам.</span><span class="sxs-lookup"><span data-stu-id="4a611-180">`az storage account create/update`: Add --allow-blob-public-access to allow or disallow public access for blob and containers</span></span>
* <span data-ttu-id="4a611-181">`az storage account create/update`: добавлен параметр `--min-tls-version` для настройки минимальной версии TLS, используемой при выполнении запросов к хранилищу.</span><span class="sxs-lookup"><span data-stu-id="4a611-181">`az storage account create/update`: Add `--min-tls-version` to support setting the minimum TLS version to be permitted on requests to storage.</span></span>
* <span data-ttu-id="4a611-182">Удален возврат учетных данных маркера.</span><span class="sxs-lookup"><span data-stu-id="4a611-182">Remove check in token credential</span></span>
* <span data-ttu-id="4a611-183">Исправлено имя учетной записи хранения в примерах.</span><span class="sxs-lookup"><span data-stu-id="4a611-183">Fix the storage account name in examples</span></span>

### <a name="webapp"></a><span data-ttu-id="4a611-184">Веб-приложения</span><span class="sxs-lookup"><span data-stu-id="4a611-184">Webapp</span></span>

* <span data-ttu-id="4a611-185">Исправление. az webapp log deployment show: возврат журналов развертывания вместо метаданных журнала.</span><span class="sxs-lookup"><span data-stu-id="4a611-185">Bugfix: az webapp log deployment show - return deployment logs instead of log metadata</span></span>
* <span data-ttu-id="4a611-186">Исправление. az webapp vnet-integration add: исправлена обработка ошибок при неправильном имени виртуальной сети и включена поддержка идентификатора ресурса виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="4a611-186">Bugfix: az webapp vnet-integration add - fix error handling if bad vnet name, support vnet resource ID</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="4a611-187">23 июня 2020 года</span><span class="sxs-lookup"><span data-stu-id="4a611-187">June 23, 2020</span></span>

<span data-ttu-id="4a611-188">Версия 2.8.0</span><span class="sxs-lookup"><span data-stu-id="4a611-188">Version 2.8.0</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-189">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-189">ACR</span></span>

* <span data-ttu-id="4a611-190">Добавлена поддержка отключения конечных точек региона и отключения маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="4a611-190">Add support for region endpoint disable / routing disable</span></span>
* <span data-ttu-id="4a611-191">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.]  `az acr login --expose-token` не принимает имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="4a611-191">[BREAKING CHANGE] `az acr login --expose-token` does not accept username and password</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-192">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-192">ACS</span></span>

* <span data-ttu-id="4a611-193">Удален частный кластер и API 2019-10-27-preview.</span><span class="sxs-lookup"><span data-stu-id="4a611-193">Remove private cluster and 2019-10-27-preview API</span></span>

### <a name="aks"></a><span data-ttu-id="4a611-194">AKS</span><span class="sxs-lookup"><span data-stu-id="4a611-194">AKS</span></span>

* <span data-ttu-id="4a611-195">Включена поддержка параметра --yes для команды az aks upgrade.</span><span class="sxs-lookup"><span data-stu-id="4a611-195">Support --yes for az aks upgrade</span></span>
* <span data-ttu-id="4a611-196">Отменено изменение SKU виртуальной машины по умолчанию на Standard_D2s_v3 (№ 13541).</span><span class="sxs-lookup"><span data-stu-id="4a611-196">Revert "change default vm sku to Standard_D2s_v3 (#13541)"</span></span>
* <span data-ttu-id="4a611-197">Добавлена команда az aks update --uptime-sla.</span><span class="sxs-lookup"><span data-stu-id="4a611-197">Add "az aks update --uptime-sla"</span></span>
* <span data-ttu-id="4a611-198">Исправлена опечатка в команде az aks update.</span><span class="sxs-lookup"><span data-stu-id="4a611-198">Fix typo in az aks update command</span></span>
* <span data-ttu-id="4a611-199">Включена поддержка пула агентов узла 0 и блокировка ручного масштабирования для пула с поддержкой CAS.</span><span class="sxs-lookup"><span data-stu-id="4a611-199">Change to support 0 node agent pool and block manual scale for CAS enabled pool</span></span>
* <span data-ttu-id="4a611-200">Исправлена опечатка в VirtualMachineScaleSets и обновлены ссылки на версии Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="4a611-200">Fix typo on VirtualMachineScaleSets and update references to Kubernetes versions</span></span>

### <a name="ams"></a><span data-ttu-id="4a611-201">AMS</span><span class="sxs-lookup"><span data-stu-id="4a611-201">AMS</span></span>

* <span data-ttu-id="4a611-202">Изменен текст справки по параметру --expires.</span><span class="sxs-lookup"><span data-stu-id="4a611-202">CHANGE help text for "--expiry" parameter.</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-203">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-203">AppService</span></span>

* <span data-ttu-id="4a611-204">`az webapp log deployment show`: включено отображение журнала последнего развертывания или журналов конкретного развертывания, если указан идентификатор развертывания.</span><span class="sxs-lookup"><span data-stu-id="4a611-204">`az webapp log deployment show`: Show the latest deployment log, or the deployment logs of a specific deployment if deployment-id is specified</span></span>
* <span data-ttu-id="4a611-205">`az webapp log deployment list`: список доступных журналов развертывания.</span><span class="sxs-lookup"><span data-stu-id="4a611-205">`az webapp log deployment list`: List of deployment logs available</span></span>
* <span data-ttu-id="4a611-206">Исправление: ошибка поверхности при указании недопустимого имени веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="4a611-206">Fix: Surface error when invalid webapp name provided</span></span>
* <span data-ttu-id="4a611-207">Исправлена ошибка № 13261, и-за которой az webapp list-runtimes использует статический список до появления новых доступных API стеков.</span><span class="sxs-lookup"><span data-stu-id="4a611-207">Fix #13261 az webapp list-runtimes use static list until new Available Stacks API is available</span></span>
* <span data-ttu-id="4a611-208">`az appservice ase create`: исправлена ошибка создания № 13361.</span><span class="sxs-lookup"><span data-stu-id="4a611-208">`az appservice ase create`: Fix create issue #13361</span></span>
* <span data-ttu-id="4a611-209">`az appservice ase list-addresses`: исправлена ошибка изменения SDK № 13140.</span><span class="sxs-lookup"><span data-stu-id="4a611-209">`az appservice ase list-addresses`: Fix change of SDK #13140.</span></span>
* <span data-ttu-id="4a611-210">Исправлена ошибка создания слота или веб-приложения для контейнеров Windows.</span><span class="sxs-lookup"><span data-stu-id="4a611-210">Fix webapp/slot creation for Windows Containers</span></span>
* <span data-ttu-id="4a611-211">`az webapp auth update`: добавлен необязательный параметр для обновления версии среды выполнения.</span><span class="sxs-lookup"><span data-stu-id="4a611-211">`az webapp auth update`: Add optional parameter to update runtime-version</span></span>
* <span data-ttu-id="4a611-212">Включена поддержка перечисления, удаления, утверждения и отклонения подключения к частной конечной точке для веб-приложения в интерфейсе командной строки.</span><span class="sxs-lookup"><span data-stu-id="4a611-212">Support list, delete, approve and reject private endpoint connection for webapp in CLI</span></span>
* <span data-ttu-id="4a611-213">Исправлена ошибка № 13888: включена поддержка команд get, list, create для статических веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="4a611-213">Fix #13888 : Add support for Static WebApps: get, list, create commands</span></span>
* <span data-ttu-id="4a611-214">Улучшены сообщения об ошибках для подключения туннеля SSH.</span><span class="sxs-lookup"><span data-stu-id="4a611-214">Improved error messages for SSH Tunnel Connection</span></span>

### <a name="arm"></a><span data-ttu-id="4a611-215">ARM</span><span class="sxs-lookup"><span data-stu-id="4a611-215">ARM</span></span>

* <span data-ttu-id="4a611-216">`az tag`: добавлены примеры для параметра -h.</span><span class="sxs-lookup"><span data-stu-id="4a611-216">`az tag`: Add examples for -h</span></span>
* <span data-ttu-id="4a611-217">`az deployment group/sub what-if`: добавлен параметр --exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="4a611-217">`az deployment group/sub what-if`: Add --exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="4a611-218">`az deployment group/sub/mg/tenant create`: добавлен параметр --what-if-exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="4a611-218">`az deployment group/sub/mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="4a611-219">`az deployment group/sub/mg/tenant validate`: улучшен формат отображения сообщений об ошибках.</span><span class="sxs-lookup"><span data-stu-id="4a611-219">`az deployment group/sub/mg/tenant validate`: Show error messages in a better format.</span></span>
* <span data-ttu-id="4a611-220">`az group export`: добавлены новые параметры `--skip-resource-name-params` и `--skip-all-params` для включения поддержки параметризации с целью пропуска.</span><span class="sxs-lookup"><span data-stu-id="4a611-220">`az group export`: Add new parameters `--skip-resource-name-params` and `--skip-all-params` to support skip parameterization</span></span>
* <span data-ttu-id="4a611-221">Добавлена команда az feature unregister api.</span><span class="sxs-lookup"><span data-stu-id="4a611-221">Add az feature unregister api</span></span>

### <a name="aro"></a><span data-ttu-id="4a611-222">ARO</span><span class="sxs-lookup"><span data-stu-id="4a611-222">ARO</span></span>

* <span data-ttu-id="4a611-223">Добавлены атрибуты Public и Private в параметры для получения справки по видимости входящего трафика или сервера API.</span><span class="sxs-lookup"><span data-stu-id="4a611-223">Add Public, Private to params for help with ingress/apiserver visibility</span></span>

### <a name="batch"></a><span data-ttu-id="4a611-224">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-224">Batch</span></span>

* <span data-ttu-id="4a611-225">`az batch account create`: добавлен новый параметр `--public-network-access`.</span><span class="sxs-lookup"><span data-stu-id="4a611-225">`az batch account create`: Add new parameter `--public-network-access`</span></span>
* <span data-ttu-id="4a611-226">`az batch account create`: добавлен новый параметр `--identity-type`.</span><span class="sxs-lookup"><span data-stu-id="4a611-226">`az batch account create`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="4a611-227">`az batch account set`: добавлен новый параметр `--identity-type`.</span><span class="sxs-lookup"><span data-stu-id="4a611-227">`az batch account set`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="4a611-228">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az batch pool create. При создании пула с помощью пользовательского образа свойство --image теперь может ссылаться только на образ Общей коллекции образов.</span><span class="sxs-lookup"><span data-stu-id="4a611-228">[BREAKING CHANGE] az batch pool create: When creating a pool using a custom image, the --image property of can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="4a611-229">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az batch pool create. При создании пула с параметром --json-file и указании networkConfiguration свойство publicIPs было перемещено в новое свойство publicIPAddressConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4a611-229">[BREAKING CHANGE] az batch pool create: When creating a pool with --json-file option and specifying a networkConfiguration, the publicIPs property has moved in to a new property publicIPAddressConfiguration.</span></span> <span data-ttu-id="4a611-230">Это новое свойство также поддерживает новое свойство ipAddressProvisioningType, которое определяет, как пул должен выделять IP-адреса, и свойство publicIPs, которое позволяет настроить список ресурсов PublicIP для использования, когда для ipAddressProvisioningType указано значение UserManaged.</span><span class="sxs-lookup"><span data-stu-id="4a611-230">This new property also supports a new ipAddressProvisioningType property which specifies how the pool should allocate IP's and a publicIPs property which allows for configuration of a list of PublicIP resources to use in the case ipAddressProvisioningType is set to UserManaged</span></span>
* <span data-ttu-id="4a611-231">`az network private-link-resource`: включена поддержка ресурса Microsoft.Batch batchAccount.</span><span class="sxs-lookup"><span data-stu-id="4a611-231">`az network private-link-resource`: Add support for the Microsoft.Batch batchAccount resource</span></span>
* <span data-ttu-id="4a611-232">`az network private-endpoint-connection`: включена поддержка ресурса Microsoft.Batch batchAccount.</span><span class="sxs-lookup"><span data-stu-id="4a611-232">`az network private-endpoint-connection`: Add support for the Microsoft.Batch batchAccount resource</span></span>

### <a name="cdn"></a><span data-ttu-id="4a611-233">CDN</span><span class="sxs-lookup"><span data-stu-id="4a611-233">CDN</span></span>

* <span data-ttu-id="4a611-234">`az cdn custom-domain enable-https`: включена поддержка BYOC.</span><span class="sxs-lookup"><span data-stu-id="4a611-234">`az cdn custom-domain enable-https`: Add BYOC support.</span></span>
* <span data-ttu-id="4a611-235">`az cdn custom-domain enable-https`: исправлена ошибка включения пользовательского HTTPS с использованием управляемых CDN сертификатов для SKU Standard_Verizon и Standard_Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4a611-235">`az cdn custom-domain enable-https`: Fix enabling custom HTTPS with CDN managed certificates for Standard_Verizon and Standard_Microsoft SKUs.</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4a611-236">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4a611-236">Cognitive Services</span></span>

* <span data-ttu-id="4a611-237">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.]  `az cognitiveservices account` теперь имеет единую структуру для всех команд.</span><span class="sxs-lookup"><span data-stu-id="4a611-237">[BREAKING CHANGE] `az cognitiveservices account` now have a unified structure for all commands.</span></span>
* <span data-ttu-id="4a611-238">`az cognitiveservices account identity`: добавлена возможность управления удостоверениями для Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="4a611-238">`az cognitiveservices account identity`: Add identity management for Cognitive Services.</span></span>

### <a name="compute"></a><span data-ttu-id="4a611-239">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4a611-239">Compute</span></span>

* <span data-ttu-id="4a611-240">`az image builder`: обновлена версия API до 2020-02-14.</span><span class="sxs-lookup"><span data-stu-id="4a611-240">`az image builder`: Upgrade API version to 2020-02-14</span></span>
* <span data-ttu-id="4a611-241">`az image builder create`: добавлен параметр `--identity` для включения поддержки конфигурации удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4a611-241">`az image builder create`: Add `--identity` to support identity configuration</span></span>
* <span data-ttu-id="4a611-242">`az image builder customizer add`: включена поддержка настройщика Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="4a611-242">`az image builder customizer add`: Support Windows update customizer</span></span>
* <span data-ttu-id="4a611-243">Новая команда `az image builder cancel`.</span><span class="sxs-lookup"><span data-stu-id="4a611-243">New command `az image builder cancel`</span></span>
* <span data-ttu-id="4a611-244">Включено отображение предупреждения, когда пользователь развертывает VMSS, прикрепленные к конкретной версии образа, а не к последней.</span><span class="sxs-lookup"><span data-stu-id="4a611-244">Show a warning when a user deploys a VMSS pinned to a specific image version rather than latest</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="4a611-245">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-245">Cosmos DB</span></span>

* <span data-ttu-id="4a611-246">`az cosmosdb`: добавлена команда exists в базу данных и группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4a611-246">`az cosmosdb`: Add exists command to database and container groups</span></span>
* <span data-ttu-id="4a611-247">Разрешено создание фиксированных коллекций.</span><span class="sxs-lookup"><span data-stu-id="4a611-247">Allow creating fixed collections</span></span>

### <a name="eventhub"></a><span data-ttu-id="4a611-248">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="4a611-248">EventHub</span></span>

* <span data-ttu-id="4a611-249">`az eventhubs namespace create` : добавлены параметры управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4a611-249">`az eventhubs namespace create` : Add managed identity parameters</span></span>

### <a name="extension"></a><span data-ttu-id="4a611-250">Расширение</span><span class="sxs-lookup"><span data-stu-id="4a611-250">Extension</span></span>

* <span data-ttu-id="4a611-251">Добавлен параметр --version для включения поддержки установки из конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="4a611-251">Add --version to support to install from a specific version</span></span>
* <span data-ttu-id="4a611-252">Включены расширения CLI для включения пакетов в пространство имен Azure.</span><span class="sxs-lookup"><span data-stu-id="4a611-252">Enable CLI extensions to include packages in the 'azure' namespace</span></span>

### <a name="iot-hub"></a><span data-ttu-id="4a611-253">Центр Интернета вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-253">Iot Hub</span></span>

* <span data-ttu-id="4a611-254">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az iot hub job: удалены устаревшие команды заданий.</span><span class="sxs-lookup"><span data-stu-id="4a611-254">[BREAKING CHANGE] az iot hub job: Remove deprecated job commands</span></span>

### <a name="keyvault"></a><span data-ttu-id="4a611-255">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4a611-255">KeyVault</span></span>

* <span data-ttu-id="4a611-256">`az keyvault key import`: включена поддержка импорта из строк с помощью двух новых параметров.</span><span class="sxs-lookup"><span data-stu-id="4a611-256">`az keyvault key import`: Supports importing from strings via two new parameters.</span></span>
* <span data-ttu-id="4a611-257">Включена поддержка шифрования и расшифровки строк или байтов с помощью хранимых ключей.</span><span class="sxs-lookup"><span data-stu-id="4a611-257">Support string/bytes encryption and decryption with stored keys</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-258">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-258">Monitor</span></span>

* <span data-ttu-id="4a611-259">Включена поддержка возможности не дожидаться создания кластера.</span><span class="sxs-lookup"><span data-stu-id="4a611-259">Support no wait for cluster creation</span></span>
* <span data-ttu-id="4a611-260">`az monitor log-analytics workspace saved-search`: включена поддержка новых команд для сохраненного поиска.</span><span class="sxs-lookup"><span data-stu-id="4a611-260">`az monitor log-analytics workspace saved-search`: Support new commands for saved search</span></span>

### <a name="network"></a><span data-ttu-id="4a611-261">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-261">Network</span></span>

* <span data-ttu-id="4a611-262">`az network application-gateway address-pool update`: уточнено справочное сообщение и добавлены примеры.</span><span class="sxs-lookup"><span data-stu-id="4a611-262">`az network application-gateway address-pool update`: Refine help message and add examples.</span></span>
* <span data-ttu-id="4a611-263">`az network vnet create`: включена поддержка аргумента --nsg.</span><span class="sxs-lookup"><span data-stu-id="4a611-263">`az network vnet create`: Support --nsg argument</span></span>
* <span data-ttu-id="4a611-264">`az network lb address-pool`: включена поддержка создания внутреннего пула балансировки нагрузки с внутренним адресом.</span><span class="sxs-lookup"><span data-stu-id="4a611-264">`az network lb address-pool`: Support create lb backend pool with backend address.</span></span>
* <span data-ttu-id="4a611-265">`az network application-gateway address-pool`: исправлена ошибка с аргументом --add.</span><span class="sxs-lookup"><span data-stu-id="4a611-265">`az network application-gateway address-pool`: Fix for --add argument</span></span>

### <a name="rbac"></a><span data-ttu-id="4a611-266">RBAC</span><span class="sxs-lookup"><span data-stu-id="4a611-266">RBAC</span></span>

* <span data-ttu-id="4a611-267">`az ad sp create-for-rabc`: включена поддержка имен с пробелом, косой чертой и обратной косой чертой.</span><span class="sxs-lookup"><span data-stu-id="4a611-267">`az ad sp create-for-rabc`: Support name with space, slash and back slash</span></span>
* <span data-ttu-id="4a611-268">`az ad sp create-for-rbac`: уточнено сообщение об ошибке при указании недопустимой области пользователем.</span><span class="sxs-lookup"><span data-stu-id="4a611-268">`az ad sp create-for-rbac`: Refine error message when user specify an invalid scope</span></span>

### <a name="security"></a><span data-ttu-id="4a611-269">Безопасность</span><span class="sxs-lookup"><span data-stu-id="4a611-269">Security</span></span>

* <span data-ttu-id="4a611-270">Добавлены команды оценки безопасности.</span><span class="sxs-lookup"><span data-stu-id="4a611-270">Add security assessment commands</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-271">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-271">SQL</span></span>

* <span data-ttu-id="4a611-272">`az sql db ltr-policy/ltr-backup`: обновление и отображение политик долгосрочного хранения, отображение и удаление долгосрочных резервных копий, восстановление долгосрочных резервных копий.</span><span class="sxs-lookup"><span data-stu-id="4a611-272">`az sql db ltr-policy/ltr-backup`: update/show long term retention policy, show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-273">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-273">Storage</span></span>

* <span data-ttu-id="4a611-274">Исправлена проблема с проверкой подлинности для включения поддержки получения токена для параметра --subscription.</span><span class="sxs-lookup"><span data-stu-id="4a611-274">Fix authentication issue to support get token for --subscription</span></span>
* <span data-ttu-id="4a611-275">`az storage remove`: исправлена ошибка № 13459 с возникновением исключения при сбое операции.</span><span class="sxs-lookup"><span data-stu-id="4a611-275">`az storage remove`: Fix issue #13459 to raise exception for operation failure</span></span>
* <span data-ttu-id="4a611-276">Устранены ошибки № 13012, 13632 и 13657 для удаления неиспользуемых аргументов для команд, связанных с generate-sas.</span><span class="sxs-lookup"><span data-stu-id="4a611-276">Fix issues #13012, #13632 and #13657 to remove unused arguments for generate-sas related commands</span></span>
* <span data-ttu-id="4a611-277">`az storage logging update`: добавлена проверка версии ведения журнала.</span><span class="sxs-lookup"><span data-stu-id="4a611-277">`az storage logging update`: Add check for logging version</span></span>
* <span data-ttu-id="4a611-278">`az storage blob show`: добавлены дополнительные свойства для большого двоичного объекта с использованием пакета SDK для Track 2.</span><span class="sxs-lookup"><span data-stu-id="4a611-278">`az storage blob show`: Add more properties for blob with track 2 SDK</span></span>
* <span data-ttu-id="4a611-279">Исправление № 13708: уточнены предупреждающие сообщения об учетных данных.</span><span class="sxs-lookup"><span data-stu-id="4a611-279">Fix #13708: Refine warning message for credential</span></span>
* <span data-ttu-id="4a611-280">`az storage share-rm create/update`: включена поддержка протокола NFS и корневого сжатия.</span><span class="sxs-lookup"><span data-stu-id="4a611-280">`az storage share-rm create/update`: Add NFS protocol and root squash support</span></span>
* <span data-ttu-id="4a611-281">`az storage account create`: включена поддержка двойного шифрования.</span><span class="sxs-lookup"><span data-stu-id="4a611-281">`az storage account create`: Add support for double encryption</span></span>
* <span data-ttu-id="4a611-282">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.]  `az storage blob/container/file/share/table/queue generate-sas`: параметры --expiry и --permissions являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="4a611-282">[BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: make --expiry and --permissions required</span></span>
* <span data-ttu-id="4a611-283">`az storage blob set-tier`: миграция на Track 2 для включения поддержки настройки приоритета восстановления.</span><span class="sxs-lookup"><span data-stu-id="4a611-283">`az storage blob set-tier`: Migrate to Track 2 to support setting rehydrate priority</span></span>

## <a name="june-02-2020"></a><span data-ttu-id="4a611-284">02 июня 2020 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-284">June 02, 2020</span></span>

<span data-ttu-id="4a611-285">Версия 2.7.0</span><span class="sxs-lookup"><span data-stu-id="4a611-285">Version 2.7.0</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-286">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-286">ACR</span></span>

* <span data-ttu-id="4a611-287">Исправлена опечатка в сообщении об ошибке, возникающем при создании токена.</span><span class="sxs-lookup"><span data-stu-id="4a611-287">Fix a typo in an error message of token creation</span></span>

### <a name="aks"></a><span data-ttu-id="4a611-288">AKS</span><span class="sxs-lookup"><span data-stu-id="4a611-288">AKS</span></span>

* <span data-ttu-id="4a611-289">Номер SKU виртуальной машины по умолчанию изменен на Standard_D2s_v3.</span><span class="sxs-lookup"><span data-stu-id="4a611-289">Change default vm sku to Standard_D2s_v3</span></span>
* <span data-ttu-id="4a611-290">Исправлен процесс создания назначения ролей для кластера MSI и настраиваемой подсети.</span><span class="sxs-lookup"><span data-stu-id="4a611-290">Fix creating role assignment for MSI clsuter plus custom subnet</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-291">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-291">AppService</span></span>

* <span data-ttu-id="4a611-292">Исправлена ошибка 12739, из-за которой команда az appservice list-locations возвращает недопустимые расположения.</span><span class="sxs-lookup"><span data-stu-id="4a611-292">Fix #12739 az appservice list-locations returns some invalid locations</span></span>

### <a name="arm"></a><span data-ttu-id="4a611-293">ARM</span><span class="sxs-lookup"><span data-stu-id="4a611-293">ARM</span></span>

* <span data-ttu-id="4a611-294">`az deployment`: Исправлена ошибка 13159, из-за которой отображается неправильное сообщение JSON после удаления комментариев и сжатия.</span><span class="sxs-lookup"><span data-stu-id="4a611-294">`az deployment`: Fix issue #13159 of incorrect message of JSON after removing comments and compressing</span></span>
* <span data-ttu-id="4a611-295">`az resource tag`: Исправлена ошибка 13255, связанная с добавлением тегов к ресурсам с помощью типа ресурса `Microsoft.ContainerRegistry/registries/webhooks`.</span><span class="sxs-lookup"><span data-stu-id="4a611-295">`az resource tag`: Fix issue #13255 of tagging resources with resource type `Microsoft.ContainerRegistry/registries/webhooks`</span></span>
* <span data-ttu-id="4a611-296">Улучшены примеры для модуля ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a611-296">Improve the examples for the resource module</span></span>

### <a name="aro"></a><span data-ttu-id="4a611-297">ARO</span><span class="sxs-lookup"><span data-stu-id="4a611-297">ARO</span></span>

* <span data-ttu-id="4a611-298">Исправлена ошибка CLIError, связанная с неправильным флагом для --worker-vm-disk-size-gb.</span><span class="sxs-lookup"><span data-stu-id="4a611-298">Change CLIError to correct flag for --worker-vm-disk-size-gb</span></span>

### <a name="eventhub"></a><span data-ttu-id="4a611-299">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="4a611-299">EventHub</span></span>

* <span data-ttu-id="4a611-300">Исправлена ошибка 12406, из-за которой аргумент --capture-interval не обновляет intervalInSeconds.</span><span class="sxs-lookup"><span data-stu-id="4a611-300">Fix for issue #12406 Argument --capture-interval does not update the "intervalInSeconds"</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4a611-301">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4a611-301">HDInsight</span></span>

* <span data-ttu-id="4a611-302">Объект get_json_object изменен на shell_safe_json_parse.</span><span class="sxs-lookup"><span data-stu-id="4a611-302">Change get_json_object to shell_safe_json_parse</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-303">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-303">Monitor</span></span>

* <span data-ttu-id="4a611-304">`az monitor metrics alert`: уточнены нескольких справочных сообщений.</span><span class="sxs-lookup"><span data-stu-id="4a611-304">`az monitor metrics alert`: refine several help messages</span></span>
* <span data-ttu-id="4a611-305">`az monitor diagnostic-settings create`: включена поддержка аргумента --export-to-resource-specific.</span><span class="sxs-lookup"><span data-stu-id="4a611-305">`az monitor diagnostic-settings create`: support --export-to-resource-specific argument</span></span>
* <span data-ttu-id="4a611-306">Включена поддержка восстановления рабочей области LA.</span><span class="sxs-lookup"><span data-stu-id="4a611-306">Support LA workspace recover</span></span>

### <a name="network"></a><span data-ttu-id="4a611-307">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-307">Network</span></span>

* <span data-ttu-id="4a611-308">`az network dns zone`: включена поддержка символа -.</span><span class="sxs-lookup"><span data-stu-id="4a611-308">`az network dns zone`: support - character</span></span>
* <span data-ttu-id="4a611-309">`az network vpn-connection ipsec-policy`: изменены значения --sa-lifetime и --sa-max-size на более крупные в примере.</span><span class="sxs-lookup"><span data-stu-id="4a611-309">`az network vpn-connection ipsec-policy`: change the --sa-lifetime and --sa-max-size to larger values in example</span></span>
* <span data-ttu-id="4a611-310">Обновление сети до версии 2020-04-01</span><span class="sxs-lookup"><span data-stu-id="4a611-310">Bump network to 2020-04-01</span></span>
* <span data-ttu-id="4a611-311">`az network private-endpoint-connection`: включена поддержка Сетки событий.</span><span class="sxs-lookup"><span data-stu-id="4a611-311">`az network private-endpoint-connection`: support event grid</span></span>
* <span data-ttu-id="4a611-312">`az network express-route list-route-tables`: исправлена ошибка, из-за которой нельзя было перечислять маршруты в виде таблицы.</span><span class="sxs-lookup"><span data-stu-id="4a611-312">`az network express-route list-route-tables`: fix bug that cannot list routes as table</span></span>

### <a name="packaging"></a><span data-ttu-id="4a611-313">Упаковка</span><span class="sxs-lookup"><span data-stu-id="4a611-313">Packaging</span></span>

* <span data-ttu-id="4a611-314">Добавлен пакет Ubuntu Focal.</span><span class="sxs-lookup"><span data-stu-id="4a611-314">Add Ubuntu Focal Package</span></span>

### <a name="rbac"></a><span data-ttu-id="4a611-315">RBAC</span><span class="sxs-lookup"><span data-stu-id="4a611-315">RBAC</span></span>

* <span data-ttu-id="4a611-316">`az ad sp credential reset`: изменен процесс создания учетных данных, чтобы не использовать проблемные специальные символы.</span><span class="sxs-lookup"><span data-stu-id="4a611-316">`az ad sp credential reset`: modify credential generation to avoid troublesome special characters</span></span>

### <a name="redis"></a><span data-ttu-id="4a611-317">Redis</span><span class="sxs-lookup"><span data-stu-id="4a611-317">Redis</span></span>

* <span data-ttu-id="4a611-318">Исправление 13529: изменена документация по параметру enable_non_ssl_port.</span><span class="sxs-lookup"><span data-stu-id="4a611-318">Fix #13529: Change documentation of parameter enable_non_ssl_port</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-319">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-319">Storage</span></span>

* <span data-ttu-id="4a611-320">`az storage copy`: Добавлен параметр `--follow-symlinks` для включения поддержки символических ссылок.</span><span class="sxs-lookup"><span data-stu-id="4a611-320">`az storage copy`: Add parameter `--follow-symlinks` to support symlinks</span></span>
* <span data-ttu-id="4a611-321">Включен локальный контекст для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="4a611-321">Enable local context for storage account</span></span>
* <span data-ttu-id="4a611-322">`az storage logging`: Исправление 11969: уточнено сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="4a611-322">`az storage logging`: Fix issue #11969 to refine error message</span></span>

## <a name="may-19-2020"></a><span data-ttu-id="4a611-323">19 мая 2020 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-323">May 19, 2020</span></span>

<span data-ttu-id="4a611-324">Версия 2.6.0</span><span class="sxs-lookup"><span data-stu-id="4a611-324">Version 2.6.0</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-325">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-325">ACR</span></span>

* <span data-ttu-id="4a611-326">Добавлено время ожидания по умолчанию (5 минут) для любых запросов ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-326">Add default timeout of 5 minutes for any requests to ACR</span></span>
* <span data-ttu-id="4a611-327">Добавлена поддержка отключения доступа к общедоступной сети</span><span class="sxs-lookup"><span data-stu-id="4a611-327">Support disable public network access</span></span>
* <span data-ttu-id="4a611-328">`az acr token create`: предоставляет аргумент --days</span><span class="sxs-lookup"><span data-stu-id="4a611-328">`az acr token create`: expose --days argument</span></span>
* <span data-ttu-id="4a611-329">`az acr import`: принимает значения аргумента --source, которые содержат имя для входа в имени сервера, добавленное путем исправления на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="4a611-329">`az acr import`: accept --source argument values which contain login in server name through client end correction</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-330">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-330">ACS</span></span>

* <span data-ttu-id="4a611-331">Исправление ошибки: удаление больше не существующих полей</span><span class="sxs-lookup"><span data-stu-id="4a611-331">Bug fix: remove fields cleanup for fields that no longer exist</span></span>

### <a name="aks"></a><span data-ttu-id="4a611-332">AKS</span><span class="sxs-lookup"><span data-stu-id="4a611-332">AKS</span></span>

* <span data-ttu-id="4a611-333">Обновлен контекст справки команды uptime-sla</span><span class="sxs-lookup"><span data-stu-id="4a611-333">Update uptime-sla command help context</span></span>
* <span data-ttu-id="4a611-334">Удалена проверка диапазона для обновления числа минут для автомасштабирования</span><span class="sxs-lookup"><span data-stu-id="4a611-334">Remove range check for updating min count for autoscaler</span></span>
* <span data-ttu-id="4a611-335">Исправлена ошибка, из-за которой CLI не выдает ошибку, когда пользователь указывает только пароль Windows</span><span class="sxs-lookup"><span data-stu-id="4a611-335">Fix that cli doe not fail when user only specifies Windows password</span></span>

### <a name="ams"></a><span data-ttu-id="4a611-336">AMS</span><span class="sxs-lookup"><span data-stu-id="4a611-336">AMS</span></span>

* <span data-ttu-id="4a611-337">`az ams transform create`: добавлена возможность создания преобразования с предустановкой FaceDetector</span><span class="sxs-lookup"><span data-stu-id="4a611-337">`az ams transform create`: Add ability to create a transform with a FaceDetector preset</span></span>
* <span data-ttu-id="4a611-338">`az ams content-key-policy create` : добавлена возможность создания политики ключа содержимого FairPlay с конфигурацией автономной аренды</span><span class="sxs-lookup"><span data-stu-id="4a611-338">`az ams content-key-policy create` : Add ability to create a FairPlay content key policy with an offline rental configuration</span></span>

### <a name="appconfig"></a><span data-ttu-id="4a611-339">AppConfig</span><span class="sxs-lookup"><span data-stu-id="4a611-339">AppConfig</span></span>

* <span data-ttu-id="4a611-340">Исправлена ошибка при отображении значений ключей с полями</span><span class="sxs-lookup"><span data-stu-id="4a611-340">Bug fix for list key values with fields</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-341">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-341">AppService</span></span>

* <span data-ttu-id="4a611-342">`az functionapp create`: параметр AzureWebJobsDashboard будет задан только в случае отключения AppInsights</span><span class="sxs-lookup"><span data-stu-id="4a611-342">`az functionapp create`: AzureWebJobsDashboard will only be set if AppInsights is disabled</span></span>
* <span data-ttu-id="4a611-343">Исправление № 10664 — интеграция виртуальной сети — проблема проверки расположения и исправление № 13257 — сбой веб-приложения az в случае необходимости создания группы ресурсов</span><span class="sxs-lookup"><span data-stu-id="4a611-343">Fix #10664- VNet Integration - Location Check Issue & fix #13257- az webapp up failing when RG needs to be created</span></span>
* <span data-ttu-id="4a611-344">`az webapp|functionapp config ssl import`: добавлен поиск хранилища ключей в группах ресурсов в подписке и улучшены справка и примеры.</span><span class="sxs-lookup"><span data-stu-id="4a611-344">`az webapp|functionapp config ssl import`: Lookup key vault across resources groups in subscription and improve help and examples.</span></span>
* <span data-ttu-id="4a611-345">Подключен локальный контекст для службы приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-345">Onboard local context for app service</span></span>

### <a name="arm"></a><span data-ttu-id="4a611-346">ARM</span><span class="sxs-lookup"><span data-stu-id="4a611-346">ARM</span></span>

* <span data-ttu-id="4a611-347">`az deployment`: устранена проблема, из-за которой templateLink не возвращается при развертывании или проверке template-uri</span><span class="sxs-lookup"><span data-stu-id="4a611-347">`az deployment`: Fix the problem that the templateLink will not be returned when deploying or validating template-uri</span></span>
* <span data-ttu-id="4a611-348">`az deployment`: устранена проблема, из-за которой развертывание или проверка не поддерживает специально закодированный символ</span><span class="sxs-lookup"><span data-stu-id="4a611-348">`az deployment`: Fix the problem that deployment/validate does not support specially encoded character</span></span>
* <span data-ttu-id="4a611-349">`az deployment sub/group what-if`: исправлены выравнивание массива и обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="4a611-349">`az deployment sub/group what-if`: Fix array alignment and error handling</span></span>
* <span data-ttu-id="4a611-350">`az deployment operation`: изменение сведений об устаревании</span><span class="sxs-lookup"><span data-stu-id="4a611-350">`az deployment operation`: Modify the deprecate information</span></span>

### <a name="aro"></a><span data-ttu-id="4a611-351">ARO</span><span class="sxs-lookup"><span data-stu-id="4a611-351">ARO</span></span>

* <span data-ttu-id="4a611-352">Добавлены примеры в az aro create, list, list-credentials, show, delete</span><span class="sxs-lookup"><span data-stu-id="4a611-352">Add examples to az aro create, list, list-credentials, show, delete</span></span>
* <span data-ttu-id="4a611-353">Добавлена функция generate_random_id</span><span class="sxs-lookup"><span data-stu-id="4a611-353">Add generate_random_id function</span></span>

### <a name="backup"></a><span data-ttu-id="4a611-354">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="4a611-354">Backup</span></span>

* <span data-ttu-id="4a611-355">Разрешен параметр FriendlyName при включении защиты для команды AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="4a611-355">Allow FriendlyName in enable protection for AzureFileShare command</span></span>
* <span data-ttu-id="4a611-356">Исправлена restore-disks в IaasVM</span><span class="sxs-lookup"><span data-stu-id="4a611-356">Fix in IaasVM restore-disks Command</span></span>
* <span data-ttu-id="4a611-357">Добавлен тип BackupManagementType "MAB" в команду item list</span><span class="sxs-lookup"><span data-stu-id="4a611-357">Add "MAB" BackupManagementType to item list command</span></span>
* <span data-ttu-id="4a611-358">Добавлена поддержка повторного обновления политики для элементов с ошибками.</span><span class="sxs-lookup"><span data-stu-id="4a611-358">Add support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="4a611-359">Добавлена функция защиты от возобновления для виртуальной машины Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-359">Add Resume Protection functionality for Azure Virtual Machine</span></span>
* <span data-ttu-id="4a611-360">Добавлена поддержка возможности указывать группу ресурсов для хранения instantRP во время создания или изменения политики</span><span class="sxs-lookup"><span data-stu-id="4a611-360">Add support to specify ResourceGroup for storing instantRP during Create or Modify Policy</span></span>

### <a name="ci"></a><span data-ttu-id="4a611-361">CI</span><span class="sxs-lookup"><span data-stu-id="4a611-361">CI</span></span>

* <span data-ttu-id="4a611-362">Поддержка flake8 3.8.0</span><span class="sxs-lookup"><span data-stu-id="4a611-362">Support flake8 3.8.0</span></span>

### <a name="compute"></a><span data-ttu-id="4a611-363">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4a611-363">Compute</span></span>

* <span data-ttu-id="4a611-364">Новая команда az vm auto-shutdown</span><span class="sxs-lookup"><span data-stu-id="4a611-364">New command az vm auto-shutdown</span></span>
* <span data-ttu-id="4a611-365">`az vm list-skus`: обновлено поведение для параметра --zone — теперь он возвращает все номера SKU типов</span><span class="sxs-lookup"><span data-stu-id="4a611-365">`az vm list-skus`: Update --zone behavior, return all type skus now</span></span>

### <a name="core"></a><span data-ttu-id="4a611-366">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-366">Core</span></span>

* <span data-ttu-id="4a611-367">Обновлено состояние включения и выключения локального контекста на уровне глобального пользователя</span><span class="sxs-lookup"><span data-stu-id="4a611-367">Update local context on/off status to global user level</span></span>

### <a name="extension"></a><span data-ttu-id="4a611-368">Расширение</span><span class="sxs-lookup"><span data-stu-id="4a611-368">Extension</span></span>

* <span data-ttu-id="4a611-369">`az extension add`: добавлен параметр --system для включения установки расширений по системному пути</span><span class="sxs-lookup"><span data-stu-id="4a611-369">`az extension add`: Add --system to enable installing extensions in a system path</span></span>
* <span data-ttu-id="4a611-370">Реализована поддержка .egg-info для хранения метаданных расширения типа wheel</span><span class="sxs-lookup"><span data-stu-id="4a611-370">Support .egg-info to store wheel type extension metadata</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-371">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-371">IoT</span></span>

* <span data-ttu-id="4a611-372">`az iot`: теперь в сообщении для информирования о первом запуске модуля команд Интернета вещей используется точный и современный идентификатор `azure-iot`, который не считается нерекомендуемым.</span><span class="sxs-lookup"><span data-stu-id="4a611-372">`az iot`: Update the IoT command module first run extension awareness message to the accurate, non-deprecated modern Id `azure-iot`.</span></span>

### <a name="iot-hub"></a><span data-ttu-id="4a611-373">Центр Интернета вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-373">IoT Hub</span></span>

* <span data-ttu-id="4a611-374">Добавлена поддержка API 2020-03-01 и команд сетевой изоляции</span><span class="sxs-lookup"><span data-stu-id="4a611-374">Support for 2020-03-01 API and Network Isolation commands</span></span>

### <a name="netappfiles"></a><span data-ttu-id="4a611-375">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="4a611-375">NetAppFiles</span></span>

* <span data-ttu-id="4a611-376">`az volume create`: добавлен параметр snapshot-id для создания тома. Это позволит пользователям создавать тома из существующего моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="4a611-376">`az volume create`: Adds snapshot-id as a parameter to create volume this will allow users to create a volume from existing snapshot.</span></span>

### <a name="network"></a><span data-ttu-id="4a611-377">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-377">Network</span></span>

* <span data-ttu-id="4a611-378">Исправлена ошибка, из-за которой значение ttl изменялось непредвиденным образом для add-record для dns</span><span class="sxs-lookup"><span data-stu-id="4a611-378">Fix ttl value changed unintended for dns add-record</span></span>
* <span data-ttu-id="4a611-379">`az network public-ip create`: информирование клиентов о выпуске критического изменения</span><span class="sxs-lookup"><span data-stu-id="4a611-379">`az network public-ip create`: Inform customers of a coming breaking change</span></span>
* <span data-ttu-id="4a611-380">Поддержка универсальных команд для сценария Приватного канала</span><span class="sxs-lookup"><span data-stu-id="4a611-380">Support generic commands for private link scenario</span></span>
* <span data-ttu-id="4a611-381">`az network private-endpoint-connection`: поддержка типов mysql, postgre и mariadb</span><span class="sxs-lookup"><span data-stu-id="4a611-381">`az network private-endpoint-connection`: Support mysql, postgre and mariadb types</span></span>
* <span data-ttu-id="4a611-382">`az network private-endpoint-connection`: поддержка типов cosmosdb</span><span class="sxs-lookup"><span data-stu-id="4a611-382">`az network private-endpoint-connection`: Support cosmosdb types</span></span>
* <span data-ttu-id="4a611-383">`az network private-endpoint`: параметр --group-ids теперь является нерекомендуемым и перенаправляется на --group-id</span><span class="sxs-lookup"><span data-stu-id="4a611-383">`az network private-endpoint`: deprecate --group-ids and redirect to --group-id</span></span>

### <a name="output"></a><span data-ttu-id="4a611-384">Выходные данные</span><span class="sxs-lookup"><span data-stu-id="4a611-384">Output</span></span>

* <span data-ttu-id="4a611-385">Отображение обновленной инструкции для find, feedback и --help</span><span class="sxs-lookup"><span data-stu-id="4a611-385">Show update instruction in find, feedback and --help</span></span>

### <a name="packaging"></a><span data-ttu-id="4a611-386">Упаковка</span><span class="sxs-lookup"><span data-stu-id="4a611-386">Packaging</span></span>

* <span data-ttu-id="4a611-387">Создание пакетов MSI/Homebrew с зависимостями, разрешенным из requirements.txt</span><span class="sxs-lookup"><span data-stu-id="4a611-387">Build MSI/Homebrew packages with dependecies resolved from requirements.txt</span></span>

### <a name="rbac"></a><span data-ttu-id="4a611-388">RBAC</span><span class="sxs-lookup"><span data-stu-id="4a611-388">RBAC</span></span>

* <span data-ttu-id="4a611-389">`az ad sp credential reset`: устранена возможность создания слабых учетных данных</span><span class="sxs-lookup"><span data-stu-id="4a611-389">`az ad sp credential reset`: fix weak credential generation</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-390">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-390">Storage</span></span>

* <span data-ttu-id="4a611-391">`az storage account file-service-properties update/show`: добавлена поддержка свойств файлов для учетной записи хранения</span><span class="sxs-lookup"><span data-stu-id="4a611-391">`az storage account file-service-properties update/show`: Add File Properties Support for Storage Account</span></span>
* <span data-ttu-id="4a611-392">`az storage container create`: исправление № 13373 путем добавления проверяющего элемента управления для общего доступа</span><span class="sxs-lookup"><span data-stu-id="4a611-392">`az storage container create`: Fix #13373 by adding validator for public access</span></span>
* <span data-ttu-id="4a611-393">Добавлена поддержка track2 для ADLS 2-го поколения</span><span class="sxs-lookup"><span data-stu-id="4a611-393">Add ADLS Gen2 track2 support</span></span>
* <span data-ttu-id="4a611-394">`az storage blob sync`: Включена поддержка `--connection-string`.</span><span class="sxs-lookup"><span data-stu-id="4a611-394">`az storage blob sync`: Support `--connection-string`</span></span>
* <span data-ttu-id="4a611-395">`az storage blob sync`: исправлено неверное сообщение об ошибке, которое отображается, когда azcopy не удается найти расположение установки</span><span class="sxs-lookup"><span data-stu-id="4a611-395">`az storage blob sync`: Fix the incorrect error message when azcopy cannot find the installation location</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="4a611-396">30 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-396">April 30, 2020</span></span>

<span data-ttu-id="4a611-397">Версия 2.5.1</span><span class="sxs-lookup"><span data-stu-id="4a611-397">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-398">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-398">ACR</span></span>

* <span data-ttu-id="4a611-399">`az acr check-health`: исправлена ошибка DOCKER_PULL_ERROR в Windows.</span><span class="sxs-lookup"><span data-stu-id="4a611-399">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="4a611-400">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4a611-400">Compute</span></span>

* <span data-ttu-id="4a611-401">`az vm list-ip-addresses`: Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="4a611-401">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="4a611-402">Исправлена ошибка создания виртуальной машины, которая возникает, если в профиле облака не задано значение endpoint_vm_image_alias_doc.</span><span class="sxs-lookup"><span data-stu-id="4a611-402">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="4a611-403">`az vmss create`: добавлен параметр --os-disk-size-gb.</span><span class="sxs-lookup"><span data-stu-id="4a611-403">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="4a611-404">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-404">Cosmos DB</span></span>

* <span data-ttu-id="4a611-405">`az cosmosdb create/update`: добавлена поддержка --enable-public-network.</span><span class="sxs-lookup"><span data-stu-id="4a611-405">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="4a611-406">Расширение</span><span class="sxs-lookup"><span data-stu-id="4a611-406">Extension</span></span>

* <span data-ttu-id="4a611-407">Исправлена загрузка неправильных метаданных для расширения типа колеса.</span><span class="sxs-lookup"><span data-stu-id="4a611-407">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="4a611-408">Упаковка</span><span class="sxs-lookup"><span data-stu-id="4a611-408">Packaging</span></span>

* <span data-ttu-id="4a611-409">Добавлен скрипт az для Git Bash/Cygwin в Windows.</span><span class="sxs-lookup"><span data-stu-id="4a611-409">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-410">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-410">SQL</span></span>

* <span data-ttu-id="4a611-411">`az sql instance-pool`: добавлена группа команд для пулов экземпляров.</span><span class="sxs-lookup"><span data-stu-id="4a611-411">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-412">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-412">Storage</span></span>

* <span data-ttu-id="4a611-413">Пакет azure-multiapi-storage обновлен до версии 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="4a611-413">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="4a611-414">Добавлена поддержка GZRS при создании и обновлении учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="4a611-414">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="4a611-415">`az storage account failover`: добавлена поддержка отработки отказа учетной записи хранения GRS или GZRS.</span><span class="sxs-lookup"><span data-stu-id="4a611-415">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="4a611-416">`az storage blob upload`: добавлен параметр --encryption-scope для указания сведений об области шифрования.</span><span class="sxs-lookup"><span data-stu-id="4a611-416">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="4a611-417">28 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-417">April 28, 2020</span></span>

<span data-ttu-id="4a611-418">Версия 2.5.0</span><span class="sxs-lookup"><span data-stu-id="4a611-418">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-419">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-419">ACS</span></span>

* <span data-ttu-id="4a611-420">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az openshift create: удален параметр --vnet-peer.</span><span class="sxs-lookup"><span data-stu-id="4a611-420">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="4a611-421">`az openshift create`: добавлены флаги для поддержки частного кластера.</span><span class="sxs-lookup"><span data-stu-id="4a611-421">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="4a611-422">`az openshift`: обновление до версии API `2019-10-27-preview`.</span><span class="sxs-lookup"><span data-stu-id="4a611-422">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="4a611-423">`az openshift`: добавлена команда `update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-423">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="4a611-424">AKS</span><span class="sxs-lookup"><span data-stu-id="4a611-424">AKS</span></span>

* <span data-ttu-id="4a611-425">`az aks create`: включена поддержка Windows.</span><span class="sxs-lookup"><span data-stu-id="4a611-425">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-426">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-426">AppService</span></span>

* <span data-ttu-id="4a611-427">`az webapp deployment source config-zip`: удалена функция перевода в спящий режим после выполнения request.get().</span><span class="sxs-lookup"><span data-stu-id="4a611-427">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="4a611-428">ARM</span><span class="sxs-lookup"><span data-stu-id="4a611-428">ARM</span></span>

* <span data-ttu-id="4a611-429">Добавлены команды What-If развертывания шаблона.</span><span class="sxs-lookup"><span data-stu-id="4a611-429">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="4a611-430">ARO</span><span class="sxs-lookup"><span data-stu-id="4a611-430">ARO</span></span>

* <span data-ttu-id="4a611-431">`az aro`: исправлены выходные данные таблицы.</span><span class="sxs-lookup"><span data-stu-id="4a611-431">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="4a611-432">CI</span><span class="sxs-lookup"><span data-stu-id="4a611-432">CI</span></span>

* <span data-ttu-id="4a611-433">Включена поддержка PyTest и прекращена поддержка Nose для автотестов.</span><span class="sxs-lookup"><span data-stu-id="4a611-433">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="4a611-434">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4a611-434">Compute</span></span>

* <span data-ttu-id="4a611-435">`az vmss disk detach`: устранена проблема с NoneType для диска данных.</span><span class="sxs-lookup"><span data-stu-id="4a611-435">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="4a611-436">`az vm availability-set list`: включена поддержка отображения списка виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="4a611-436">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="4a611-437">`az vm list-skus`: исправлена проблема с отображением формата таблицы.</span><span class="sxs-lookup"><span data-stu-id="4a611-437">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="4a611-438">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4a611-438">KeyVault</span></span>

* <span data-ttu-id="4a611-439">Добавлен новый параметр `--enable-rbac-authorization` для использования во время создания или обновления.</span><span class="sxs-lookup"><span data-stu-id="4a611-439">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-440">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-440">Monitor</span></span>

* <span data-ttu-id="4a611-441">Включена поддержка компонентов CMK в кластере LA.</span><span class="sxs-lookup"><span data-stu-id="4a611-441">Support LA cluster CMK features</span></span>
* <span data-ttu-id="4a611-442">`az monitor log-analytics workspace linked-storage`: включена поддержка функций BYOS.</span><span class="sxs-lookup"><span data-stu-id="4a611-442">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="4a611-443">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-443">Network</span></span>

* <span data-ttu-id="4a611-444">`az network security-partner`: включена поддержка поставщика партнера по безопасности.</span><span class="sxs-lookup"><span data-stu-id="4a611-444">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="4a611-445">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="4a611-445">Privatedns</span></span>

* <span data-ttu-id="4a611-446">Добавлена функция в частной зоне DNS для импорта и экспорта файла зоны.</span><span class="sxs-lookup"><span data-stu-id="4a611-446">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="4a611-447">21 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-447">April 21, 2020</span></span>

<span data-ttu-id="4a611-448">Версия 2.4.0</span><span class="sxs-lookup"><span data-stu-id="4a611-448">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-449">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-449">ACR</span></span>

* <span data-ttu-id="4a611-450">`az acr run --cmd`: отключает переопределение рабочего каталога.</span><span class="sxs-lookup"><span data-stu-id="4a611-450">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="4a611-451">Включена поддержка выделенной конечной точки данных.</span><span class="sxs-lookup"><span data-stu-id="4a611-451">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="4a611-452">AKS</span><span class="sxs-lookup"><span data-stu-id="4a611-452">AKS</span></span>

* <span data-ttu-id="4a611-453">`az aks list -o table` теперь показывает privateFqdn как FQDN для частных кластеров.</span><span class="sxs-lookup"><span data-stu-id="4a611-453">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="4a611-454">Добавлен параметр --uptime-sla.</span><span class="sxs-lookup"><span data-stu-id="4a611-454">Add --uptime-sla</span></span>
* <span data-ttu-id="4a611-455">Обновлен пакет containerservice.</span><span class="sxs-lookup"><span data-stu-id="4a611-455">Update containerservice package</span></span>
* <span data-ttu-id="4a611-456">Включена поддержка общедоступных IP-адресов узлов.</span><span class="sxs-lookup"><span data-stu-id="4a611-456">Add node public IP support</span></span>
* <span data-ttu-id="4a611-457">Исправлена опечатка в команде справки.</span><span class="sxs-lookup"><span data-stu-id="4a611-457">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="4a611-458">AppConfig</span><span class="sxs-lookup"><span data-stu-id="4a611-458">AppConfig</span></span>

* <span data-ttu-id="4a611-459">Разрешена ссылка на хранилище ключей для команд kv list и export.</span><span class="sxs-lookup"><span data-stu-id="4a611-459">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="4a611-460">Исправлена ошибка при отображении значений ключей.</span><span class="sxs-lookup"><span data-stu-id="4a611-460">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-461">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-461">AppService</span></span>

* <span data-ttu-id="4a611-462">`az functionapp create`: изменен способ настройки linuxFxVersion для приложений-функций dotnet в Linux.</span><span class="sxs-lookup"><span data-stu-id="4a611-462">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="4a611-463">Это должно исправить ошибку, препятствующую созданию приложений dotnet для использования в Linux.</span><span class="sxs-lookup"><span data-stu-id="4a611-463">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="4a611-464">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az webapp create` Исправлена ошибка для сохранения существующих параметров AppSettings с помощью az webapp create.</span><span class="sxs-lookup"><span data-stu-id="4a611-464">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="4a611-465">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az webapp up` Исправлена ошибка для создания группы ресурсов для команды az webapp up при использовании флага -g.</span><span class="sxs-lookup"><span data-stu-id="4a611-465">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="4a611-466">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az webapp config` Исправлена ошибка для отображения значений для выходных данных не в формате JSON с помощью команды az webapp config connection-string list.</span><span class="sxs-lookup"><span data-stu-id="4a611-466">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="4a611-467">ARM</span><span class="sxs-lookup"><span data-stu-id="4a611-467">ARM</span></span>

* <span data-ttu-id="4a611-468">`az deployment create/validate`: добавлен параметр `--no-prompt` для пропуска запроса отсутствующих параметров для шаблона ARM.</span><span class="sxs-lookup"><span data-stu-id="4a611-468">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="4a611-469">`az deployment group/mg/sub/tenant validate`: включена поддержка комментариев в файле параметров развертывания.</span><span class="sxs-lookup"><span data-stu-id="4a611-469">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="4a611-470">`az deployment`: удалено значение `is_preview` для параметра `--handle-extended-json-format`.</span><span class="sxs-lookup"><span data-stu-id="4a611-470">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="4a611-471">`az deployment group/mg/sub/tenant cancel`: включена поддержка отмены развертывания для шаблона ARM.</span><span class="sxs-lookup"><span data-stu-id="4a611-471">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="4a611-472">`az deployment group/mg/sub/tenant validate`: улучшено отображение сообщения об ошибке при сбое проверки развертывания.</span><span class="sxs-lookup"><span data-stu-id="4a611-472">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="4a611-473">`az deployment-scripts`: добавлена новая команда для DeploymentScripts.</span><span class="sxs-lookup"><span data-stu-id="4a611-473">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="4a611-474">`az resource tag`: добавлен параметр `--is-incremental` для инкрементного добавления тегов к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="4a611-474">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="4a611-475">ARO</span><span class="sxs-lookup"><span data-stu-id="4a611-475">ARO</span></span>

* <span data-ttu-id="4a611-476">`az aro`:  добавлен модуль команды aro Azure RedHat OpenShift версии 4.</span><span class="sxs-lookup"><span data-stu-id="4a611-476">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="4a611-477">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-477">Batch</span></span>

* <span data-ttu-id="4a611-478">Обновлен API пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="4a611-478">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="4a611-479">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4a611-479">Compute</span></span>

* <span data-ttu-id="4a611-480">`az sig image-version create`: добавлен тип учетной записи хранения Premium_LRS.</span><span class="sxs-lookup"><span data-stu-id="4a611-480">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="4a611-481">`az vmss update`: устранена проблема с обновлением уведомления о завершении.</span><span class="sxs-lookup"><span data-stu-id="4a611-481">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="4a611-482">`az vm/vmss create`: включена поддержка версии специализированного образа.</span><span class="sxs-lookup"><span data-stu-id="4a611-482">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="4a611-483">API SIG версии 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="4a611-483">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="4a611-484">`az sig image-version create`: добавлен параметр --target-region-encryption.</span><span class="sxs-lookup"><span data-stu-id="4a611-484">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="4a611-485">Исправлена ошибка, из-за которой тесты завершались сбоем при последовательном выполнении из-за дублирования имени хранилища ключей в глобальном кэше в памяти.</span><span class="sxs-lookup"><span data-stu-id="4a611-485">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4a611-486">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-486">CosmosDB</span></span>

* <span data-ttu-id="4a611-487">Включена поддержка `az cosmosdb private-link-resource/private-endpoint-connection`.</span><span class="sxs-lookup"><span data-stu-id="4a611-487">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="4a611-488">IoT Central</span><span class="sxs-lookup"><span data-stu-id="4a611-488">IoT Central</span></span>

* <span data-ttu-id="4a611-489">Прекращена поддержка `az iotcentral`.</span><span class="sxs-lookup"><span data-stu-id="4a611-489">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="4a611-490">Добавлен модуль команды `az iot central`.</span><span class="sxs-lookup"><span data-stu-id="4a611-490">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-491">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-491">Monitor</span></span>

* <span data-ttu-id="4a611-492">Включена поддержка сценария приватного канала для монитора.</span><span class="sxs-lookup"><span data-stu-id="4a611-492">Support private link scenario for monitor</span></span>
* <span data-ttu-id="4a611-493">Исправлен неправильный способ имитации в test_monitor_general_operations.py.</span><span class="sxs-lookup"><span data-stu-id="4a611-493">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="4a611-494">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-494">Network</span></span>

* <span data-ttu-id="4a611-495">Прекращена поддержка SKU для команды public ip update.</span><span class="sxs-lookup"><span data-stu-id="4a611-495">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="4a611-496">`az network private-endpoint`: включена поддержка закрытой группы зон DNS.</span><span class="sxs-lookup"><span data-stu-id="4a611-496">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="4a611-497">Включена функция локального контекста для параметра vnet/subnet.</span><span class="sxs-lookup"><span data-stu-id="4a611-497">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="4a611-498">Исправлен неправильный пример использования в test_nw_flow_log_delete.</span><span class="sxs-lookup"><span data-stu-id="4a611-498">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="4a611-499">Упаковка</span><span class="sxs-lookup"><span data-stu-id="4a611-499">Packaging</span></span>

* <span data-ttu-id="4a611-500">Прекращена поддержка пакета Ubuntu/Disco.</span><span class="sxs-lookup"><span data-stu-id="4a611-500">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="4a611-501">RBAC</span><span class="sxs-lookup"><span data-stu-id="4a611-501">RBAC</span></span>

* <span data-ttu-id="4a611-502">`az ad app create/update`: включена поддержка параметра --optional-claims.</span><span class="sxs-lookup"><span data-stu-id="4a611-502">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="4a611-503">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4a611-503">RDBMS</span></span>

* <span data-ttu-id="4a611-504">Добавлены команды администратора Azure Active Directory для PostgreSQL и MySQL.</span><span class="sxs-lookup"><span data-stu-id="4a611-504">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4a611-505">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4a611-505">Service Fabric</span></span>

* <span data-ttu-id="4a611-506">Исправление 12891: `az sf application update --application-parameters` удаляет старые параметры, отсутствующие в запросе.</span><span class="sxs-lookup"><span data-stu-id="4a611-506">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="4a611-507">Исправление 12470: включена поддержка az sf create cluster, исправлены ошибки, связанные с устойчивостью и надежностью обновления, поиск VMSS выполняется корректно в коде при указании имени типа узла.</span><span class="sxs-lookup"><span data-stu-id="4a611-507">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-508">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-508">SQL</span></span>

* <span data-ttu-id="4a611-509">Добавлены команды `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`.</span><span class="sxs-lookup"><span data-stu-id="4a611-509">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="4a611-510">`az sql midb`: обновление и отображение политик долгосрочного хранения, отображение и удаление долгосрочных резервных копий, восстановление долгосрочных резервных копий.</span><span class="sxs-lookup"><span data-stu-id="4a611-510">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-511">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-511">Storage</span></span>

* <span data-ttu-id="4a611-512">Обновлена версия azure-mgmt-storage до 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="4a611-512">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="4a611-513">`az storage logging off`: включено отключение ведения журналов для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="4a611-513">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="4a611-514">`az storage account update`: включена автоматическая смена ключа для CMK.</span><span class="sxs-lookup"><span data-stu-id="4a611-514">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="4a611-515">`az storage account encryption-scope create/update/list/show`: включена настройка области шифрования.</span><span class="sxs-lookup"><span data-stu-id="4a611-515">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="4a611-516">`az storage container create`: добавлены параметры --default-encryption-scope и --deny-encryption-scope-override для настройки области шифрования на уровне контейнера.</span><span class="sxs-lookup"><span data-stu-id="4a611-516">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="4a611-517">Опрос</span><span class="sxs-lookup"><span data-stu-id="4a611-517">Survey</span></span>

* <span data-ttu-id="4a611-518">Добавлен параметр для отключения ссылки опроса.</span><span class="sxs-lookup"><span data-stu-id="4a611-518">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="4a611-519">01 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-519">April 01, 2020</span></span>

<span data-ttu-id="4a611-520">Версия 2.3.1</span><span class="sxs-lookup"><span data-stu-id="4a611-520">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-521">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-521">ACR</span></span>

* <span data-ttu-id="4a611-522">Исправлена неправильная версия azure-mgmt-containerregistry для Linux.</span><span class="sxs-lookup"><span data-stu-id="4a611-522">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-523">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-523">Profile</span></span>

* <span data-ttu-id="4a611-524">az login: Исправлена ошибка входа в облачных профилях, отличающихся от `latest`.</span><span class="sxs-lookup"><span data-stu-id="4a611-524">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="4a611-525">31 марта 2020 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-525">March 31, 2020</span></span>

<span data-ttu-id="4a611-526">Версия 2.3.0</span><span class="sxs-lookup"><span data-stu-id="4a611-526">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-527">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-527">ACR</span></span>

* <span data-ttu-id="4a611-528">az acr task update: исключение пустого указателя.</span><span class="sxs-lookup"><span data-stu-id="4a611-528">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="4a611-529">`az acr import`: Отредактировано справочное сообщение и сообщение об ошибке для уточнения того, как использовать параметры --source и --registry.</span><span class="sxs-lookup"><span data-stu-id="4a611-529">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="4a611-530">Добавлено средство проверки для аргумента registry_name.</span><span class="sxs-lookup"><span data-stu-id="4a611-530">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="4a611-531">`az acr login`: удален флаг предпросмотра для --expose-token.</span><span class="sxs-lookup"><span data-stu-id="4a611-531">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="4a611-532">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр ветви az acr task create/update.</span><span class="sxs-lookup"><span data-stu-id="4a611-532">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="4a611-533">Клиент az acr task update теперь может независимо обновлять контекст, токен GitHub и триггеры.</span><span class="sxs-lookup"><span data-stu-id="4a611-533">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="4a611-534">az acr agentpool: новая функция.</span><span class="sxs-lookup"><span data-stu-id="4a611-534">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="4a611-535">AKS</span><span class="sxs-lookup"><span data-stu-id="4a611-535">AKS</span></span>

* <span data-ttu-id="4a611-536">Исправлена ошибка с apiServerAccessProfile при обновлении --api-server-authorized-ip-ranges.</span><span class="sxs-lookup"><span data-stu-id="4a611-536">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="4a611-537">Обновление AKS: при обновлении исходящие IP-адреса переопределяются с помощью входных значений.</span><span class="sxs-lookup"><span data-stu-id="4a611-537">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="4a611-538">Не создаются имена субъектов-служб для кластеров MSI и реализована поддержка присоединение ACR к кластерам MSI.</span><span class="sxs-lookup"><span data-stu-id="4a611-538">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="4a611-539">AMS</span><span class="sxs-lookup"><span data-stu-id="4a611-539">AMS</span></span>

* <span data-ttu-id="4a611-540">Исправление 12469: не удается добавить content-key-policy для FairPlay из-за проблем с параметром ask.</span><span class="sxs-lookup"><span data-stu-id="4a611-540">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="4a611-541">AppConfig</span><span class="sxs-lookup"><span data-stu-id="4a611-541">AppConfig</span></span>

* <span data-ttu-id="4a611-542">Добавлен параметр --skip-keyvault для экспорта kv.</span><span class="sxs-lookup"><span data-stu-id="4a611-542">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-543">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-543">AppService</span></span>

* <span data-ttu-id="4a611-544">Исправление 12509: удален тег, добавлявшийся по умолчанию при создании приложения с помощью az webapp up.</span><span class="sxs-lookup"><span data-stu-id="4a611-544">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="4a611-545">az functionapp create: обновлено меню справки для --runtime-version и добавлено предупреждение, когда пользователь указывает параметр --runtime-version для DotNet.</span><span class="sxs-lookup"><span data-stu-id="4a611-545">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="4a611-546">az functionapp create: изменен способ установки JavaVersion для приложений-функций Windows.</span><span class="sxs-lookup"><span data-stu-id="4a611-546">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="4a611-547">ARM</span><span class="sxs-lookup"><span data-stu-id="4a611-547">ARM</span></span>

* <span data-ttu-id="4a611-548">az deployment create/validate: по умолчанию используется параметр --handle-extended-json-format.</span><span class="sxs-lookup"><span data-stu-id="4a611-548">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="4a611-549">az lock create: в справочную документацию добавлены примеры создания подресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a611-549">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="4a611-550">Список az deployment {group/mg/sub/tenant}: реализована поддержка фильтрации ProvisioningState.</span><span class="sxs-lookup"><span data-stu-id="4a611-550">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="4a611-551">az deployment: исправлена ошибка синтаксического анализа комментария в последнем аргументе.</span><span class="sxs-lookup"><span data-stu-id="4a611-551">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="4a611-552">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="4a611-552">Backup</span></span>

* <span data-ttu-id="4a611-553">Добавлена возможность восстановления нескольких файлов.</span><span class="sxs-lookup"><span data-stu-id="4a611-553">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="4a611-554">Добавлена возможность резервного копирования только дисков с ОС.</span><span class="sxs-lookup"><span data-stu-id="4a611-554">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="4a611-555">Добавлен параметр restore-as-unmanaged-disk, позволяющий задать неуправляемое восстановление.</span><span class="sxs-lookup"><span data-stu-id="4a611-555">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="4a611-556">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4a611-556">Compute</span></span>

* <span data-ttu-id="4a611-557">az vm create: для --nsg-rule добавлен вариант NONE.</span><span class="sxs-lookup"><span data-stu-id="4a611-557">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="4a611-558">az vmss create/update: удален тег предпросмотра для автоматического восстановления VMSS.</span><span class="sxs-lookup"><span data-stu-id="4a611-558">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="4a611-559">az vm update: реализована поддержка --workspace.</span><span class="sxs-lookup"><span data-stu-id="4a611-559">az vm update: Support --workspace</span></span>
* <span data-ttu-id="4a611-560">Исправлена ошибка в коде инициализации VirtualMachineScaleSetExtension.</span><span class="sxs-lookup"><span data-stu-id="4a611-560">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="4a611-561">Версия VMAccessAgent обновлена до 2.4.</span><span class="sxs-lookup"><span data-stu-id="4a611-561">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="4a611-562">az vmss set-orchestration-service-state: реализована поддержка состояния службы оркестрации наборов VMSS.</span><span class="sxs-lookup"><span data-stu-id="4a611-562">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="4a611-563">Версия API диска обновлена до 2019-11-01.</span><span class="sxs-lookup"><span data-stu-id="4a611-563">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="4a611-564">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun.</span><span class="sxs-lookup"><span data-stu-id="4a611-564">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="4a611-565">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-565">Cosmos DB</span></span>

* <span data-ttu-id="4a611-566">Добавлен отсутствовавший параметр --type для перенаправления в связи с устареванием.</span><span class="sxs-lookup"><span data-stu-id="4a611-566">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="4a611-567">Docker</span><span class="sxs-lookup"><span data-stu-id="4a611-567">Docker</span></span>

* <span data-ttu-id="4a611-568">Обновление до Alpine 3.11 и Python 3.6.10.</span><span class="sxs-lookup"><span data-stu-id="4a611-568">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="4a611-569">Расширение</span><span class="sxs-lookup"><span data-stu-id="4a611-569">Extension</span></span>

* <span data-ttu-id="4a611-570">Добавлена возможность загрузки расширений в системный путь через пакеты.</span><span class="sxs-lookup"><span data-stu-id="4a611-570">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4a611-571">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4a611-571">HDInsight</span></span>

* <span data-ttu-id="4a611-572">(az hdinsight create:) Добавлена возможность указания клиентами минимальной поддерживаемой версии TLS с помощью параметра `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="4a611-572">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="4a611-573">Допустимые значения: 1.0,1.1,1.2.</span><span class="sxs-lookup"><span data-stu-id="4a611-573">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-574">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-574">IoT</span></span>

* <span data-ttu-id="4a611-575">Добавлен параметр codeowner.</span><span class="sxs-lookup"><span data-stu-id="4a611-575">Add codeowner</span></span>
* <span data-ttu-id="4a611-576">az iot hub create: номер SKU по умолчанию изменен с F1 на S1.</span><span class="sxs-lookup"><span data-stu-id="4a611-576">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="4a611-577">iot hub: реализована поддержка IotHub в профиле 2019-03-01-hybrid.</span><span class="sxs-lookup"><span data-stu-id="4a611-577">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="4a611-578">IoT Central</span><span class="sxs-lookup"><span data-stu-id="4a611-578">IoTCentral</span></span>

* <span data-ttu-id="4a611-579">Обновлены сведения об ошибках, шаблон приложения по умолчанию и сообщение с подсказкой.</span><span class="sxs-lookup"><span data-stu-id="4a611-579">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="4a611-580">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4a611-580">KeyVault</span></span>

* <span data-ttu-id="4a611-581">Реализована поддержка резервного копирования и восстановления сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4a611-581">Support certificate backup/restore</span></span>
* <span data-ttu-id="4a611-582">keyvault create/update: добавлена поддержка параметра --retention-days.</span><span class="sxs-lookup"><span data-stu-id="4a611-582">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="4a611-583">При перечислении больше не показываются управляемые ключи и секреты.</span><span class="sxs-lookup"><span data-stu-id="4a611-583">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="4a611-584">az keyvault create: реализована поддержка `--network-acls`, `--network-acls-ips` и `--network-acls-vnets` для указания сетевых правил при создании хранилища.</span><span class="sxs-lookup"><span data-stu-id="4a611-584">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="4a611-585">Блокировка</span><span class="sxs-lookup"><span data-stu-id="4a611-585">Lock</span></span>

* <span data-ttu-id="4a611-586">Исправлена ошибка с командой az lock delete, не работавшей с Microsoft.DocumentDB.</span><span class="sxs-lookup"><span data-stu-id="4a611-586">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-587">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-587">Monitor</span></span>

* <span data-ttu-id="4a611-588">az monitor clone: добавлена возможность клонирования правил метрики из одного ресурса в другой.</span><span class="sxs-lookup"><span data-stu-id="4a611-588">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="4a611-589">Исправлена ошибка IcM179210086: не удается создать настраиваемое оповещение для метрики Application Insights.</span><span class="sxs-lookup"><span data-stu-id="4a611-589">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="4a611-590">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="4a611-590">NetAppFiles</span></span>

* <span data-ttu-id="4a611-591">az volume create: для томов защиты данных добавлены операции репликации (approve, suspend, resume, status, remove).</span><span class="sxs-lookup"><span data-stu-id="4a611-591">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="4a611-592">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-592">Network</span></span>

* <span data-ttu-id="4a611-593">az network application-gateway waf-policy managed-rule rule-set add: добавлена поддержка Microsoft_BotManagerRuleSet.</span><span class="sxs-lookup"><span data-stu-id="4a611-593">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="4a611-594">Журнал потоков наблюдателя за сетями: исправлены неправильные сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="4a611-594">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="4a611-595">Добавлена поддержка имен узлов в прослушивателе шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="4a611-595">support host names in application gateway listener</span></span>
* <span data-ttu-id="4a611-596">az network nat gateway: добавлена возможность создания пустого ресурса без общедоступного IP-адреса или общедоступного IP-префикса.</span><span class="sxs-lookup"><span data-stu-id="4a611-596">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="4a611-597">Добавлена возможность создания VPN-шлюза.</span><span class="sxs-lookup"><span data-stu-id="4a611-597">Support vpn gateway generation</span></span>
* <span data-ttu-id="4a611-598">Реализована поддержка `--if-none-match` для `az network dns record-set {} add-record`.</span><span class="sxs-lookup"><span data-stu-id="4a611-598">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="4a611-599">Упаковка</span><span class="sxs-lookup"><span data-stu-id="4a611-599">Packaging</span></span>

* <span data-ttu-id="4a611-600">Прекращена поддержка Python 3.5.</span><span class="sxs-lookup"><span data-stu-id="4a611-600">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-601">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-601">Profile</span></span>

* <span data-ttu-id="4a611-602">az login: добавлен показ предупреждений об ошибках MFA.</span><span class="sxs-lookup"><span data-stu-id="4a611-602">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="4a611-603">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4a611-603">RDBMS</span></span>

* <span data-ttu-id="4a611-604">Добавлены команды управления ключами шифрования данных сервера для PostgreSQL и MySQL.</span><span class="sxs-lookup"><span data-stu-id="4a611-604">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="4a611-605">10 марта 2020 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-605">March 10, 2020</span></span>

<span data-ttu-id="4a611-606">Версия 2.2.0</span><span class="sxs-lookup"><span data-stu-id="4a611-606">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-607">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-607">ACR</span></span>

* <span data-ttu-id="4a611-608">Исправлена команда `az acr login`, которая неправильно вызывала ошибку.</span><span class="sxs-lookup"><span data-stu-id="4a611-608">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="4a611-609">Добавлена новая команда `az acr helm install-cli`.</span><span class="sxs-lookup"><span data-stu-id="4a611-609">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="4a611-610">Добавлена частная ссылка и включена поддержка CMK.</span><span class="sxs-lookup"><span data-stu-id="4a611-610">Add private link and CMK support</span></span>
* <span data-ttu-id="4a611-611">Добавлена команда private-link-resource list.</span><span class="sxs-lookup"><span data-stu-id="4a611-611">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="4a611-612">AKS</span><span class="sxs-lookup"><span data-stu-id="4a611-612">AKS</span></span>

* <span data-ttu-id="4a611-613">Исправлена функция поиска AKS в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="4a611-613">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="4a611-614">az aks: устранены ошибки NoneType при мониторинге надстроек и пула агентов.</span><span class="sxs-lookup"><span data-stu-id="4a611-614">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="4a611-615">Добавлен параметр --nodepool-tags в пуле узлов при создании кластера Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="4a611-615">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="4a611-616">Добавлен параметр --tags при добавлении пула узлов в кластер или его обновлении.</span><span class="sxs-lookup"><span data-stu-id="4a611-616">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="4a611-617">aks create: добавлен параметр `--enable-private-cluster`.</span><span class="sxs-lookup"><span data-stu-id="4a611-617">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="4a611-618">Добавлен параметр --nodepool-labels в пуле узлов при создании кластера Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="4a611-618">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="4a611-619">Добавлен параметр --labels при добавлении нового пула узлов в кластер Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="4a611-619">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="4a611-620">Добавлен отсутствующий символ / в URL-адрес панели мониторинга.</span><span class="sxs-lookup"><span data-stu-id="4a611-620">add missing / in the dashboard url</span></span>
* <span data-ttu-id="4a611-621">Включена поддержка создания кластеров AKS для управляемых удостоверений</span><span class="sxs-lookup"><span data-stu-id="4a611-621">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="4a611-622">az aks: включена проверка состояния сетевого подключаемого модуля: Azure или Kubenet.</span><span class="sxs-lookup"><span data-stu-id="4a611-622">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="4a611-623">az aks: включена поддержка ключа сеанса AAD.</span><span class="sxs-lookup"><span data-stu-id="4a611-623">az aks: Add aad session key support</span></span>
* <span data-ttu-id="4a611-624">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az aks: включена поддержка изменений MSI для GF и BF для omsagent (мониторинг контейнеров) (1)</span><span class="sxs-lookup"><span data-stu-id="4a611-624">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="4a611-625">az aks use-dev-spaces: добавлен параметр типа конечной точки в команду use-dev-spaces для настройки конечной точки, созданной в контроллере Azure Dev Spaces.</span><span class="sxs-lookup"><span data-stu-id="4a611-625">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="4a611-626">AppConfig</span><span class="sxs-lookup"><span data-stu-id="4a611-626">AppConfig</span></span>

* <span data-ttu-id="4a611-627">Включена разблокировка с использованием kv set для добавления функции и ссылки на хранилище ключей.</span><span class="sxs-lookup"><span data-stu-id="4a611-627">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-628">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-628">AppService</span></span>

* <span data-ttu-id="4a611-629">az webapp create: устранена проблема с выполнением команды с параметром --runtime.</span><span class="sxs-lookup"><span data-stu-id="4a611-629">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="4a611-630">az functionapp deployment source config-zip: добавлено сообщение об ошибке, если группа ресурсов или имя функции недействительны или не существуют.</span><span class="sxs-lookup"><span data-stu-id="4a611-630">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="4a611-631">functionapp create: исправлено сообщение с предупреждением, которое появляется с `functionapp create` и в котором указан флаг `--functions_version`, но в имени флага ошибочно используется `_` вместо `-`.</span><span class="sxs-lookup"><span data-stu-id="4a611-631">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="4a611-632">az functionapp create: обновлен способ настройки linuxFxVersion и имени образа контейнера для приложений с функциями Linux.</span><span class="sxs-lookup"><span data-stu-id="4a611-632">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="4a611-633">az functionapp deployment source config-zip: устранена проблема, вызванная изменением параметров приложения во время развертывания ZIP, что приводит к ошибкам 5xx во время развертывания.</span><span class="sxs-lookup"><span data-stu-id="4a611-633">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="4a611-634">Исправление 5720946: не удается задать имя с помощью az webapp backup.</span><span class="sxs-lookup"><span data-stu-id="4a611-634">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="4a611-635">ARM</span><span class="sxs-lookup"><span data-stu-id="4a611-635">ARM</span></span>

* <span data-ttu-id="4a611-636">az resource: улучшены примеры для модуля ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a611-636">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="4a611-637">az policy assignment list: Включена поддержка списков назначений политик в области группы управления.</span><span class="sxs-lookup"><span data-stu-id="4a611-637">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="4a611-638">Добавлены команды `az deployment group` и `az deployment operation group` для развертывания шаблонов в группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a611-638">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="4a611-639">Это дубликат `az group deployment` и `az group deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="4a611-639">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="4a611-640">Добавлены команды `az deployment sub` и `az deployment operation sub` для развертывания шаблонов в области подписки.</span><span class="sxs-lookup"><span data-stu-id="4a611-640">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="4a611-641">Это дубликат `az deployment` и `az deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="4a611-641">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="4a611-642">Добавлены команды `az deployment mg` и `az deployment operation mg` для развертывания шаблонов в группах управления.</span><span class="sxs-lookup"><span data-stu-id="4a611-642">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="4a611-643">Добавлены команды `az deployment tenant` и `az deployment operation tenant` для развертывания шаблонов в области арендатора.</span><span class="sxs-lookup"><span data-stu-id="4a611-643">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="4a611-644">az policy assignment create: добавлено описание параметра `--location`.</span><span class="sxs-lookup"><span data-stu-id="4a611-644">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="4a611-645">az group deployment create: добавлен параметр `--aux-tenants` для включения поддержки перекрестных арендаторов.</span><span class="sxs-lookup"><span data-stu-id="4a611-645">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="4a611-646">CDN</span><span class="sxs-lookup"><span data-stu-id="4a611-646">CDN</span></span>

* <span data-ttu-id="4a611-647">Добавлены команды WAF CDN.</span><span class="sxs-lookup"><span data-stu-id="4a611-647">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="4a611-648">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4a611-648">Compute</span></span>

* <span data-ttu-id="4a611-649">az sig image-version: добавлен параметр --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="4a611-649">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="4a611-650">az ppg show: добавлен параметр --colocation-status, чтобы включить выборку состояния совместного размещения всех ресурсов в группе размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="4a611-650">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="4a611-651">az vmss create/update: включена поддержка автоматического исправления.</span><span class="sxs-lookup"><span data-stu-id="4a611-651">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="4a611-652">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az image template: шаблон переименован в построитель.</span><span class="sxs-lookup"><span data-stu-id="4a611-652">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="4a611-653">az image builder create: добавлен параметр --image-template.</span><span class="sxs-lookup"><span data-stu-id="4a611-653">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="4a611-654">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-654">Cosmos DB</span></span>

* <span data-ttu-id="4a611-655">Добавлены командлеты хранимой процедуры SQL, определяемых пользователем функций и триггеров.</span><span class="sxs-lookup"><span data-stu-id="4a611-655">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="4a611-656">az cosmosdb create: добавлен параметр --key-uri для добавления сведений о шифровании хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="4a611-656">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="4a611-657">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4a611-657">KeyVault</span></span>

* <span data-ttu-id="4a611-658">keyvault create: включена функция обратимого удаления по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-658">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-659">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-659">Monitor</span></span>

* <span data-ttu-id="4a611-660">az monitor metrics alert create: включена поддержка `~` в `--condition`.</span><span class="sxs-lookup"><span data-stu-id="4a611-660">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="4a611-661">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-661">Network</span></span>

* <span data-ttu-id="4a611-662">az network application-gateway rewrite-rule create: включена поддержка конфигурации URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="4a611-662">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="4a611-663">az network dns zone import: для параметра --zone-name в будущем можно будет не учитывать регистр.</span><span class="sxs-lookup"><span data-stu-id="4a611-663">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="4a611-664">az network private-endpoint/private-link-service: удалена метка предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="4a611-664">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="4a611-665">az network bastion: включена поддержка бастиона.</span><span class="sxs-lookup"><span data-stu-id="4a611-665">az network bastion: support bastion</span></span>
* <span data-ttu-id="4a611-666">az network vnet list-available-ips: включена поддержка списка доступных IP-адресов в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="4a611-666">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="4a611-667">az network watcher flow-log create/list/delete/update: добавлены новые команды для управления журналами потоков Наблюдателя и предоставлен параметр --location для явного определения Наблюдателя.</span><span class="sxs-lookup"><span data-stu-id="4a611-667">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="4a611-668">az network watcher flow-log configure: поддержка прекращена.</span><span class="sxs-lookup"><span data-stu-id="4a611-668">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="4a611-669">az network watcher flow-log show: включена поддержка параметров --location и --name для получения результатов в формате ARM; поддержка предыдущего форматированного вывода прекращена.</span><span class="sxs-lookup"><span data-stu-id="4a611-669">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="4a611-670">Политика</span><span class="sxs-lookup"><span data-stu-id="4a611-670">Policy</span></span>

* <span data-ttu-id="4a611-671">az policy assignment create: исправлена ошибка, из-за которой автоматически генерируемое имя назначения политики превышало предельное значение.</span><span class="sxs-lookup"><span data-stu-id="4a611-671">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="4a611-672">RBAC</span><span class="sxs-lookup"><span data-stu-id="4a611-672">RBAC</span></span>

* <span data-ttu-id="4a611-673">az ad group show: исправлено значение --group, обрабатываемое как проблема с регулярными выражениями.</span><span class="sxs-lookup"><span data-stu-id="4a611-673">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="4a611-674">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4a611-674">RDBMS</span></span>

* <span data-ttu-id="4a611-675">Обновлена версия пакета SDK azure-mgmt-rdbms до 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="4a611-675">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="4a611-676">az postgres private-endpoint-connection: включено управление подключениями частных конечных точек Postgres.</span><span class="sxs-lookup"><span data-stu-id="4a611-676">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="4a611-677">az postgres private-link-resource: включено управление ресурсами частных ссылок Postgres.</span><span class="sxs-lookup"><span data-stu-id="4a611-677">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="4a611-678">az mysql private-endpoint-connection: включено управление подключениями частных конечных точек MySQL.</span><span class="sxs-lookup"><span data-stu-id="4a611-678">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="4a611-679">az mysql private-link-resource: включено управление ресурсами частных ссылок MySQL.</span><span class="sxs-lookup"><span data-stu-id="4a611-679">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="4a611-680">az mariadb private-endpoint-connection: включено управление подключениями частных конечных точек MariaDB.</span><span class="sxs-lookup"><span data-stu-id="4a611-680">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="4a611-681">az mariadb private-link-resource: включено управление ресурсами частных ссылок MariaDB.</span><span class="sxs-lookup"><span data-stu-id="4a611-681">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="4a611-682">Обновление тестов частной конечной точки RDBMS</span><span class="sxs-lookup"><span data-stu-id="4a611-682">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-683">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-683">SQL</span></span>

* <span data-ttu-id="4a611-684">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention.</span><span class="sxs-lookup"><span data-stu-id="4a611-684">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="4a611-685">(sql server create:) добавлен необязательный флаг включения и отключения доступа к общедоступным сетям в команду создания SQL Server.</span><span class="sxs-lookup"><span data-stu-id="4a611-685">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="4a611-686">(sql server update:) внесены некоторые изменения для клиентов.</span><span class="sxs-lookup"><span data-stu-id="4a611-686">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="4a611-687">Добавлено свойство minimal_tls_version для MI и SQL DB.</span><span class="sxs-lookup"><span data-stu-id="4a611-687">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-688">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-688">Storage</span></span>

* <span data-ttu-id="4a611-689">az storage blob delete-batch: исправлено неправильное поведение флага `--dryrun`.</span><span class="sxs-lookup"><span data-stu-id="4a611-689">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="4a611-690">az storage account network-rule add (исправление): добавлено требование того, чтобы операция была идемпотентной.</span><span class="sxs-lookup"><span data-stu-id="4a611-690">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="4a611-691">az storage account create/update: включена поддержка предпочтения маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="4a611-691">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="4a611-692">Обновлена версия azure-mgmt-storage до 8.0.0.</span><span class="sxs-lookup"><span data-stu-id="4a611-692">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="4a611-693">az storage container immutability create: добавлен параметр --allow-protected-append-write.</span><span class="sxs-lookup"><span data-stu-id="4a611-693">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="4a611-694">az storage account private-link-resource list: включена поддержка вывода списка ресурсов частной ссылки для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="4a611-694">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="4a611-695">az storage account private-endpoint-connection approve/reject/show/delete: включена поддержка управления подключениями к частным конечным точкам.</span><span class="sxs-lookup"><span data-stu-id="4a611-695">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="4a611-696">az storage account blob-service-properties update: добавлены параметры --enable-restore-policy и --restore-days.</span><span class="sxs-lookup"><span data-stu-id="4a611-696">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="4a611-697">az storage blob restore: включена поддержка восстановления диапазонов BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="4a611-697">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="4a611-698">18 февраля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-698">February 18, 2020</span></span>

<span data-ttu-id="4a611-699">Версия 2.1.0</span><span class="sxs-lookup"><span data-stu-id="4a611-699">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-700">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-700">ACR</span></span>

* <span data-ttu-id="4a611-701">Добавлен новый аргумент `--expose-token` для `az acr login`.</span><span class="sxs-lookup"><span data-stu-id="4a611-701">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="4a611-702">Исправлены неправильные выходные данные `az acr task identity show -n Name -r Registry -o table`.</span><span class="sxs-lookup"><span data-stu-id="4a611-702">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="4a611-703">az acr login: отображение CLIError при наличии ошибок, возвращаемых командой docker.</span><span class="sxs-lookup"><span data-stu-id="4a611-703">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-704">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-704">ACS</span></span>

* <span data-ttu-id="4a611-705">aks create/update: добавление проверки `--vnet-subnet-id`.</span><span class="sxs-lookup"><span data-stu-id="4a611-705">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="4a611-706">Aladdin</span><span class="sxs-lookup"><span data-stu-id="4a611-706">Aladdin</span></span>

* <span data-ttu-id="4a611-707">Выполнение синтаксического анализа созданных примеров в _help.py для команд.</span><span class="sxs-lookup"><span data-stu-id="4a611-707">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="4a611-708">AMS</span><span class="sxs-lookup"><span data-stu-id="4a611-708">AMS</span></span>

* <span data-ttu-id="4a611-709">az ams теперь предоставляется в общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="4a611-709">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="4a611-710">AppConfig</span><span class="sxs-lookup"><span data-stu-id="4a611-710">AppConfig</span></span>

* <span data-ttu-id="4a611-711">Исправлено справочное сообщение, чтобы исключить неподдерживаемый фильтр ключей или меток.</span><span class="sxs-lookup"><span data-stu-id="4a611-711">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="4a611-712">Удален тег preview для большинства команд, кроме управляемого удостоверения и флагов функций.</span><span class="sxs-lookup"><span data-stu-id="4a611-712">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="4a611-713">Добавлен управляемый ключ клиента при обновлении магазинов.</span><span class="sxs-lookup"><span data-stu-id="4a611-713">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-714">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-714">AppService</span></span>

* <span data-ttu-id="4a611-715">az webapp list-runtimes: исправлена ошибка для list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="4a611-715">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="4a611-716">Добавлена команда az webapp|functionapp config ssl create.</span><span class="sxs-lookup"><span data-stu-id="4a611-716">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="4a611-717">Включена поддержка приложений-функций версии 3 и Node 12.</span><span class="sxs-lookup"><span data-stu-id="4a611-717">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="4a611-718">ARM</span><span class="sxs-lookup"><span data-stu-id="4a611-718">ARM</span></span>

* <span data-ttu-id="4a611-719">az policy assignment create: исправлено сообщение об ошибке, если параметр `--policy` является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="4a611-719">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="4a611-720">az group deployment create: Устранена ошибка stat: path too long for Windows при использовании большого файла parameters.json.</span><span class="sxs-lookup"><span data-stu-id="4a611-720">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="4a611-721">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="4a611-721">Backup</span></span>

* <span data-ttu-id="4a611-722">Исправлен поток восстановления на уровне элемента в OLR.</span><span class="sxs-lookup"><span data-stu-id="4a611-722">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="4a611-723">Включена поддержка восстановления в виде файлов для баз данных SQL и SAP.</span><span class="sxs-lookup"><span data-stu-id="4a611-723">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="4a611-724">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4a611-724">Compute</span></span>

* <span data-ttu-id="4a611-725">vm/vmss/availability-set update: add --ppg: разрешено обновление ProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="4a611-725">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="4a611-726">vmss create: add --data-disk-iops and --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="4a611-726">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="4a611-727">az vm host: удален тег preview для `vm host` и `vm host group`.</span><span class="sxs-lookup"><span data-stu-id="4a611-727">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="4a611-728">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправление 10728. `az vm create`: автоматическое создание подсети, если указанные виртуальная сеть и подсеть не существуют.</span><span class="sxs-lookup"><span data-stu-id="4a611-728">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="4a611-729">Повышена надежность списка образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="4a611-729">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="4a611-730">Eventhub</span><span class="sxs-lookup"><span data-stu-id="4a611-730">Eventhub</span></span>

* <span data-ttu-id="4a611-731">Включена поддержка Azure Stack для профиля 2019-03-01-hybrid.</span><span class="sxs-lookup"><span data-stu-id="4a611-731">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="4a611-732">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4a611-732">KeyVault</span></span>

* <span data-ttu-id="4a611-733">az keyvault key create: добавлено новое значение `import` для параметра `--ops`.</span><span class="sxs-lookup"><span data-stu-id="4a611-733">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="4a611-734">az keyvault key list-versions: включена поддержка параметров `--id` для определения ключей.</span><span class="sxs-lookup"><span data-stu-id="4a611-734">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="4a611-735">Включена поддержка подключений к частным конечным точкам.</span><span class="sxs-lookup"><span data-stu-id="4a611-735">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="4a611-736">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-736">Network</span></span>

* <span data-ttu-id="4a611-737">Выполнена активация azure-mgmt-network 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="4a611-737">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="4a611-738">az network private-link-service update/create: включена поддержка --enable-proxy-protocol.</span><span class="sxs-lookup"><span data-stu-id="4a611-738">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="4a611-739">Добавлена функция монитора подключения версии 2.</span><span class="sxs-lookup"><span data-stu-id="4a611-739">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="4a611-740">Упаковка</span><span class="sxs-lookup"><span data-stu-id="4a611-740">Packaging</span></span>

* <span data-ttu-id="4a611-741">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка Python 2.7.</span><span class="sxs-lookup"><span data-stu-id="4a611-741">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-742">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-742">Profile</span></span>

* <span data-ttu-id="4a611-743">Предварительный просмотр: В учетные записи подписок добавлены новые атрибуты `homeTenantId` и `managedByTenants`.</span><span class="sxs-lookup"><span data-stu-id="4a611-743">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="4a611-744">Чтобы изменения вступили в силу, повторно выполните команду `az login`.</span><span class="sxs-lookup"><span data-stu-id="4a611-744">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="4a611-745">az login: отображение предупреждения, если подписка связана с несколькими клиентами, но по умолчанию используется с первым из них</span><span class="sxs-lookup"><span data-stu-id="4a611-745">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="4a611-746">(чтобы выбрать определенный клиент при доступе к этой подписке, включите `--tenant` в `az login`).</span><span class="sxs-lookup"><span data-stu-id="4a611-746">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="4a611-747">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-747">Role</span></span>

* <span data-ttu-id="4a611-748">az role assignment create: исправлена ошибка с кодом HTTP 400, возникающая при присвоении роли субъекту-службе по отображаемому имени.</span><span class="sxs-lookup"><span data-stu-id="4a611-748">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-749">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-749">SQL</span></span>

* <span data-ttu-id="4a611-750">Обновлен командлет `az sql mi update` Управляемого экземпляра SQL (добавлены два новых параметра: tier и family).</span><span class="sxs-lookup"><span data-stu-id="4a611-750">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-751">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-751">Storage</span></span>

* <span data-ttu-id="4a611-752">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az storage account create`: Тип учетной записи хранения по умолчанию изменен на StorageV2.</span><span class="sxs-lookup"><span data-stu-id="4a611-752">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="4a611-753">4 февраля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-753">February 04, 2020</span></span>

<span data-ttu-id="4a611-754">Версия 2.0.81</span><span class="sxs-lookup"><span data-stu-id="4a611-754">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-755">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-755">ACS</span></span>

* <span data-ttu-id="4a611-756">Добавлена возможность задания выделенных исходящих портов и времени ожидания подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="4a611-756">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="4a611-757">Выполнено обновление до API версии 2019-11-01.</span><span class="sxs-lookup"><span data-stu-id="4a611-757">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-758">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-758">ACR</span></span>

* <span data-ttu-id="4a611-759">[Критическое изменение] `az acr delete` будет выводить запрос.</span><span class="sxs-lookup"><span data-stu-id="4a611-759">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="4a611-760">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда az acr task delete будет выводить запрос.</span><span class="sxs-lookup"><span data-stu-id="4a611-760">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="4a611-761">Добавлена новая группа команд az acr taskrun show/list/delete для управления выполнением задач.</span><span class="sxs-lookup"><span data-stu-id="4a611-761">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="4a611-762">AKS</span><span class="sxs-lookup"><span data-stu-id="4a611-762">AKS</span></span>

* <span data-ttu-id="4a611-763">Каждый кластер получает отдельный субъект-службу для улучшения изоляции.</span><span class="sxs-lookup"><span data-stu-id="4a611-763">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="4a611-764">AppConfig</span><span class="sxs-lookup"><span data-stu-id="4a611-764">AppConfig</span></span>

* <span data-ttu-id="4a611-765">Поддержка импорта ссылок на хранилище ключей из службы приложений и их экспорта в нее.</span><span class="sxs-lookup"><span data-stu-id="4a611-765">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="4a611-766">Поддержка импорта и экспорта всех меток между файлами appconfig.</span><span class="sxs-lookup"><span data-stu-id="4a611-766">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="4a611-767">Проверка имен ключей и функций перед настройкой и импортом.</span><span class="sxs-lookup"><span data-stu-id="4a611-767">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="4a611-768">Предоставление изменений номера SKU в хранилище конфигураций.</span><span class="sxs-lookup"><span data-stu-id="4a611-768">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="4a611-769">Новая группа команд для управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4a611-769">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-770">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-770">AppService</span></span>

* <span data-ttu-id="4a611-771">Azure Stack: команды поверхности в профиле 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="4a611-771">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="4a611-772">functionapp: добавлена возможность создавать приложения-функции Java в Linux.</span><span class="sxs-lookup"><span data-stu-id="4a611-772">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="4a611-773">ARM</span><span class="sxs-lookup"><span data-stu-id="4a611-773">ARM</span></span>

* <span data-ttu-id="4a611-774">Исправление ошибки 10246: аварийное завершение `az resource tag` в случае, если переданный параметр `--ids` являлся идентификатором группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a611-774">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="4a611-775">Исправление ошибки 11658: команда `az group export` не поддерживала параметры `--query` и `--output`.</span><span class="sxs-lookup"><span data-stu-id="4a611-775">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="4a611-776">Исправление ошибки 10279: код выхода `az group deployment validate` был равен 0, если проверка не пройдена.</span><span class="sxs-lookup"><span data-stu-id="4a611-776">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="4a611-777">Исправление ошибки 9916: улучшено сообщение об ошибке из-за конфликта между тегом и другими условиями фильтра для команды `az resource list`.</span><span class="sxs-lookup"><span data-stu-id="4a611-777">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="4a611-778">Добавлен новый параметр `--managed-by` для добавления данных managedBy для команды `az group create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-778">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="4a611-779">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="4a611-779">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="4a611-780">Добавлена подгруппа `monitor` для управления мониторингом Log Analytics в кластере Azure Red Hat OpensShift.</span><span class="sxs-lookup"><span data-stu-id="4a611-780">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="4a611-781">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4a611-781">BotService</span></span>

* <span data-ttu-id="4a611-782">Исправление ошибки 11697: команда `az bot create` не являлась идемпотентной.</span><span class="sxs-lookup"><span data-stu-id="4a611-782">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="4a611-783">Проверки исправления имен изменены для выполнения только в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="4a611-783">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="4a611-784">CDN</span><span class="sxs-lookup"><span data-stu-id="4a611-784">CDN</span></span>

* <span data-ttu-id="4a611-785">Добавлена поддержка функции rulesEngine.</span><span class="sxs-lookup"><span data-stu-id="4a611-785">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="4a611-786">Добавлена новая группа команд cdn endpoint rule для управления правилами.</span><span class="sxs-lookup"><span data-stu-id="4a611-786">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="4a611-787">Пакет azure-mgmt-cdn обновлен до версии 4.0.0 для использования API версии 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="4a611-787">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="4a611-788">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="4a611-788">Deployment Manager</span></span>

* <span data-ttu-id="4a611-789">Добавлена операция вывода списка всех ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a611-789">Add list operation for all resources.</span></span>
* <span data-ttu-id="4a611-790">Улучшен ресурс шага для нового типа шага.</span><span class="sxs-lookup"><span data-stu-id="4a611-790">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="4a611-791">Пакет azure-mgmt-deploymentmanager обновлен для использования версии 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="4a611-791">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-792">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-792">IoT</span></span>

* <span data-ttu-id="4a611-793">Команды IoT hub Job объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="4a611-793">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="4a611-794">IoT Central</span><span class="sxs-lookup"><span data-stu-id="4a611-794">IoT Central</span></span>

* <span data-ttu-id="4a611-795">Добавлена поддержка создания и обновления приложений с новыми SKU: ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="4a611-795">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="4a611-796">Key Vault</span><span class="sxs-lookup"><span data-stu-id="4a611-796">Key Vault</span></span>

* <span data-ttu-id="4a611-797">Добавлена новая команда `az keyvault key download` для скачивания ключей.</span><span class="sxs-lookup"><span data-stu-id="4a611-797">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="4a611-798">Разное</span><span class="sxs-lookup"><span data-stu-id="4a611-798">Misc</span></span>

* <span data-ttu-id="4a611-799">Исправление ошибки 6371: поддержка завершения имен файлов и переменных среды в Bash.</span><span class="sxs-lookup"><span data-stu-id="4a611-799">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="4a611-800">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-800">Network</span></span>

* <span data-ttu-id="4a611-801">Исправление ошибки 2092: для команды az network dns record-set add/remove добавлено предупреждение, отображаемое, если набор записей не найден.</span><span class="sxs-lookup"><span data-stu-id="4a611-801">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="4a611-802">В будущем для подтверждения этого автоматического создания будет добавлен дополнительный аргумент.</span><span class="sxs-lookup"><span data-stu-id="4a611-802">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="4a611-803">Политика</span><span class="sxs-lookup"><span data-stu-id="4a611-803">Policy</span></span>

* <span data-ttu-id="4a611-804">Добавлена новая команда `az policy metadata` для получения ресурсов метаданных расширенной политики.</span><span class="sxs-lookup"><span data-stu-id="4a611-804">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="4a611-805">`az policy remediation create`: С помощью параметра `--resource-discovery-mode` можно указать, следует ли повторно оценить соответствие перед исправлением.</span><span class="sxs-lookup"><span data-stu-id="4a611-805">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-806">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-806">Profile</span></span>

* <span data-ttu-id="4a611-807">`az account get-access-token`: Добавлен параметр `--tenant` для получения маркера для арендатора напрямую, без необходимости указывать подписку.</span><span class="sxs-lookup"><span data-stu-id="4a611-807">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="4a611-808">RBAC</span><span class="sxs-lookup"><span data-stu-id="4a611-808">RBAC</span></span>

* <span data-ttu-id="4a611-809">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправление ошибки 11883: `az role assignment create`: пустая область приведет к ошибке.</span><span class="sxs-lookup"><span data-stu-id="4a611-809">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="4a611-810">Безопасность</span><span class="sxs-lookup"><span data-stu-id="4a611-810">Security</span></span>

* <span data-ttu-id="4a611-811">Добавлены новые команды `az atp show` и `az atp update` для просмотра и настройки дополнительных параметров защиты от угроз для учетных записей хранения.</span><span class="sxs-lookup"><span data-stu-id="4a611-811">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-812">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-812">SQL</span></span>

* <span data-ttu-id="4a611-813">`sql dw create`: параметры `--zone-redundant` и `--read-replica-count` объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="4a611-813">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="4a611-814">Эти параметры не применяются к хранилищу данных.</span><span class="sxs-lookup"><span data-stu-id="4a611-814">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="4a611-815">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql db create`: Значения WideWorldImportersStd и WideWorldImportersFull больше не являются задокументированным допустимыми значениями для команды az sql db create --sample-name.</span><span class="sxs-lookup"><span data-stu-id="4a611-815">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="4a611-816">Эти примеры базы данных всегда будут приводить к сбою создания.</span><span class="sxs-lookup"><span data-stu-id="4a611-816">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="4a611-817">Добавлены новые команды `sql db classification show/list/update/delete` и `sql db classification recommendation list/enable/disable` для управления классификациями конфиденциальности баз данных SQL.</span><span class="sxs-lookup"><span data-stu-id="4a611-817">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="4a611-818">`az sql db audit-policy`: устранены пустые действия аудита и группы.</span><span class="sxs-lookup"><span data-stu-id="4a611-818">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-819">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-819">Storage</span></span>

* <span data-ttu-id="4a611-820">Добавлена новая группа команд `az storage share-rm` для использования поставщика ресурсов Microsoft.Storage в операциях управления файловыми ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="4a611-820">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="4a611-821">Исправление ошибки 11415: ошибка разрешения для `az storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-821">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="4a611-822">Добавлены интеграция AzCopy 10.3.3 и поддержка Win32.</span><span class="sxs-lookup"><span data-stu-id="4a611-822">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="4a611-823">`az storage copy`: добавлены параметры `--include-path`, `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="4a611-823">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="4a611-824">`az storage remove`: параметры `--inlcude` и `--exclude` заменены параметрами `--include-path`, `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="4a611-824">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="4a611-825">`az storage sync`: добавлены параметры `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="4a611-825">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="4a611-826">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4a611-826">ServiceFabric</span></span>

* <span data-ttu-id="4a611-827">Добавлены новые команды для управления приложениями и службами.</span><span class="sxs-lookup"><span data-stu-id="4a611-827">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="4a611-828">13 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-828">January 13, 2020</span></span>

<span data-ttu-id="4a611-829">Версия 2.0.80</span><span class="sxs-lookup"><span data-stu-id="4a611-829">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="4a611-830">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4a611-830">Compute</span></span>

* <span data-ttu-id="4a611-831">Обновление диска: добавлены параметры --disk-encryption-set и --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="4a611-831">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="4a611-832">Создание и обновление моментального снимка: добавлены параметры --disk-encryption-set и --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="4a611-832">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-833">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-833">Storage</span></span>

* <span data-ttu-id="4a611-834">Обновление azure-mgmt-storage до версии 7.1.0</span><span class="sxs-lookup"><span data-stu-id="4a611-834">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="4a611-835">`az storage account create`: добавлены параметры `--encryption-key-type-for-table` и `--encryption-key-type-for-queue` для включения поддержки службы шифрования таблиц и очередей.</span><span class="sxs-lookup"><span data-stu-id="4a611-835">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="4a611-836">7 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-836">January 07, 2020</span></span>

<span data-ttu-id="4a611-837">Версия 2.0.79</span><span class="sxs-lookup"><span data-stu-id="4a611-837">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-838">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-838">ACR</span></span>

* <span data-ttu-id="4a611-839">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --os для команд acr build, acr task create/update, acr run и acr pack.</span><span class="sxs-lookup"><span data-stu-id="4a611-839">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="4a611-840">Вместо этого используется параметр --platform.</span><span class="sxs-lookup"><span data-stu-id="4a611-840">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="4a611-841">AppConfig</span><span class="sxs-lookup"><span data-stu-id="4a611-841">AppConfig</span></span>

* <span data-ttu-id="4a611-842">Добавлена поддержка импорта и экспорта флагов функций.</span><span class="sxs-lookup"><span data-stu-id="4a611-842">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="4a611-843">Добавлена новая команда az appconfig kv set-keyvault для создания ссылки на хранилище ключей.</span><span class="sxs-lookup"><span data-stu-id="4a611-843">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="4a611-844">Добавлена поддержка различных соглашений об именовании при экспорте флагов функций в файл.</span><span class="sxs-lookup"><span data-stu-id="4a611-844">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-845">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-845">AppService</span></span>

* <span data-ttu-id="4a611-846">Устранена проблема № 7154: обновлена документация по команде <> — теперь в ней используются обратные, а не одинарные кавычки.</span><span class="sxs-lookup"><span data-stu-id="4a611-846">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="4a611-847">Устранена проблема № 11287 (webapp up): по умолчанию для приложения, созданного с использованием этого флага, должен быть включен SSL.</span><span class="sxs-lookup"><span data-stu-id="4a611-847">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="4a611-848">Устранена проблема № 11592: добавлен флаг az webapp up для статических сайтов HTML.</span><span class="sxs-lookup"><span data-stu-id="4a611-848">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="4a611-849">ARM</span><span class="sxs-lookup"><span data-stu-id="4a611-849">ARM</span></span>

* <span data-ttu-id="4a611-850">Исправлена ошибка с командой `az resource tag`: невозможно было обновить теги хранилища Служб восстановления.</span><span class="sxs-lookup"><span data-stu-id="4a611-850">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="4a611-851">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="4a611-851">Backup</span></span>

* <span data-ttu-id="4a611-852">Добавлена новая команда backup protection undelete для включения функции обратимого удаления рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="4a611-852">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="4a611-853">Добавлен новый параметр --soft-delete-feature-state для команды set backup-properties.</span><span class="sxs-lookup"><span data-stu-id="4a611-853">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="4a611-854">Добавлена поддержка исключения диска для рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="4a611-854">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="4a611-855">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4a611-855">Compute</span></span>

* <span data-ttu-id="4a611-856">Исправлен сбой `vm create` в профиле Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="4a611-856">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="4a611-857">Добавлена поддержка определений списков и метрик запросов для виртуальной машины (vm monitor metrics tail/list-definitions).</span><span class="sxs-lookup"><span data-stu-id="4a611-857">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="4a611-858">Добавлено новое действия повторного применения команды az vm</span><span class="sxs-lookup"><span data-stu-id="4a611-858">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4a611-859">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4a611-859">HDInsight</span></span>

* <span data-ttu-id="4a611-860">Включена поддержка создания кластера Kafka с помощью прокси-сервера Kafka RESTful.</span><span class="sxs-lookup"><span data-stu-id="4a611-860">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="4a611-861">Обновление azure-mgmt-hdinsight до версии 1.3.0</span><span class="sxs-lookup"><span data-stu-id="4a611-861">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="4a611-862">Прочее</span><span class="sxs-lookup"><span data-stu-id="4a611-862">Misc.</span></span>

* <span data-ttu-id="4a611-863">Добавлена команда `az version show` предварительного просмотра для отображения версий модулей и расширений Azure CLI в формате JSON по умолчанию или в формате, настроенном с помощью параметра --output</span><span class="sxs-lookup"><span data-stu-id="4a611-863">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="4a611-864">Центры событий</span><span class="sxs-lookup"><span data-stu-id="4a611-864">Event Hubs</span></span>

* <span data-ttu-id="4a611-865">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az eventhubs eventhub update и az eventhubs eventhub create.</span><span class="sxs-lookup"><span data-stu-id="4a611-865">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="4a611-866">Данный параметр недопустим для сущностей концентратора событий.</span><span class="sxs-lookup"><span data-stu-id="4a611-866">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="4a611-867">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="4a611-867">Service Bus</span></span>

* <span data-ttu-id="4a611-868">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az servicebus topic create, az servicebus topic update, az servicebus queue create и az servicebus queue update.</span><span class="sxs-lookup"><span data-stu-id="4a611-868">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="4a611-869">Этот параметр является недопустимым для разделов и очередей служебной шины.</span><span class="sxs-lookup"><span data-stu-id="4a611-869">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="4a611-870">RBAC</span><span class="sxs-lookup"><span data-stu-id="4a611-870">RBAC</span></span>

* <span data-ttu-id="4a611-871">Устранена проблема № 11712: команда `az ad app/sp show` не возвращала код выхода 3, если приложение или субъект-служба не существует.</span><span class="sxs-lookup"><span data-stu-id="4a611-871">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-872">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-872">Storage</span></span>

* <span data-ttu-id="4a611-873">`az storage account create`: удален флаг предварительного просмотра для параметра --enable-hierarchical-namespace.</span><span class="sxs-lookup"><span data-stu-id="4a611-873">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="4a611-874">Хранилище azure-mgmt-storage обновлено до версии 7.0.0 для использования API версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="4a611-874">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="4a611-875">Добавлены новые параметры (`--enable-delete-retention` и `--delete-retention-days`) для поддержки управления политикой хранения удаленных свойств службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="4a611-875">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="4a611-876">17 декабря 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-876">December 17, 2019</span></span>

<span data-ttu-id="4a611-877">2.0.78</span><span class="sxs-lookup"><span data-stu-id="4a611-877">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-878">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-878">ACR</span></span>

* <span data-ttu-id="4a611-879">Добавлена поддержка локального контекста во время выполнения задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="4a611-879">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-880">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-880">ACS</span></span>

* <span data-ttu-id="4a611-881">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде az openshift create параметр `--workspace-resource-id` переименован на `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="4a611-881">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="4a611-882">AMS</span><span class="sxs-lookup"><span data-stu-id="4a611-882">AMS</span></span>

* <span data-ttu-id="4a611-883">Команды show обновлены для возвращения ответа 3, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="4a611-883">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="4a611-884">AppConfig</span><span class="sxs-lookup"><span data-stu-id="4a611-884">AppConfig</span></span>

* <span data-ttu-id="4a611-885">Исправлена ошибка, возникающая при добавлении api-version в URL-адрес запроса.</span><span class="sxs-lookup"><span data-stu-id="4a611-885">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="4a611-886">Имеющееся решение не работает с разбивкой на страницы.</span><span class="sxs-lookup"><span data-stu-id="4a611-886">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="4a611-887">Добавлена поддержка отображения языков, кроме английского, так как наша внутренняя служба поддерживает Юникод для глобализации.</span><span class="sxs-lookup"><span data-stu-id="4a611-887">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-888">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-888">AppService</span></span>

* <span data-ttu-id="4a611-889">Устранена проблема № 11217 (webapp): теперь команда az webapp config ssl upload поддерживает параметр слота.</span><span class="sxs-lookup"><span data-stu-id="4a611-889">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="4a611-890">Устранена проблема № 10965. Ошибка: Имя не может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="4a611-890">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="4a611-891">Разрешено удаление по IP-адресу и подсети.</span><span class="sxs-lookup"><span data-stu-id="4a611-891">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="4a611-892">Добавлена поддержка импорта сертификатов из хранилища ключей: `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="4a611-892">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="4a611-893">ARM</span><span class="sxs-lookup"><span data-stu-id="4a611-893">ARM</span></span>

* <span data-ttu-id="4a611-894">Обновлен пакет ресурсов azure-mgmt-resource для использования версии 6.0.0</span><span class="sxs-lookup"><span data-stu-id="4a611-894">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="4a611-895">Добавлена межклиентская поддержка команды `az group deployment create` путем добавления нового параметра `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="4a611-895">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="4a611-896">Добавлен новый параметр `--metadata` для поддержки добавления метаданных определений наборов политик.</span><span class="sxs-lookup"><span data-stu-id="4a611-896">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="4a611-897">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="4a611-897">Backup</span></span>

* <span data-ttu-id="4a611-898">Добавлена поддержка резервного копирования для рабочей нагрузки SQL и SAP HANA.</span><span class="sxs-lookup"><span data-stu-id="4a611-898">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="4a611-899">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4a611-899">BotService</span></span>

* <span data-ttu-id="4a611-900">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг --version из предварительной версии команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="4a611-900">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="4a611-901">Поддерживаются только боты пакетов SDK версии 4.</span><span class="sxs-lookup"><span data-stu-id="4a611-901">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="4a611-902">Добавлена проверка доступности имени для команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="4a611-902">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="4a611-903">Добавлена поддержка обновления URL-адреса значка для бота с помощью команды az bot update.</span><span class="sxs-lookup"><span data-stu-id="4a611-903">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="4a611-904">Добавлена поддержка обновления канала Direct Line с помощью команды az bot directline update.</span><span class="sxs-lookup"><span data-stu-id="4a611-904">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="4a611-905">Добавлена поддержка флага --enable-enhanced-auth в команде az bot directline create.</span><span class="sxs-lookup"><span data-stu-id="4a611-905">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="4a611-906">Следующие группы команд предоставляются в общедоступной, а не в предварительной версии: az bot authsetting.</span><span class="sxs-lookup"><span data-stu-id="4a611-906">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="4a611-907">Следующие команды в az bot предоставляются в общедоступной, а не в предварительной версии: create, prepare-deploy, show, delete и update.</span><span class="sxs-lookup"><span data-stu-id="4a611-907">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="4a611-908">Устранена проблема с командой az bot prepare-deploy, которая изменяла значение параметра --proj-file-path на нижний регистр (например, с Test.csproj на test.csproj).</span><span class="sxs-lookup"><span data-stu-id="4a611-908">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="4a611-909">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4a611-909">Compute</span></span>

* <span data-ttu-id="4a611-910">vmss create/update: добавлен параметр --scale-on-policy, который определяет, какие виртуальные машины выбираются для удаления при масштабировании VMSS.</span><span class="sxs-lookup"><span data-stu-id="4a611-910">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="4a611-911">vm/vmss update: добавлен параметр --priority.</span><span class="sxs-lookup"><span data-stu-id="4a611-911">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="4a611-912">vm/vmss update: добавлен параметр --max-price.</span><span class="sxs-lookup"><span data-stu-id="4a611-912">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="4a611-913">Добавлена группа команд для шифрования дисков (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="4a611-913">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="4a611-914">disk create: добавлены параметры --encryption-type и --disk-encryption-set.</span><span class="sxs-lookup"><span data-stu-id="4a611-914">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="4a611-915">vm/vmss create. Добавлены параметры --os-disk-encryption-set и --data-disk-encryption-sets.</span><span class="sxs-lookup"><span data-stu-id="4a611-915">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="4a611-916">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-916">Core</span></span>

* <span data-ttu-id="4a611-917">Удалена поддержка Python версии 3.4.</span><span class="sxs-lookup"><span data-stu-id="4a611-917">Removed support for Python 3.4</span></span>
* <span data-ttu-id="4a611-918">Подключение к опросу HaTS в нескольких командах.</span><span class="sxs-lookup"><span data-stu-id="4a611-918">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="4a611-919">DLS</span><span class="sxs-lookup"><span data-stu-id="4a611-919">DLS</span></span>

* <span data-ttu-id="4a611-920">Обновлена версия пакета SDK для ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="4a611-920">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="4a611-921">Установка</span><span class="sxs-lookup"><span data-stu-id="4a611-921">Install</span></span>

* <span data-ttu-id="4a611-922">Добавлена поддержка установки скриптов Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="4a611-922">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-923">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-923">IOT</span></span>

* <span data-ttu-id="4a611-924">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --failover-region из команды manual-failover.</span><span class="sxs-lookup"><span data-stu-id="4a611-924">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="4a611-925">Теперь она будет выполнять отработку отказа в назначенный геопарный дополнительный регион.</span><span class="sxs-lookup"><span data-stu-id="4a611-925">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="4a611-926">Key Vault</span><span class="sxs-lookup"><span data-stu-id="4a611-926">Key Vault</span></span>

* <span data-ttu-id="4a611-927">Устранена проблема № 8095: (`az keyvault storage remove`): улучшено справочное сообщение.</span><span class="sxs-lookup"><span data-stu-id="4a611-927">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="4a611-928">Устранена проблема № 8921 (`az keyvault key/secret/certificate list/list-deleted/list-versions`): исправлена ошибка проверки в параметре `--maxresults`.</span><span class="sxs-lookup"><span data-stu-id="4a611-928">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="4a611-929">Устранена проблема № 10512 (`az keyvault set-policy`): улучшено сообщение об ошибке, возвращаемое, если не указан ни один из параметров `--object-id`, `--spn` или `--upn`.</span><span class="sxs-lookup"><span data-stu-id="4a611-929">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="4a611-930">Устранена проблема № 10846 (`az keyvault secret show-deleted`): при указании значения `--id` значение `--name/-n` не требовалось.</span><span class="sxs-lookup"><span data-stu-id="4a611-930">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="4a611-931">Устранена проблема № 11084: (`az keyvault secret download`): улучшено справочное сообщение параметра `--encoding`.</span><span class="sxs-lookup"><span data-stu-id="4a611-931">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="4a611-932">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-932">Network</span></span>

* <span data-ttu-id="4a611-933">az network application-gateway probe: добавлена поддержка параметра --port, позволяющего указать порт, который используется для проверки внутренних серверов при создании и обновлении.</span><span class="sxs-lookup"><span data-stu-id="4a611-933">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="4a611-934">az network application-gateway url-path-map create/update: исправлена ошибка с `--waf-policy`.</span><span class="sxs-lookup"><span data-stu-id="4a611-934">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="4a611-935">az network application-gateway: добавлена поддержка параметра `--rewrite-rule-set`.</span><span class="sxs-lookup"><span data-stu-id="4a611-935">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="4a611-936">az network list-service-aliases: добавлена поддержка перечисления псевдонимов служб, которые можно использовать для политик конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="4a611-936">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="4a611-937">az network dns zone import: добавлена поддержка символа .@ в имени записи.</span><span class="sxs-lookup"><span data-stu-id="4a611-937">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="4a611-938">Упаковка</span><span class="sxs-lookup"><span data-stu-id="4a611-938">Packaging</span></span>

* <span data-ttu-id="4a611-939">Снова добавлены сборки Edge для установки PIP.</span><span class="sxs-lookup"><span data-stu-id="4a611-939">Added back edge builds for pip install</span></span>
* <span data-ttu-id="4a611-940">Добавлен пакет Ubuntu eoan.</span><span class="sxs-lookup"><span data-stu-id="4a611-940">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="4a611-941">Политика</span><span class="sxs-lookup"><span data-stu-id="4a611-941">Policy</span></span>

* <span data-ttu-id="4a611-942">Добавлена поддержка API Политики версии 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="4a611-942">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="4a611-943">az policy set-definition: добавлена поддержка группирования в определениях наборов политик с помощью параметра `--definition-groups`.</span><span class="sxs-lookup"><span data-stu-id="4a611-943">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="4a611-944">Redis</span><span class="sxs-lookup"><span data-stu-id="4a611-944">Redis</span></span>

* <span data-ttu-id="4a611-945">В команду `az redis create` добавлена предварительная версия параметра `--replicas-per-master`.</span><span class="sxs-lookup"><span data-stu-id="4a611-945">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="4a611-946">Обновлена версия azure-mgmt-redis с 6.0.0 на 7.0.0 RC1.</span><span class="sxs-lookup"><span data-stu-id="4a611-946">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="4a611-947">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4a611-947">ServiceFabric</span></span>

* <span data-ttu-id="4a611-948">Исправлена логика добавления типа узла, а также устранена проблема № 10963: при добавлении нового типа узла с уровнем устойчивости Gold возникала ошибка CLI.</span><span class="sxs-lookup"><span data-stu-id="4a611-948">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="4a611-949">Обновлена версия параметра ServiceFabricNodeVmExt до 1.1 в шаблоне создания.</span><span class="sxs-lookup"><span data-stu-id="4a611-949">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-950">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-950">SQL</span></span>

* <span data-ttu-id="4a611-951">В команды create и update базы данных SQL добавлены параметры --read-scale и --read-replicas для поддержки управления масштабированием операций чтения.</span><span class="sxs-lookup"><span data-stu-id="4a611-951">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-952">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-952">Storage</span></span>

* <span data-ttu-id="4a611-953">Выпущена общедоступная версия больших файловых ресурсов для команды создания и обновления учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="4a611-953">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="4a611-954">Выпущена общедоступная версия поддержки маркера SAS для делегирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="4a611-954">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="4a611-955">Добавлены новые команды (`az storage account blob-service-properties show` и `az storage account blob-service-properties update --enable-change-feed`) для управления свойствами службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="4a611-955">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="4a611-956">[ОЖИДАЕТСЯ КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] `az storage copy`: символ `*` больше не поддерживается в качестве подстановочного знака в URL-адресе. Тем не менее новые параметры--include-pattern и--exclude-pattern будут добавлены с поддержкой подстановочных знаков `*`.</span><span class="sxs-lookup"><span data-stu-id="4a611-956">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="4a611-957">Устранена проблема № 11043: добавлена поддержка удаления всего контейнера или общего ресурса в команде `az storage remove`.</span><span class="sxs-lookup"><span data-stu-id="4a611-957">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="4a611-958">26 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-958">November 26, 2019</span></span>

<span data-ttu-id="4a611-959">Версия 2.0.77</span><span class="sxs-lookup"><span data-stu-id="4a611-959">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-960">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-960">ACR</span></span>

* <span data-ttu-id="4a611-961">Параметр `--branch`, используемый при обновлении или создании задачи ACR, объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="4a611-961">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="4a611-962">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="4a611-962">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="4a611-963">Добавлен флаг `--workspace-resource-id` для создания кластера Azure Red Hat Openshift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="4a611-963">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="4a611-964">Добавлен флаг `monitor_profile` для создания кластера Azure Red Hat OpenShift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="4a611-964">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="4a611-965">AKS</span><span class="sxs-lookup"><span data-stu-id="4a611-965">AKS</span></span>

* <span data-ttu-id="4a611-966">Включена поддержка операции смены сертификата кластера с использованием команды az aks rotate-certs.</span><span class="sxs-lookup"><span data-stu-id="4a611-966">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="4a611-967">AppConfig</span><span class="sxs-lookup"><span data-stu-id="4a611-967">AppConfig</span></span>

* <span data-ttu-id="4a611-968">Включена поддержка использования символа ":" для разделителя `as az appconfig kv import`.</span><span class="sxs-lookup"><span data-stu-id="4a611-968">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="4a611-969">Исправлена проблема с перечислением значений ключей с несколькими метками, включая метку NULL.</span><span class="sxs-lookup"><span data-stu-id="4a611-969">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="4a611-970">Обновлен пакет SDK для плоскости управления, azure-mgmt-appconfiguration, до версии 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="4a611-970">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="4a611-971">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-971">AppService</span></span>

* <span data-ttu-id="4a611-972">Исправлена ошибка № 11100. Использование AttributeError для az webapp up при создании плана службы.</span><span class="sxs-lookup"><span data-stu-id="4a611-972">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="4a611-973">az webapp up. При принудительном создании или развертывании сайта для поддерживаемых языков значения по умолчанию не используются.</span><span class="sxs-lookup"><span data-stu-id="4a611-973">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="4a611-974">Включена поддержка Среды службы приложений: az appservice ase show | list | list-addresses | list-plans | create | update | delete.</span><span class="sxs-lookup"><span data-stu-id="4a611-974">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="4a611-975">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="4a611-975">Backup</span></span>

* <span data-ttu-id="4a611-976">Исправлена проблема в команде az backup policy list-associated-items.</span><span class="sxs-lookup"><span data-stu-id="4a611-976">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="4a611-977">Добавлен необязательный параметр BackupManagementType.</span><span class="sxs-lookup"><span data-stu-id="4a611-977">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="4a611-978">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4a611-978">Compute</span></span>

* <span data-ttu-id="4a611-979">Обновлена версия API вычислений, дисков, моментальных снимков до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="4a611-979">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="4a611-980">vmss create. Улучшение для --orchestration-mode.</span><span class="sxs-lookup"><span data-stu-id="4a611-980">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="4a611-981">sig image-definition create. Добавлен параметр --os-state для указания того, являются ли виртуальные машины, созданные в этом образе, универсальными или специализированными.</span><span class="sxs-lookup"><span data-stu-id="4a611-981">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="4a611-982">sig image-definition create. Добавлен параметр --hyper-v-generation для указания создания гипервизора.</span><span class="sxs-lookup"><span data-stu-id="4a611-982">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="4a611-983">sig image-version create. Включена поддержка параметров --os-snapshot и --data-snapshots.</span><span class="sxs-lookup"><span data-stu-id="4a611-983">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="4a611-984">image create. Включена поддержка параметра --data-disk-caching для указания параметра кэширования для дисков данных.</span><span class="sxs-lookup"><span data-stu-id="4a611-984">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="4a611-985">Обновлена версия пакета SDK для вычислений Python до 10.0.0.</span><span class="sxs-lookup"><span data-stu-id="4a611-985">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="4a611-986">vm/vmss create. Добавлен фрагмент Spot в свойство перечисления Priority.</span><span class="sxs-lookup"><span data-stu-id="4a611-986">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="4a611-987">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименование параметра --max-billing в --max-price для виртуальных машин и Масштабируемых наборов виртуальных машин в соответствии с командлетами Swagger и PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4a611-987">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="4a611-988">vm monitor log show. Включена поддержка запроса журналов в связанной рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="4a611-988">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-989">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-989">IOT</span></span>

* <span data-ttu-id="4a611-990">Исправление № 2531. Добавлены вспомогательные аргументы для обновления концентратора.</span><span class="sxs-lookup"><span data-stu-id="4a611-990">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="4a611-991">Исправление № 8323. Добавлены недостающие параметры для создания пользовательской конечной точки хранилища.</span><span class="sxs-lookup"><span data-stu-id="4a611-991">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="4a611-992">Исправлена ошибка регрессии. Отменены изменения, переопределяющие конечную точку хранилища по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-992">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="4a611-993">Key Vault</span><span class="sxs-lookup"><span data-stu-id="4a611-993">Key Vault</span></span>

* <span data-ttu-id="4a611-994">Исправление № 11121. При использовании `az keyvault certificate list` для передачи `--include-pending` теперь не требуется значение `true` или `false`.</span><span class="sxs-lookup"><span data-stu-id="4a611-994">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="4a611-995">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="4a611-995">NetAppFiles</span></span>

* <span data-ttu-id="4a611-996">Обновлена версия azure-mgmt-netapp до 0.7.0, которая включает некоторые дополнительные свойства тома, связанные с предстоящими операциями репликации.</span><span class="sxs-lookup"><span data-stu-id="4a611-996">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="4a611-997">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-997">Network</span></span>

* <span data-ttu-id="4a611-998">application-gateway waf-config. Не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="4a611-998">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="4a611-999">application-gateway waf-policy. Добавлены управляемые правила подгрупп для контроля управляемых наборов правил и правил исключения.</span><span class="sxs-lookup"><span data-stu-id="4a611-999">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="4a611-1000">application-gateway waf-policy. Добавлен параметр политики подгруппы для управления глобальной конфигурацией политики WAF.</span><span class="sxs-lookup"><span data-stu-id="4a611-1000">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="4a611-1001">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] application-gateway waf-policy. Переименовано правило подгруппы в пользовательское правило.</span><span class="sxs-lookup"><span data-stu-id="4a611-1001">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="4a611-1002">application-gateway http-listener. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="4a611-1002">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="4a611-1003">application-gateway url-path-map rule. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="4a611-1003">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="4a611-1004">Упаковка</span><span class="sxs-lookup"><span data-stu-id="4a611-1004">Packaging</span></span>

* <span data-ttu-id="4a611-1005">Удалена команда az wrapper в Python.</span><span class="sxs-lookup"><span data-stu-id="4a611-1005">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="4a611-1006">Включена поддержка Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="4a611-1006">Added support for Python 3.8</span></span>
* <span data-ttu-id="4a611-1007">Изменена версия на Python 3 для пакета RPM.</span><span class="sxs-lookup"><span data-stu-id="4a611-1007">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-1008">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-1008">Profile</span></span>

* <span data-ttu-id="4a611-1009">Исправлена ошибка при выполнении `az login -u {} -p {}` с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="4a611-1009">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="4a611-1010">Исправлена ошибка с `SSLError` при выполнении `az login` за прокси-сервером с самозаверяющим корневым сертификатом.</span><span class="sxs-lookup"><span data-stu-id="4a611-1010">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="4a611-1011">Исправлена ошибка № 10578. `az login` зависает при одновременном запуске нескольких экземпляров в Windows или WSL.</span><span class="sxs-lookup"><span data-stu-id="4a611-1011">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="4a611-1012">Исправлена ошибка № 11059. Сбой выполнения `az login --allow-no-subscriptions`, если в клиенте есть подписки.</span><span class="sxs-lookup"><span data-stu-id="4a611-1012">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="4a611-1013">Исправлена ошибка № 11238. После переименования подписки вход с помощью MSI приведет к тому, что одна и та же подписка появится дважды.</span><span class="sxs-lookup"><span data-stu-id="4a611-1013">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="4a611-1014">RBAC</span><span class="sxs-lookup"><span data-stu-id="4a611-1014">RBAC</span></span>

* <span data-ttu-id="4a611-1015">Исправлена ошибка № 10996. Исправлена ошибка с `--force-change-password-next-login` в `az ad user update`, если `--password` не указывается.</span><span class="sxs-lookup"><span data-stu-id="4a611-1015">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="4a611-1016">Redis</span><span class="sxs-lookup"><span data-stu-id="4a611-1016">Redis</span></span>

* <span data-ttu-id="4a611-1017">Исправлена ошибка № 2902. Предотвращена настройка конфигураций памяти при обновлении кэша с номером SKU "Базовый".</span><span class="sxs-lookup"><span data-stu-id="4a611-1017">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="4a611-1018">Резервирование</span><span class="sxs-lookup"><span data-stu-id="4a611-1018">Reservations</span></span>

* <span data-ttu-id="4a611-1019">Обновлена версия пакета SDK до 0.6.0</span><span class="sxs-lookup"><span data-stu-id="4a611-1019">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="4a611-1020">Добавлены сведения о плане выставления счетов после вызова Get-Catalogs.</span><span class="sxs-lookup"><span data-stu-id="4a611-1020">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="4a611-1021">Добавлена новая команда `az reservations reservation-order calculate` для вычисления стоимости резервирования.</span><span class="sxs-lookup"><span data-stu-id="4a611-1021">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="4a611-1022">Добавлена новая команда `az reservations reservation-order purchase` для приобретения нового резервирования.</span><span class="sxs-lookup"><span data-stu-id="4a611-1022">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="4a611-1023">Rest</span><span class="sxs-lookup"><span data-stu-id="4a611-1023">Rest</span></span>
* <span data-ttu-id="4a611-1024">Изменена версия `az rest` на общедоступную.</span><span class="sxs-lookup"><span data-stu-id="4a611-1024">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-1025">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-1025">SQL</span></span>

* <span data-ttu-id="4a611-1026">Обновлена версия azure-mgmt-sql до 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="4a611-1026">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-1027">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-1027">Storage</span></span>

* <span data-ttu-id="4a611-1028">storage account create. Добавлен параметр --enable-hierarchical-namespace для включения поддержки семантики файловой системы в службе больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1028">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="4a611-1029">Удалено несвязанное исключение из сообщения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="4a611-1029">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="4a611-1030">Исправлены проблемы, из-за которых появлялось неверное сообщение об отсутствии нужных разрешений на выполнение требуемой операции</span><span class="sxs-lookup"><span data-stu-id="4a611-1030">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="4a611-1031">при блокировке правилами сети (AuthenticationFailed).</span><span class="sxs-lookup"><span data-stu-id="4a611-1031">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="4a611-1032">4 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1032">November 4, 2019</span></span>

<span data-ttu-id="4a611-1033">Версия 2.0.76</span><span class="sxs-lookup"><span data-stu-id="4a611-1033">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-1034">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-1034">ACR</span></span>

* <span data-ttu-id="4a611-1035">В команду `az acr pack build` добавлен параметр предварительной версии `--pack-image-tag`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1035">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="4a611-1036">Добавлена поддержка включения аудита при создании реестра.</span><span class="sxs-lookup"><span data-stu-id="4a611-1036">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="4a611-1037">Включена поддержка функции RBAC, распространяющаяся на репозиторий.</span><span class="sxs-lookup"><span data-stu-id="4a611-1037">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="4a611-1038">AKS</span><span class="sxs-lookup"><span data-stu-id="4a611-1038">AKS</span></span>

* <span data-ttu-id="4a611-1039">В команду `az aks create` добавлены `--enable-cluster-autoscaler`, `--min-count` и `--max-count`, что позволяет автоматически масштабировать кластер для пула узлов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1039">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="4a611-1040">Добавлены указанные выше флаги, а также `--update-cluster-autoscaler` и `--disable-cluster-autoscaler` в команду `az aks update`, что позволяет обновлять средство автоматического масштабирования кластера.</span><span class="sxs-lookup"><span data-stu-id="4a611-1040">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="4a611-1041">AppConfig</span><span class="sxs-lookup"><span data-stu-id="4a611-1041">AppConfig</span></span>

* <span data-ttu-id="4a611-1042">Добавлена группа команд функции appconfig для управления флагами функций, хранимыми в Конфигурации приложений.</span><span class="sxs-lookup"><span data-stu-id="4a611-1042">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="4a611-1043">Исправлена незначительная ошибка команды экспорта в файл appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="4a611-1043">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="4a611-1044">Прерывание чтения содержимого конечного файла во время экспорта.</span><span class="sxs-lookup"><span data-stu-id="4a611-1044">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-1045">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-1045">AppService</span></span>

* <span data-ttu-id="4a611-1046">`az appservice plan create`: Добавлена поддержка определения persitescaling при создании плана appservice.</span><span class="sxs-lookup"><span data-stu-id="4a611-1046">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="4a611-1047">Исправлена проблема, из-за которой операция webapp config ssl bind удаляла существующие теги из ресурса.</span><span class="sxs-lookup"><span data-stu-id="4a611-1047">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="4a611-1048">Добавлен флаг `--build-remote` для `az functionapp deployment source config-zip` для включения поддержки действия удаленной сборки во время развертывания приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="4a611-1048">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="4a611-1049">Изменена версия узла по умолчанию для приложений-функций на ~10 для Windows</span><span class="sxs-lookup"><span data-stu-id="4a611-1049">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="4a611-1050">В `az functionapp create` добавлено свойство `--runtime-version`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1050">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="4a611-1051">ARM</span><span class="sxs-lookup"><span data-stu-id="4a611-1051">ARM</span></span>

* <span data-ttu-id="4a611-1052">`az deployment/group deployment validate`: В `--handle-extended-json-format` добавлен параметр для включения поддержки многострочности и комментариев в шаблоне JSON при развертывании.</span><span class="sxs-lookup"><span data-stu-id="4a611-1052">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="4a611-1053">Версия azure-mgmt-resource обновлена до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="4a611-1053">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="4a611-1054">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="4a611-1054">Backup</span></span>

* <span data-ttu-id="4a611-1055">Добавлена поддержка резервного копирования AzureFiles.</span><span class="sxs-lookup"><span data-stu-id="4a611-1055">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="4a611-1056">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4a611-1056">Compute</span></span>

* <span data-ttu-id="4a611-1057">`az vm create`: Добавлено предупреждение при одновременном определении ускоренной сети и существующей сетевой карты.</span><span class="sxs-lookup"><span data-stu-id="4a611-1057">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="4a611-1058">`az vm create`: Добавлен параметр `--vmss` для определения существующего масштабируемого набора виртуальных машин, которому должна быть назначена виртуальная машина.</span><span class="sxs-lookup"><span data-stu-id="4a611-1058">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="4a611-1059">`az vm/vmss create`: Добавлена локальная копия файла псевдонима изображения, к которой можно получить доступ в ограниченной сетевой среде.</span><span class="sxs-lookup"><span data-stu-id="4a611-1059">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="4a611-1060">`az vmss create`: Добавлен параметр `--orchestration-mode` для определения того, как виртуальные машины управляются масштабируемым набором.</span><span class="sxs-lookup"><span data-stu-id="4a611-1060">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="4a611-1061">`az vm/vmss update`: Добавлен параметр `--ultra-ssd-enabled`, чтобы разрешить обновление параметра Ultra SSD.</span><span class="sxs-lookup"><span data-stu-id="4a611-1061">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="4a611-1062">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az vm extension set`: Исправлена ошибка, из-за которой пользователям не удавалось определять расширение на виртуальной машине с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1062">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="4a611-1063">Добавлены новые команды `az vm image terms accept/cancel/show` для управления условиями использования образов Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="4a611-1063">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="4a611-1064">Расширение VMAccessForLinux обновлено до версии 1.5.</span><span class="sxs-lookup"><span data-stu-id="4a611-1064">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4a611-1065">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-1065">CosmosDB</span></span>

* <span data-ttu-id="4a611-1066">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql container create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4a611-1066">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="4a611-1067">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az gremlin graph create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4a611-1067">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="4a611-1068">`az sql container create`: Добавлены команды `--unique-key-policy` и `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1068">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="4a611-1069">`az sql container create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-1069">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="4a611-1070">`gremlin graph create`: Добавлена команда `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1070">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="4a611-1071">`gremlin graph create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-1071">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="4a611-1072">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="4a611-1072">Fixed typo in help message</span></span>
* <span data-ttu-id="4a611-1073">База данных: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="4a611-1073">database: Added deprecation information</span></span>
* <span data-ttu-id="4a611-1074">Коллекция: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="4a611-1074">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-1075">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-1075">IoT</span></span>

* <span data-ttu-id="4a611-1076">Добавлен новый тип источника маршрутизации: DigitalTwinChangeEvents.</span><span class="sxs-lookup"><span data-stu-id="4a611-1076">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="4a611-1077">Добавлены отсутствующие компоненты в `az iot hub create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1077">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="4a611-1078">Key Vault</span><span class="sxs-lookup"><span data-stu-id="4a611-1078">Key Vault</span></span>

* <span data-ttu-id="4a611-1079">Исправлена непредвиденная ошибка с отсутствием файла сертификата.</span><span class="sxs-lookup"><span data-stu-id="4a611-1079">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="4a611-1080">Исправлена ошибка с неработающей командой `az keyvault recover/purge`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1080">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="4a611-1081">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="4a611-1081">NetAppFiles</span></span>

* <span data-ttu-id="4a611-1082">Пакет azure-mgmt-netapp обновлен до версии 0.6.0 для включения поддержки API версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="4a611-1082">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="4a611-1083">Эта новая версия API включает:</span><span class="sxs-lookup"><span data-stu-id="4a611-1083">This new API version includes:</span></span>

    - <span data-ttu-id="4a611-1084">При создании тома с использованием `--protocol-types` допускается NFSv4.1 вместо NFSv4.</span><span class="sxs-lookup"><span data-stu-id="4a611-1084">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="4a611-1085">Свойство политики экспорта томов теперь называется nfsv41, а не nfsv4.</span><span class="sxs-lookup"><span data-stu-id="4a611-1085">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="4a611-1086">Параметр `--creation-token` для тома переименован в `--file-path`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1086">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="4a611-1087">Дата создания моментального снимка теперь имеет значение Created.</span><span class="sxs-lookup"><span data-stu-id="4a611-1087">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="4a611-1088">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-1088">Network</span></span>

* <span data-ttu-id="4a611-1089">`az network private-dns link vnet create/update`: Добавлена поддержка связывания виртуальных сетей между клиентами.</span><span class="sxs-lookup"><span data-stu-id="4a611-1089">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="4a611-1090">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az network vnet subnet list`: Параметры `--resource-group` и `--vnet-name` теперь являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="4a611-1090">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="4a611-1091">`az network public-ip prefix create`: Включена поддержка определения версии IP-адреса (IPv4, IPv6) при создании.</span><span class="sxs-lookup"><span data-stu-id="4a611-1091">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="4a611-1092">Версия azure-mgmt-network обновлена до 7.0.0 и версия api-version до 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="4a611-1092">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="4a611-1093">`az network vrouter`: Включена поддержка нового виртуального маршрутизатора службы и пиринга виртуальных маршрутизаторов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1093">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="4a611-1094">`az network express-route gateway connection`: Добавлена поддержка параметра `--internet-security`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1094">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-1095">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-1095">Profile</span></span>

* <span data-ttu-id="4a611-1096">Исправлена ошибка с неработающей командой `az account get-access-token --resource-type ms-graph`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1096">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="4a611-1097">Удалено предупреждение из `az login`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1097">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="4a611-1098">RBAC</span><span class="sxs-lookup"><span data-stu-id="4a611-1098">RBAC</span></span>

* <span data-ttu-id="4a611-1099">Исправление `az ad app update --id {} --display-name {}` не работает.</span><span class="sxs-lookup"><span data-stu-id="4a611-1099">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="4a611-1100">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4a611-1100">ServiceFabric</span></span>

* <span data-ttu-id="4a611-1101">`az sf cluster create`: Исправлена проблема путем изменения VMSS для вычислений с использованием файла template.json для Service Fabric Linux и Windows со стандартных дисков на управляемые.</span><span class="sxs-lookup"><span data-stu-id="4a611-1101">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-1102">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-1102">SQL</span></span>

* <span data-ttu-id="4a611-1103">Добавлены параметры `--compute-model`, `--auto-pause-delay` и `--min-capacity` для включения поддержки операций CRUD для нового предложения Базы данных SQL: Модель бессерверных вычислений.</span><span class="sxs-lookup"><span data-stu-id="4a611-1103">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-1104">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-1104">Storage</span></span>

* <span data-ttu-id="4a611-1105">`az storage account create/update`: Добавлен параметр --enable-files-adds и группа аргументов свойств Azure Active Directory для включения поддержки аутентификации доменных служб Azure Active Directory для Файлов Azure.</span><span class="sxs-lookup"><span data-stu-id="4a611-1105">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="4a611-1106">Расширена команда `az storage account keys list/renew` для включения поддержки перечисления или повторного создания ключей Kerberos для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="4a611-1106">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="4a611-1107">15 октября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1107">October 15, 2019</span></span>

<span data-ttu-id="4a611-1108">Версия 2.0.75</span><span class="sxs-lookup"><span data-stu-id="4a611-1108">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="4a611-1109">AKS</span><span class="sxs-lookup"><span data-stu-id="4a611-1109">AKS</span></span>

* <span data-ttu-id="4a611-1110">Для параметра `--load-balancer-sku` изменено значение по умолчанию на `standard`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="4a611-1110">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="4a611-1111">Для параметра `--vm-set-type` изменено значение по умолчанию на `virtualmachinescalesets`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="4a611-1111">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="4a611-1112">AMS</span><span class="sxs-lookup"><span data-stu-id="4a611-1112">AMS</span></span>

* <span data-ttu-id="4a611-1113">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя `job start` изменено на `job create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1113">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="4a611-1114">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В параметре `--ask` команды `content-key-policy create` вместо кодировки UTF8 теперь используется шестнадцатеричная строка из 32 символов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1114">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-1115">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-1115">AppService</span></span>

* <span data-ttu-id="4a611-1116">Добавлены команды `webapp config access-restriction show|set|add|remove`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1116">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="4a611-1117">Улучшена обработка ошибок в `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1117">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="4a611-1118">Для `appservice plan update` добавлена поддержка номера SKU `Isolated`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1118">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="4a611-1119">ARM</span><span class="sxs-lookup"><span data-stu-id="4a611-1119">ARM</span></span>

* <span data-ttu-id="4a611-1120">В `deployment create` добавлен параметр `--handle-extended-json-format` для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="4a611-1120">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="4a611-1121">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4a611-1121">Compute</span></span>

* <span data-ttu-id="4a611-1122">Добавлен параметр `--enable-agent` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1122">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="4a611-1123">Внесены изменения в `vm create`, позволяющие автоматически использовать номер SKU "Стандартный" для общедоступных IP-адресов при использовании зон.</span><span class="sxs-lookup"><span data-stu-id="4a611-1123">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="4a611-1124">Внесены изменения в `vm create`, позволяющие автоматически создавать допустимое имя для виртуальной машины, если оно не задано.</span><span class="sxs-lookup"><span data-stu-id="4a611-1124">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="4a611-1125">В `vmss create` добавлен параметр `--computer-name-prefix` для поддержки пользовательского префикса имени для виртуальных машин в VMSS.</span><span class="sxs-lookup"><span data-stu-id="4a611-1125">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="4a611-1126">В `vm create` добавлен параметр `--workspace` для автоматического включения рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="4a611-1126">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="4a611-1127">API коллекций обновлен до версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="4a611-1127">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="4a611-1128">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-1128">Core</span></span>

* <span data-ttu-id="4a611-1129">Добавлена проверка синтаксиса для параметра `--set` в универсальной команде обновления.</span><span class="sxs-lookup"><span data-stu-id="4a611-1129">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-1130">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-1130">IoT</span></span>

* <span data-ttu-id="4a611-1131">Исправлена проблема, при которой `iot hub show` неправильно выдавал ошибку "Ресурс не найден".</span><span class="sxs-lookup"><span data-stu-id="4a611-1131">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-1132">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-1132">Monitor</span></span>

* <span data-ttu-id="4a611-1133">В `monitor log-analytics workspace` добавлена поддержка CRUD.</span><span class="sxs-lookup"><span data-stu-id="4a611-1133">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="4a611-1134">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-1134">Network</span></span>

* <span data-ttu-id="4a611-1135">В `network private-dns link vnet [create|update]` добавлена поддержка виртуального канала для клиентов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1135">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="4a611-1136">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для `network vnet subnet list` теперь требуются параметры `--resource-group` и `--vnet-name`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1136">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-1137">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-1137">SQL</span></span>

* <span data-ttu-id="4a611-1138">В `sql mi ad-admin` добавлены команды, которые поддерживают назначение администратора AAD в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="4a611-1138">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-1139">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-1139">Storage</span></span>

* <span data-ttu-id="4a611-1140">В `storage copy` добавлен параметр `--preserve-s2s-access-tier`, позволяющий сохранить уровень доступа во время копирования между службами.</span><span class="sxs-lookup"><span data-stu-id="4a611-1140">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="4a611-1141">В `storage account [create|update]` добавлен параметр `--enable-large-file-share` для поддержки общих папок большого размера в учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="4a611-1141">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="4a611-1142">24 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1142">September 24, 2019</span></span>

<span data-ttu-id="4a611-1143">Версия 2.0.74</span><span class="sxs-lookup"><span data-stu-id="4a611-1143">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-1144">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-1144">ACR</span></span>

* <span data-ttu-id="4a611-1145">В `acr config retention update` добавлен обязательный параметр `--type`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1145">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="4a611-1146">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованный параметр `--name -n` изменен на `--registry -r ` для группы команд `acr config`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1146">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="4a611-1147">AKS</span><span class="sxs-lookup"><span data-stu-id="4a611-1147">AKS</span></span>

* <span data-ttu-id="4a611-1148">В команду `aks create` добавлен параметр `--load-balancer-sku`, позволяющий создать кластер AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="4a611-1148">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="4a611-1149">В команды `aks [create|update]` добавлены параметры `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` и `--load-balancer-outbound-ip-prefixes`, позволяющие обновлять профиль подсистемы балансировки нагрузки у кластера AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="4a611-1149">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="4a611-1150">В команду `aks create` добавлен параметр `--vm-set-type`, позволяющий указывать типы виртуальных машин в кластере AKS.</span><span class="sxs-lookup"><span data-stu-id="4a611-1150">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="4a611-1151">ARM</span><span class="sxs-lookup"><span data-stu-id="4a611-1151">ARM</span></span>

* <span data-ttu-id="4a611-1152">В команду `group deployment create` добавлен параметр `--handle-extended-json-format`, для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="4a611-1152">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="4a611-1153">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4a611-1153">Compute</span></span>

* <span data-ttu-id="4a611-1154">В команды `vmss [create|update]` добавлен параметр `--terminate-notification-time`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="4a611-1154">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="4a611-1155">В команду `vmss update` добавлен параметр `--enable-terminate-notification`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="4a611-1155">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="4a611-1156">В команды `[vm|vmss] create` добавлены параметры `--priority,`, `--eviction-policy,` и `--max-billing`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1156">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="4a611-1157">Изменена команда `disk create`, которая теперь позволяет указать точный размер отправки на диск.</span><span class="sxs-lookup"><span data-stu-id="4a611-1157">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="4a611-1158">В `snapshot create` добавлена поддержка добавочных моментальных снимков для управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="4a611-1158">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="4a611-1159">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-1159">Cosmos DB</span></span>

* <span data-ttu-id="4a611-1160">В команду `cosmosdb keys list` добавлен параметр `--type <key-type>` для отображения ключей, ключей только для чтения или строк подключения.</span><span class="sxs-lookup"><span data-stu-id="4a611-1160">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="4a611-1161">Добавлена команда `cosmosdb keys regenerate`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1161">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="4a611-1162">[УСТАРЕЛО] Команды `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` и `cosmosdb list-read-only-keys` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="4a611-1162">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="4a611-1163">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="4a611-1163">EventGrid</span></span>

* <span data-ttu-id="4a611-1164">Исправлен текст справки по конечной точке — дана ссылка на правильный параметр.</span><span class="sxs-lookup"><span data-stu-id="4a611-1164">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="4a611-1165">Key Vault</span><span class="sxs-lookup"><span data-stu-id="4a611-1165">Key Vault</span></span>

* <span data-ttu-id="4a611-1166">Исправлена проблема, из-за которой вход с помощью клиента (`login -t`) мог приводить к сбою `keyvault create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1166">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-1167">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-1167">Monitor</span></span>

* <span data-ttu-id="4a611-1168">Исправлена проблема с тем, что символ `:` являлся недопустимым в аргументе `--condition` для `monitor metrics alert create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1168">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="4a611-1169">Политика</span><span class="sxs-lookup"><span data-stu-id="4a611-1169">Policy</span></span>

* <span data-ttu-id="4a611-1170">Добавлена поддержка API Политики версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="4a611-1170">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="4a611-1171">В команду `policy assignment create` добавлен параметр `--enforcement-mode`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1171">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-1172">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-1172">Storage</span></span>

* <span data-ttu-id="4a611-1173">В команду `az storage copy` добавлен параметр `--blob-type`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1173">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="4a611-1174">10 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1174">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-1175">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-1175">ACR</span></span>

* <span data-ttu-id="4a611-1176">Добавлена группа команд `acr config retention` для настройки политики хранения.</span><span class="sxs-lookup"><span data-stu-id="4a611-1176">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="4a611-1177">AKS</span><span class="sxs-lookup"><span data-stu-id="4a611-1177">AKS</span></span>

* <span data-ttu-id="4a611-1178">Добавлена возможность интеграции ACR с помощью следующих команд:</span><span class="sxs-lookup"><span data-stu-id="4a611-1178">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="4a611-1179">В `aks [create|update]` добавлен параметр `--attach-acr` для подключения ACR к кластеру AKS.</span><span class="sxs-lookup"><span data-stu-id="4a611-1179">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="4a611-1180">В `aks update` добавлен параметр `--detach-acr` для отключения ACR от кластера AKS.</span><span class="sxs-lookup"><span data-stu-id="4a611-1180">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="4a611-1181">ARM</span><span class="sxs-lookup"><span data-stu-id="4a611-1181">ARM</span></span>

* <span data-ttu-id="4a611-1182">Добавлена возможность использования API версии 2019-05-10.</span><span class="sxs-lookup"><span data-stu-id="4a611-1182">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="4a611-1183">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-1183">Batch</span></span>

* <span data-ttu-id="4a611-1184">Добавлены новые параметры конфигурации JSON в `--json-file` для `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="4a611-1184">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="4a611-1185">Добавлен параметр `MountConfigurations` для подключений файловой системы (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="4a611-1185">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="4a611-1186">Добавлено необязательное свойство `publicIPs` в `NetworkConfiguration` для общедоступных IP-адресов в пулах (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="4a611-1186">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="4a611-1187">В `--image` добавлена поддержка коллекций общих образов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1187">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="4a611-1188">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `--start-task-wait-for-success` в `batch pool create` изменено на `true`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1188">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="4a611-1189">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `Scope` в `AutoUserSpecification` задано как Pool (ранее `Task` на узлах Windows и `Pool` на узлах Linux).</span><span class="sxs-lookup"><span data-stu-id="4a611-1189">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="4a611-1190">Этот аргумент можно задать только в конфигурации JSON с помощью `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1190">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4a611-1191">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4a611-1191">HDInsight</span></span>

* <span data-ttu-id="4a611-1192">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="4a611-1192">GA release</span></span>
* <span data-ttu-id="4a611-1193">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--workernode-count/-c` в `az hdinsight resize` теперь является обязательным.</span><span class="sxs-lookup"><span data-stu-id="4a611-1193">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="4a611-1194">Key Vault</span><span class="sxs-lookup"><span data-stu-id="4a611-1194">Key Vault</span></span>

* <span data-ttu-id="4a611-1195">Исправлена проблема, когда подсети не удавалось удалить из сетевых правил.</span><span class="sxs-lookup"><span data-stu-id="4a611-1195">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="4a611-1196">Исправлена проблема, когда дублированные подсети и IP-адреса могли быть добавлены к сетевым правилам.</span><span class="sxs-lookup"><span data-stu-id="4a611-1196">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="4a611-1197">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-1197">Network</span></span>

* <span data-ttu-id="4a611-1198">Добавлен параметр `--interval` в `network watcher flow-log` для выбора значения интервала анализа трафика.</span><span class="sxs-lookup"><span data-stu-id="4a611-1198">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="4a611-1199">Добавлена команда `network application-gateway identity` для управления удостоверением шлюза.</span><span class="sxs-lookup"><span data-stu-id="4a611-1199">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="4a611-1200">Добавлена возможность указать идентификатор Key Vault в команде `network application-gateway ssl-cert`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1200">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="4a611-1201">Добавлена команда `network express-route peering peer-connection [show|list]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1201">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="4a611-1202">Политика</span><span class="sxs-lookup"><span data-stu-id="4a611-1202">Policy</span></span>

* <span data-ttu-id="4a611-1203">Добавлена возможность использования API версии 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="4a611-1203">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="4a611-1204">27 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1204">August 27, 2019</span></span>

<span data-ttu-id="4a611-1205">Версия 2.0.72</span><span class="sxs-lookup"><span data-stu-id="4a611-1205">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-1206">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-1206">ACR</span></span>

* <span data-ttu-id="4a611-1207">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка SKU `classic`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1207">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="4a611-1208">Управление API</span><span class="sxs-lookup"><span data-stu-id="4a611-1208">API Management</span></span>

* <span data-ttu-id="4a611-1209">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена группа команд `apim`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1209">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-1210">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-1210">AppService</span></span>

* <span data-ttu-id="4a611-1211">Исправлена проблема с командой `webapp webjob continuous start` при указании слота.</span><span class="sxs-lookup"><span data-stu-id="4a611-1211">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="4a611-1212">Изменена команда `webapp up` для обнаружения и удаления папки `env` из файла, используемого для развертывания.</span><span class="sxs-lookup"><span data-stu-id="4a611-1212">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="4a611-1213">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4a611-1213">Keyvault</span></span>

* <span data-ttu-id="4a611-1214">Исправлена ошибка в команде `keyvault secret set`, которая игнорировала аргумент `--expires`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1214">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="4a611-1215">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-1215">Network</span></span>

* <span data-ttu-id="4a611-1216">Добавлена поддержка IPv6-адресов для аргументов `--private-ip-address-version`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1216">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="4a611-1217">Добавлены новые команды `network private-endpoint [create|update|list-types]` для управления закрытыми конечными точками.</span><span class="sxs-lookup"><span data-stu-id="4a611-1217">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="4a611-1218">Добавлена группа команд для `network private-link-service`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1218">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="4a611-1219">Добавлены аргументы `--private-endpoint-network-policies` и `--private-link-service-network-policies` для команды `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="4a611-1219">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="4a611-1220">RBAC</span><span class="sxs-lookup"><span data-stu-id="4a611-1220">RBAC</span></span>

* <span data-ttu-id="4a611-1221">Исправлена проблема с `ad app update --homepage`, когда домашнюю страницу нельзя было обновить.</span><span class="sxs-lookup"><span data-stu-id="4a611-1221">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="4a611-1222">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4a611-1222">ServiceFabric</span></span>

* <span data-ttu-id="4a611-1223">Добавлена поддержка имен Key Vault в смешанном регистре.</span><span class="sxs-lookup"><span data-stu-id="4a611-1223">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="4a611-1224">Исправлена проблема с использованием сертификатов в Key Vault.</span><span class="sxs-lookup"><span data-stu-id="4a611-1224">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="4a611-1225">Исправлена проблема с использованием файлов сертификатов PFX.</span><span class="sxs-lookup"><span data-stu-id="4a611-1225">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="4a611-1226">Исправлена проблема с `sf cluster certificate add`, когда группа ресурсов Key Vault не была указана.</span><span class="sxs-lookup"><span data-stu-id="4a611-1226">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="4a611-1227">Исправлена проблема с неработающей командой `sf cluster set`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1227">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="4a611-1228">SignalR</span><span class="sxs-lookup"><span data-stu-id="4a611-1228">SignalR</span></span>

* <span data-ttu-id="4a611-1229">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="4a611-1229">Added new commands:</span></span>
  * <span data-ttu-id="4a611-1230">`signalr cors`: Управление CORS SignalR</span><span class="sxs-lookup"><span data-stu-id="4a611-1230">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="4a611-1231">`signalr restart`: Перезапуск службы SignalR</span><span class="sxs-lookup"><span data-stu-id="4a611-1231">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="4a611-1232">`signalr update`: Обновление службы SignalR</span><span class="sxs-lookup"><span data-stu-id="4a611-1232">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="4a611-1233">Добавлен аргумент `--service-mode` для команды `signalr create`</span><span class="sxs-lookup"><span data-stu-id="4a611-1233">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-1234">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-1234">Storage</span></span>

* <span data-ttu-id="4a611-1235">Добавлена команда `storage account revoke-delegation-keys`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1235">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="4a611-1236">13 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1236">August 13, 2019</span></span>

<span data-ttu-id="4a611-1237">Версия 2.0.71</span><span class="sxs-lookup"><span data-stu-id="4a611-1237">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-1238">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-1238">AppService</span></span>

* <span data-ttu-id="4a611-1239">Исправлена проблема, из-за которой выполнение команд `webapp webjob continuous` для слотов завершалось сбоем.</span><span class="sxs-lookup"><span data-stu-id="4a611-1239">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="4a611-1240">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4a611-1240">BotService</span></span>

* <span data-ttu-id="4a611-1241">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка создания ботов на основе пакета SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="4a611-1241">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="4a611-1242">Cognitive Services:</span><span class="sxs-lookup"><span data-stu-id="4a611-1242">CognitiveServices</span></span>

* <span data-ttu-id="4a611-1243">Добавлены команды `cognitiveservices account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1243">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="4a611-1244">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-1244">Cosmos DB</span></span>

* <span data-ttu-id="4a611-1245">Удалено предупреждение при обновлении нескольких расположений для записи.</span><span class="sxs-lookup"><span data-stu-id="4a611-1245">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="4a611-1246">Добавлены команды CRUD для ресурсов CosmosDB SQL, MongoDB, Cassandra, Gremlin и ресурсов таблиц, а также пропускной способности ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1246">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4a611-1247">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4a611-1247">HDInsight</span></span>

<span data-ttu-id="4a611-1248">Этот выпуск содержит большое число критических изменений.</span><span class="sxs-lookup"><span data-stu-id="4a611-1248">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="4a611-1249">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="4a611-1249">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="4a611-1250">Переименование `--storage-default-container` в `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="4a611-1250">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="4a611-1251">Переименование `--storage-default-filesystem` в `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="4a611-1251">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="4a611-1252">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--name` для `application create`, чтобы представлять имя приложения вместо имени кластера.</span><span class="sxs-lookup"><span data-stu-id="4a611-1252">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="4a611-1253">Добавлен аргумент `--cluster-name` для `application create`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1253">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="4a611-1254">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="4a611-1254">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="4a611-1255">Переименование `--application-type` в `--type`</span><span class="sxs-lookup"><span data-stu-id="4a611-1255">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="4a611-1256">Переименование `--marketplace-identifier` в `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="4a611-1256">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="4a611-1257">Переименование `--https-endpoint-access-mode` в `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="4a611-1257">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="4a611-1258">Переименован аргумент `--https-endpoint-destination-port` на `--destination-port`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1258">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="4a611-1259">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="4a611-1259">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="4a611-1260">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Переименован аргумент `--target-instance-count` на `--workernode-count` для `hdinsight resize`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1260">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="4a611-1261">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены все команды в группе `hdinsight script-action`, чтобы использовать параметр `--name` в качестве имени действия скрипта.</span><span class="sxs-lookup"><span data-stu-id="4a611-1261">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="4a611-1262">Добавлен аргумент `--cluster-name` для всех команд `hdinsight script-action`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1262">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="4a611-1263">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименован аргумент `--script-execution-id` на `--execution-id`для всех команд `hdinsight script-action`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1263">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="4a611-1264">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `hdinsight script-action show` переименована в `hdinsight script-action show-execution-details`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1264">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="4a611-1265">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Изменены параметры для `hdinsight script-action execute --roles`, чтобы они разделялись пробелами, а не запятыми.</span><span class="sxs-lookup"><span data-stu-id="4a611-1265">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="4a611-1266">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--persisted` для `hdinsight script-action list`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1266">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="4a611-1267">Изменен параметр `hdinsight create --cluster-configurations`, чтобы принимать путь к локальному файлу JSON или строке JSON.</span><span class="sxs-lookup"><span data-stu-id="4a611-1267">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="4a611-1268">Добавлена команда `hdinsight script-action list-execution-history`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1268">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="4a611-1269">Изменен параметр `hdinsight monitor enable --workspace`, чтобы принимать идентификатор или имя рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="4a611-1269">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="4a611-1270">Добавлен аргумент `hdinsight monitor enable --primary-key`, который требуется, если в качестве параметра указан идентификатор рабочей области.</span><span class="sxs-lookup"><span data-stu-id="4a611-1270">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="4a611-1271">Добавлены дополнительные примеры и обновленные описания для справочных сообщений.</span><span class="sxs-lookup"><span data-stu-id="4a611-1271">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="4a611-1272">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="4a611-1272">Interactive</span></span>

* <span data-ttu-id="4a611-1273">Исправлена ошибка загрузки.</span><span class="sxs-lookup"><span data-stu-id="4a611-1273">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="4a611-1274">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="4a611-1274">Kubernetes</span></span>

* <span data-ttu-id="4a611-1275">Теперь используется `https`, если порт контейнера панели мониторинга использует `https`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1275">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="4a611-1276">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-1276">Network</span></span>

* <span data-ttu-id="4a611-1277">Добавлен аргумент `--yes` для `network dns record-set cname delete`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1277">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-1278">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-1278">Profile</span></span>

* <span data-ttu-id="4a611-1279">Добавлен аргумент `--resource-type` для `account get-access-token`, чтобы получать маркеры доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="4a611-1279">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="4a611-1280">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4a611-1280">ServiceFabric</span></span>

* <span data-ttu-id="4a611-1281">Добавлены все поддерживаемые версии ОС для команды sf cluster create.</span><span class="sxs-lookup"><span data-stu-id="4a611-1281">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="4a611-1282">Исправлена ошибка проверки основного сертификата.</span><span class="sxs-lookup"><span data-stu-id="4a611-1282">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-1283">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-1283">Storage</span></span>

* <span data-ttu-id="4a611-1284">Добавлена команда `storage copy`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1284">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="4a611-1285">30 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1285">July 30, 2019</span></span>

<span data-ttu-id="4a611-1286">Версия 2.0.70</span><span class="sxs-lookup"><span data-stu-id="4a611-1286">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-1287">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-1287">ACR</span></span>

* <span data-ttu-id="4a611-1288">Исправлена проблема № 9952 (регрессия в команде `acr pack build`).</span><span class="sxs-lookup"><span data-stu-id="4a611-1288">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="4a611-1289">Удалено имя образа построителя по умолчанию в `acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1289">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-1290">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-1290">Appservice</span></span>

* <span data-ttu-id="4a611-1291">Команда `webapp config ssl` изменена для отображения сообщения, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="4a611-1291">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="4a611-1292">Исправлена проблема, когда команда `functionapp create` не принимала тип учетной записи хранения `Standard_RAGRS`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1292">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="4a611-1293">Исправлена проблема, когда команда `webapp up` завершала работу со сбоем в случае выполнения со старой версией Python.</span><span class="sxs-lookup"><span data-stu-id="4a611-1293">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="4a611-1294">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-1294">Network</span></span>

* <span data-ttu-id="4a611-1295">Удален недопустимый параметр `--ids` из `network nic ip-config add` (исправление проблемы № 9861).</span><span class="sxs-lookup"><span data-stu-id="4a611-1295">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="4a611-1296">Исправлена проблема № 9604.</span><span class="sxs-lookup"><span data-stu-id="4a611-1296">Fixes #9604.</span></span> <span data-ttu-id="4a611-1297">Добавлен параметр `--root-certs` в `network application-gateway http-settings [create|update]` для поддержки связанных с пользователем доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1297">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="4a611-1298">Исправлен аргумент `--subscription` для `network dns record-set ns create` (проблема № 9965).</span><span class="sxs-lookup"><span data-stu-id="4a611-1298">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="4a611-1299">RBAC</span><span class="sxs-lookup"><span data-stu-id="4a611-1299">RBAC</span></span>

* <span data-ttu-id="4a611-1300">Добавлена команда `user update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1300">Added `user update` command</span></span>
* <span data-ttu-id="4a611-1301">[УСТАРЕЛО]`--upn-or-object-id` не рекомендуется использовать в связанных с пользователями командах.</span><span class="sxs-lookup"><span data-stu-id="4a611-1301">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="4a611-1302">Вместо этого применяйте аргумент `--id`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1302">Use replacement argument `--id`</span></span>
* <span data-ttu-id="4a611-1303">Добавлен аргумент `--id` в связанные с пользователями команды.</span><span class="sxs-lookup"><span data-stu-id="4a611-1303">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-1304">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-1304">SQL</span></span>

* <span data-ttu-id="4a611-1305">Добавлены команды управления для ключей и предохранителя TDE управляемого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="4a611-1305">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-1306">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-1306">Storage</span></span>

* <span data-ttu-id="4a611-1307">Добавлена команда `storage remove`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1307">Added `storage remove` command</span></span>
* <span data-ttu-id="4a611-1308">Исправлена проблема с `storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1308">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-1309">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-1309">VM</span></span>

* <span data-ttu-id="4a611-1310">Изменена команда `list-skus` для использования новой версии API для вывода сведений о зонах.</span><span class="sxs-lookup"><span data-stu-id="4a611-1310">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="4a611-1311">Изменено значение по умолчанию параметра `--single-placement-group` на `false` для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1311">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="4a611-1312">Добавлена возможность выбирать номера SKU хранилища ZRS для `[snapshot|disk] create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1312">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="4a611-1313">Добавлена новая группа команд `vm host` для поддержки выделенных узлов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1313">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="4a611-1314">Добавлены параметры `--host` и `--host-group` в команде `vm create` для указания выделенного узла виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="4a611-1314">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="4a611-1315">16 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1315">July 16, 2019</span></span>

<span data-ttu-id="4a611-1316">Версия 2.0.69</span><span class="sxs-lookup"><span data-stu-id="4a611-1316">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-1317">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-1317">Appservice</span></span>

* <span data-ttu-id="4a611-1318">Изменены команды `webapp identity`. Теперь они возвращают правильное сообщение об ошибке, если параметр ResourceGroupName или имя приложения недопустимы.</span><span class="sxs-lookup"><span data-stu-id="4a611-1318">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="4a611-1319">Исправлена команда `webapp list`. Теперь она возвращает правильное значение для параметра numberOfSites, если не указан параметр ResourceGroup.</span><span class="sxs-lookup"><span data-stu-id="4a611-1319">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="4a611-1320">Исправлены побочные эффекты для команд `appservice plan create` и `webapp create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1320">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="4a611-1321">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-1321">Core</span></span>

* <span data-ttu-id="4a611-1322">Исправлена ошибка, при которой отображался параметр `--subscription`, хотя он был неприменим.</span><span class="sxs-lookup"><span data-stu-id="4a611-1322">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="4a611-1323">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-1323">Batch</span></span>

* <span data-ttu-id="4a611-1324">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `batch pool node-agent-skus list` заменена на `batch pool supported-images list`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1324">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="4a611-1325">Добавлена поддержка правил безопасности, которые блокируют сетевой доступ к пулу на основе исходного порта трафика при использовании параметра `--json-file` команды `batch pool create network`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1325">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="4a611-1326">Добавлена поддержка выполнения задачи в рабочей папке контейнера или рабочей папке задачи пакета при использовании параметра `--json-file` команды `batch task create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1326">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="4a611-1327">Исправлена ошибка в параметре `--application-package-references` команды `batch pool create`, которая позволяла работать только со значениями по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-1327">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="4a611-1328">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="4a611-1328">Eventhubs</span></span>

* <span data-ttu-id="4a611-1329">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1329">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="4a611-1330">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4a611-1330">RDBMS</span></span>

* <span data-ttu-id="4a611-1331">Добавлен необязательный параметр для указания номера SKU реплики в команде создания реплики.</span><span class="sxs-lookup"><span data-stu-id="4a611-1331">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="4a611-1332">Исправлена ошибка теста CI при создании реплики MySQL.</span><span class="sxs-lookup"><span data-stu-id="4a611-1332">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="4a611-1333">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="4a611-1333">Relay</span></span>

* <span data-ttu-id="4a611-1334">Исправлена проблема с гибридным подключением при выключенной авторизации клиента ([8775](https://github.com/azure/azure-cli/issues/8775)).</span><span class="sxs-lookup"><span data-stu-id="4a611-1334">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="4a611-1335">Добавлен параметр `--requires-transport-security` для команды `relay wcfrelay create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1335">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="4a611-1336">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="4a611-1336">Servicebus</span></span>

* <span data-ttu-id="4a611-1337">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1337">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-1338">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-1338">Storage</span></span>

* <span data-ttu-id="4a611-1339">Добавлена возможность обновления учетной записи хранения для AADDS в службе "Файлы".</span><span class="sxs-lookup"><span data-stu-id="4a611-1339">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="4a611-1340">Устранена проблема, описанная здесь: `storage blob service-properties update --set`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1340">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="4a611-1341">2 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1341">July 2, 2019</span></span>

<span data-ttu-id="4a611-1342">Версия 2.0.68</span><span class="sxs-lookup"><span data-stu-id="4a611-1342">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="4a611-1343">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-1343">Core</span></span>

* <span data-ttu-id="4a611-1344">Командные модули теперь объединены в один распространяемый пакет Python.</span><span class="sxs-lookup"><span data-stu-id="4a611-1344">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="4a611-1345">В результате этого прекращается непосредственное использование множества пакетов `azure-cli-` в PyPI.</span><span class="sxs-lookup"><span data-stu-id="4a611-1345">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="4a611-1346">Это также должно уменьшить размер установки и повлияет только на пользователей, которые выполняли установку непосредственно через `pip`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1346">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-1347">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-1347">ACR</span></span>

* <span data-ttu-id="4a611-1348">В заданиях добавлена поддержка триггеров таймера.</span><span class="sxs-lookup"><span data-stu-id="4a611-1348">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-1349">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-1349">Appservice</span></span>

* <span data-ttu-id="4a611-1350">Внесены изменения в `functionapp create` для включения Application Insights по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-1350">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="4a611-1351">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена устаревшая команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1351">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="4a611-1352">Вместо нее используйте новую команду `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1352">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="4a611-1353">В `functionapp deployment config-zip` добавлена поддержка плана потребления приложения-функции Linux.</span><span class="sxs-lookup"><span data-stu-id="4a611-1353">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="4a611-1354">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-1354">Cosmos DB</span></span>

* <span data-ttu-id="4a611-1355">Добавлена возможность отключения TTL.</span><span class="sxs-lookup"><span data-stu-id="4a611-1355">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="4a611-1356">DLS</span><span class="sxs-lookup"><span data-stu-id="4a611-1356">DLS</span></span>

* <span data-ttu-id="4a611-1357">Обновленная версия ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="4a611-1357">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="4a611-1358">Отзывы</span><span class="sxs-lookup"><span data-stu-id="4a611-1358">Feedback</span></span>

* <span data-ttu-id="4a611-1359">При сообщении о сбое при выполнении команды расширения `az feedback` теперь пытается открыть браузер по URL-адресу репозитория или проекта расширения из индекса.</span><span class="sxs-lookup"><span data-stu-id="4a611-1359">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4a611-1360">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4a611-1360">HDInsight</span></span>

* <span data-ttu-id="4a611-1361">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя группы команд `oms` изменилось на `monitor`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1361">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="4a611-1362">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--http-password/-p` стал обязательным.</span><span class="sxs-lookup"><span data-stu-id="4a611-1362">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="4a611-1363">Добавлены средства заполнения для `--cluster-admin-account` и средство заполнения для параметров `cluster-users-group-dns`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1363">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="4a611-1364">Параметр `cluster-users-group-dns` стал обязательным, если присутствует `—esp`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1364">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="4a611-1365">Добавлено время ожидания для всех существующих средств автоматического заполнения аргументов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1365">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="4a611-1366">Добавлено время ожидания для преобразования имени ресурса в идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="4a611-1366">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="4a611-1367">Внесены изменения в средства автоматического заполнения для выбора ресурсов из любой группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1367">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="4a611-1368">Это может быть группа ресурсов, отличная от той, которая указана с помощью `-g`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1368">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="4a611-1369">Добавлена поддержка параметров `--sub-domain-suffix` и `--disable_gateway_auth` в команде `hdinsight application create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1369">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="4a611-1370">Управляемые службы</span><span class="sxs-lookup"><span data-stu-id="4a611-1370">Managed Services</span></span>

* <span data-ttu-id="4a611-1371">Командный модуль управляемых служб выпущен в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="4a611-1371">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-1372">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-1372">Profile</span></span>
* <span data-ttu-id="4a611-1373">Аргумент `--subscription` подавляется для команды выхода.</span><span class="sxs-lookup"><span data-stu-id="4a611-1373">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="4a611-1374">RBAC</span><span class="sxs-lookup"><span data-stu-id="4a611-1374">RBAC</span></span>

* <span data-ttu-id="4a611-1375">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален аргумент `--password` для `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1375">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="4a611-1376">В команду `create` добавлен параметр `--assignee-principal-type` для устранения периодических сбоев из-за задержки репликации сервера AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="4a611-1376">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="4a611-1377">Исправлен сбой в `ad signed-in-user` при перечислении собственных объектов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1377">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="4a611-1378">Исправлена проблема, при которой `ad sp` не удавалось найти нужное приложение в субъекте-службе.</span><span class="sxs-lookup"><span data-stu-id="4a611-1378">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="4a611-1379">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4a611-1379">RDBMS</span></span>

* <span data-ttu-id="4a611-1380">Добавлена поддержка репликации MariaDB.</span><span class="sxs-lookup"><span data-stu-id="4a611-1380">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-1381">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-1381">SQL</span></span>

* <span data-ttu-id="4a611-1382">Описаны допустимые значения для `sql db create --sample-name`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1382">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-1383">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-1383">Storage</span></span>

* <span data-ttu-id="4a611-1384">В `storage blob generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1384">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="4a611-1385">В `storage container generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1385">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="4a611-1386">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-1386">VM</span></span>

* <span data-ttu-id="4a611-1387">Исправлена ошибка, при которой команда `vmss create` возвращала сообщение об ошибке при выполнении с `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1387">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="4a611-1388">Прекращена проверка `vmss create --single-placement-group` на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="4a611-1388">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="4a611-1389">Команда не завершается сбоем, если для `--single-placement-group` задано значение `true`, а значение `--instance-count` больше 100 или указаны зоны доступности. Сама проверка теперь выполняется службой вычислений.</span><span class="sxs-lookup"><span data-stu-id="4a611-1389">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="4a611-1390">Исправлена ошибка, при которой команда `[vm|vmss] extension image list` завершалась сбоем при указании `--latest`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1390">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="4a611-1391">18 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1391">June 18, 2019</span></span>

<span data-ttu-id="4a611-1392">Версия 2.0.67</span><span class="sxs-lookup"><span data-stu-id="4a611-1392">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="4a611-1393">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-1393">Core</span></span>

<span data-ttu-id="4a611-1394">В этом выпуске добавлен новый тег [Предварительная версия], который яснее дает понять, что группа команд, команда или аргумент находятся в состоянии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="4a611-1394">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="4a611-1395">Ранее это указывалось в тексте справки или подразумевалось в номере версии командного модуля.</span><span class="sxs-lookup"><span data-stu-id="4a611-1395">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="4a611-1396">В будущем в интерфейсе командной строки номера версий отдельных пакетов не будут указываться.</span><span class="sxs-lookup"><span data-stu-id="4a611-1396">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="4a611-1397">Если команда доступна в предварительной версии, это также касается и всех ее аргументов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1397">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="4a611-1398">Если группа команд помечается как находящаяся в предварительной версии, значит все команды и аргументы также считаются доступными в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="4a611-1398">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="4a611-1399">В результате этого изменения несколько групп команд могут "внезапно" оказаться в состоянии предварительной версии в этом выпуске.</span><span class="sxs-lookup"><span data-stu-id="4a611-1399">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="4a611-1400">В действительности большинство пакетов, которые находились в состоянии предварительной версии, в этом выпуске будут считаться общедоступными.</span><span class="sxs-lookup"><span data-stu-id="4a611-1400">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-1401">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-1401">ACR</span></span>
* <span data-ttu-id="4a611-1402">Добавлена команда acr check-health.</span><span class="sxs-lookup"><span data-stu-id="4a611-1402">Added 'acr check-health' command</span></span>
* <span data-ttu-id="4a611-1403">Улучшена обработка ошибок с маркерами безопасности AAD и ошибок при получении внешних команд.</span><span class="sxs-lookup"><span data-stu-id="4a611-1403">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-1404">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-1404">ACS</span></span>
* <span data-ttu-id="4a611-1405">Устаревшие команды ACS теперь скрыты в тексте справки.</span><span class="sxs-lookup"><span data-stu-id="4a611-1405">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="4a611-1406">AMS</span><span class="sxs-lookup"><span data-stu-id="4a611-1406">AMS</span></span>
* <span data-ttu-id="4a611-1407">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в возврате строк времени ISO 8601 для archive-window-length и key-frame-interval-duration.</span><span class="sxs-lookup"><span data-stu-id="4a611-1407">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-1408">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-1408">AppService</span></span>
* <span data-ttu-id="4a611-1409">Добавлена маршрутизация на основе расположение для `webapp deleted list` и `webapp deleted restore`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1409">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="4a611-1410">Исправлена проблема, при которой целевой URL-адрес веб-приложения ("Вы можете запустить приложение в...") не был активным в Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="4a611-1410">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="4a611-1411">Устранена проблема, при которой создание приложений в некоторых SKU завершалось сбоем с ошибкой AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="4a611-1411">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="4a611-1412">Добавлена предварительная проверка в `[appservice|webapp] create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1412">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="4a611-1413">Исправлено `[webapp|functionapp] traffic-routing` для использования правильного actionHostName.</span><span class="sxs-lookup"><span data-stu-id="4a611-1413">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="4a611-1414">Добавлена поддержка слотов для команд `functionapp`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1414">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="4a611-1415">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-1415">Batch</span></span>
* <span data-ttu-id="4a611-1416">Исправлена регрессия проверки подлинности AAD, которую вызывал чрезмерный поток уведомлений об авторизации с помощью общего ключа.</span><span class="sxs-lookup"><span data-stu-id="4a611-1416">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="4a611-1417">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4a611-1417">BatchAI</span></span>
* <span data-ttu-id="4a611-1418">Команды BatchAI теперь признаны устаревшими и скрыты.</span><span class="sxs-lookup"><span data-stu-id="4a611-1418">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="4a611-1419">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4a611-1419">BotService</span></span>
* <span data-ttu-id="4a611-1420">Добавлены предупреждающие сообщения о прекращении поддержки и режиме обслуживания для команд, которые поддерживают пакет SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="4a611-1420">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4a611-1421">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-1421">CosmosDB</span></span>
* <span data-ttu-id="4a611-1422">[УСТАРЕЛО] использовать команду `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1422">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="4a611-1423">Добавлена команда `cosmosdb keys list`, заменяющая `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1423">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="4a611-1424">`cosmsodb create/update`: Добавлен новый формат для --location, который позволяет задавать свойство isZoneRedundant.</span><span class="sxs-lookup"><span data-stu-id="4a611-1424">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="4a611-1425">Нерекомендуемый старый формат.</span><span class="sxs-lookup"><span data-stu-id="4a611-1425">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="4a611-1426">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="4a611-1426">EventGrid</span></span>
* <span data-ttu-id="4a611-1427">Добавлены команды `eventgrid domain` для операций CRUD домена.</span><span class="sxs-lookup"><span data-stu-id="4a611-1427">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="4a611-1428">Добавлены команды `eventgrid domain topic` для операций CRUD разделов домена.</span><span class="sxs-lookup"><span data-stu-id="4a611-1428">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="4a611-1429">В `eventgrid [topic|event-subscription] list` добавлен аргумент `--odata-query` для фильтрации результатов с использованием синтаксиса OData.</span><span class="sxs-lookup"><span data-stu-id="4a611-1429">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="4a611-1430">`event-subscription create/update`: Добавлена ServiceBusQueue в качестве новых значений для параметра `--endpoint-type`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1430">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="4a611-1431">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в прекращении поддержки `--included-event-types All` с `eventgrid event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1431">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4a611-1432">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4a611-1432">HDInsight</span></span>
* <span data-ttu-id="4a611-1433">Добавлена поддержка параметра `--ssh-public-key` в команде `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1433">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-1434">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-1434">IoT</span></span>
* <span data-ttu-id="4a611-1435">Добавлена поддержка для повторного создания ключей политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="4a611-1435">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="4a611-1436">Добавлен пакет SDK и поддержка для службы подготовки репозитория DigitalTwin.</span><span class="sxs-lookup"><span data-stu-id="4a611-1436">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="4a611-1437">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-1437">Network</span></span>
* <span data-ttu-id="4a611-1438">Добавлена поддержка зон для Шлюза NAT.</span><span class="sxs-lookup"><span data-stu-id="4a611-1438">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="4a611-1439">Добавлена команда `network list-service-tags`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1439">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="4a611-1440">Исправлена проблема с `dns zone import`, при которой пользователям не удавалось импортировать записи А с подстановочным знаком.</span><span class="sxs-lookup"><span data-stu-id="4a611-1440">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="4a611-1441">Исправлена проблема с `watcher flow-log configure`, при которой не удавалось включить ведение журнала потоков в определенных регионах.</span><span class="sxs-lookup"><span data-stu-id="4a611-1441">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-1442">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-1442">Resource</span></span>
* <span data-ttu-id="4a611-1443">Добавлена команда `az rest` для вызовов REST.</span><span class="sxs-lookup"><span data-stu-id="4a611-1443">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="4a611-1444">Исправлена ошибка, возникавшая при использовании `policy assignment list` с группой ресурсов или уровнем подписки `--scope`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1444">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="4a611-1445">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="4a611-1445">ServiceBus</span></span>
* <span data-ttu-id="4a611-1446">Устранена проблема № [9319](https://github.com/azure/azure-cli/issues/9319) с `servicebus topic create --max-size`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1446">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-1447">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-1447">SQL</span></span>
* <span data-ttu-id="4a611-1448">Параметр `--location` стал необязательным для `sql [server|mi] create`. Если он не указан, используется расположение группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1448">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="4a611-1449">Исправлена ошибка "Объект NoneType не подлежит итерации" с `sql db list-editions --available`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1449">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="4a611-1450">SQLVm</span><span class="sxs-lookup"><span data-stu-id="4a611-1450">SQLVm</span></span>
* <span data-ttu-id="4a611-1451">Критическое изменение. Для `sql vm create` теперь требуется параметр `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1451">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="4a611-1452">Внесены изменения, позволяющие задавать SKU образа SQL при создании или обновлении виртуальной машины SQL.</span><span class="sxs-lookup"><span data-stu-id="4a611-1452">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-1453">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-1453">Storage</span></span>
* <span data-ttu-id="4a611-1454">Исправлена проблема с отсутствующим ключом учетной записи для `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1454">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="4a611-1455">Исправлена проблема с `storage blob sync` на платформе Linux.</span><span class="sxs-lookup"><span data-stu-id="4a611-1455">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-1456">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-1456">VM</span></span>
* <span data-ttu-id="4a611-1457">[Предварительная версия] Добавлены команды `vm image template` для создания образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="4a611-1457">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="4a611-1458">4 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1458">June 4, 2019</span></span>

<span data-ttu-id="4a611-1459">Версия 2.0.66</span><span class="sxs-lookup"><span data-stu-id="4a611-1459">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="4a611-1460">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-1460">Core</span></span>
* <span data-ttu-id="4a611-1461">Исправлена ошибка, из-за которой выполнение команды завершалось со сбоем, если параметр `--output yaml` использовался с параметром `--query`</span><span class="sxs-lookup"><span data-stu-id="4a611-1461">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-1462">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-1462">ACR</span></span>
* <span data-ttu-id="4a611-1463">Добавлена группа команд acr pack для создания заданий быстрой сборки с помощью пакетов сборок.</span><span class="sxs-lookup"><span data-stu-id="4a611-1463">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-1464">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-1464">ACS</span></span>
* <span data-ttu-id="4a611-1465">Разрешено включение и отключение надстройки панели мониторинга Kubernetes для AKS.</span><span class="sxs-lookup"><span data-stu-id="4a611-1465">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="4a611-1466">Если подписку нельзя использовать с Azure Red Hat OpenShift, будет отображаться соответствующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="4a611-1466">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="4a611-1467">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-1467">Batch</span></span>
* <span data-ttu-id="4a611-1468">Улучшена обработка ошибок, если не выполнен вход в учетную запись \[[№ 9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[№ 8978](https://github.com/Azure/azure-cli/issues/8978)\].</span><span class="sxs-lookup"><span data-stu-id="4a611-1468">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-1469">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-1469">IoT</span></span>
* <span data-ttu-id="4a611-1470">Добавлена поддержка для перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="4a611-1470">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="4a611-1471">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-1471">Network</span></span>
* <span data-ttu-id="4a611-1472">Добавлены команды `network application-gateway waf-policy` для поддержки настраиваемых правил WAF.</span><span class="sxs-lookup"><span data-stu-id="4a611-1472">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="4a611-1473">Добавлены аргументы `--waf-policy` и `--max-capacity` для команды `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4a611-1473">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="4a611-1474">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-1474">Resource</span></span>
* <span data-ttu-id="4a611-1475">Улучшен вывод сообщения команды `deployment create` при отсутствии TTY.</span><span class="sxs-lookup"><span data-stu-id="4a611-1475">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="4a611-1476">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-1476">Role</span></span>
* <span data-ttu-id="4a611-1477">Обновлен текст справки.</span><span class="sxs-lookup"><span data-stu-id="4a611-1477">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="4a611-1478">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4a611-1478">Compute</span></span>
* <span data-ttu-id="4a611-1479">Добавлена поддержка команды `vm create` для создания виртуальных машин из управляемого образа с номерами LUN дисков данных, которые не начинаются с 0 или для которых пропущены номера.</span><span class="sxs-lookup"><span data-stu-id="4a611-1479">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="4a611-1480">21 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1480">May 21, 2019</span></span>

<span data-ttu-id="4a611-1481">Версия 2.0.65</span><span class="sxs-lookup"><span data-stu-id="4a611-1481">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="4a611-1482">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-1482">Core</span></span>
* <span data-ttu-id="4a611-1483">Улучшена функция обратной связи при ошибках аутентификации.</span><span class="sxs-lookup"><span data-stu-id="4a611-1483">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="4a611-1484">Исправлена проблема, из-за которой интерфейс командной строки загружал расширения, которые не были совместимы с его базовой версией.</span><span class="sxs-lookup"><span data-stu-id="4a611-1484">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="4a611-1485">Исправлена проблема с запуском и неисправностью `clouds.config`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1485">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-1486">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-1486">ACR</span></span>
* <span data-ttu-id="4a611-1487">Добавлена поддержка управляемых удостоверений в Задачи.</span><span class="sxs-lookup"><span data-stu-id="4a611-1487">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-1488">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-1488">ACS</span></span>
* <span data-ttu-id="4a611-1489">Исправлена команда `openshift create`, используемая с пользовательским клиентом AAD.</span><span class="sxs-lookup"><span data-stu-id="4a611-1489">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-1490">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-1490">AppService</span></span>
* <span data-ttu-id="4a611-1491">[УСТАРЕЛО] Команда `functionapp devops-build` устарела и будет удалена в следующем выпуске.</span><span class="sxs-lookup"><span data-stu-id="4a611-1491">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="4a611-1492">Внесено изменение в `functionapp devops-pipeline` для получения журнала сборки из Azure DevOps в режиме подробного протоколирования.</span><span class="sxs-lookup"><span data-stu-id="4a611-1492">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="4a611-1493">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален неподдерживаемый флаг `--use_local_settings` из команды `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1493">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="4a611-1494">Внесено изменение в `webapp up` для возврата выходных данных JSON, если `--logs` не используется.</span><span class="sxs-lookup"><span data-stu-id="4a611-1494">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="4a611-1495">Добавлена поддержка записи ресурсов по умолчанию в локальную конфигурацию для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1495">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="4a611-1496">Добавлена поддержка `webapp up` для повторного развертывания приложения без использования аргумента `--location`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1496">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="4a611-1497">Устранена проблема, из-за которой нельзя было создать для Linux номер SKU с планом службы приложений "Бесплатный".</span><span class="sxs-lookup"><span data-stu-id="4a611-1497">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="4a611-1498">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4a611-1498">BotService</span></span>
* <span data-ttu-id="4a611-1499">Внесено изменение для включения поддержки всех регистров в параметрах `--lang` для команд.</span><span class="sxs-lookup"><span data-stu-id="4a611-1499">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="4a611-1500">Обновлено описание модуля команды.</span><span class="sxs-lookup"><span data-stu-id="4a611-1500">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="4a611-1501">Потребление</span><span class="sxs-lookup"><span data-stu-id="4a611-1501">Consumption</span></span>
* <span data-ttu-id="4a611-1502">Добавлен отсутствующий обязательный параметр при выполнении `consumption usage list --billing-period-name`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1502">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-1503">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-1503">IoT</span></span>
* <span data-ttu-id="4a611-1504">Добавлена поддержка перечисления всех ключей.</span><span class="sxs-lookup"><span data-stu-id="4a611-1504">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="4a611-1505">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-1505">Network</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="4a611-1507">Добавлен аргумент `--nat-gateway` для `network vnet subnet [create|update]` для подключения к шлюзу NAT.</span><span class="sxs-lookup"><span data-stu-id="4a611-1507">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="4a611-1508">Исправлена проблема с `dns zone import`, из-за которой имена записей не сопоставлялись с типом записей.</span><span class="sxs-lookup"><span data-stu-id="4a611-1508">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="4a611-1509">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4a611-1509">RDBMS</span></span>
* <span data-ttu-id="4a611-1510">Добавлена поддержка Postgres и MySQL для георепликации.</span><span class="sxs-lookup"><span data-stu-id="4a611-1510">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="4a611-1511">RBAC</span><span class="sxs-lookup"><span data-stu-id="4a611-1511">RBAC</span></span>
* <span data-ttu-id="4a611-1512">Добавлена поддержка области группы управления для `role assignment`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1512">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-1513">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-1513">Storage</span></span>
* <span data-ttu-id="4a611-1514">`storage blob sync`: добавьте команду синхронизации для хранилища BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1514">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="4a611-1515">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="4a611-1515">Compute</span></span>
* <span data-ttu-id="4a611-1516">Добавлен параметр `--computer-name` для `vm create` для установки имени виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="4a611-1516">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="4a611-1517">Переименован параметр `--ssh-key-value` в `--ssh-key-values` для `[vm|vmss] create` для приема нескольких значений пути или открытого ключа SSH.</span><span class="sxs-lookup"><span data-stu-id="4a611-1517">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="4a611-1518">__Примечание.__ Это **не** критическое изменение, благодаря которому `--ssh-key-value` будет правильно анализироваться, так как соответствует только `--ssh-key-values`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1518">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="4a611-1519">Внесено изменение в аргумент `ppg create` для `--type` — теперь он необязательный.</span><span class="sxs-lookup"><span data-stu-id="4a611-1519">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="4a611-1520">6 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1520">May 6, 2019</span></span>

<span data-ttu-id="4a611-1521">Версия 2.0.64</span><span class="sxs-lookup"><span data-stu-id="4a611-1521">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-1522">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-1522">ACS</span></span>
* <span data-ttu-id="4a611-1523">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--fqdn` из команд `openshift`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1523">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="4a611-1524">Внесено изменение для использования общедоступной версии API для Azure Red Hat Openshift.</span><span class="sxs-lookup"><span data-stu-id="4a611-1524">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="4a611-1525">Добавлен флаг `customer-admin-group-id` в `openshift create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1525">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="4a611-1526">[Общедоступная версия.] `(PREVIEW)` больше не используется для `aks create` в параметре `--network-policy`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1526">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-1527">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-1527">Appservice</span></span>
* <span data-ttu-id="4a611-1528">[УСТАРЕЛО] Команда `functionapp devops-build` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="4a611-1528">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="4a611-1529">Команда переименована в `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1529">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="4a611-1530">Исправлен процесс получения правильного имени пользователя для Cloud Shell, приводивший к ошибке выполнения `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1530">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="4a611-1531">Обновлена документация по `appservice plan --sku` в соответствии с поддерживаемыми планами службы приложений.</span><span class="sxs-lookup"><span data-stu-id="4a611-1531">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="4a611-1532">Добавлены необязательные аргументы для группы ресурсов и план для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1532">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="4a611-1533">Добавлена поддержка `webapp ssh` в соответствии с переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1533">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="4a611-1534">Добавлена поддержка `appserviceplan create` для ценовой категории "Бесплатный" в Linux.</span><span class="sxs-lookup"><span data-stu-id="4a611-1534">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="4a611-1535">Внесено изменение в `webapp up` для перевода в спящий режим на 30 с после установки параметра приложения `SCM_DO_BUILD_DURING_DEPLOYMENT=true` для обработки холодного запуска Kudu.</span><span class="sxs-lookup"><span data-stu-id="4a611-1535">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="4a611-1536">Добавлена поддержка среды выполнения `powershell` для `functionapp create` в Windows.</span><span class="sxs-lookup"><span data-stu-id="4a611-1536">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="4a611-1537">Добавлена команда `create-remote-connection`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1537">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="4a611-1538">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-1538">Batch</span></span>
* <span data-ttu-id="4a611-1539">Исправлена ошибка в проверяющем элементе управления для параметров `--application-package-references`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1539">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="4a611-1540">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4a611-1540">Botservice</span></span>
* <span data-ttu-id="4a611-1541">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` для создания пустого бота веб-приложения по умолчанию (т. е. бот не развертывается в Службе приложений).</span><span class="sxs-lookup"><span data-stu-id="4a611-1541">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="4a611-1542">Добавлен флаг `--echo` в `bot create` для использования старого поведения с `-v v4`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1542">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="4a611-1543">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено значение по умолчанию `--version` на `v4`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1543">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="4a611-1544">__ПРИМЕЧАНИЕ.__ `bot prepare-publish` по-прежнему использует старое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-1544">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="4a611-1545">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `--lang` — значение `Csharp` больше не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-1545">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="4a611-1546">Если команда требует `--lang`, который не указан, команда завершит работу с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="4a611-1546">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="4a611-1547">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в аргументы `--appid` и `--password` для `bot create` — теперь они являются обязательными и их можно создать с помощью `ad app create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1547">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="4a611-1548">Добавлена проверка `--appid` и `--password`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1548">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="4a611-1549">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4`, чтобы не создавать или не использовать учетную запись хранения или Application Insights.</span><span class="sxs-lookup"><span data-stu-id="4a611-1549">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="4a611-1550">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v3`, чтобы требовать регион, где доступна служба Application Insights.</span><span class="sxs-lookup"><span data-stu-id="4a611-1550">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="4a611-1551">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot update`, чтобы влиять только на определенные свойства бота.</span><span class="sxs-lookup"><span data-stu-id="4a611-1551">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="4a611-1552">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в флаг `--lang` для принятия `Javascript` вместо `Node`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1552">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="4a611-1553">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`Node` больше не используется как допустимое значение `--lang`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1553">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="4a611-1554">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` — значение `SCM_DO_BUILD_DURING_DEPLOYMENT` больше не равно true.</span><span class="sxs-lookup"><span data-stu-id="4a611-1554">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="4a611-1555">Все развертывания через Kudu будут работать в соответствии с поведением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-1555">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="4a611-1556">Внесено изменение в `bot download` для ботов без файлов `.bot`, чтобы создавать файл конфигурации для определенного языка со значениями из параметров приложения для бота.</span><span class="sxs-lookup"><span data-stu-id="4a611-1556">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="4a611-1557">В команду `bot prepare-deploy` добавлена поддержка параметра `Typescript`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1557">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="4a611-1558">Добавлено предупреждающее сообщение в `bot prepare-deploy` для ботов `Javascript` и `Typescript`, когда `--code-dir` не содержит `package.json`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1558">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="4a611-1559">Внесено изменение в `bot prepare-deploy` для возврата `true` при успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="4a611-1559">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="4a611-1560">Включено ведение подробного журнала для `bot prepare-deploy`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1560">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="4a611-1561">Добавлены более доступные регионы Application Insights для `az bot create -v v3`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1561">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="4a611-1562">Configure</span><span class="sxs-lookup"><span data-stu-id="4a611-1562">Configure</span></span>
* <span data-ttu-id="4a611-1563">Добавлена поддержка конфигурации по умолчанию для аргумента на основе папки.</span><span class="sxs-lookup"><span data-stu-id="4a611-1563">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="4a611-1564">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="4a611-1564">Eventhubs</span></span>
* <span data-ttu-id="4a611-1565">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1565">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="4a611-1566">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1566">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="4a611-1567">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-1567">Network</span></span>
* <span data-ttu-id="4a611-1568">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--cache` на `--defer` для `vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1568">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="4a611-1569">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="4a611-1569">Policy Insights</span></span>
* <span data-ttu-id="4a611-1570">Добавлена поддержка `--expand PolicyEvaluationDetails` для результатов оценки политики запросов для ресурса.</span><span class="sxs-lookup"><span data-stu-id="4a611-1570">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="4a611-1571">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-1571">Role</span></span>
* <span data-ttu-id="4a611-1572">[УСТАРЕЛО] Внесено изменение в `create-for-rbac` для скрытия аргумента --password (поддержка прекращается в мае 2019 г.).</span><span class="sxs-lookup"><span data-stu-id="4a611-1572">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="4a611-1573">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="4a611-1573">Service Bus</span></span>
* <span data-ttu-id="4a611-1574">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1574">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="4a611-1575">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1575">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="4a611-1576">Внесено исправление в `topic [create|update]` — теперь `--max-size` поддерживает значения 10, 20, 40 и 80 ГБ для номера SKU ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="4a611-1576">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-1577">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-1577">SQL</span></span>
* <span data-ttu-id="4a611-1578">Добавлены команды `sql virtual-cluster [list|show|delete]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1578">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-1579">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-1579">VM</span></span>
* <span data-ttu-id="4a611-1580">Добавлены параметры `--protect-from-scale-in` и `--protect-from-scale-set-actions` для `vmss update`, чтобы включать обновления политики защиты для экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="4a611-1580">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="4a611-1581">Добавлены параметры `--instance-id` для `vmss update` для включения общего обновления экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="4a611-1581">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="4a611-1582">Добавлен параметр `--instance-id` для команды `vmss wait`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1582">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="4a611-1583">Добавлена новая группа команд `ppg` для управления группами размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="4a611-1583">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="4a611-1584">Добавлен параметр `--ppg` для `[vm|vmss] create` и `vm availability-set create` для управления PPG.</span><span class="sxs-lookup"><span data-stu-id="4a611-1584">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="4a611-1585">Добавлен параметр `--hyper-v-generation` для команды `image create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1585">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="4a611-1586">23 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1586">April 23, 2019</span></span>

<span data-ttu-id="4a611-1587">Версия 2.0.63</span><span class="sxs-lookup"><span data-stu-id="4a611-1587">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-1588">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-1588">ACS</span></span>
* <span data-ttu-id="4a611-1589">Внесено изменение в `aks get-credentials` для запроса на перезапись повторяющихся значений.</span><span class="sxs-lookup"><span data-stu-id="4a611-1589">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="4a611-1590">Удалено описание `(PREVIEW)` из команд Dev Spaces aks use-dev-spaces и aks remove-dev-spaces.</span><span class="sxs-lookup"><span data-stu-id="4a611-1590">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="4a611-1591">AMS</span><span class="sxs-lookup"><span data-stu-id="4a611-1591">AMS</span></span>
* <span data-ttu-id="4a611-1592">Исправлена ошибка с обновлением фильтров ресурсов и учетных записей.</span><span class="sxs-lookup"><span data-stu-id="4a611-1592">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-1593">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-1593">AppService</span></span>
* <span data-ttu-id="4a611-1594">Добавлена поддержка ASE и времени ожидания для `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1594">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="4a611-1595">Добавлена возможность настройки непрерывной интеграции и развертывания в конвейере Azure DevOps из репозитория Github для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="4a611-1595">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="4a611-1596">Добавлен аргумент `--github-pat` для `functionapp devops-build create` для получения личного маркера доступа Github.</span><span class="sxs-lookup"><span data-stu-id="4a611-1596">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="4a611-1597">Добавлен аргумент `--github-repository` для `functionapp devops-build create` для подключения репозитория Github, который содержит исходный код приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="4a611-1597">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="4a611-1598">Исправлена проблема со сбоем `az webapp up --logs` и обновлением .Net Core до версии 2.1 по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-1598">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="4a611-1599">Удалены ненужные параметры приложения-функции при создании приложения-функции с помощью плана потребления.</span><span class="sxs-lookup"><span data-stu-id="4a611-1599">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="4a611-1600">Внесены изменения в `webapp up`, чтобы строка ASP по умолчанию добавляла номера в конец для создания плана службы приложений на основе параметров SKU.</span><span class="sxs-lookup"><span data-stu-id="4a611-1600">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="4a611-1601">Добавлен параметр `-b` для `webapp up` для запуска приложения в браузере.</span><span class="sxs-lookup"><span data-stu-id="4a611-1601">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="4a611-1602">Внесены изменения в `webapp deployment source config zip` для обработки переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1602">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="4a611-1603">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="4a611-1603">Deployment Manager</span></span>
* <span data-ttu-id="4a611-1604">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Создание и администрирование артефактов, которые поддерживают развертывания</span><span class="sxs-lookup"><span data-stu-id="4a611-1604">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="4a611-1605">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="4a611-1605">Lab</span></span>
* <span data-ttu-id="4a611-1606">Исправлена ошибка, которая приводила к неожиданному завершению работы.</span><span class="sxs-lookup"><span data-stu-id="4a611-1606">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="4a611-1607">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-1607">Network</span></span>
* <span data-ttu-id="4a611-1608">Добавлено автоматическое делегирование сервера имен для `dns zone create` в родительском объекте во время создания дочерней зоны.</span><span class="sxs-lookup"><span data-stu-id="4a611-1608">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-1609">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-1609">Resource</span></span>
* <span data-ttu-id="4a611-1610">[УСТАРЕЛО] Не рекомендуются к использованию аргументы `--link-id`, `--target-id` и `--filter-string` для `resource link`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1610">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="4a611-1611">Используйте вместо них аргументы `--link`, `--target` и `--filter`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1611">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="4a611-1612">Исправлена проблема, из-за которой команды `resource link [create|update]` не работали.</span><span class="sxs-lookup"><span data-stu-id="4a611-1612">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="4a611-1613">Исправлена проблема, из-за которой удаление с помощью идентификатора ресурса приводило к сбою или ошибке.</span><span class="sxs-lookup"><span data-stu-id="4a611-1613">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-1614">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-1614">SQL</span></span>
* <span data-ttu-id="4a611-1615">Добавлена поддержка пользовательского часового пояса в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="4a611-1615">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="4a611-1616">Внесено изменение, чтобы разрешить использовать имя эластичного пула с `sql db update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1616">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="4a611-1617">В команду `sql server [create|update]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1617">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="4a611-1618">Добавлена команда `sql server wait`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1618">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-1619">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-1619">Storage</span></span>
* <span data-ttu-id="4a611-1620">Устранена проблема с двойной кодировкой маркеров SAS в `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1620">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-1621">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-1621">VM</span></span>
* <span data-ttu-id="4a611-1622">Добавлен флаг `--skip-shutdown` для `vm|vmss stop` для выключения виртуальных машин без завершения работы.</span><span class="sxs-lookup"><span data-stu-id="4a611-1622">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="4a611-1623">Добавлен аргумент `--storage-account-type` для `sig image-version create` настройки типа учетной записи профиля публикации.</span><span class="sxs-lookup"><span data-stu-id="4a611-1623">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="4a611-1624">Добавлен аргумент `--target-regions` для `sig image-version create` для указания типов учетных записей хранения, связанных с регионами.</span><span class="sxs-lookup"><span data-stu-id="4a611-1624">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="4a611-1625">9 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1625">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="4a611-1626">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-1626">Core</span></span>
* <span data-ttu-id="4a611-1627">Исправлена проблема, из-за которой для некоторых расширений отображалась версия `Unknown` и ее невозможно было обновить.</span><span class="sxs-lookup"><span data-stu-id="4a611-1627">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-1628">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-1628">ACR</span></span>
* <span data-ttu-id="4a611-1629">Добавлена поддержка запуска образа без контекста.</span><span class="sxs-lookup"><span data-stu-id="4a611-1629">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="4a611-1630">AMS</span><span class="sxs-lookup"><span data-stu-id="4a611-1630">AMS</span></span>
* [УСТАРЕЛО]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="4a611-1633">Добавлена поддержка новых параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1633">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="4a611-1634">Добавлен новый параметр `--filters` для `ams streaming-locator create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1634">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-1635">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-1635">AppService</span></span>
* <span data-ttu-id="4a611-1636">В команду `webapp up` добавлена поддержка параметра `--logs`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1636">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="4a611-1637">Исправлены ошибки в команде `functionapp devops-build create` при создании файла `azure-pipelines.yml`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1637">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="4a611-1638">Улучшена обработка и индикаторы ошибок с `unctionapp devops-build create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1638">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="4a611-1639">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--local-git` для команды `devops-build`. Обнаружение и обработка локального репозитория Git являются обязательными для создания конвейеров DevOps в Azure.</span><span class="sxs-lookup"><span data-stu-id="4a611-1639">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="4a611-1640">Добавлена поддержка создания плана функций Linux.</span><span class="sxs-lookup"><span data-stu-id="4a611-1640">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="4a611-1641">Добавлена возможность менять план для приложения-функции с помощью `functionapp update --plan`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1641">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="4a611-1642">Добавлена поддержка параметров горизонтального увеличения масштаба плана "Премиум" для Функций Azure.</span><span class="sxs-lookup"><span data-stu-id="4a611-1642">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="4a611-1643">CDN</span><span class="sxs-lookup"><span data-stu-id="4a611-1643">CDN</span></span>
* <span data-ttu-id="4a611-1644">Добавлена поддержка `Microsoft_Standard` и `Standard_ChinaCdn`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1644">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="4a611-1645">Отзывы</span><span class="sxs-lookup"><span data-stu-id="4a611-1645">Feedback</span></span>
* <span data-ttu-id="4a611-1646">Внесены изменения в `feedback` для отображения метаданных недавно выполненных команд.</span><span class="sxs-lookup"><span data-stu-id="4a611-1646">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="4a611-1647">Внесены изменения в `feedback`. Теперь при регистрации проблемы отображается запрос, в соответствии с которым пользователь должен открыть браузер и воспользоваться шаблоном проблемы.</span><span class="sxs-lookup"><span data-stu-id="4a611-1647">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="4a611-1648">Внесены изменения в `feedback`. Теперь текст проблемы выводится при запуске с параметром --verbose.</span><span class="sxs-lookup"><span data-stu-id="4a611-1648">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-1649">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-1649">Monitor</span></span>
* <span data-ttu-id="4a611-1650">Исправлена проблема, из-за которой у параметра count было недопустимое значение в `metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1650">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="4a611-1651">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-1651">Network</span></span>
* <span data-ttu-id="4a611-1652">Исправлен формат таблицы, которая не отображалась с помощью `vnet-gateway list-bgp-peer-status`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1652">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="4a611-1653">Добавлены команды `list-request-headers` и `list-response-headers` для `application-gateway rewrite-rule`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1653">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="4a611-1654">Добавлена команда `list-server-variables` для `application-gateway rewrite-rule condition`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1654">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="4a611-1655">Исправлена проблема, из-за которой обновление состояния соединения на порту ExpressRoute вызывало неизвестное исключение атрибута `express-route port update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1655">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="4a611-1656">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="4a611-1656">PrivateDNS</span></span>
* <span data-ttu-id="4a611-1657">Добавлена команда `network private-dns` для частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="4a611-1657">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-1658">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-1658">Resource</span></span>
* <span data-ttu-id="4a611-1659">Исправлена проблема с `deployment create` и `group deployment create`, из-за которой файл параметров с пустым набором параметров не работал.</span><span class="sxs-lookup"><span data-stu-id="4a611-1659">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="4a611-1660">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-1660">Role</span></span>
* <span data-ttu-id="4a611-1661">Внесены исправления в `create-for-rbac`. Теперь `--years` обрабатывается правильно.</span><span class="sxs-lookup"><span data-stu-id="4a611-1661">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="4a611-1662">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `role assignment delete`. Теперь появляется запрос при удалении всех назначений в рамках подписки без дополнительных условий.</span><span class="sxs-lookup"><span data-stu-id="4a611-1662">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-1663">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-1663">SQL</span></span>
* <span data-ttu-id="4a611-1664">Команда `sql mi [create|update]` обновлена с помощью свойств proxyOverride и publicDataEndpointEnabled.</span><span class="sxs-lookup"><span data-stu-id="4a611-1664">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-1665">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-1665">Storage</span></span>
* <span data-ttu-id="4a611-1666">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален результат выполнения `storage blob delete`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1666">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="4a611-1667">В команду `storage blob generate-sas` добавлен параметр `--full-uri` для создания полного URI большого двоичного объекта с помощью SAS.</span><span class="sxs-lookup"><span data-stu-id="4a611-1667">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="4a611-1668">В команду `storage file copy start` добавлен параметр `--file-snapshot` для копирования файла из моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="4a611-1668">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="4a611-1669">Внесены изменения в `storage blob copy cancel`. Теперь вместо исключения для NoPendingCopyOperation отображается только сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="4a611-1669">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="4a611-1670">26 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1670">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="4a611-1671">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-1671">Core</span></span>
* <span data-ttu-id="4a611-1672">Устранены проблемы с несовместимостью расширений для разработки.</span><span class="sxs-lookup"><span data-stu-id="4a611-1672">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="4a611-1673">Функция обработки ошибок теперь указывает клиентам на страницу проблем.</span><span class="sxs-lookup"><span data-stu-id="4a611-1673">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="4a611-1674">Cloud</span><span class="sxs-lookup"><span data-stu-id="4a611-1674">Cloud</span></span>
* <span data-ttu-id="4a611-1675">Исправлена ошибка с сообщением о не найденной подписке в `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1675">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-1676">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-1676">ACR</span></span>
* <span data-ttu-id="4a611-1677">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="4a611-1677">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="4a611-1678">Добавлено `--auth-mode` в команды `acr build`, `acr run`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1678">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="4a611-1679">Добавлена команда acr task credential для управления учетными данными для задачи.</span><span class="sxs-lookup"><span data-stu-id="4a611-1679">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="4a611-1680">Добавлено --no-wait в команду `acr build`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1680">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-1681">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-1681">AppService</span></span>
* <span data-ttu-id="4a611-1682">Исправлена ошибка с `webapp up`, из-за которой нельзя было правильно выполнить запуск из пустого каталога или скрипта неизвестного кода.</span><span class="sxs-lookup"><span data-stu-id="4a611-1682">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="4a611-1683">Исправлена ошибка, из-за которой не работали слоты для `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1683">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="4a611-1684">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4a611-1684">BOT Service</span></span>
* <span data-ttu-id="4a611-1685">Добавлено `bot prepare-deploy` для подготовки к развертыванию ботов с помощью `webapp`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1685">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="4a611-1686">Изменено `bot create --kind registration` для отображения пароля, если пароль не указан.</span><span class="sxs-lookup"><span data-stu-id="4a611-1686">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="4a611-1687">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--endpoint` в `bot create --kind registration` на пустую строку (по умолчанию) вместо запрашиваемой.</span><span class="sxs-lookup"><span data-stu-id="4a611-1687">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="4a611-1688">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="4a611-1688">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="4a611-1689">CDN</span><span class="sxs-lookup"><span data-stu-id="4a611-1689">CDN</span></span>
* <span data-ttu-id="4a611-1690">Добавлена поддержка параметра `--no-wait` в команде `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1690">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="4a611-1691">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено поведение кэширования строки запроса `cdn endpoint create` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-1691">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="4a611-1692">IgnoreQueryString больше не используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-1692">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="4a611-1693">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="4a611-1693">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4a611-1694">Сosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-1694">Cosmosdb</span></span>
* <span data-ttu-id="4a611-1695">Добавлена поддержка `--enable-multiple-write-locations` для обновления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="4a611-1695">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="4a611-1696">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="4a611-1696">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="4a611-1697">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="4a611-1697">Interactive</span></span>
* <span data-ttu-id="4a611-1698">Исправлена несовместимость с интерактивным расширением, установленным с помощью azdev.</span><span class="sxs-lookup"><span data-stu-id="4a611-1698">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-1699">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-1699">Monitor</span></span>
* <span data-ttu-id="4a611-1700">Внесено изменение, разрешающее использовать значение измерения `*` для `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1700">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="4a611-1701">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-1701">Network</span></span>
* <span data-ttu-id="4a611-1702">Добавлена группа команд `rewrite-rule` для `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1702">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-1703">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-1703">Profile</span></span>
* <span data-ttu-id="4a611-1704">Включена поддержка учетной записи уровня клиентов для управляемого удостоверения службы для `login`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1704">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="4a611-1705">Postgres</span><span class="sxs-lookup"><span data-stu-id="4a611-1705">Postgres</span></span> 
* <span data-ttu-id="4a611-1706">Добавлены команды postgresql `replica` и команда `restart server`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1706">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="4a611-1707">Внесены изменения для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="4a611-1707">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-1708">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-1708">Resource</span></span>
* <span data-ttu-id="4a611-1709">Улучшены табличные выходные данные для `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1709">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="4a611-1710">Исправлена проблема с `deployment [create|validate]`, из-за которой secureObject типа не распознавался.</span><span class="sxs-lookup"><span data-stu-id="4a611-1710">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="4a611-1711">График</span><span class="sxs-lookup"><span data-stu-id="4a611-1711">Graph</span></span>
* <span data-ttu-id="4a611-1712">Добавлена поддержка параметра `--end-date` в команде `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1712">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="4a611-1713">Добавлена поддержка разрешений для `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1713">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="4a611-1714">Исправлена проблема с `ad app permission list`, из-за которой отсутствовали разрешения.</span><span class="sxs-lookup"><span data-stu-id="4a611-1714">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="4a611-1715">Изменено `ad sp delete` для пропуска удаления назначения роли, если текущая учетная запись не содержит подписок.</span><span class="sxs-lookup"><span data-stu-id="4a611-1715">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="4a611-1716">Изменено `ad app create` для использования `--identifier-uris` пустого списка (по умолчанию), если список не указан.</span><span class="sxs-lookup"><span data-stu-id="4a611-1716">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-1717">носителей.</span><span class="sxs-lookup"><span data-stu-id="4a611-1717">storage</span></span>
* <span data-ttu-id="4a611-1718">Добавлено `--snapshot` для `storage file download-batch` для скачивания из моментального снимка общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="4a611-1718">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="4a611-1719">Изменен индикатор выполнения `storage blob [download-batch|upload-batch]`, чтобы обобщить сведения и указать текущий большой двоичный объект.</span><span class="sxs-lookup"><span data-stu-id="4a611-1719">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="4a611-1720">Исправлена проблема с `storage account update` при обновлении параметров шифрования.</span><span class="sxs-lookup"><span data-stu-id="4a611-1720">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="4a611-1721">Исправлена проблема со сбоем `storage blob show` при использовании OAuth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="4a611-1721">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-1722">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-1722">VM</span></span>
* <span data-ttu-id="4a611-1723">Добавлена команда `image update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1723">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="4a611-1724">12 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1724">March 12, 2019</span></span>

<span data-ttu-id="4a611-1725">Версия 2.0.60</span><span class="sxs-lookup"><span data-stu-id="4a611-1725">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="4a611-1726">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-1726">Core</span></span>

* <span data-ttu-id="4a611-1727">Исправлена недопустимая ошибка в `cloud set` о том, что подписка не найдена.</span><span class="sxs-lookup"><span data-stu-id="4a611-1727">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-1728">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-1728">ACR</span></span>

* <span data-ttu-id="4a611-1729">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="4a611-1729">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-1730">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-1730">ACS</span></span>

* <span data-ttu-id="4a611-1731">Внесены изменения, в соответствии с которыми параметр `--listen-address` для `aks browse` игнорируется, если он не поддерживается kubectl.</span><span class="sxs-lookup"><span data-stu-id="4a611-1731">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="4a611-1732">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-1732">AppService</span></span>

* <span data-ttu-id="4a611-1733">Добавлено `[webapp|functionapp] deployment list-publishing-credentials` для получения URL-адреса публикации Kudu и связанных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="4a611-1733">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="4a611-1734">Удалена ошибочная инструкция печати для `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1734">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="4a611-1735">Исправлено `functionapp` для настройки правильного образа для среды выполнения в планах службы приложений Linux.</span><span class="sxs-lookup"><span data-stu-id="4a611-1735">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="4a611-1736">Удален тег предварительной версии для `webapp up` и добавлены усовершенствования в команду.</span><span class="sxs-lookup"><span data-stu-id="4a611-1736">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="4a611-1737">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4a611-1737">Botservice</span></span>

* <span data-ttu-id="4a611-1738">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="4a611-1738">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="4a611-1739">Добавлено `Microsoft-BotFramework-AppId` и `Microsoft-BotFramework-AppPassword` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="4a611-1739">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="4a611-1740">Удалены одинарные кавычки из выходных данных команды `bot publish` в конце `bot create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1740">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="4a611-1741">Изменено `bot publish` для включения поддержки асинхронных операций.</span><span class="sxs-lookup"><span data-stu-id="4a611-1741">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="4a611-1742">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-1742">Container</span></span>

* <span data-ttu-id="4a611-1743">Добавлен аргумент `--no-wait` для команды `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="4a611-1743">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="4a611-1744">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="4a611-1744">EventHub</span></span>

* <span data-ttu-id="4a611-1745">Добавлен флаг `--skip-empty-archives` для `eventhub create|update` для включения поддержки пустых архивов при записи.</span><span class="sxs-lookup"><span data-stu-id="4a611-1745">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="4a611-1746">Поиск</span><span class="sxs-lookup"><span data-stu-id="4a611-1746">Find</span></span>

* <span data-ttu-id="4a611-1747">Основные обновления функций</span><span class="sxs-lookup"><span data-stu-id="4a611-1747">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4a611-1748">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4a611-1748">HDInsight</span></span>

* <span data-ttu-id="4a611-1749">Добавлен параметр `--storage-account-managed-identity` для `hdinsight create` для включения поддержки MSI ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="4a611-1749">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="4a611-1750">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-1750">Network</span></span>

* <span data-ttu-id="4a611-1751">Исправлена проблема с `vpn-connection update`, когда обновление VPN-подключения между шлюзами в разных подписках завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="4a611-1751">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="4a611-1752">Rdbms</span><span class="sxs-lookup"><span data-stu-id="4a611-1752">Rdbms</span></span>

* <span data-ttu-id="4a611-1753">Незначительные исправления для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="4a611-1753">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="4a611-1754">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-1754">Role</span></span>

* <span data-ttu-id="4a611-1755">Исправлено `role definition update` для использования идентификатора для правильного разрешения определения.</span><span class="sxs-lookup"><span data-stu-id="4a611-1755">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="4a611-1756">Изменено `ad app credential reset` для исключения предположения о том, что субъект-служба приложения всегда существует.</span><span class="sxs-lookup"><span data-stu-id="4a611-1756">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4a611-1757">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4a611-1757">Service Fabric</span></span>

* <span data-ttu-id="4a611-1758">Исправлена проблема с `sf cluster list` и невозможностью итерации.</span><span class="sxs-lookup"><span data-stu-id="4a611-1758">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="4a611-1759">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1759">February 26, 2019</span></span>

<span data-ttu-id="4a611-1760">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="4a611-1760">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="4a611-1761">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-1761">Core</span></span>

* <span data-ttu-id="4a611-1762">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="4a611-1762">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-1763">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-1763">ACR</span></span>

* <span data-ttu-id="4a611-1764">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1764">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="4a611-1765">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="4a611-1765">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-1766">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-1766">ACS</span></span>

* <span data-ttu-id="4a611-1767">Добавлен параметр `--listen-address` для команды `aks port-forward`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1767">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-1768">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-1768">AppService</span></span>

* <span data-ttu-id="4a611-1769">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1769">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="4a611-1770">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-1770">Batch</span></span>
* <span data-ttu-id="4a611-1771">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1771">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="4a611-1772">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1772">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="4a611-1773">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="4a611-1773">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="4a611-1774">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1774">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="4a611-1775">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="4a611-1775">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="4a611-1776">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4a611-1776">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4a611-1777">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-1777">CosmosDB</span></span>

* <span data-ttu-id="4a611-1778">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="4a611-1778">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="4a611-1779">Kusto</span><span class="sxs-lookup"><span data-stu-id="4a611-1779">Kusto</span></span>

* <span data-ttu-id="4a611-1780">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="4a611-1780">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="4a611-1781">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-1781">Network</span></span>

* <span data-ttu-id="4a611-1782">Добавлен аргумент `--express-route-gateway-bypass` для команды `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4a611-1782">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="4a611-1783">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1783">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="4a611-1784">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1784">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="4a611-1785">Добавлен аргумент `--legacy-mode` в команду `express-route peering [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1785">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="4a611-1786">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1786">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="4a611-1787">Добавлен аргумент `--gateway-default-site` для команды `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4a611-1787">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="4a611-1788">Добавлены команды `ipsec-policy` для `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1788">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-1789">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-1789">Resource</span></span>

* <span data-ttu-id="4a611-1790">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="4a611-1790">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="4a611-1791">Добавлена поддержка файла параметров на основе URI для `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1791">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="4a611-1792">Добавлена поддержка определений и параметров на основе URI для `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1792">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="4a611-1793">Исправлена обработка параметров и правил для `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1793">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="4a611-1794">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="4a611-1794">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="4a611-1795">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-1795">Role</span></span>

* <span data-ttu-id="4a611-1796">Добавлена поддержка ролей приложений для `ad app [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1796">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-1797">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-1797">VM</span></span>

* <span data-ttu-id="4a611-1798">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="4a611-1798">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="4a611-1799">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1799">February 12, 2019</span></span>

<span data-ttu-id="4a611-1800">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="4a611-1800">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="4a611-1801">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-1801">Core</span></span>

* <span data-ttu-id="4a611-1802">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="4a611-1802">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="4a611-1803">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="4a611-1803">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-1804">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-1804">ACR</span></span>
* <span data-ttu-id="4a611-1805">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1805">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="4a611-1806">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1806">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-1807">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-1807">ACS</span></span>
* <span data-ttu-id="4a611-1808">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="4a611-1808">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="4a611-1809">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1809">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="4a611-1810">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="4a611-1810">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="4a611-1811">AMS</span><span class="sxs-lookup"><span data-stu-id="4a611-1811">AMS</span></span>
* <span data-ttu-id="4a611-1812">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1812">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="4a611-1813">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1813">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-1814">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-1814">Appservice</span></span>
* <span data-ttu-id="4a611-1815">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="4a611-1815">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="4a611-1816">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="4a611-1816">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="4a611-1817">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1817">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="4a611-1818">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="4a611-1818">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="4a611-1819">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="4a611-1819">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="4a611-1820">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4a611-1820">Botservice</span></span>
* <span data-ttu-id="4a611-1821">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1821">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="4a611-1822">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1822">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="4a611-1823">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1823">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="4a611-1824">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="4a611-1824">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="4a611-1825">[УСТАРЕЛО] Аргумент `--proj-name` не рекомендуется к использованию. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1825">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="4a611-1826">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="4a611-1826">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="4a611-1827">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="4a611-1827">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="4a611-1828">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="4a611-1828">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="4a611-1829">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="4a611-1829">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="4a611-1830">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="4a611-1830">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="4a611-1831">Key Vault</span><span class="sxs-lookup"><span data-stu-id="4a611-1831">Key Vault</span></span>
* <span data-ttu-id="4a611-1832">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1832">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-1833">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-1833">Monitor</span></span>
* <span data-ttu-id="4a611-1834">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1834">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="4a611-1835">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-1835">Network</span></span>
* <span data-ttu-id="4a611-1836">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="4a611-1836">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="4a611-1837">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="4a611-1837">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="4a611-1838">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="4a611-1838">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="4a611-1839">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1839">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="4a611-1840">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="4a611-1840">Policy Insights</span></span>
* <span data-ttu-id="4a611-1841">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1841">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="4a611-1842">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4a611-1842">RDBMS</span></span>
* <span data-ttu-id="4a611-1843">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="4a611-1843">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="4a611-1844">Redis</span><span class="sxs-lookup"><span data-stu-id="4a611-1844">Redis</span></span>
* <span data-ttu-id="4a611-1845">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="4a611-1845">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="4a611-1846">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="4a611-1846">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="4a611-1847">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="4a611-1847">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="4a611-1848">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="4a611-1848">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="4a611-1849">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1849">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="4a611-1850">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="4a611-1850">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="4a611-1851">[УСТАРЕЛО] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a611-1851">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="4a611-1852">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-1852">Role</span></span>
* <span data-ttu-id="4a611-1853">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1853">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="4a611-1854">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-1854">SQL VM</span></span>
* <span data-ttu-id="4a611-1855">[УСТАРЕЛО] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="4a611-1855">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-1856">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-1856">VM</span></span>
* <span data-ttu-id="4a611-1857">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1857">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="4a611-1858">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1858">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="4a611-1859">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="4a611-1859">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="4a611-1860">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1860">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="4a611-1861">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1861">January 31, 2019</span></span>

<span data-ttu-id="4a611-1862">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="4a611-1862">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="4a611-1863">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-1863">Core</span></span>

* <span data-ttu-id="4a611-1864">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="4a611-1864">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="4a611-1865">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1865">January 28, 2019</span></span>

<span data-ttu-id="4a611-1866">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="4a611-1866">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-1867">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-1867">ACR</span></span>
* <span data-ttu-id="4a611-1868">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1868">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-1869">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-1869">ACS</span></span>
* <span data-ttu-id="4a611-1870">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1870">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="4a611-1871">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="4a611-1871">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="4a611-1872">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1872">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="4a611-1873">AMS</span><span class="sxs-lookup"><span data-stu-id="4a611-1873">AMS</span></span>
* <span data-ttu-id="4a611-1874">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1874">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="4a611-1875">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1875">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-1876">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-1876">Appservice</span></span>
* <span data-ttu-id="4a611-1877">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1877">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="4a611-1878">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="4a611-1878">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="4a611-1879">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="4a611-1879">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="4a611-1880">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-1880">Container</span></span>
* <span data-ttu-id="4a611-1881">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1881">Added `container start` command</span></span>
* <span data-ttu-id="4a611-1882">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4a611-1882">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="4a611-1883">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="4a611-1883">EventGrid</span></span>
* <span data-ttu-id="4a611-1884">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1884">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="4a611-1885">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1885">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="4a611-1886">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="4a611-1886">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="4a611-1887">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="4a611-1887">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="4a611-1888">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="4a611-1888">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4a611-1889">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4a611-1889">HDInsight</span></span>
* <span data-ttu-id="4a611-1890">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1890">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="4a611-1891">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1891">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="4a611-1892">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1892">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="4a611-1893">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="4a611-1893">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="4a611-1894">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1894">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="4a611-1895">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1895">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-1896">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-1896">IoT</span></span>
* <span data-ttu-id="4a611-1897">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="4a611-1897">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="4a611-1898">Kusto</span><span class="sxs-lookup"><span data-stu-id="4a611-1898">Kusto</span></span>
* <span data-ttu-id="4a611-1899">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="4a611-1899">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-1900">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-1900">Monitor</span></span>
* <span data-ttu-id="4a611-1901">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="4a611-1901">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-1902">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-1902">Profile</span></span>
* <span data-ttu-id="4a611-1903">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="4a611-1903">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="4a611-1904">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-1904">Network</span></span>
* <span data-ttu-id="4a611-1905">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1905">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="4a611-1906">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="4a611-1906">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-1907">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-1907">Resource</span></span>
* <span data-ttu-id="4a611-1908">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1908">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="4a611-1909">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1909">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="4a611-1910">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-1910">SQL Virtual Machine</span></span>
* <span data-ttu-id="4a611-1911">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="4a611-1911">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-1912">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-1912">Storage</span></span>
* <span data-ttu-id="4a611-1913">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="4a611-1913">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="4a611-1914">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="4a611-1914">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-1915">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-1915">VM</span></span>
* <span data-ttu-id="4a611-1916">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="4a611-1916">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="4a611-1917">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1917">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="4a611-1918">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1918">January 15, 2019</span></span>

<span data-ttu-id="4a611-1919">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="4a611-1919">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-1920">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-1920">ACR</span></span>
* <span data-ttu-id="4a611-1921">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="4a611-1921">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="4a611-1922">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="4a611-1922">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="4a611-1923">[УСТАРЕЛО] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="4a611-1923">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="4a611-1924">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-1924">ACS</span></span>
* <span data-ttu-id="4a611-1925">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="4a611-1925">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-1926">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-1926">Appservice</span></span>
* <span data-ttu-id="4a611-1927">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="4a611-1927">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="4a611-1928">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="4a611-1928">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="4a611-1929">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="4a611-1929">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="4a611-1930">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1930">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="4a611-1931">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4a611-1931">Botservice</span></span>
* <span data-ttu-id="4a611-1932">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1932">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="4a611-1933">Configure</span><span class="sxs-lookup"><span data-stu-id="4a611-1933">Configure</span></span>
* <span data-ttu-id="4a611-1934">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1934">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4a611-1935">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-1935">CosmosDB</span></span>
* <span data-ttu-id="4a611-1936">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="4a611-1936">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4a611-1937">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4a611-1937">HDInsight</span></span>
* <span data-ttu-id="4a611-1938">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="4a611-1938">Added commands for managing applications</span></span>
* <span data-ttu-id="4a611-1939">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1939">Added commands for managing script actions</span></span>
* <span data-ttu-id="4a611-1940">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="4a611-1940">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="4a611-1941">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1941">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="4a611-1942">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-1942">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="4a611-1943">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-1943">Network</span></span>
* <span data-ttu-id="4a611-1944">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4a611-1944">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="4a611-1945">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="4a611-1945">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="4a611-1946">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4a611-1946">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="4a611-1947">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1947">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="4a611-1948">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-1948">Role</span></span>
* <span data-ttu-id="4a611-1949">[УСТАРЕЛО] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a611-1949">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="4a611-1950">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="4a611-1950">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="4a611-1951">Безопасность</span><span class="sxs-lookup"><span data-stu-id="4a611-1951">Security</span></span>
* <span data-ttu-id="4a611-1952">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="4a611-1952">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-1953">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-1953">Storage</span></span>
* <span data-ttu-id="4a611-1954">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="4a611-1954">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="4a611-1955">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1955">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="4a611-1956">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1956">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="4a611-1957">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1957">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="4a611-1958">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1958">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-1959">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-1959">VM</span></span>
* <span data-ttu-id="4a611-1960">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="4a611-1960">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="4a611-1961">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1961">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="4a611-1962">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1962">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="4a611-1963">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="4a611-1963">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="4a611-1964">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-1964">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="4a611-1965">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="4a611-1965">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="4a611-1966">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1966">December 20, 2018</span></span>

<span data-ttu-id="4a611-1967">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="4a611-1967">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="4a611-1968">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-1968">Appservice</span></span>
* <span data-ttu-id="4a611-1969">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="4a611-1969">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="4a611-1970">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="4a611-1970">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="4a611-1971">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="4a611-1971">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="4a611-1972">IoT Central</span><span class="sxs-lookup"><span data-stu-id="4a611-1972">IoTCentral</span></span>
* <span data-ttu-id="4a611-1973">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="4a611-1973">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="4a611-1974">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-1974">Role</span></span>
* <span data-ttu-id="4a611-1975">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1975">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-1976">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-1976">SQL</span></span>
* <span data-ttu-id="4a611-1977">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="4a611-1977">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-1978">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-1978">VM</span></span>
* <span data-ttu-id="4a611-1979">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1979">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="4a611-1980">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1980">December 18, 2018</span></span>

<span data-ttu-id="4a611-1981">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="4a611-1981">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="4a611-1982">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-1982">ACR</span></span>
* <span data-ttu-id="4a611-1983">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4a611-1983">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="4a611-1984">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="4a611-1984">Condensed the table layout for task list</span></span>
* <span data-ttu-id="4a611-1985">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="4a611-1985">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-1986">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-1986">ACS</span></span>
* <span data-ttu-id="4a611-1987">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1987">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="4a611-1988">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="4a611-1988">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="4a611-1989">[УСТАРЕЛО] Команды `az acs` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="4a611-1989">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="4a611-1990">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-1990">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="4a611-1991">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="4a611-1991">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="4a611-1992">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="4a611-1992">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-1993">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-1993">Appservice</span></span>
* <span data-ttu-id="4a611-1994">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1994">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="4a611-1995">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4a611-1995">Botservice</span></span>
* <span data-ttu-id="4a611-1996">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="4a611-1996">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="4a611-1997">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="4a611-1997">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="4a611-1998">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="4a611-1998">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="4a611-1999">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="4a611-1999">Reduced Kudu network calls</span></span>
* <span data-ttu-id="4a611-2000">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="4a611-2000">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="4a611-2001">Потребление</span><span class="sxs-lookup"><span data-stu-id="4a611-2001">Consumption</span></span>
* <span data-ttu-id="4a611-2002">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="4a611-2002">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4a611-2003">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-2003">CosmosDB</span></span>
* <span data-ttu-id="4a611-2004">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="4a611-2004">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="4a611-2005">Maps</span><span class="sxs-lookup"><span data-stu-id="4a611-2005">Maps</span></span>
* <span data-ttu-id="4a611-2006">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="4a611-2006">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="4a611-2007">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-2007">Network</span></span>
* <span data-ttu-id="4a611-2008">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2008">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="4a611-2009">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="4a611-2009">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-2010">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-2010">Resource</span></span>
* <span data-ttu-id="4a611-2011">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2011">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="4a611-2012">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2012">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-2013">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-2013">Storage</span></span>
*  <span data-ttu-id="4a611-2014">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="4a611-2014">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2015">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2015">VM</span></span>
* <span data-ttu-id="4a611-2016">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="4a611-2016">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="4a611-2017">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2017">December 4, 2018</span></span>

<span data-ttu-id="4a611-2018">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="4a611-2018">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="4a611-2019">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-2019">Core</span></span>
* <span data-ttu-id="4a611-2020">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="4a611-2020">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="4a611-2021">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="4a611-2021">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-2022">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-2022">Appservice</span></span>
* <span data-ttu-id="4a611-2023">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="4a611-2023">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="4a611-2024">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="4a611-2024">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="4a611-2025">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-2025">Network</span></span>
* <span data-ttu-id="4a611-2026">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="4a611-2026">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="4a611-2027">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-2027">Role</span></span>
* <span data-ttu-id="4a611-2028">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="4a611-2028">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="4a611-2029">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2029">VM</span></span>
* <span data-ttu-id="4a611-2030">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a611-2030">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="4a611-2031">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="4a611-2031">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="4a611-2032">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="4a611-2032">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="4a611-2033">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="4a611-2033">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="4a611-2034">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2034">November 20, 2018</span></span>

<span data-ttu-id="4a611-2035">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="4a611-2035">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="4a611-2036">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-2036">Core</span></span>
* <span data-ttu-id="4a611-2037">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="4a611-2037">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-2038">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-2038">ACR</span></span>
* <span data-ttu-id="4a611-2039">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="4a611-2039">Added context token to task step</span></span>
* <span data-ttu-id="4a611-2040">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="4a611-2040">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="4a611-2041">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2041">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-2042">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-2042">Appservice</span></span>
* <span data-ttu-id="4a611-2043">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="4a611-2043">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="4a611-2044">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-2044">Updated the default `node_version`.</span></span> <span data-ttu-id="4a611-2045">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="4a611-2045">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="4a611-2046">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="4a611-2046">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="4a611-2047">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="4a611-2047">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="4a611-2048">IotCentral</span><span class="sxs-lookup"><span data-stu-id="4a611-2048">IotCentral</span></span>
* <span data-ttu-id="4a611-2049">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="4a611-2049">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="4a611-2050">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4a611-2050">KeyVault</span></span>
* <span data-ttu-id="4a611-2051">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="4a611-2051">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="4a611-2052">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-2052">Network</span></span>
* <span data-ttu-id="4a611-2053">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2053">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="4a611-2054">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2054">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="4a611-2055">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="4a611-2055">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="4a611-2056">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2056">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="4a611-2057">Rdbms</span><span class="sxs-lookup"><span data-stu-id="4a611-2057">Rdbms</span></span>
* <span data-ttu-id="4a611-2058">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="4a611-2058">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="4a611-2059">RBAC:</span><span class="sxs-lookup"><span data-stu-id="4a611-2059">Rbac</span></span>
* <span data-ttu-id="4a611-2060">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2060">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="4a611-2061">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="4a611-2061">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="4a611-2062">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-2062">Storage</span></span>
* <span data-ttu-id="4a611-2063">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="4a611-2063">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="4a611-2064">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2064">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="4a611-2065">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="4a611-2065">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="4a611-2066">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2066">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2067">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2067">VM</span></span>
* <span data-ttu-id="4a611-2068">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="4a611-2068">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="4a611-2069">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2069">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="4a611-2070">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2070">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="4a611-2071">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="4a611-2071">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="4a611-2072">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2072">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="4a611-2073">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2073">Added `snapshot wait` command</span></span>
* <span data-ttu-id="4a611-2074">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2074">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="4a611-2075">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2075">November 6, 2018</span></span>

<span data-ttu-id="4a611-2076">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="4a611-2076">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="4a611-2077">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-2077">Core</span></span>
* <span data-ttu-id="4a611-2078">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="4a611-2078">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-2079">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-2079">ACR</span></span>
* <span data-ttu-id="4a611-2080">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="4a611-2080">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="4a611-2081">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="4a611-2081">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-2082">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-2082">ACS</span></span>
* <span data-ttu-id="4a611-2083">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-2083">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="4a611-2084">Помощник</span><span class="sxs-lookup"><span data-stu-id="4a611-2084">Advisor</span></span>
* <span data-ttu-id="4a611-2085">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="4a611-2085">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="4a611-2086">AMS</span><span class="sxs-lookup"><span data-stu-id="4a611-2086">AMS</span></span>
* <span data-ttu-id="4a611-2087">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="4a611-2087">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="4a611-2088">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="4a611-2088">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="4a611-2089">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2089">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="4a611-2090">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="4a611-2090">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="4a611-2091">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2091">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="4a611-2092">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2092">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="4a611-2093">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2093">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="4a611-2094">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2094">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="4a611-2095">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2095">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="4a611-2096">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2096">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="4a611-2097">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2097">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="4a611-2098">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2098">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="4a611-2099">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="4a611-2099">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="4a611-2100">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="4a611-2100">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="4a611-2101">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2101">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="4a611-2102">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="4a611-2102">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="4a611-2103">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="4a611-2103">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-2104">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-2104">AppService</span></span>
* <span data-ttu-id="4a611-2105">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="4a611-2105">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="4a611-2106">Configure</span><span class="sxs-lookup"><span data-stu-id="4a611-2106">Configure</span></span>
* <span data-ttu-id="4a611-2107">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="4a611-2107">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="4a611-2108">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-2108">Container</span></span>
* <span data-ttu-id="4a611-2109">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="4a611-2109">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="4a611-2110">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="4a611-2110">EventHub</span></span>
* <span data-ttu-id="4a611-2111">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2111">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="4a611-2112">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="4a611-2112">Interactive</span></span>
* <span data-ttu-id="4a611-2113">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="4a611-2113">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-2114">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-2114">Monitor</span></span>
* <span data-ttu-id="4a611-2115">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2115">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="4a611-2116">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-2116">Network</span></span>
* <span data-ttu-id="4a611-2117">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2117">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="4a611-2118">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="4a611-2118">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="4a611-2119">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2119">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="4a611-2120">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-2120">Profile</span></span>
* <span data-ttu-id="4a611-2121">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2121">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="4a611-2122">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4a611-2122">RDBMS</span></span>
* <span data-ttu-id="4a611-2123">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="4a611-2123">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-2124">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-2124">Resource</span></span>
* <span data-ttu-id="4a611-2125">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2125">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="4a611-2126">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-2126">Role</span></span>
* <span data-ttu-id="4a611-2127">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="4a611-2127">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="4a611-2128">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="4a611-2128">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="4a611-2129">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="4a611-2129">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-2130">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-2130">Storage</span></span>
* <span data-ttu-id="4a611-2131">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2131">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2132">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2132">VM</span></span>
* <span data-ttu-id="4a611-2133">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="4a611-2133">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="4a611-2134">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="4a611-2134">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="4a611-2135">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="4a611-2135">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="4a611-2136">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="4a611-2136">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="4a611-2137">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="4a611-2137">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="4a611-2138">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2138">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="4a611-2139">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2139">October 23, 2018</span></span>

<span data-ttu-id="4a611-2140">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="4a611-2140">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="4a611-2141">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-2141">Core</span></span>
* <span data-ttu-id="4a611-2142">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2142">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="4a611-2143">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2143">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-2144">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-2144">ACR</span></span>
* <span data-ttu-id="4a611-2145">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="4a611-2145">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="4a611-2146">CDN</span><span class="sxs-lookup"><span data-stu-id="4a611-2146">CDN</span></span>
* <span data-ttu-id="4a611-2147">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-2147">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="4a611-2148">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="4a611-2148">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="4a611-2149">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-2149">Container</span></span>
* <span data-ttu-id="4a611-2150">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="4a611-2150">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="4a611-2151">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="4a611-2151">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="4a611-2152">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2152">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="4a611-2153">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4a611-2153">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="4a611-2154">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="4a611-2154">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="4a611-2155">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="4a611-2155">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="4a611-2156">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2156">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4a611-2157">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-2157">CosmosDB</span></span>
* <span data-ttu-id="4a611-2158">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2158">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="4a611-2159">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="4a611-2159">Interactive</span></span>
* <span data-ttu-id="4a611-2160">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="4a611-2160">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="4a611-2161">IoT Central</span><span class="sxs-lookup"><span data-stu-id="4a611-2161">IoT Central</span></span>
* <span data-ttu-id="4a611-2162">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="4a611-2162">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="4a611-2163">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="4a611-2163">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-2164">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-2164">Monitor</span></span>
* <span data-ttu-id="4a611-2165">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="4a611-2165">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="4a611-2166">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="4a611-2166">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="4a611-2167">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="4a611-2167">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="4a611-2168">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="4a611-2168">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="4a611-2169">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2169">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="4a611-2170">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="4a611-2170">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="4a611-2171">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="4a611-2171">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="4a611-2172">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="4a611-2172">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="4a611-2173">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="4a611-2173">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="4a611-2174">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2174">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="4a611-2175">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-2175">Network</span></span>
* <span data-ttu-id="4a611-2176">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="4a611-2176">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="4a611-2177">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="4a611-2177">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="4a611-2178">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="4a611-2178">ServiceBus</span></span>
* <span data-ttu-id="4a611-2179">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="4a611-2179">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-2180">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-2180">SQL</span></span>
* <span data-ttu-id="4a611-2181">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="4a611-2181">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-2182">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-2182">Storage</span></span>
* <span data-ttu-id="4a611-2183">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="4a611-2183">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="4a611-2184">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="4a611-2184">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2185">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2185">VM</span></span>
* <span data-ttu-id="4a611-2186">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="4a611-2186">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="4a611-2187">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="4a611-2187">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="4a611-2188">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="4a611-2188">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="4a611-2189">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2189">October 16, 2018</span></span>

<span data-ttu-id="4a611-2190">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="4a611-2190">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2191">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2191">VM</span></span>
* <span data-ttu-id="4a611-2192">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="4a611-2192">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="4a611-2193">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2193">October 9, 2018</span></span>

<span data-ttu-id="4a611-2194">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="4a611-2194">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="4a611-2195">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-2195">Core</span></span>
* <span data-ttu-id="4a611-2196">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="4a611-2196">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-2197">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-2197">ACR</span></span>
* <span data-ttu-id="4a611-2198">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="4a611-2198">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-2199">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-2199">ACS</span></span>
* <span data-ttu-id="4a611-2200">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="4a611-2200">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="4a611-2201">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="4a611-2201">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="4a611-2202">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2202">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="4a611-2203">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="4a611-2203">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="4a611-2204">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-2204">Container</span></span>
* <span data-ttu-id="4a611-2205">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="4a611-2205">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="4a611-2206">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="4a611-2206">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="4a611-2207">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="4a611-2207">Event Hub</span></span>
* <span data-ttu-id="4a611-2208">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2208">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="4a611-2209">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="4a611-2209">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="4a611-2210">Модули</span><span class="sxs-lookup"><span data-stu-id="4a611-2210">Extensions</span></span>
* <span data-ttu-id="4a611-2211">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="4a611-2211">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="4a611-2212">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4a611-2212">HDInsight</span></span>
* <span data-ttu-id="4a611-2213">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="4a611-2213">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-2214">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-2214">IoT</span></span>
* <span data-ttu-id="4a611-2215">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="4a611-2215">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="4a611-2216">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4a611-2216">KeyVault</span></span>
* <span data-ttu-id="4a611-2217">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="4a611-2217">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="4a611-2218">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-2218">Network</span></span>
* <span data-ttu-id="4a611-2219">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-2219">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="4a611-2220">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="4a611-2220">See #6052</span></span>
* <span data-ttu-id="4a611-2221">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2221">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="4a611-2222">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="4a611-2222">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="4a611-2223">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2223">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="4a611-2224">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2224">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="4a611-2225">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2225">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="4a611-2226">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2226">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="4a611-2227">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-2227">Role</span></span>
* <span data-ttu-id="4a611-2228">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2228">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="4a611-2229">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2229">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="4a611-2230">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="4a611-2230">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="4a611-2231">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="4a611-2231">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="4a611-2232">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="4a611-2232">Service Bus</span></span>
* <span data-ttu-id="4a611-2233">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="4a611-2233">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2234">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2234">VM</span></span>
* <span data-ttu-id="4a611-2235">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2235">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="4a611-2236">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="4a611-2236">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="4a611-2237">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2237">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="4a611-2238">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2238">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="4a611-2239">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="4a611-2239">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="4a611-2240">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="4a611-2240">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="4a611-2241">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2241">September 21, 2018</span></span>

<span data-ttu-id="4a611-2242">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="4a611-2242">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-2243">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-2243">ACR</span></span>
* <span data-ttu-id="4a611-2244">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="4a611-2244">Added ACR Task commands</span></span>
* <span data-ttu-id="4a611-2245">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="4a611-2245">Added quick run command</span></span>
* <span data-ttu-id="4a611-2246">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="4a611-2246">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="4a611-2247">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="4a611-2247">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="4a611-2248">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="4a611-2248">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="4a611-2249">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="4a611-2249">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-2250">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-2250">ACS</span></span>
* <span data-ttu-id="4a611-2251">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="4a611-2251">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="4a611-2252">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="4a611-2252">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-2253">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-2253">AppService</span></span>

* <span data-ttu-id="4a611-2254">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="4a611-2254">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="4a611-2255">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="4a611-2255">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="4a611-2256">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="4a611-2256">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="4a611-2257">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="4a611-2257">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="4a611-2258">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-2258">Batch</span></span>
* <span data-ttu-id="4a611-2259">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="4a611-2259">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="4a611-2260">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2260">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="4a611-2261">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2261">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="4a611-2262">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="4a611-2262">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4a611-2263">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4a611-2263">Batch AI</span></span> 
* <span data-ttu-id="4a611-2264">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2264">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4a611-2265">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4a611-2265">Cognitive Services</span></span>
* <span data-ttu-id="4a611-2266">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2266">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="4a611-2267">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2267">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="4a611-2268">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2268">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="4a611-2269">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2269">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="4a611-2270">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="4a611-2270">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="4a611-2271">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2271">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="4a611-2272">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-2272">Container</span></span>
* <span data-ttu-id="4a611-2273">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4a611-2273">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="4a611-2274">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="4a611-2274">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="4a611-2275">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="4a611-2275">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="4a611-2276">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4a611-2276">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="4a611-2277">Data Lake</span><span class="sxs-lookup"><span data-stu-id="4a611-2277">Datalake</span></span>
* <span data-ttu-id="4a611-2278">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="4a611-2278">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="4a611-2279">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="4a611-2279">Interactive Shell</span></span>
* <span data-ttu-id="4a611-2280">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="4a611-2280">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="4a611-2281">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2281">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-2282">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-2282">IoT</span></span>
* <span data-ttu-id="4a611-2283">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="4a611-2283">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="4a611-2284">Key Vault</span><span class="sxs-lookup"><span data-stu-id="4a611-2284">Key Vault</span></span>
* <span data-ttu-id="4a611-2285">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="4a611-2285">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="4a611-2286">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-2286">Network</span></span>
* <span data-ttu-id="4a611-2287">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2287">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="4a611-2288">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="4a611-2288">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="4a611-2289">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="4a611-2289">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="4a611-2290">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2290">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="4a611-2291">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2291">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="4a611-2292">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2292">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="4a611-2293">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="4a611-2293">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="4a611-2294">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2294">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="4a611-2295">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2295">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="4a611-2296">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2296">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="4a611-2297">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2297">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="4a611-2298">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2298">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="4a611-2299">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2299">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="4a611-2300">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="4a611-2300">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="4a611-2301">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2301">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="4a611-2302">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="4a611-2302">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="4a611-2303">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="4a611-2303">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="4a611-2304">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="4a611-2304">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="4a611-2305">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4a611-2305">RDBMS</span></span>
* <span data-ttu-id="4a611-2306">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="4a611-2306">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="4a611-2307">резервирование.</span><span class="sxs-lookup"><span data-stu-id="4a611-2307">Reservation</span></span>
* <span data-ttu-id="4a611-2308">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2308">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="4a611-2309">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="4a611-2309">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="4a611-2310">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="4a611-2310">Manage App</span></span>
* <span data-ttu-id="4a611-2311">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="4a611-2311">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="4a611-2312">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="4a611-2312">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="4a611-2313">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-2313">Role</span></span>
* <span data-ttu-id="4a611-2314">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="4a611-2314">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="4a611-2315">SignalR</span><span class="sxs-lookup"><span data-stu-id="4a611-2315">SignalR</span></span>
* <span data-ttu-id="4a611-2316">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="4a611-2316">First release</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-2317">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-2317">Storage</span></span>
* <span data-ttu-id="4a611-2318">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="4a611-2318">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="4a611-2319">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="4a611-2319">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2320">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2320">VM</span></span>
* <span data-ttu-id="4a611-2321">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="4a611-2321">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="4a611-2322">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2322">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="4a611-2323">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2323">August 28, 2018</span></span>

<span data-ttu-id="4a611-2324">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="4a611-2324">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="4a611-2325">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-2325">Core</span></span>

* <span data-ttu-id="4a611-2326">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="4a611-2326">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="4a611-2327">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="4a611-2327">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-2328">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-2328">ACR</span></span>

* <span data-ttu-id="4a611-2329">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="4a611-2329">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="4a611-2330">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2330">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-2331">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-2331">ACS</span></span>

* <span data-ttu-id="4a611-2332">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2332">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="4a611-2333">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="4a611-2333">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-2334">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-2334">AppService</span></span>

* <span data-ttu-id="4a611-2335">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="4a611-2335">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="4a611-2336">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="4a611-2336">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="4a611-2337">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="4a611-2337">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="4a611-2338">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="4a611-2338">Backup</span></span>

* <span data-ttu-id="4a611-2339">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="4a611-2339">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="4a611-2340">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="4a611-2340">Bot Service</span></span>

* <span data-ttu-id="4a611-2341">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="4a611-2341">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4a611-2342">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4a611-2342">Cognitive Services</span></span>

* <span data-ttu-id="4a611-2343">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="4a611-2343">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-2344">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-2344">IoT</span></span>

* <span data-ttu-id="4a611-2345">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="4a611-2345">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-2346">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-2346">Monitor</span></span>

* <span data-ttu-id="4a611-2347">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="4a611-2347">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="4a611-2348">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="4a611-2348">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="4a611-2349">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-2349">Network</span></span>

* <span data-ttu-id="4a611-2350">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="4a611-2350">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-2351">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-2351">Resource</span></span>

* <span data-ttu-id="4a611-2352">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="4a611-2352">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-2353">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-2353">Storage</span></span>

* <span data-ttu-id="4a611-2354">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="4a611-2354">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2355">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2355">VM</span></span>

* <span data-ttu-id="4a611-2356">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="4a611-2356">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="4a611-2357">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2357">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="4a611-2358">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2358">Auguest 14, 2018</span></span>

<span data-ttu-id="4a611-2359">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="4a611-2359">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="4a611-2360">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-2360">Core</span></span>

* <span data-ttu-id="4a611-2361">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2361">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="4a611-2362">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="4a611-2362">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="4a611-2363">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="4a611-2363">Telemetry</span></span>

* <span data-ttu-id="4a611-2364">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="4a611-2364">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-2365">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-2365">ACR</span></span>

* <span data-ttu-id="4a611-2366">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2366">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="4a611-2367">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2367">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-2368">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-2368">ACS</span></span>

* <span data-ttu-id="4a611-2369">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="4a611-2369">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="4a611-2370">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="4a611-2370">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="4a611-2371">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="4a611-2371">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="4a611-2372">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="4a611-2372">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="4a611-2373">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="4a611-2373">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="4a611-2374">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-2374">AppService</span></span>

* <span data-ttu-id="4a611-2375">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2375">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="4a611-2376">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="4a611-2376">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="4a611-2377">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4a611-2377">BatchAI</span></span>

* <span data-ttu-id="4a611-2378">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="4a611-2378">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="4a611-2379">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-2379">Container</span></span>

* <span data-ttu-id="4a611-2380">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="4a611-2380">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="4a611-2381">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-2381">IoT</span></span>

* <span data-ttu-id="4a611-2382">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="4a611-2382">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="4a611-2383">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2383">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="4a611-2384">IoT Central</span><span class="sxs-lookup"><span data-stu-id="4a611-2384">Iot Central</span></span>

* <span data-ttu-id="4a611-2385">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="4a611-2385">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="4a611-2386">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4a611-2386">KeyVault</span></span>


* <span data-ttu-id="4a611-2387">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="4a611-2387">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="4a611-2388">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="4a611-2388">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="4a611-2389">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="4a611-2389">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="4a611-2390">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="4a611-2390">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="4a611-2391">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="4a611-2391">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="4a611-2392">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="4a611-2392">Relay</span></span>

* <span data-ttu-id="4a611-2393">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="4a611-2393">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-2394">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-2394">Sql</span></span>

* <span data-ttu-id="4a611-2395">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2395">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-2396">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-2396">Storage</span></span>

* <span data-ttu-id="4a611-2397">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="4a611-2397">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="4a611-2398">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="4a611-2398">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="4a611-2399">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="4a611-2399">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="4a611-2400">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="4a611-2400">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="4a611-2401">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="4a611-2401">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2402">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2402">VM</span></span>

* <span data-ttu-id="4a611-2403">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="4a611-2403">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="4a611-2404">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2404">July 31, 2018</span></span>

<span data-ttu-id="4a611-2405">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="4a611-2405">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-2406">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-2406">ACR</span></span>

* <span data-ttu-id="4a611-2407">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2407">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="4a611-2408">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2408">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-2409">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-2409">ACS</span></span>

* <span data-ttu-id="4a611-2410">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="4a611-2410">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="4a611-2411">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-2411">Batch</span></span>

* <span data-ttu-id="4a611-2412">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="4a611-2412">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="4a611-2413">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-2413">Container</span></span>

* <span data-ttu-id="4a611-2414">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="4a611-2414">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="4a611-2415">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-2415">Network</span></span>

* <span data-ttu-id="4a611-2416">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="4a611-2416">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="4a611-2417">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-2417">Resource</span></span>

* <span data-ttu-id="4a611-2418">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="4a611-2418">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="4a611-2419">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="4a611-2419">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="4a611-2420">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-2420">Role</span></span>

* <span data-ttu-id="4a611-2421">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="4a611-2421">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="4a611-2422">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="4a611-2422">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="4a611-2423">Поиск</span><span class="sxs-lookup"><span data-stu-id="4a611-2423">Search</span></span>

* <span data-ttu-id="4a611-2424">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="4a611-2424">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="4a611-2425">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="4a611-2425">Service Bus</span></span>

* <span data-ttu-id="4a611-2426">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="4a611-2426">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="4a611-2427">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="4a611-2427">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="4a611-2428">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="4a611-2428">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="4a611-2429">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2429">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-2430">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-2430">Storage</span></span>

* <span data-ttu-id="4a611-2431">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="4a611-2431">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="4a611-2432">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="4a611-2432">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2433">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2433">VM</span></span>

* <span data-ttu-id="4a611-2434">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="4a611-2434">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="4a611-2435">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2435">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="4a611-2436">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="4a611-2436">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="4a611-2437">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="4a611-2437">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="4a611-2438">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2438">July 18, 2018</span></span>

<span data-ttu-id="4a611-2439">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="4a611-2439">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="4a611-2440">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-2440">Core</span></span>

* <span data-ttu-id="4a611-2441">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="4a611-2441">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="4a611-2442">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="4a611-2442">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="4a611-2443">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="4a611-2443">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-2444">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-2444">ACR</span></span>

* <span data-ttu-id="4a611-2445">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="4a611-2445">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="4a611-2446">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2446">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="4a611-2447">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="4a611-2447">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="4a611-2448">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="4a611-2448">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-2449">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-2449">ACS</span></span>

* <span data-ttu-id="4a611-2450">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="4a611-2450">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-2451">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-2451">AppService</span></span>

* <span data-ttu-id="4a611-2452">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="4a611-2452">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="4a611-2453">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-2453">Batch</span></span>

* <span data-ttu-id="4a611-2454">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="4a611-2454">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="4a611-2455">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="4a611-2455">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4a611-2456">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4a611-2456">Batch AI</span></span>

* <span data-ttu-id="4a611-2457">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2457">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="4a611-2458">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-2458">Container</span></span>

* <span data-ttu-id="4a611-2459">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="4a611-2459">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="4a611-2460">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="4a611-2460">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="4a611-2461">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-2461">Network</span></span>

* <span data-ttu-id="4a611-2462">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2462">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="4a611-2463">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2463">Added `network nic wait`</span></span>
* <span data-ttu-id="4a611-2464">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="4a611-2464">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="4a611-2465">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="4a611-2465">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="4a611-2466">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-2466">Resource</span></span>

* <span data-ttu-id="4a611-2467">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2467">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="4a611-2468">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2468">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="4a611-2469">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2469">Added `deployment wait` command</span></span>
* <span data-ttu-id="4a611-2470">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="4a611-2470">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-2471">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-2471">SQL</span></span>

* <span data-ttu-id="4a611-2472">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2472">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="4a611-2473">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2473">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="4a611-2474">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2474">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-2475">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-2475">Storage</span></span>

* <span data-ttu-id="4a611-2476">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2476">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2477">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2477">VM</span></span>

* <span data-ttu-id="4a611-2478">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-2478">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="4a611-2479">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2479">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="4a611-2480">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2480">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="4a611-2481">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2481">July 3, 2018</span></span>

<span data-ttu-id="4a611-2482">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="4a611-2482">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="4a611-2483">AKS</span><span class="sxs-lookup"><span data-stu-id="4a611-2483">AKS</span></span>

* <span data-ttu-id="4a611-2484">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="4a611-2484">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="4a611-2485">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2485">July 3, 2018</span></span>

<span data-ttu-id="4a611-2486">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="4a611-2486">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="4a611-2487">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-2487">Core</span></span>

* <span data-ttu-id="4a611-2488">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="4a611-2488">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-2489">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-2489">ACR</span></span>

* <span data-ttu-id="4a611-2490">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="4a611-2490">Added polling build status</span></span>
* <span data-ttu-id="4a611-2491">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="4a611-2491">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="4a611-2492">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2492">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-2493">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-2493">ACS</span></span>

* <span data-ttu-id="4a611-2494">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-2494">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="4a611-2495">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-2495">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="4a611-2496">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2496">Updated options for `aks browse` command.</span></span> <span data-ttu-id="4a611-2497">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2497">Added `--listen-port` support</span></span>
* <span data-ttu-id="4a611-2498">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2498">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="4a611-2499">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="4a611-2499">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="4a611-2500">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2500">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-2501">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-2501">AppService</span></span>

* <span data-ttu-id="4a611-2502">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2502">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="4a611-2503">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="4a611-2503">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="4a611-2504">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="4a611-2504">Backup</span></span>

* <span data-ttu-id="4a611-2505">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="4a611-2505">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="4a611-2506">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4a611-2506">BatchAI</span></span>

* <span data-ttu-id="4a611-2507">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2507">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="4a611-2508">Cloud</span><span class="sxs-lookup"><span data-stu-id="4a611-2508">Cloud</span></span>

* <span data-ttu-id="4a611-2509">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2509">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="4a611-2510">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-2510">Container</span></span>

* <span data-ttu-id="4a611-2511">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="4a611-2511">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="4a611-2512">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2512">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="4a611-2513">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="4a611-2513">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="4a611-2514">Расширение</span><span class="sxs-lookup"><span data-stu-id="4a611-2514">Extension</span></span>

* <span data-ttu-id="4a611-2515">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="4a611-2515">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="4a611-2516">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-2516">Network</span></span>

* <span data-ttu-id="4a611-2517">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="4a611-2517">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="4a611-2518">Rdbms</span><span class="sxs-lookup"><span data-stu-id="4a611-2518">Rdbms</span></span>

* <span data-ttu-id="4a611-2519">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2519">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-2520">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-2520">Resource</span></span>

* <span data-ttu-id="4a611-2521">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2521">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2522">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2522">VM</span></span>

* <span data-ttu-id="4a611-2523">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="4a611-2523">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="4a611-2524">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2524">June 25, 2018</span></span>

<span data-ttu-id="4a611-2525">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="4a611-2525">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="4a611-2526">CLI</span><span class="sxs-lookup"><span data-stu-id="4a611-2526">CLI</span></span>

* <span data-ttu-id="4a611-2527">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="4a611-2527">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="4a611-2528">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2528">June 19, 2018</span></span>

<span data-ttu-id="4a611-2529">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="4a611-2529">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="4a611-2530">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-2530">Core</span></span>

* <span data-ttu-id="4a611-2531">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="4a611-2531">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-2532">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-2532">ACR</span></span>

* <span data-ttu-id="4a611-2533">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2533">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="4a611-2534">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="4a611-2534">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-2535">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-2535">ACS</span></span>

* <span data-ttu-id="4a611-2536">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2536">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="4a611-2537">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2537">Added `--update` support</span></span>
* <span data-ttu-id="4a611-2538">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2538">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="4a611-2539">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2539">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="4a611-2540">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2540">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="4a611-2541">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2541">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="4a611-2542">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2542">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="4a611-2543">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2543">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-2544">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-2544">AppService</span></span>

* <span data-ttu-id="4a611-2545">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="4a611-2545">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="4a611-2546">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2546">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="4a611-2547">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-2547">Batch</span></span>

* <span data-ttu-id="4a611-2548">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2548">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4a611-2549">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4a611-2549">Batch AI</span></span>

* <span data-ttu-id="4a611-2550">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="4a611-2550">Added support for workspaces.</span></span> <span data-ttu-id="4a611-2551">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2551">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="4a611-2552">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2552">Added support for experiments.</span></span> <span data-ttu-id="4a611-2553">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="4a611-2553">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="4a611-2554">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="4a611-2554">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="4a611-2555">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2555">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="4a611-2556">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2556">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="4a611-2557">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2557">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="4a611-2558">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="4a611-2558">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="4a611-2559">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2559">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="4a611-2560">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2560">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="4a611-2561">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2561">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="4a611-2562">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2562">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="4a611-2563">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2563">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="4a611-2564">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2564">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="4a611-2565">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="4a611-2565">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="4a611-2566">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2566">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="4a611-2567">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="4a611-2567">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="4a611-2568">[`--config`, `-c`] переименовано в [`--config-file`, `-f`].</span><span class="sxs-lookup"><span data-stu-id="4a611-2568">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="4a611-2569">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="4a611-2569">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="4a611-2570">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="4a611-2570">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="4a611-2571">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="4a611-2571">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="4a611-2572">Maps</span><span class="sxs-lookup"><span data-stu-id="4a611-2572">Maps</span></span>

* <span data-ttu-id="4a611-2573">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2573">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="4a611-2574">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-2574">Network</span></span>

* <span data-ttu-id="4a611-2575">Добавлена поддержка `https` в `network lb probe create` ([№ 6571](https://github.com/Azure/azure-cli/issues/6571)).</span><span class="sxs-lookup"><span data-stu-id="4a611-2575">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="4a611-2576">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="4a611-2576">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="4a611-2577">#6502</span><span class="sxs-lookup"><span data-stu-id="4a611-2577">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="4a611-2578">Резервирование</span><span class="sxs-lookup"><span data-stu-id="4a611-2578">Reservations</span></span>

* <span data-ttu-id="4a611-2579">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2579">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="4a611-2580">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2580">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="4a611-2581">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2581">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="4a611-2582">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2582">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="4a611-2583">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2583">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="4a611-2584">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2584">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="4a611-2585">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-2585">Role</span></span>

* <span data-ttu-id="4a611-2586">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="4a611-2586">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-2587">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-2587">SQL</span></span>

* <span data-ttu-id="4a611-2588">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="4a611-2588">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-2589">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-2589">Storage</span></span>

* <span data-ttu-id="4a611-2590">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="4a611-2590">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2591">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2591">VM</span></span>

* <span data-ttu-id="4a611-2592">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2592">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="4a611-2593">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2593">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="4a611-2594">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="4a611-2594">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="4a611-2595">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2595">June 13, 2018</span></span>

<span data-ttu-id="4a611-2596">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="4a611-2596">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="4a611-2597">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-2597">Core</span></span>

* <span data-ttu-id="4a611-2598">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="4a611-2598">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="4a611-2599">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2599">June 13, 2018</span></span>

<span data-ttu-id="4a611-2600">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="4a611-2600">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="4a611-2601">AKS</span><span class="sxs-lookup"><span data-stu-id="4a611-2601">AKS</span></span>

* <span data-ttu-id="4a611-2602">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="4a611-2602">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="4a611-2603">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="4a611-2603">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="4a611-2604">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="4a611-2604">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="4a611-2605">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="4a611-2605">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="4a611-2606">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4a611-2606">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-2607">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-2607">AppService</span></span>

* <span data-ttu-id="4a611-2608">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="4a611-2608">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="4a611-2609">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2609">June 5, 2018</span></span>

<span data-ttu-id="4a611-2610">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="4a611-2610">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="4a611-2611">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="4a611-2611">Interactive</span></span>

* <span data-ttu-id="4a611-2612">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="4a611-2612">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="4a611-2613">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2613">June 5, 2018</span></span>

<span data-ttu-id="4a611-2614">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="4a611-2614">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="4a611-2615">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-2615">Core</span></span>

* <span data-ttu-id="4a611-2616">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="4a611-2616">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="4a611-2617">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="4a611-2617">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-2618">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-2618">ACR</span></span>

* <span data-ttu-id="4a611-2619">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="4a611-2619">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="4a611-2620">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2620">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="4a611-2621">AKS</span><span class="sxs-lookup"><span data-stu-id="4a611-2621">AKS</span></span>

* <span data-ttu-id="4a611-2622">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="4a611-2622">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="4a611-2623">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-2623">Batch</span></span>

* <span data-ttu-id="4a611-2624">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="4a611-2624">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-2625">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-2625">IOT</span></span>

* <span data-ttu-id="4a611-2626">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="4a611-2626">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="4a611-2627">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-2627">Network</span></span>

* <span data-ttu-id="4a611-2628">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2628">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="4a611-2629">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="4a611-2629">Policy Insights</span></span>

* <span data-ttu-id="4a611-2630">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="4a611-2630">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="4a611-2631">ARM</span><span class="sxs-lookup"><span data-stu-id="4a611-2631">ARM</span></span>

* <span data-ttu-id="4a611-2632">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2632">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-2633">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-2633">SQL</span></span>

* <span data-ttu-id="4a611-2634">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="4a611-2634">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="4a611-2635">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="4a611-2635">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="4a611-2636">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-2636">Storage</span></span>

* <span data-ttu-id="4a611-2637">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2637">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2638">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2638">VM</span></span>

* <span data-ttu-id="4a611-2639">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2639">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="4a611-2640">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2640">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="4a611-2641">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2641">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="4a611-2642">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2642">May 22, 2018</span></span>

<span data-ttu-id="4a611-2643">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="4a611-2643">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="4a611-2644">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-2644">Core</span></span>

* <span data-ttu-id="4a611-2645">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2645">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-2646">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-2646">ACS</span></span>

* <span data-ttu-id="4a611-2647">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2647">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="4a611-2648">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="4a611-2648">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-2649">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-2649">AppService</span></span>

* <span data-ttu-id="4a611-2650">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="4a611-2650">Improved generic update commands</span></span>
* <span data-ttu-id="4a611-2651">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2651">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="4a611-2652">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-2652">Container</span></span>

* <span data-ttu-id="4a611-2653">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="4a611-2653">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="4a611-2654">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4a611-2654">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="4a611-2655">Расширение</span><span class="sxs-lookup"><span data-stu-id="4a611-2655">Extension</span></span>

* <span data-ttu-id="4a611-2656">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="4a611-2656">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="4a611-2657">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="4a611-2657">Interactive</span></span>

* <span data-ttu-id="4a611-2658">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="4a611-2658">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="4a611-2659">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="4a611-2659">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="4a611-2660">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4a611-2660">KeyVault</span></span>

* <span data-ttu-id="4a611-2661">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="4a611-2661">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="4a611-2662">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-2662">Network</span></span>

* <span data-ttu-id="4a611-2663">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="4a611-2663">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="4a611-2664">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="4a611-2664">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-2665">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-2665">SQL</span></span>

* <span data-ttu-id="4a611-2666">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="4a611-2666">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="4a611-2667">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2667">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="4a611-2668">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2668">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="4a611-2669">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="4a611-2669">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="4a611-2670">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="4a611-2670">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="4a611-2671">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2671">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="4a611-2672">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2672">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="4a611-2673">`edition`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2673">`edition`.</span></span> <span data-ttu-id="4a611-2674">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2674">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="4a611-2675">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2675">`elasticPoolName`.</span></span> <span data-ttu-id="4a611-2676">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2676">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="4a611-2677">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="4a611-2677">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="4a611-2678">`edition`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2678">`edition`.</span></span> <span data-ttu-id="4a611-2679">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2679">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="4a611-2680">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2680">`dtu`.</span></span> <span data-ttu-id="4a611-2681">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2681">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="4a611-2682">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2682">`databaseDtuMin`.</span></span> <span data-ttu-id="4a611-2683">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2683">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="4a611-2684">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2684">`databaseDtuMax`.</span></span> <span data-ttu-id="4a611-2685">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2685">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="4a611-2686">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2686">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="4a611-2687">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2687">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-2688">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-2688">Storage</span></span>

* <span data-ttu-id="4a611-2689">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2689">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="4a611-2690">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2690">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2691">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2691">VM</span></span>

* <span data-ttu-id="4a611-2692">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2692">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="4a611-2693">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2693">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="4a611-2694">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2694">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="4a611-2695">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="4a611-2695">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="4a611-2696">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2696">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="4a611-2697">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2697">May 7, 2018</span></span>

<span data-ttu-id="4a611-2698">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="4a611-2698">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="4a611-2699">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-2699">Core</span></span>

* <span data-ttu-id="4a611-2700">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="4a611-2700">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="4a611-2701">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2701">Added limited support for positional arguments</span></span>
* <span data-ttu-id="4a611-2702">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2702">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="4a611-2703">#5591</span><span class="sxs-lookup"><span data-stu-id="4a611-2703">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="4a611-2704">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2704">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="4a611-2705">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="4a611-2705">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="4a611-2706">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="4a611-2706">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="4a611-2707">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2707">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="4a611-2708">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="4a611-2708">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-2709">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-2709">ACR</span></span>

* <span data-ttu-id="4a611-2710">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="4a611-2710">Added ACR Build commands</span></span>
* <span data-ttu-id="4a611-2711">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="4a611-2711">Improved resource not found error messages</span></span>
* <span data-ttu-id="4a611-2712">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="4a611-2712">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="4a611-2713">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="4a611-2713">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="4a611-2714">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="4a611-2714">Improved repository commands error messages</span></span>
* <span data-ttu-id="4a611-2715">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="4a611-2715">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-2716">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-2716">ACS</span></span>

* <span data-ttu-id="4a611-2717">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="4a611-2717">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="4a611-2718">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="4a611-2718">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="4a611-2719">AMS</span><span class="sxs-lookup"><span data-stu-id="4a611-2719">AMS</span></span>

* <span data-ttu-id="4a611-2720">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="4a611-2720">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-2721">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-2721">Appservice</span></span>

* <span data-ttu-id="4a611-2722">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="4a611-2722">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="4a611-2723">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2723">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="4a611-2724">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="4a611-2724">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="4a611-2725">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4a611-2725">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="4a611-2726">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4a611-2726">Batch AI</span></span>

* <span data-ttu-id="4a611-2727">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="4a611-2727">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4a611-2728">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4a611-2728">Cognitive Services</span></span>

* <span data-ttu-id="4a611-2729">Исправлена опечатка в примере для `cognitiveservices account create` ([№ 5603](https://github.com/Azure/azure-cli/issues/5603)).</span><span class="sxs-lookup"><span data-stu-id="4a611-2729">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="4a611-2730">Потребление</span><span class="sxs-lookup"><span data-stu-id="4a611-2730">Consumption</span></span>

* <span data-ttu-id="4a611-2731">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="4a611-2731">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="4a611-2732">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-2732">Container</span></span>

* <span data-ttu-id="4a611-2733">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="4a611-2733">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="4a611-2734">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-2734">Cosmos DB</span></span>

* <span data-ttu-id="4a611-2735">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-2735">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="4a611-2736">DMS</span><span class="sxs-lookup"><span data-stu-id="4a611-2736">DMS</span></span>

* <span data-ttu-id="4a611-2737">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="4a611-2737">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="4a611-2738">Расширение</span><span class="sxs-lookup"><span data-stu-id="4a611-2738">Extension</span></span>

* <span data-ttu-id="4a611-2739">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="4a611-2739">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="4a611-2740">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="4a611-2740">Interactive</span></span>

* <span data-ttu-id="4a611-2741">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="4a611-2741">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="4a611-2742">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="4a611-2742">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="4a611-2743">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="4a611-2743">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="4a611-2744">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="4a611-2744">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="4a611-2745">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="4a611-2745">Lab</span></span>

* <span data-ttu-id="4a611-2746">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="4a611-2746">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="4a611-2747">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-2747">Network</span></span>

* <span data-ttu-id="4a611-2748">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="4a611-2748">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="4a611-2749">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-2749">Profile</span></span>

* <span data-ttu-id="4a611-2750">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2750">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="4a611-2751">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="4a611-2751">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="4a611-2752">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2752">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="4a611-2753">Redis</span><span class="sxs-lookup"><span data-stu-id="4a611-2753">Redis</span></span>

* <span data-ttu-id="4a611-2754">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2754">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="4a611-2755">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="4a611-2755">Deprecated `redis list-all`.</span></span> <span data-ttu-id="4a611-2756">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2756">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="4a611-2757">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2757">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="4a611-2758">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="4a611-2758">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="4a611-2759">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-2759">Role</span></span>

* <span data-ttu-id="4a611-2760">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="4a611-2760">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-2761">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-2761">Storage</span></span>

* <span data-ttu-id="4a611-2762">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="4a611-2762">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="4a611-2763">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="4a611-2763">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="4a611-2764">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="4a611-2764">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="4a611-2765">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="4a611-2765">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="4a611-2766">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="4a611-2766">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2767">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2767">VM</span></span>

* <span data-ttu-id="4a611-2768">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="4a611-2768">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="4a611-2769">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="4a611-2769">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="4a611-2770">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="4a611-2770">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="4a611-2771">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2771">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="4a611-2772">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="4a611-2772">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="4a611-2773">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="4a611-2773">Added write accelerator support</span></span>
* <span data-ttu-id="4a611-2774">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2774">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="4a611-2775">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="4a611-2775">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="4a611-2776">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="4a611-2776">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="4a611-2777">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2777">April 10, 2018</span></span>

<span data-ttu-id="4a611-2778">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="4a611-2778">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-2779">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-2779">ACR</span></span>

* <span data-ttu-id="4a611-2780">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="4a611-2780">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-2781">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-2781">ACS</span></span>

* <span data-ttu-id="4a611-2782">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="4a611-2782">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-2783">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-2783">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="4a611-2785">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="4a611-2785">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="4a611-2786">Batch AI</span><span class="sxs-lookup"><span data-stu-id="4a611-2786">BatchAI</span></span>

* <span data-ttu-id="4a611-2787">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="4a611-2787">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="4a611-2788">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="4a611-2788">Job level mounting</span></span>
  - <span data-ttu-id="4a611-2789">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2789">Environment variables with secret values</span></span>
  - <span data-ttu-id="4a611-2790">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="4a611-2790">Performance counters settings</span></span>
  - <span data-ttu-id="4a611-2791">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="4a611-2791">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="4a611-2792">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2792">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="4a611-2793">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="4a611-2793">Usage and limits reporting</span></span>
  - <span data-ttu-id="4a611-2794">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2794">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="4a611-2795">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2795">Support for custom images</span></span>
  - <span data-ttu-id="4a611-2796">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="4a611-2796">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="4a611-2797">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="4a611-2797">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="4a611-2798">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2798">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="4a611-2799">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="4a611-2799">National clouds are supported</span></span>
* <span data-ttu-id="4a611-2800">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="4a611-2800">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="4a611-2801">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="4a611-2801">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="4a611-2802">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="4a611-2802">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="4a611-2803">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="4a611-2803">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="4a611-2804">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="4a611-2804">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="4a611-2805">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="4a611-2805">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="4a611-2806">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2806">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="4a611-2807">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="4a611-2807">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="4a611-2808">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="4a611-2808">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="4a611-2809">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2809">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="4a611-2810">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="4a611-2810">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="4a611-2811">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2811">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="4a611-2812">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2812">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="4a611-2813">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="4a611-2813">Billing</span></span>

* <span data-ttu-id="4a611-2814">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="4a611-2814">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="4a611-2815">Потребление</span><span class="sxs-lookup"><span data-stu-id="4a611-2815">Consumption</span></span>

* <span data-ttu-id="4a611-2816">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2816">Added `marketplace` commands</span></span>
* <span data-ttu-id="4a611-2817">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2817">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="4a611-2818">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2818">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="4a611-2819">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2819">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="4a611-2820">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2820">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="4a611-2821">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2821">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="4a611-2822">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-2822">Container</span></span>

* <span data-ttu-id="4a611-2823">Добавлены параметры подключения тома репозитория Git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2823">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="4a611-2824">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="4a611-2824">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="4a611-2825">Расширение</span><span class="sxs-lookup"><span data-stu-id="4a611-2825">Extension</span></span>

* <span data-ttu-id="4a611-2826">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="4a611-2826">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="4a611-2827">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="4a611-2827">Interactive</span></span>

* <span data-ttu-id="4a611-2828">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="4a611-2828">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="4a611-2829">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="4a611-2829">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="4a611-2830">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2830">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="4a611-2831">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-2831">Network</span></span>

* <span data-ttu-id="4a611-2832">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2832">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="4a611-2833">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2833">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="4a611-2834">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="4a611-2834">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="4a611-2835">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="4a611-2835">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="4a611-2836">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="4a611-2836">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="4a611-2837">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2837">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="4a611-2838">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2838">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="4a611-2839">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="4a611-2839">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-2840">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-2840">Profile</span></span>

* <span data-ttu-id="4a611-2841">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2841">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="4a611-2842">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi` & `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2842">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="4a611-2843">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4a611-2843">RDBMS</span></span>

* <span data-ttu-id="4a611-2844">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2844">Added `georestore` command</span></span>
* <span data-ttu-id="4a611-2845">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="4a611-2845">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-2846">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-2846">Resource</span></span>

* <span data-ttu-id="4a611-2847">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2847">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="4a611-2848">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2848">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-2849">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-2849">SQL</span></span>

* <span data-ttu-id="4a611-2850">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2850">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-2851">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-2851">Storage</span></span>

* <span data-ttu-id="4a611-2852">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="4a611-2852">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2853">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2853">VM</span></span>

* <span data-ttu-id="4a611-2854">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="4a611-2854">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="4a611-2855">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="4a611-2855">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="4a611-2857">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2857">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="4a611-2858">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="4a611-2858">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="4a611-2859">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="4a611-2859">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="4a611-2860">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="4a611-2860">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="4a611-2861">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2861">March 27, 2018</span></span>

<span data-ttu-id="4a611-2862">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="4a611-2862">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="4a611-2863">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-2863">Core</span></span>

* <span data-ttu-id="4a611-2864">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="4a611-2864">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-2865">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-2865">ACS</span></span>

* <span data-ttu-id="4a611-2866">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="4a611-2866">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-2867">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-2867">Appservice</span></span>

* <span data-ttu-id="4a611-2868">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2868">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="4a611-2869">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2869">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="4a611-2870">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="4a611-2870">Backup</span></span>

* <span data-ttu-id="4a611-2871">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2871">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="4a611-2872">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="4a611-2872">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="4a611-2873">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="4a611-2873">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="4a611-2874">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2874">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="4a611-2875">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-2875">Container</span></span>

* <span data-ttu-id="4a611-2876">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2876">Added `container exec` command.</span></span> <span data-ttu-id="4a611-2877">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4a611-2877">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="4a611-2878">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4a611-2878">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="4a611-2879">Расширение</span><span class="sxs-lookup"><span data-stu-id="4a611-2879">Extension</span></span>

* <span data-ttu-id="4a611-2880">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="4a611-2880">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="4a611-2881">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2881">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="4a611-2882">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-2882">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="4a611-2883">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="4a611-2883">Interactive</span></span>

* <span data-ttu-id="4a611-2884">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="4a611-2884">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="4a611-2885">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2885">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="4a611-2886">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="4a611-2886">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="4a611-2887">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="4a611-2887">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="4a611-2888">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="4a611-2888">Lab</span></span>

* <span data-ttu-id="4a611-2889">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2889">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-2890">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-2890">Monitor</span></span>

* <span data-ttu-id="4a611-2891">Добавлена поддержка аргументов `--top`, `--orderby` и `--namespace` для `metrics list` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="4a611-2891">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="4a611-2892">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="4a611-2892">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="4a611-2893">Добавлена поддержка `--namespace` для `metrics list-definitions` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="4a611-2893">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="4a611-2894">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-2894">Network</span></span>

* <span data-ttu-id="4a611-2895">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="4a611-2895">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-2896">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-2896">Profile</span></span>

* <span data-ttu-id="4a611-2897">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2897">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="4a611-2898">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4a611-2898">RDBMS</span></span>

* <span data-ttu-id="4a611-2899">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="4a611-2899">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-2900">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-2900">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="4a611-2902">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-2902">Role</span></span>

* <span data-ttu-id="4a611-2903">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2903">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="4a611-2904">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="4a611-2904">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="4a611-2905">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="4a611-2905">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="4a611-2906">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2906">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="4a611-2907">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2907">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-2908">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-2908">Storage</span></span>

* <span data-ttu-id="4a611-2909">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="4a611-2909">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="4a611-2910">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="4a611-2910">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2911">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2911">VM</span></span>

* <span data-ttu-id="4a611-2912">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="4a611-2912">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="4a611-2913">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2913">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="4a611-2914">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="4a611-2914">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="4a611-2915">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="4a611-2915">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="4a611-2916">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-2916">March 13, 2018</span></span>

<span data-ttu-id="4a611-2917">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="4a611-2917">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-2918">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-2918">ACR</span></span>

* <span data-ttu-id="4a611-2919">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2919">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="4a611-2920">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="4a611-2920">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="4a611-2921">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="4a611-2921">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-2922">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-2922">ACS</span></span>

* <span data-ttu-id="4a611-2923">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="4a611-2923">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="4a611-2924">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="4a611-2924">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="4a611-2925">Помощник</span><span class="sxs-lookup"><span data-stu-id="4a611-2925">Advisor</span></span>

* <span data-ttu-id="4a611-2926">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2926">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="4a611-2927">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2927">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="4a611-2928">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2928">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="4a611-2929">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2929">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="4a611-2930">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2930">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-2931">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-2931">Appservice</span></span>

* <span data-ttu-id="4a611-2932">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="4a611-2932">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="4a611-2933">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2933">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="4a611-2934">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="4a611-2934">Eventhubs</span></span>

* <span data-ttu-id="4a611-2935">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="4a611-2935">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="4a611-2936">Расширение</span><span class="sxs-lookup"><span data-stu-id="4a611-2936">Extension</span></span>

* <span data-ttu-id="4a611-2937">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="4a611-2937">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="4a611-2938">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="4a611-2938">Interactive</span></span>

* <span data-ttu-id="4a611-2939">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="4a611-2939">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="4a611-2940">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="4a611-2940">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="4a611-2941">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="4a611-2941">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="4a611-2942">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="4a611-2942">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-2943">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-2943">Monitor</span></span>

* <span data-ttu-id="4a611-2944">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="4a611-2944">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="4a611-2945">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2945">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="4a611-2946">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2946">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="4a611-2947">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2947">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="4a611-2948">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-2948">Network</span></span>

* <span data-ttu-id="4a611-2949">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2949">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="4a611-2950">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="4a611-2950">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="4a611-2951">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2951">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="4a611-2952">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2952">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-2953">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-2953">Profile</span></span>

* <span data-ttu-id="4a611-2954">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="4a611-2954">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="4a611-2955">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2955">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="4a611-2956">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4a611-2956">RDBMS</span></span>

* <span data-ttu-id="4a611-2957">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="4a611-2957">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="4a611-2958">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="4a611-2958">Service Bus</span></span>

* <span data-ttu-id="4a611-2959">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="4a611-2959">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-2960">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-2960">Storage</span></span>

* <span data-ttu-id="4a611-2961">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="4a611-2961">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="4a611-2962">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="4a611-2962">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2963">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2963">VM</span></span>

* <span data-ttu-id="4a611-2964">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="4a611-2964">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="4a611-2965">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="4a611-2965">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="4a611-2966">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2966">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="4a611-2967">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="4a611-2967">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="4a611-2968">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="4a611-2968">February 27, 2018</span></span>

<span data-ttu-id="4a611-2969">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="4a611-2969">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="4a611-2970">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-2970">Core</span></span>

* <span data-ttu-id="4a611-2971">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="4a611-2971">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="4a611-2972">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="4a611-2972">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="4a611-2973">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2973">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-2974">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-2974">ACS</span></span>

* <span data-ttu-id="4a611-2975">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-2975">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="4a611-2976">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="4a611-2976">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="4a611-2977">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2977">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="4a611-2978">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2978">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-2979">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-2979">Appservice</span></span>

* <span data-ttu-id="4a611-2980">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="4a611-2980">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="4a611-2981">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="4a611-2981">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="4a611-2982">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="4a611-2982">Cognitive Services</span></span>

* <span data-ttu-id="4a611-2983">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="4a611-2983">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="4a611-2984">Потребление</span><span class="sxs-lookup"><span data-stu-id="4a611-2984">Consumption</span></span>

* <span data-ttu-id="4a611-2985">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="4a611-2985">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="4a611-2986">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="4a611-2986">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="4a611-2987">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-2987">Container</span></span>

* <span data-ttu-id="4a611-2988">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="4a611-2988">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="4a611-2989">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-2989">Network</span></span>

* <span data-ttu-id="4a611-2990">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2990">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-2991">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-2991">Resource</span></span>

* <span data-ttu-id="4a611-2992">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="4a611-2992">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="4a611-2993">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-2993">Role</span></span>

* <span data-ttu-id="4a611-2994">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="4a611-2994">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-2995">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-2995">SQL</span></span>

* <span data-ttu-id="4a611-2996">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="4a611-2996">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-2997">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-2997">Storage</span></span>

* <span data-ttu-id="4a611-2998">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-2998">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-2999">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-2999">VM</span></span>

* <span data-ttu-id="4a611-3000">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="4a611-3000">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="4a611-3001">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-3001">February 13, 2018</span></span>

<span data-ttu-id="4a611-3002">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="4a611-3002">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="4a611-3003">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-3003">Core</span></span>

* <span data-ttu-id="4a611-3004">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="4a611-3004">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-3005">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-3005">ACS</span></span>

* <span data-ttu-id="4a611-3006">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="4a611-3006">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="4a611-3007">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3007">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="4a611-3008">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="4a611-3008">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="4a611-3009">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="4a611-3009">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="4a611-3010">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="4a611-3010">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="4a611-3011">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3011">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="4a611-3012">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="4a611-3012">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="4a611-3013">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3013">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-3014">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-3014">Appservice</span></span>

* <span data-ttu-id="4a611-3015">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="4a611-3015">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="4a611-3016">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3016">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="4a611-3017">CDN</span><span class="sxs-lookup"><span data-stu-id="4a611-3017">CDN</span></span>

* <span data-ttu-id="4a611-3018">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3018">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="4a611-3019">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-3019">Container</span></span>

* <span data-ttu-id="4a611-3020">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="4a611-3020">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="4a611-3021">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4a611-3021">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4a611-3022">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-3022">CosmosDB</span></span>

* <span data-ttu-id="4a611-3023">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="4a611-3023">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="4a611-3024">Расширение</span><span class="sxs-lookup"><span data-stu-id="4a611-3024">Extension</span></span>

* <span data-ttu-id="4a611-3025">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3025">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="4a611-3026">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3026">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="4a611-3027">Отзывы</span><span class="sxs-lookup"><span data-stu-id="4a611-3027">Feedback</span></span>

* <span data-ttu-id="4a611-3028">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="4a611-3028">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="4a611-3029">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="4a611-3029">Interactive</span></span>

* <span data-ttu-id="4a611-3030">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="4a611-3030">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="4a611-3031">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="4a611-3031">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-3032">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-3032">IoT</span></span>

* <span data-ttu-id="4a611-3033">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="4a611-3033">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="4a611-3034">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="4a611-3034">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="4a611-3035">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3035">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="4a611-3036">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="4a611-3036">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-3037">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-3037">Monitor</span></span>

* <span data-ttu-id="4a611-3038">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3038">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="4a611-3039">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-3039">Network</span></span>

* <span data-ttu-id="4a611-3040">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="4a611-3040">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="4a611-3041">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-3041">Profile</span></span>

* <span data-ttu-id="4a611-3042">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="4a611-3042">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-3043">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-3043">Resource</span></span>

* <span data-ttu-id="4a611-3044">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3044">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="4a611-3045">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-3045">Role</span></span>

* <span data-ttu-id="4a611-3046">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="4a611-3046">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-3047">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-3047">SQL</span></span>

* <span data-ttu-id="4a611-3048">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3048">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="4a611-3049">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3049">Added `sql db rename`</span></span>
* <span data-ttu-id="4a611-3050">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="4a611-3050">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-3051">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-3051">Storage</span></span>

* <span data-ttu-id="4a611-3052">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="4a611-3052">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-3053">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-3053">VM</span></span>

* <span data-ttu-id="4a611-3054">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="4a611-3054">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="4a611-3055">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="4a611-3055">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="4a611-3056">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="4a611-3056">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="4a611-3057">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-3057">January 31, 2018</span></span>

<span data-ttu-id="4a611-3058">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="4a611-3058">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="4a611-3059">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-3059">Core</span></span>

* <span data-ttu-id="4a611-3060">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="4a611-3060">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="4a611-3061">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="4a611-3061">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="4a611-3062">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="4a611-3062">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="4a611-3063">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="4a611-3063">Use `--verbose` to see</span></span>
* <span data-ttu-id="4a611-3064">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="4a611-3064">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-3065">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-3065">ACS</span></span>

* <span data-ttu-id="4a611-3066">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3066">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="4a611-3067">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3067">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-3068">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-3068">Appservice</span></span>

* <span data-ttu-id="4a611-3069">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="4a611-3069">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="4a611-3070">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="4a611-3070">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="4a611-3071">CDN</span><span class="sxs-lookup"><span data-stu-id="4a611-3071">CDN</span></span>

* <span data-ttu-id="4a611-3072">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3072">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4a611-3073">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-3073">CosmosDB</span></span>

* <span data-ttu-id="4a611-3074">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="4a611-3074">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="4a611-3075">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="4a611-3075">Interactive</span></span>

* <span data-ttu-id="4a611-3076">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="4a611-3076">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="4a611-3077">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-3077">Network</span></span>

* <span data-ttu-id="4a611-3078">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3078">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="4a611-3079">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-3079">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="4a611-3080">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3080">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="4a611-3081">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3081">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="4a611-3082">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3082">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="4a611-3083">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="4a611-3083">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="4a611-3084">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="4a611-3084">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="4a611-3085">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="4a611-3085">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="4a611-3086">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3086">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="4a611-3087">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3087">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-3088">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-3088">Profile</span></span>

* <span data-ttu-id="4a611-3089">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="4a611-3089">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-3090">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-3090">Resource</span></span>

* <span data-ttu-id="4a611-3091">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="4a611-3091">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-3092">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-3092">Storage</span></span>

* <span data-ttu-id="4a611-3093">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="4a611-3093">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="4a611-3094">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="4a611-3094">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="4a611-3095">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3095">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="4a611-3096">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3096">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="4a611-3097">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="4a611-3097">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-3098">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-3098">VM</span></span>

* <span data-ttu-id="4a611-3099">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="4a611-3099">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="4a611-3100">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4a611-3100">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="4a611-3101">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="4a611-3101">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="4a611-3102">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3102">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="4a611-3103">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-3103">January 17, 2018</span></span>

<span data-ttu-id="4a611-3104">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="4a611-3104">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-3105">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-3105">ACR</span></span>

* <span data-ttu-id="4a611-3106">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="4a611-3106">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="4a611-3107">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="4a611-3107">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-3108">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-3108">ACS</span></span>

* <span data-ttu-id="4a611-3109">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3109">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="4a611-3110">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="4a611-3110">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-3111">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-3111">Appservice</span></span>

* <span data-ttu-id="4a611-3112">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="4a611-3112">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="4a611-3113">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="4a611-3113">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="4a611-3114">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3114">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="4a611-3115">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="4a611-3115">Backup</span></span>

* <span data-ttu-id="4a611-3116">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="4a611-3116">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="4a611-3117">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="4a611-3117">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="4a611-3118">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="4a611-3118">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="4a611-3119">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="4a611-3119">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="4a611-3120">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="4a611-3120">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="4a611-3121">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-3121">Batch</span></span>

* <span data-ttu-id="4a611-3122">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="4a611-3122">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="4a611-3123">Cloud</span><span class="sxs-lookup"><span data-stu-id="4a611-3123">Cloud</span></span>

* <span data-ttu-id="4a611-3124">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="4a611-3124">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="4a611-3125">Потребление</span><span class="sxs-lookup"><span data-stu-id="4a611-3125">Consumption</span></span>

* <span data-ttu-id="4a611-3126">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3126">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="4a611-3127">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-3127">Event Grid</span></span>

* <span data-ttu-id="4a611-3128">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3128">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="4a611-3129">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3129">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="4a611-3130">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3130">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="4a611-3131">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3131">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="4a611-3132">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3132">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="4a611-3133">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3133">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="4a611-3134">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3134">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="4a611-3135">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="4a611-3135">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="4a611-3136">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="4a611-3136">Interactive</span></span>

* <span data-ttu-id="4a611-3137">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="4a611-3137">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="4a611-3138">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="4a611-3138">Fixed errors on startup</span></span>
* <span data-ttu-id="4a611-3139">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="4a611-3139">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-3140">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-3140">IoT</span></span>

* <span data-ttu-id="4a611-3141">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="4a611-3141">Added support for device provisioning service</span></span>
* <span data-ttu-id="4a611-3142">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="4a611-3142">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="4a611-3143">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="4a611-3143">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-3144">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-3144">Monitor</span></span>

* <span data-ttu-id="4a611-3145">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="4a611-3145">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="4a611-3146">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3146">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="4a611-3147">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="4a611-3147">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="4a611-3148">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-3148">Network</span></span>

* <span data-ttu-id="4a611-3149">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="4a611-3149">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="4a611-3150">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="4a611-3150">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-3151">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-3151">Profile</span></span>

* <span data-ttu-id="4a611-3152">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4a611-3152">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="4a611-3153">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-3153">Role</span></span>

* <span data-ttu-id="4a611-3154">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="4a611-3154">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4a611-3155">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4a611-3155">Service Fabric</span></span>

* <span data-ttu-id="4a611-3156">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="4a611-3156">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="4a611-3157">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="4a611-3157">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-3158">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-3158">VM</span></span>

* <span data-ttu-id="4a611-3159">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3159">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="4a611-3160">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="4a611-3160">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="4a611-3161">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3161">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="4a611-3162">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="4a611-3162">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="4a611-3163">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="4a611-3163">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="4a611-3164">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3164">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="4a611-3165">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3165">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="4a611-3166">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3166">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="4a611-3167">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-3167">December 19, 2017</span></span>

<span data-ttu-id="4a611-3168">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="4a611-3168">Version 2.0.23</span></span>

* <span data-ttu-id="4a611-3169">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4a611-3169">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="4a611-3170">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-3170">Container</span></span>

* <span data-ttu-id="4a611-3171">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4a611-3171">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="4a611-3172">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-3172">Network</span></span>

* <span data-ttu-id="4a611-3173">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4a611-3173">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="4a611-3174">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4a611-3174">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-3175">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-3175">Storage</span></span>

* <span data-ttu-id="4a611-3176">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="4a611-3176">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-3177">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-3177">VM</span></span>

* <span data-ttu-id="4a611-3178">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="4a611-3178">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="4a611-3179">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-3179">December 5, 2017</span></span>

<span data-ttu-id="4a611-3180">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="4a611-3180">Version 2.0.22</span></span>

* <span data-ttu-id="4a611-3181">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3181">Removed `az component` commands.</span></span> <span data-ttu-id="4a611-3182">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3182">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="4a611-3183">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-3183">Core</span></span>
* <span data-ttu-id="4a611-3184">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="4a611-3184">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="4a611-3185">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="4a611-3185">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-3186">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-3186">ACS</span></span>

* <span data-ttu-id="4a611-3187">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3187">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="4a611-3188">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3188">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="4a611-3189">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="4a611-3189">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="4a611-3190">Помощник</span><span class="sxs-lookup"><span data-stu-id="4a611-3190">Advisor</span></span>

* <span data-ttu-id="4a611-3191">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="4a611-3191">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-3192">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-3192">Appservice</span></span>

* <span data-ttu-id="4a611-3193">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3193">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="4a611-3194">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="4a611-3194">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="4a611-3195">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3195">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="4a611-3196">Потребление</span><span class="sxs-lookup"><span data-stu-id="4a611-3196">Consumption</span></span>

* <span data-ttu-id="4a611-3197">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="4a611-3197">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="4a611-3198">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-3198">Container</span></span>

* <span data-ttu-id="4a611-3199">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="4a611-3199">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-3200">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-3200">Monitor</span></span>

* <span data-ttu-id="4a611-3201">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="4a611-3201">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-3202">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-3202">Resource</span></span>

* <span data-ttu-id="4a611-3203">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="4a611-3203">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="4a611-3204">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-3204">Role</span></span>

* <span data-ttu-id="4a611-3205">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3205">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="4a611-3206">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="4a611-3206">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="4a611-3207">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3207">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-3208">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-3208">SQL</span></span>

* <span data-ttu-id="4a611-3209">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3209">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="4a611-3210">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3210">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-3211">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-3211">VM</span></span>

* <span data-ttu-id="4a611-3212">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3212">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="4a611-3213">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-3213">November 14, 2017</span></span>

<span data-ttu-id="4a611-3214">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="4a611-3214">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-3215">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-3215">ACR</span></span>

* <span data-ttu-id="4a611-3216">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="4a611-3216">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="4a611-3217">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-3217">ACS</span></span>

* <span data-ttu-id="4a611-3218">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="4a611-3218">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="4a611-3219">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="4a611-3219">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="4a611-3220">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3220">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="4a611-3221">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="4a611-3221">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="4a611-3222">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="4a611-3222">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-3223">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-3223">Appservice</span></span>

* <span data-ttu-id="4a611-3224">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="4a611-3224">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="4a611-3225">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3225">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="4a611-3226">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3226">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="4a611-3227">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3227">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="4a611-3228">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="4a611-3228">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="4a611-3229">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="4a611-3229">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="4a611-3230">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-3230">Batch</span></span>

* <span data-ttu-id="4a611-3231">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3231">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="4a611-3232">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="4a611-3232">Batchai</span></span>

* <span data-ttu-id="4a611-3233">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3233">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="4a611-3234">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3234">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="4a611-3235">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3235">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="4a611-3236">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3236">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="4a611-3237">Cloud</span><span class="sxs-lookup"><span data-stu-id="4a611-3237">Cloud</span></span>

* <span data-ttu-id="4a611-3238">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="4a611-3238">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="4a611-3239">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-3239">Container</span></span>

* <span data-ttu-id="4a611-3240">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="4a611-3240">Added support to open multiple ports</span></span>
* <span data-ttu-id="4a611-3241">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4a611-3241">Added container group restart policy</span></span>
* <span data-ttu-id="4a611-3242">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="4a611-3242">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="4a611-3243">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="4a611-3243">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4a611-3244">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4a611-3244">Data Lake Analytics</span></span>

* <span data-ttu-id="4a611-3245">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="4a611-3245">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4a611-3246">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="4a611-3246">Data Lake Store</span></span>

* <span data-ttu-id="4a611-3247">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="4a611-3247">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="4a611-3248">Расширение</span><span class="sxs-lookup"><span data-stu-id="4a611-3248">Extension</span></span>

* <span data-ttu-id="4a611-3249">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="4a611-3249">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="4a611-3250">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="4a611-3250">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-3251">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-3251">IoT</span></span>

* <span data-ttu-id="4a611-3252">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4a611-3252">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-3253">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-3253">Monitor</span></span>

* <span data-ttu-id="4a611-3254">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3254">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="4a611-3255">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-3255">Network</span></span>

* <span data-ttu-id="4a611-3256">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="4a611-3256">Added support for CAA DNS records</span></span>
* <span data-ttu-id="4a611-3257">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3257">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="4a611-3258">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="4a611-3258">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="4a611-3259">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3259">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="4a611-3260">Резервирование</span><span class="sxs-lookup"><span data-stu-id="4a611-3260">Reservations</span></span>

* <span data-ttu-id="4a611-3261">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="4a611-3261">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-3262">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-3262">Resource</span></span>

* <span data-ttu-id="4a611-3263">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3263">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-3264">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-3264">SQL</span></span>

* <span data-ttu-id="4a611-3265">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3265">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-3266">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-3266">Storage</span></span>

* <span data-ttu-id="4a611-3267">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-3267">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="4a611-3268">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="4a611-3268">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="4a611-3269">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3269">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="4a611-3270">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3270">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="4a611-3271">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3271">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="4a611-3272">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3272">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="4a611-3273">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3273">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-3274">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-3274">VM</span></span>

* <span data-ttu-id="4a611-3275">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3275">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="4a611-3276">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="4a611-3276">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="4a611-3277">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3277">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="4a611-3278">Переименование `vm format-secret` в `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="4a611-3278">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="4a611-3279">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="4a611-3279">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="4a611-3280">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-3280">October 24, 2017</span></span>

<span data-ttu-id="4a611-3281">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="4a611-3281">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="4a611-3282">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-3282">Core</span></span>

* <span data-ttu-id="4a611-3283">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="4a611-3283">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-3284">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-3284">ACR</span></span>

* <span data-ttu-id="4a611-3285">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="4a611-3285">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="4a611-3286">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="4a611-3286">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="4a611-3287">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="4a611-3287">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-3288">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-3288">ACS</span></span>

* <span data-ttu-id="4a611-3289">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="4a611-3289">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="4a611-3290">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="4a611-3290">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-3291">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-3291">Appservice</span></span>

* <span data-ttu-id="4a611-3292">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="4a611-3292">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="4a611-3293">Компонент</span><span class="sxs-lookup"><span data-stu-id="4a611-3293">Component</span></span>

* <span data-ttu-id="4a611-3294">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="4a611-3294">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-3295">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-3295">Monitor</span></span>

* <span data-ttu-id="4a611-3296">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3296">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-3297">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-3297">Resource</span></span>

* <span data-ttu-id="4a611-3298">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="4a611-3298">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="4a611-3299">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="4a611-3299">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-3300">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-3300">VM</span></span>

* <span data-ttu-id="4a611-3301">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="4a611-3301">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="4a611-3302">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-3302">October 9, 2017</span></span>

<span data-ttu-id="4a611-3303">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="4a611-3303">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="4a611-3304">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-3304">Core</span></span>

* <span data-ttu-id="4a611-3305">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="4a611-3305">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-3306">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-3306">Appservice</span></span>

* <span data-ttu-id="4a611-3307">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3307">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="4a611-3308">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-3308">Batch</span></span>

* <span data-ttu-id="4a611-3309">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="4a611-3309">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="4a611-3310">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="4a611-3310">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="4a611-3311">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="4a611-3311">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="4a611-3312">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="4a611-3312">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="4a611-3313">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="4a611-3313">Batchai</span></span>

* <span data-ttu-id="4a611-3314">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="4a611-3314">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="4a611-3315">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4a611-3315">Keyvault</span></span>

* <span data-ttu-id="4a611-3316">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="4a611-3316">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="4a611-3317">(#4448)</span><span class="sxs-lookup"><span data-stu-id="4a611-3317">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="4a611-3318">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-3318">Network</span></span>

* <span data-ttu-id="4a611-3319">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="4a611-3319">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="4a611-3320">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="4a611-3320">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-3321">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-3321">Resource</span></span>

* <span data-ttu-id="4a611-3322">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3322">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="4a611-3323">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="4a611-3323">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="4a611-3324">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="4a611-3324">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="4a611-3325">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="4a611-3325">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-3326">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-3326">Sql</span></span>

* <span data-ttu-id="4a611-3327">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="4a611-3327">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="4a611-3328">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="4a611-3328">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="4a611-3329">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="4a611-3329">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-3330">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-3330">Storage</span></span>

* <span data-ttu-id="4a611-3331">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a611-3331">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-3332">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="4a611-3332">Vm</span></span>

* <span data-ttu-id="4a611-3333">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="4a611-3333">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="4a611-3334">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3334">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="4a611-3335">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3335">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="4a611-3336">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3336">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="4a611-3337">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="4a611-3337">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="4a611-3338">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-3338">September 22, 2017</span></span>

<span data-ttu-id="4a611-3339">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="4a611-3339">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-3340">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-3340">Resource</span></span>

* <span data-ttu-id="4a611-3341">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="4a611-3341">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="4a611-3342">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="4a611-3342">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="4a611-3343">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="4a611-3343">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="4a611-3344">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3344">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="4a611-3345">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-3345">Network</span></span>

* <span data-ttu-id="4a611-3346">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="4a611-3346">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="4a611-3347">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="4a611-3347">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="4a611-3348">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="4a611-3348">Added `asg` application security group commands</span></span>
* <span data-ttu-id="4a611-3349">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="4a611-3349">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="4a611-3350">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4a611-3350">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="4a611-3351">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4a611-3351">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="4a611-3352">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3352">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-3353">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-3353">Storage</span></span>

* <span data-ttu-id="4a611-3354">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="4a611-3354">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="4a611-3355">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="4a611-3355">Eventgrid</span></span>

* <span data-ttu-id="4a611-3356">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="4a611-3356">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-3357">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-3357">SQL</span></span>

* <span data-ttu-id="4a611-3358">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="4a611-3358">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="4a611-3359">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="4a611-3359">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="4a611-3360">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4a611-3360">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="4a611-3361">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4a611-3361">Keyvault</span></span>

* <span data-ttu-id="4a611-3362">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="4a611-3362">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-3363">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-3363">VM</span></span>

* <span data-ttu-id="4a611-3364">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="4a611-3364">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="4a611-3365">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="4a611-3365">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="4a611-3366">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="4a611-3366">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="4a611-3367">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="4a611-3367">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="4a611-3368">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="4a611-3368">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="4a611-3369">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="4a611-3369">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-3370">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-3370">ACS</span></span>

* <span data-ttu-id="4a611-3371">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="4a611-3371">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-3372">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-3372">Appservice</span></span>

* <span data-ttu-id="4a611-3373">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="4a611-3373">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="4a611-3374">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="4a611-3374">Backup</span></span>

* <span data-ttu-id="4a611-3375">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="4a611-3375">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="4a611-3376">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-3376">September 11, 2017</span></span>

<span data-ttu-id="4a611-3377">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="4a611-3377">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="4a611-3378">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-3378">Core</span></span>

* <span data-ttu-id="4a611-3379">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="4a611-3379">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="4a611-3380">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="4a611-3380">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-3381">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-3381">Acs</span></span>

* <span data-ttu-id="4a611-3382">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3382">Added `acs list-locations` command</span></span>
* <span data-ttu-id="4a611-3383">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-3383">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-3384">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-3384">Appservice</span></span>

* <span data-ttu-id="4a611-3385">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="4a611-3385">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="4a611-3386">CDN</span><span class="sxs-lookup"><span data-stu-id="4a611-3386">CDN</span></span>

* <span data-ttu-id="4a611-3387">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3387">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="4a611-3388">Расширение</span><span class="sxs-lookup"><span data-stu-id="4a611-3388">Extension</span></span>

* <span data-ttu-id="4a611-3389">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="4a611-3389">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="4a611-3390">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4a611-3390">Keyvault</span></span>

* <span data-ttu-id="4a611-3391">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3391">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="4a611-3392">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-3392">Network</span></span>

* <span data-ttu-id="4a611-3393">Переименование `vnet list-private-access-services` в `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="4a611-3393">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4a611-3394">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3394">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="4a611-3395">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3395">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="4a611-3396">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3396">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4a611-3397">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3397">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-3398">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-3398">Resource</span></span>

* <span data-ttu-id="4a611-3399">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3399">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="4a611-3400">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3400">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="4a611-3401">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="4a611-3401">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="4a611-3402">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="4a611-3402">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-3403">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-3403">SQL</span></span>

* <span data-ttu-id="4a611-3404">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3404">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-3405">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-3405">VM</span></span>

* <span data-ttu-id="4a611-3406">Исправлено: Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="4a611-3406">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="4a611-3407">Исправлено: Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="4a611-3407">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="4a611-3408">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3408">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="4a611-3409">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="4a611-3409">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="4a611-3410">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="4a611-3410">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="4a611-3411">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-3411">August 31, 2017</span></span>

<span data-ttu-id="4a611-3412">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="4a611-3412">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="4a611-3413">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4a611-3413">Keyvault</span></span>

* <span data-ttu-id="4a611-3414">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3414">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="4a611-3415">Sf</span><span class="sxs-lookup"><span data-stu-id="4a611-3415">Sf</span></span>

* <span data-ttu-id="4a611-3416">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="4a611-3416">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-3417">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-3417">Storage</span></span>

* <span data-ttu-id="4a611-3418">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="4a611-3418">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="4a611-3419">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="4a611-3419">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="4a611-3420">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-3420">August 28, 2017</span></span>

<span data-ttu-id="4a611-3421">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="4a611-3421">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="4a611-3422">CLI</span><span class="sxs-lookup"><span data-stu-id="4a611-3422">CLI</span></span>

* <span data-ttu-id="4a611-3423">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="4a611-3423">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-3424">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-3424">ACS</span></span>

* <span data-ttu-id="4a611-3425">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="4a611-3425">Corrected preview regions</span></span>
* <span data-ttu-id="4a611-3426">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3426">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="4a611-3427">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="4a611-3427">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-3428">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-3428">Appservice</span></span>

* <span data-ttu-id="4a611-3429">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3429">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="4a611-3430">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3430">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="4a611-3431">Предоставлен параметр `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3431">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="4a611-3432">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="4a611-3432">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="4a611-3433">Исправлено: Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="4a611-3433">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-3434">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-3434">IoT</span></span>

* <span data-ttu-id="4a611-3435">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="4a611-3435">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="4a611-3436">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-3436">Network</span></span>

* <span data-ttu-id="4a611-3437">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3437">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4a611-3438">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3438">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="4a611-3439">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3439">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="4a611-3440">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3440">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4a611-3441">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3441">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-3442">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-3442">Profile</span></span>

* <span data-ttu-id="4a611-3443">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="4a611-3443">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4a611-3444">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4a611-3444">Service Fabric</span></span>

* <span data-ttu-id="4a611-3445">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="4a611-3445">Preview release</span></span>
* <span data-ttu-id="4a611-3446">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="4a611-3446">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="4a611-3447">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="4a611-3447">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="4a611-3448">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3448">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-3449">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-3449">Storage</span></span>

* <span data-ttu-id="4a611-3450">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="4a611-3450">Enabled setting blob tier</span></span>
* <span data-ttu-id="4a611-3451">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="4a611-3451">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="4a611-3452">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3452">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="4a611-3453">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="4a611-3453">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="4a611-3454">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3454">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="4a611-3455">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3455">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-3456">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-3456">VM</span></span>

* <span data-ttu-id="4a611-3457">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3457">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="4a611-3458">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3458">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="4a611-3459">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="4a611-3459">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="4a611-3460">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="4a611-3460">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="4a611-3461">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="4a611-3461">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="4a611-3462">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3462">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="4a611-3463">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-3463">August 15, 2017</span></span>

<span data-ttu-id="4a611-3464">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="4a611-3464">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-3465">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-3465">ACS</span></span>

* <span data-ttu-id="4a611-3466">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="4a611-3466">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-3467">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-3467">Appservice</span></span>

* <span data-ttu-id="4a611-3468">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="4a611-3468">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="4a611-3469">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-3469">Event Grid</span></span>

* <span data-ttu-id="4a611-3470">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="4a611-3470">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="4a611-3471">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-3471">August 11, 2017</span></span>

<span data-ttu-id="4a611-3472">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="4a611-3472">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-3473">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-3473">ACS</span></span>

* <span data-ttu-id="4a611-3474">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="4a611-3474">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="4a611-3475">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-3475">Batch</span></span>

* <span data-ttu-id="4a611-3476">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="4a611-3476">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="4a611-3477">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="4a611-3477">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="4a611-3478">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a611-3478">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="4a611-3479">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="4a611-3479">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="4a611-3480">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="4a611-3480">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="4a611-3481">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="4a611-3481">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="4a611-3482">Компонент</span><span class="sxs-lookup"><span data-stu-id="4a611-3482">Component</span></span>

* <span data-ttu-id="4a611-3483">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="4a611-3483">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="4a611-3484">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4a611-3484">Container</span></span>

* <span data-ttu-id="4a611-3485">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="4a611-3485">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="4a611-3486">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="4a611-3486">Data Lake Store</span></span>

* <span data-ttu-id="4a611-3487">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="4a611-3487">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="4a611-3488">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-3488">Event Grid</span></span>

* <span data-ttu-id="4a611-3489">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="4a611-3489">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="4a611-3490">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-3490">Network</span></span>

* <span data-ttu-id="4a611-3491">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="4a611-3491">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="4a611-3492">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3492">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="4a611-3493">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3493">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="4a611-3494">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3494">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-3495">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-3495">Profile</span></span>

* <span data-ttu-id="4a611-3496">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="4a611-3496">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-3497">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-3497">Storage</span></span>

* <span data-ttu-id="4a611-3498">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="4a611-3498">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-3499">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-3499">VM</span></span>

* <span data-ttu-id="4a611-3500">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="4a611-3500">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="4a611-3501">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3501">Exposed `list-skus` command</span></span>
* <span data-ttu-id="4a611-3502">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="4a611-3502">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="4a611-3503">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="4a611-3503">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="4a611-3504">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="4a611-3504">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="4a611-3505">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-3505">July 28, 2017</span></span>

<span data-ttu-id="4a611-3506">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="4a611-3506">Version 2.0.12</span></span>

* <span data-ttu-id="4a611-3507">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4a611-3507">Added container commands</span></span>
* <span data-ttu-id="4a611-3508">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4a611-3508">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="4a611-3509">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-3509">Core</span></span>

* <span data-ttu-id="4a611-3510">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4a611-3510">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="4a611-3511">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="4a611-3511">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="4a611-3512">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="4a611-3512">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="4a611-3513">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="4a611-3513">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="4a611-3514">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="4a611-3514">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="4a611-3515">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="4a611-3515">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="4a611-3516">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="4a611-3516">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4a611-3517">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="4a611-3517">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="4a611-3518">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="4a611-3518">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="4a611-3519">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="4a611-3519">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="4a611-3520">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="4a611-3520">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="4a611-3521">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="4a611-3521">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="4a611-3522">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="4a611-3522">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="4a611-3523">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="4a611-3523">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="4a611-3524">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="4a611-3524">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="4a611-3525">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="4a611-3525">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="4a611-3526">ACR</span><span class="sxs-lookup"><span data-stu-id="4a611-3526">ACR</span></span>

* <span data-ttu-id="4a611-3527">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="4a611-3527">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="4a611-3528">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="4a611-3528">Support SKU update for managed registries</span></span>
* <span data-ttu-id="4a611-3529">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="4a611-3529">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="4a611-3530">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="4a611-3530">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="4a611-3531">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="4a611-3531">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="4a611-3532">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="4a611-3532">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-3533">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-3533">ACS</span></span>

* <span data-ttu-id="4a611-3534">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="4a611-3534">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-3535">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4a611-3535">Appservice</span></span>

* <span data-ttu-id="4a611-3536">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="4a611-3536">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="4a611-3537">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="4a611-3537">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="4a611-3538">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3538">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="4a611-3539">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="4a611-3539">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="4a611-3540">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="4a611-3540">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="4a611-3541">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="4a611-3541">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="4a611-3542">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="4a611-3542">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="4a611-3543">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="4a611-3543">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="4a611-3544">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="4a611-3544">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="4a611-3545">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3545">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="4a611-3546">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="4a611-3546">Batch</span></span>

* <span data-ttu-id="4a611-3547">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="4a611-3547">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="4a611-3548">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3548">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="4a611-3549">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3549">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="4a611-3550">CDN</span><span class="sxs-lookup"><span data-stu-id="4a611-3550">CDN</span></span>

* <span data-ttu-id="4a611-3551">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="4a611-3551">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="4a611-3552">Cloud</span><span class="sxs-lookup"><span data-stu-id="4a611-3552">Cloud</span></span>

* <span data-ttu-id="4a611-3553">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="4a611-3553">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="4a611-3554">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="4a611-3554">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="4a611-3555">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="4a611-3555">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="4a611-3556">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="4a611-3556">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="4a611-3557">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3557">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4a611-3558">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-3558">CosmosDB</span></span>

* <span data-ttu-id="4a611-3559">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="4a611-3559">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="4a611-3560">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="4a611-3560">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4a611-3561">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4a611-3561">Data Lake Analytics</span></span>

* <span data-ttu-id="4a611-3562">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3562">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="4a611-3563">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3563">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="4a611-3564">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3564">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4a611-3565">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="4a611-3565">Data Lake Store</span></span>

* <span data-ttu-id="4a611-3566">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3566">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="4a611-3567">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="4a611-3567">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="4a611-3568">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3568">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="4a611-3569">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="4a611-3569">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="4a611-3570">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="4a611-3570">Interactive</span></span>

* <span data-ttu-id="4a611-3571">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="4a611-3571">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="4a611-3572">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="4a611-3572">Increased test coverage</span></span>
* <span data-ttu-id="4a611-3573">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="4a611-3573">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="4a611-3574">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="4a611-3574">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="4a611-3575">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="4a611-3575">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="4a611-3576">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="4a611-3576">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="4a611-3577">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="4a611-3577">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4a611-3578">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3578">Added `--progress` flag</span></span>
* <span data-ttu-id="4a611-3579">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3579">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="4a611-3580">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="4a611-3580">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="4a611-3581">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4a611-3581">IoT</span></span>

* <span data-ttu-id="4a611-3582">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="4a611-3582">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="4a611-3583">(3934).</span><span class="sxs-lookup"><span data-stu-id="4a611-3583">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="4a611-3584">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4a611-3584">Key vault</span></span>

* <span data-ttu-id="4a611-3585">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="4a611-3585">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="4a611-3586">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3586">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="4a611-3587">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="4a611-3587">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4a611-3588">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3588">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4a611-3589">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3589">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="4a611-3590">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="4a611-3590">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="4a611-3591">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="4a611-3591">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="4a611-3592">(3307).</span><span class="sxs-lookup"><span data-stu-id="4a611-3592">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="4a611-3593">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="4a611-3593">Lab</span></span>

* <span data-ttu-id="4a611-3594">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3594">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="4a611-3595">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3595">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-3596">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-3596">Monitor</span></span>

* <span data-ttu-id="4a611-3597">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="4a611-3597">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="4a611-3598">Переименование `monitor alert-rule-incidents list` в `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="4a611-3598">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="4a611-3599">Переименование `monitor alert-rule-incidents show` в `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="4a611-3599">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="4a611-3600">Переименование `monitor metric-defintions list` в `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="4a611-3600">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="4a611-3601">Переименование `monitor alert-rules` в `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="4a611-3601">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="4a611-3602">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="4a611-3602">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="4a611-3603">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="4a611-3603">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="4a611-3604">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="4a611-3604">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="4a611-3605">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="4a611-3605">`location` no longer required</span></span>
  * <span data-ttu-id="4a611-3606">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="4a611-3606">Add name and ID support for target</span></span>
  * <span data-ttu-id="4a611-3607">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="4a611-3607">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="4a611-3608">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="4a611-3608">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="4a611-3609">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="4a611-3609">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="4a611-3610">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="4a611-3610">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="4a611-3611">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3611">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="4a611-3612">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3612">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="4a611-3613">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-3613">Network</span></span>

* <span data-ttu-id="4a611-3614">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3614">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="4a611-3615">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3615">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="4a611-3616">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="4a611-3616">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="4a611-3617">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3617">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="4a611-3618">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3618">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="4a611-3619">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3619">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="4a611-3620">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3620">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="4a611-3621">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3621">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="4a611-3622">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3622">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="4a611-3623">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3623">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="4a611-3624">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3624">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="4a611-3625">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3625">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="4a611-3626">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3626">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="4a611-3627">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3627">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="4a611-3628">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3628">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="4a611-3629">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3629">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="4a611-3630">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="4a611-3630">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="4a611-3631">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3631">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="4a611-3632">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3632">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="4a611-3633">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3633">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="4a611-3634">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3634">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="4a611-3635">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3635">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="4a611-3636">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3636">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="4a611-3637">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="4a611-3637">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="4a611-3638">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="4a611-3638">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="4a611-3639">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="4a611-3639">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="4a611-3640">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="4a611-3640">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-3641">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-3641">Profile</span></span>

* <span data-ttu-id="4a611-3642">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4a611-3642">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="4a611-3643">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="4a611-3643">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="4a611-3644">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="4a611-3644">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="4a611-3645">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="4a611-3645">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="4a611-3646">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="4a611-3646">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="4a611-3647">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4a611-3647">RDBMS</span></span>

* <span data-ttu-id="4a611-3648">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="4a611-3648">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="4a611-3649">Исправлена проблема с обработкой `%s` из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="4a611-3649">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="4a611-3650">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="4a611-3650">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="4a611-3651">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="4a611-3651">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-3652">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-3652">Resource</span></span>

* <span data-ttu-id="4a611-3653">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3653">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="4a611-3654">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3654">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="4a611-3655">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3655">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="4a611-3656">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3656">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="4a611-3657">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="4a611-3657">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="4a611-3658">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3658">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="4a611-3659">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="4a611-3659">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="4a611-3660">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3660">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="4a611-3661">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-3661">Role</span></span>

* <span data-ttu-id="4a611-3662">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="4a611-3662">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="4a611-3663">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="4a611-3663">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="4a611-3664">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="4a611-3664">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="4a611-3665">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="4a611-3665">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="4a611-3666">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3666">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4a611-3667">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4a611-3667">Service Fabric</span></span>
* <span data-ttu-id="4a611-3668">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="4a611-3668">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="4a611-3669">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="4a611-3669">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="4a611-3670">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="4a611-3670">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-3671">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-3671">SQL</span></span>

* <span data-ttu-id="4a611-3672">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3672">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="4a611-3673">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3673">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="4a611-3674">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3674">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-3675">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-3675">Storage</span></span>

* <span data-ttu-id="4a611-3676">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="4a611-3676">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="4a611-3677">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="4a611-3677">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="4a611-3678">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="4a611-3678">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="4a611-3679">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="4a611-3679">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="4a611-3680">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="4a611-3680">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="4a611-3681">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="4a611-3681">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-3682">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-3682">VM</span></span>

* <span data-ttu-id="4a611-3683">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="4a611-3683">Support configuring nsg</span></span>
* <span data-ttu-id="4a611-3684">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="4a611-3684">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="4a611-3685">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="4a611-3685">Support managed service identities</span></span>
* <span data-ttu-id="4a611-3686">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3686">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="4a611-3687">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="4a611-3687">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="4a611-3688">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-3688">May 10, 2017</span></span>

<span data-ttu-id="4a611-3689">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="4a611-3689">Version 2.0.6</span></span>

* <span data-ttu-id="4a611-3690">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="4a611-3690">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="4a611-3691">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="4a611-3691">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="4a611-3692">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="4a611-3692">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="4a611-3693">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="4a611-3693">Include Cognitive Services module</span></span>
* <span data-ttu-id="4a611-3694">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="4a611-3694">Include Service Fabric module</span></span>
* <span data-ttu-id="4a611-3695">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="4a611-3695">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="4a611-3696">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="4a611-3696">Add support for CDN commands</span></span>
* <span data-ttu-id="4a611-3697">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="4a611-3697">Remove Container module</span></span>
* <span data-ttu-id="4a611-3698">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3698">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="4a611-3699">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3699">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="4a611-3700">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-3700">Core</span></span>

* <span data-ttu-id="4a611-3701">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="4a611-3701">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="4a611-3702">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([#2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3702">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="4a611-3703">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3703">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="4a611-3704">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3704">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="4a611-3705">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3705">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="4a611-3706">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3706">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="4a611-3707">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3707">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="4a611-3708">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3708">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="4a611-3709">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3709">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="4a611-3710">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="4a611-3710">core: Improved performance</span></span>
* <span data-ttu-id="4a611-3711">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="4a611-3711">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="4a611-3712">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="4a611-3712">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-3713">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-3713">ACS</span></span>

* <span data-ttu-id="4a611-3714">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="4a611-3714">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="4a611-3715">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="4a611-3715">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="4a611-3716">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="4a611-3716">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="4a611-3717">Удален профиль Windows перед вызовом метода PUT для команды scale ([#2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3717">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-3718">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-3718">AppService</span></span>

* <span data-ttu-id="4a611-3719">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="4a611-3719">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="4a611-3720">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="4a611-3720">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="4a611-3721">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="4a611-3721">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="4a611-3722">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="4a611-3722">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="4a611-3723">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="4a611-3723">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="4a611-3724">Включена поддержка настройки строк подключения ([#2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3724">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="4a611-3725">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="4a611-3725">support slot swap with preview</span></span>
* <span data-ttu-id="4a611-3726">Устранены ошибки из команд службы приложений ([#2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3726">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="4a611-3727">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([#2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3727">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4a611-3728">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4a611-3728">CosmosDB</span></span>

* <span data-ttu-id="4a611-3729">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="4a611-3729">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="4a611-3730">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="4a611-3730">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="4a611-3731">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="4a611-3731">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="4a611-3732">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="4a611-3732">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4a611-3733">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4a611-3733">Data Lake Analytics</span></span>

* <span data-ttu-id="4a611-3734">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="4a611-3734">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="4a611-3735">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="4a611-3735">Add support for new catalog item type: package.</span></span> <span data-ttu-id="4a611-3736">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3736">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="4a611-3737">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="4a611-3737">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="4a611-3738">Таблица</span><span class="sxs-lookup"><span data-stu-id="4a611-3738">Table</span></span>
  * <span data-ttu-id="4a611-3739">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="4a611-3739">Table valued function</span></span>
  * <span data-ttu-id="4a611-3740">Представление</span><span class="sxs-lookup"><span data-stu-id="4a611-3740">View</span></span>
  * <span data-ttu-id="4a611-3741">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="4a611-3741">Table Statistics.</span></span> <span data-ttu-id="4a611-3742">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="4a611-3742">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4a611-3743">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="4a611-3743">Data Lake Store</span></span>

* <span data-ttu-id="4a611-3744">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="4a611-3744">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="4a611-3745">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3745">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="4a611-3746">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="4a611-3746">missed help for access show.</span></span> <span data-ttu-id="4a611-3747">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="4a611-3747">adding it.</span></span> <span data-ttu-id="4a611-3748">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="4a611-3748">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="4a611-3749">Поиск</span><span class="sxs-lookup"><span data-stu-id="4a611-3749">Find</span></span>

* <span data-ttu-id="4a611-3750">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="4a611-3750">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="4a611-3751">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4a611-3751">KeyVault</span></span>

* <span data-ttu-id="4a611-3752">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="4a611-3752">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="4a611-3753">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="4a611-3753">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="4a611-3754">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="4a611-3754">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="4a611-3755">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="4a611-3755">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="4a611-3756">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3756">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="4a611-3757">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="4a611-3757">Lab</span></span>

* <span data-ttu-id="4a611-3758">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4a611-3758">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="4a611-3759">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4a611-3759">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="4a611-3760">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4a611-3760">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="4a611-3761">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4a611-3761">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="4a611-3762">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4a611-3762">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="4a611-3763">Монитор</span><span class="sxs-lookup"><span data-stu-id="4a611-3763">Monitor</span></span>

* <span data-ttu-id="4a611-3764">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3764">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="4a611-3765">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3765">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="4a611-3766">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-3766">Network</span></span>

* <span data-ttu-id="4a611-3767">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3767">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="4a611-3768">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3768">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="4a611-3769">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="4a611-3769">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="4a611-3770">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="4a611-3770">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="4a611-3771">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="4a611-3771">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="4a611-3772">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="4a611-3772">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="4a611-3773">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="4a611-3773">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="4a611-3774">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="4a611-3774">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="4a611-3775">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3775">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="4a611-3776">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="4a611-3776">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="4a611-3777">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3777">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="4a611-3778">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3778">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="4a611-3779">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="4a611-3779">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="4a611-3780">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="4a611-3780">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="4a611-3781">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="4a611-3781">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="4a611-3782">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="4a611-3782">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="4a611-3783">Профиль</span><span class="sxs-lookup"><span data-stu-id="4a611-3783">Profile</span></span>

* <span data-ttu-id="4a611-3784">Включена поддержка входа при отсутствии подписок ([#2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3784">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="4a611-3785">Включена поддержка сокращенных имен параметров в команде az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3785">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="4a611-3786">Redis</span><span class="sxs-lookup"><span data-stu-id="4a611-3786">Redis</span></span>

* <span data-ttu-id="4a611-3787">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="4a611-3787">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="4a611-3788">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="4a611-3788">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="4a611-3789">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4a611-3789">Resource</span></span>

* <span data-ttu-id="4a611-3790">Добавлены команды определения managedapp и managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3790">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="4a611-3791">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3791">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="4a611-3792">Включена поддержка создания универсального ресурса ([#2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3792">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="4a611-3793">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="4a611-3793">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="4a611-3794">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="4a611-3794">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="4a611-3795">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="4a611-3795">Add docs for az lock update.</span></span> <span data-ttu-id="4a611-3796">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="4a611-3796">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="4a611-3797">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="4a611-3797">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="4a611-3798">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="4a611-3798">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="4a611-3799">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="4a611-3799">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="4a611-3800">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="4a611-3800">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="4a611-3801">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([#2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3801">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="4a611-3802">Роль</span><span class="sxs-lookup"><span data-stu-id="4a611-3802">Role</span></span>

* <span data-ttu-id="4a611-3803">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([#2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3803">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="4a611-3804">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3804">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="4a611-3805">Роль: устранены проблемы при обновлении определения роли ([#2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3805">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="4a611-3806">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="4a611-3806">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="4a611-3807">SQL</span><span class="sxs-lookup"><span data-stu-id="4a611-3807">SQL</span></span>

* <span data-ttu-id="4a611-3808">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="4a611-3808">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="4a611-3809">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3809">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="4a611-3810">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-3810">Storage</span></span>

* <span data-ttu-id="4a611-3811">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3811">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="4a611-3812">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="4a611-3812">Add support for incremental blob copy</span></span>
* <span data-ttu-id="4a611-3813">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="4a611-3813">Add support for large block blob upload</span></span>
* <span data-ttu-id="4a611-3814">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="4a611-3814">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-3815">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-3815">VM</span></span>

* <span data-ttu-id="4a611-3816">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="4a611-3816">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="4a611-3817">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="4a611-3817">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="4a611-3818">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="4a611-3818">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="4a611-3819">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="4a611-3819">az vm/vmss disk</span></span>
  3. <span data-ttu-id="4a611-3820">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="4a611-3820">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="4a611-3821">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="4a611-3821">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="4a611-3822">vm/vmss: добавлена поддержка создания из образа Marketplace, для которого требуются сведения о плане ([#1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3822">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="4a611-3823">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-3823">April 3, 2017</span></span>

<span data-ttu-id="4a611-3824">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="4a611-3824">Version 2.0.2</span></span>

<span data-ttu-id="4a611-3825">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="4a611-3825">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="4a611-3826">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="4a611-3826">Core</span></span>

* <span data-ttu-id="4a611-3827">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-3827">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="4a611-3828">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3828">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="4a611-3829">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3829">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="4a611-3830">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3830">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4a611-3831">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3831">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="4a611-3832">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="4a611-3832">Add prompting for missing template parameters.</span></span> <span data-ttu-id="4a611-3833">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3833">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="4a611-3834">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4a611-3834">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="4a611-3835">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="4a611-3835">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="4a611-3836">ACS</span><span class="sxs-lookup"><span data-stu-id="4a611-3836">ACS</span></span>

* <span data-ttu-id="4a611-3837">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3837">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="4a611-3838">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="4a611-3838">Add support for ssh key password prompting.</span></span> <span data-ttu-id="4a611-3839">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3839">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="4a611-3840">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="4a611-3840">Add support for windows clusters.</span></span> <span data-ttu-id="4a611-3841">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3841">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="4a611-3842">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="4a611-3842">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="4a611-3843">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3843">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="4a611-3844">AppService</span><span class="sxs-lookup"><span data-stu-id="4a611-3844">AppService</span></span>

* <span data-ttu-id="4a611-3845">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3845">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="4a611-3846">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3846">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="4a611-3847">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3847">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="4a611-3848">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3848">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="4a611-3849">Data Lake</span><span class="sxs-lookup"><span data-stu-id="4a611-3849">DataLake</span></span>

* <span data-ttu-id="4a611-3850">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="4a611-3850">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="4a611-3851">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="4a611-3851">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="4a611-3852">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="4a611-3852">DocuemntDB</span></span>

* <span data-ttu-id="4a611-3853">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3853">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="4a611-3854">ВМ</span><span class="sxs-lookup"><span data-stu-id="4a611-3854">VM</span></span>

* <span data-ttu-id="4a611-3855">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3855">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="4a611-3856">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3856">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="4a611-3857">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3857">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="4a611-3858">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3858">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4a611-3859">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3859">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="4a611-3860">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3860">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="4a611-3861">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="4a611-3861">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="4a611-3862">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4a611-3862">February 27, 2017</span></span>

<span data-ttu-id="4a611-3863">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="4a611-3863">Version 2.0.0</span></span>

<span data-ttu-id="4a611-3864">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="4a611-3864">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="4a611-3865">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="4a611-3865">Container Service (acs)</span></span>
- <span data-ttu-id="4a611-3866">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="4a611-3866">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="4a611-3867">Сеть</span><span class="sxs-lookup"><span data-stu-id="4a611-3867">Networking</span></span>
- <span data-ttu-id="4a611-3868">Память</span><span class="sxs-lookup"><span data-stu-id="4a611-3868">Storage</span></span>

<span data-ttu-id="4a611-3869">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3869">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="4a611-3870">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="4a611-3870">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="4a611-3871">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="4a611-3871">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="4a611-3872">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="4a611-3872">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="4a611-3873">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="4a611-3873">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="4a611-3874">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="4a611-3874">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="4a611-3875">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="4a611-3875">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="4a611-3876">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="4a611-3876">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="4a611-3877">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="4a611-3877">Provide feedback from the command line with the `az feedback` command</span></span>

# <a name="beta-release-notes"></a>[<span data-ttu-id="4a611-3878">Заметки о выпуске бета-версии</span><span class="sxs-lookup"><span data-stu-id="4a611-3878">Beta release notes</span></span>](#tab/azure-cli-beta)

<span data-ttu-id="4a611-3879">Бета-версия Azure CLI позволяет перейти с метода аутентификации платформы AAD (версия 1.0) на [платформу удостоверений Майкрософт (версия 2.0)](/azure/active-directory/develop/v2-overview).</span><span class="sxs-lookup"><span data-stu-id="4a611-3879">The Azure CLI beta release is a migration from the authentican method of AAD platform (v1.0) to [Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview).</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="4a611-3880">23 июня 2020 года</span><span class="sxs-lookup"><span data-stu-id="4a611-3880">June 23, 2020</span></span>

### <a name="things-to-know-about-the-new-azure-cli-beta-release"></a><span data-ttu-id="4a611-3881">Сведения о новой бета-версии Azure CLI</span><span class="sxs-lookup"><span data-stu-id="4a611-3881">Things to know about the new Azure CLI beta release</span></span>

-   <span data-ttu-id="4a611-3882">Бета-версия Azure CLI поддерживает все команды интерфейса командной строки, которые включены в текущую выпущенную версию.</span><span class="sxs-lookup"><span data-stu-id="4a611-3882">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span>
-   <span data-ttu-id="4a611-3883">После установки бета-версии требуется выполнить повторный вход.</span><span class="sxs-lookup"><span data-stu-id="4a611-3883">Relogin is required after install the beta version.</span></span>
-   <span data-ttu-id="4a611-3884">Бета-версия поддерживает только платформу Windows.</span><span class="sxs-lookup"><span data-stu-id="4a611-3884">The beta release only supports the Windows platform.</span></span>
-   <span data-ttu-id="4a611-3885">Azure Stack не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a611-3885">The Azure Stack is not supported.</span></span>
-   <span data-ttu-id="4a611-3886">Параметр `--use-cert-sn-issuer` не поддерживается, если для проверки подлинности используется ключ субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="4a611-3886">`--use-cert-sn-issuer` parameter is not supported when using service principal key to authenticate.</span></span>
-   <span data-ttu-id="4a611-3887">Пропуск проверки SSL с использованием `ADAL_PYTHON_SSL_NO_VERIFY` среды не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a611-3887">Skip SSL verification via environment `ADAL_PYTHON_SSL_NO_VERIFY` is not supported.</span></span>

<span data-ttu-id="4a611-3888">Если у вас возникли проблемы с использованием бета-версии, вы можете обратиться к группе разработчиков Azure CLI на [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span><span class="sxs-lookup"><span data-stu-id="4a611-3888">If you find any issues in the beta release, the Azure CLI engineering team welcomes your comments on [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span></span>

---
