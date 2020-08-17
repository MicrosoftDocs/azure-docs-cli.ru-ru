---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 08/06/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: f81f5a69bd5806d2081a8eaa9b62a5b00b56edf9
ms.sourcegitcommit: 04d3b43d7c960ff0e6188c9672d27046b45da6ed
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/06/2020
ms.locfileid: "87855939"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="cd667-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="cd667-103">Azure CLI release notes</span></span>

# <a name="current-release-notes"></a>[<span data-ttu-id="cd667-104">Заметки о текущем выпуске</span><span class="sxs-lookup"><span data-stu-id="cd667-104">Current release notes</span></span>](#tab/azure-cli)

## <a name="august-11-2020"></a><span data-ttu-id="cd667-105">11 августа 2020 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-105">August 11, 2020</span></span>

<span data-ttu-id="cd667-106">Версия 2.10.1</span><span class="sxs-lookup"><span data-stu-id="cd667-106">Version 2.10.1</span></span>

### <a name="app-service"></a><span data-ttu-id="cd667-107">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-107">App Service</span></span>

* <span data-ttu-id="cd667-108">Исправление № 9887: включена поддержка веб-приложений и приложений-функций, а также поддержка назначения и удаления управляемых удостоверений пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd667-108">Fix #9887 webapp and functionapp, support assigning/removing user managed identity</span></span>
* <span data-ttu-id="cd667-109">Исправление №№ 1382 и 14055: обновлены сообщения об ошибках для az webapp create и az webapp config container set.</span><span class="sxs-lookup"><span data-stu-id="cd667-109">Fix #1382, #14055: Update error messages for az webapp create and az webapp config container set</span></span>
* <span data-ttu-id="cd667-110">`az webapp up`: исправлена логика выбора ASP по умолчанию, когда параметр --plan не указан.</span><span class="sxs-lookup"><span data-stu-id="cd667-110">`az webapp up`: Fix default ASP selection logic when --plan parameter is not provided</span></span>

### <a name="appconfig"></a><span data-ttu-id="cd667-111">AppConfig</span><span class="sxs-lookup"><span data-stu-id="cd667-111">AppConfig</span></span>

* <span data-ttu-id="cd667-112">Включена поддержка включения и отключения PublicNetworkAccess во время создания хранилища.</span><span class="sxs-lookup"><span data-stu-id="cd667-112">Support enabling/disabling PublicNetworkAccess during store creation</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-113">Вычисления</span><span class="sxs-lookup"><span data-stu-id="cd667-113">Compute</span></span>

* <span data-ttu-id="cd667-114">Включена поддержка связывания диска и моментального снимка с ресурсом доступа к диску.</span><span class="sxs-lookup"><span data-stu-id="cd667-114">Support associating disk and snapshot with a disk-access resource</span></span>

### <a name="lab"></a><span data-ttu-id="cd667-115">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="cd667-115">Lab</span></span>

* <span data-ttu-id="cd667-116">Исправлена ошибка № 7904, связанная с проверкой даты при создании виртуальной машины лаборатории.</span><span class="sxs-lookup"><span data-stu-id="cd667-116">Fix for issue #7904 date validation bug in lab vm creation</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-117">Хранилище</span><span class="sxs-lookup"><span data-stu-id="cd667-117">Storage</span></span>

* <span data-ttu-id="cd667-118">`az storage blob upload-batch`: исправлена ошибка № 14660, связанная с непозиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="cd667-118">`az storage blob upload-batch`: Fix issue #14660 with unpositional arguments</span></span>

## <a name="august-04-2020"></a><span data-ttu-id="cd667-119">04 августа 2020 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-119">August 04, 2020</span></span>

<span data-ttu-id="cd667-120">Версия 2.10.0</span><span class="sxs-lookup"><span data-stu-id="cd667-120">Version 2.10.0</span></span>

### <a name="aks"></a><span data-ttu-id="cd667-121">AKS</span><span class="sxs-lookup"><span data-stu-id="cd667-121">AKS</span></span>

* <span data-ttu-id="cd667-122">`az aks update`: изменен аргумент --enable-aad для переноса кластера с поддержкой RBAC за пределами AAD в управляемый AKS кластер AAD.</span><span class="sxs-lookup"><span data-stu-id="cd667-122">`az aks update`: Change --enable-aad argument to migrate a RBAC-enabled non-AAD cluster to a AKS-managed AAD cluster</span></span>
* <span data-ttu-id="cd667-123">`az aks install-cli`: добавлены аргументы --kubelogin-version и --kubelogin-install-location для установки kubelogin.</span><span class="sxs-lookup"><span data-stu-id="cd667-123">`az aks install-cli`: Add --kubelogin-version and --kubelogin-install-location arguments to install kubelogin</span></span>
* <span data-ttu-id="cd667-124">Добавлена команда az aks nodepool get-upgrades.</span><span class="sxs-lookup"><span data-stu-id="cd667-124">Add az aks nodepool get-upgrades command</span></span>

### <a name="ams"></a><span data-ttu-id="cd667-125">AMS</span><span class="sxs-lookup"><span data-stu-id="cd667-125">AMS</span></span>

* <span data-ttu-id="cd667-126">Исправление № 14021: команда az ams account sp не является идемпотентной.</span><span class="sxs-lookup"><span data-stu-id="cd667-126">Fix #14021: az ams account sp is not idempotent</span></span>

### <a name="apim"></a><span data-ttu-id="cd667-127">APIM</span><span class="sxs-lookup"><span data-stu-id="cd667-127">APIM</span></span>

* <span data-ttu-id="cd667-128">apim api import: включена поддержка импорта API и расширены другие команды CLI уровня API.</span><span class="sxs-lookup"><span data-stu-id="cd667-128">apim api import: support API import and enchance other api level cli commands</span></span>

### <a name="app-service"></a><span data-ttu-id="cd667-129">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-129">App Service</span></span>

* <span data-ttu-id="cd667-130">Исправление № 13035: включена проверка для az webapp config access-restriction, чтобы предотвратить добавление дубликатов.</span><span class="sxs-lookup"><span data-stu-id="cd667-130">Fix #13035: Add validation for az webapp config access-restriction to avoid adding duplicates</span></span>

### <a name="appconfig"></a><span data-ttu-id="cd667-131">AppConfig</span><span class="sxs-lookup"><span data-stu-id="cd667-131">AppConfig</span></span>

* <span data-ttu-id="cd667-132">По умолчанию используется номер SKU "Стандартный", если не указано другое.</span><span class="sxs-lookup"><span data-stu-id="cd667-132">Default to standard sku if not specified</span></span>
* <span data-ttu-id="cd667-133">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Поддерживаются параметры с типом содержимого JSON.</span><span class="sxs-lookup"><span data-stu-id="cd667-133">[BREAKING CHANGE] Support settings with JSON content type</span></span>

### <a name="arm"></a><span data-ttu-id="cd667-134">ARM</span><span class="sxs-lookup"><span data-stu-id="cd667-134">ARM</span></span>

* <span data-ttu-id="cd667-135">`az resource tag`: исправлена ошибка с добавлением тегов managedApp и устранены некоторые проблемы, связанные с тестами.</span><span class="sxs-lookup"><span data-stu-id="cd667-135">`az resource tag`: Fix the bug of managedApp tagging and some related test issues</span></span>
* <span data-ttu-id="cd667-136">`az deployment mg/tenant what-if`: включена поддержка What-If для группы управления и развертывания на уровне арендатора.</span><span class="sxs-lookup"><span data-stu-id="cd667-136">`az deployment mg/tenant what-if`: Add support to management group and tenant level deployment What-If</span></span>
* <span data-ttu-id="cd667-137">`az deployment mg/tenant create`: добавлен параметр --confirm-with-what-if/-c.</span><span class="sxs-lookup"><span data-stu-id="cd667-137">`az deployment mg/tenant create`: Add --confirm-with-what-if/-c parameter.</span></span>
* <span data-ttu-id="cd667-138">`az deployment mg/tenant create`: добавлен параметр --what-if-result-format/-r.</span><span class="sxs-lookup"><span data-stu-id="cd667-138">`az deployment mg/tenant create`: Add --what-if-result-format/-r parameter.</span></span>
* <span data-ttu-id="cd667-139">`az deployment mg/tenant create`: добавлен параметр --what-if-exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="cd667-139">`az deployment mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="cd667-140">`az tag`: включена поддержка az tag для параметра идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="cd667-140">`az tag`: az tag support for resource id parameter</span></span>

### <a name="backup"></a><span data-ttu-id="cd667-141">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="cd667-141">Backup</span></span>

* <span data-ttu-id="cd667-142">Обнаружение элемента или контейнера AFS активируется только при необходимости.</span><span class="sxs-lookup"><span data-stu-id="cd667-142">Trigger AFS container/item discovery only when needed</span></span>

### <a name="cdn"></a><span data-ttu-id="cd667-143">CDN</span><span class="sxs-lookup"><span data-stu-id="cd667-143">CDN</span></span>

* <span data-ttu-id="cd667-144">Добавлены поля Приватного канала в источник.</span><span class="sxs-lookup"><span data-stu-id="cd667-144">Add private link fields to origin</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-145">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="cd667-145">Compute</span></span>

* <span data-ttu-id="cd667-146">`az vm/vmss create`: возможность выбора допустимого имени пользователя, если имя пользователя по умолчанию является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="cd667-146">`az vm/vmss create`: Select a valid username for user if the default username is invalid</span></span>
* <span data-ttu-id="cd667-147">`az vm update`: включена поддержка образа для разных арендаторов.</span><span class="sxs-lookup"><span data-stu-id="cd667-147">`az vm update`: support cross tenant image</span></span>
* <span data-ttu-id="cd667-148">`az disk-access`: добавлена новая группа команд для использования ресурса доступа к диску.</span><span class="sxs-lookup"><span data-stu-id="cd667-148">`az disk-access`: Add new command group to operate disk access resource</span></span>
* <span data-ttu-id="cd667-149">Включена поддержка автоматического размещения выделенной группы узлов.</span><span class="sxs-lookup"><span data-stu-id="cd667-149">Support dedicated host group automatic placement</span></span>
* <span data-ttu-id="cd667-150">Включена поддержка ppg и spg в режиме оркестрации Масштабируемых наборов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="cd667-150">Support ppg and spg in VMSS orchestration mode</span></span>

### <a name="config"></a><span data-ttu-id="cd667-151">Config</span><span class="sxs-lookup"><span data-stu-id="cd667-151">Config</span></span>

* <span data-ttu-id="cd667-152">`az config`: добавлен новый модуль команд `config`.</span><span class="sxs-lookup"><span data-stu-id="cd667-152">`az config`: Add new `config` command module</span></span>

### <a name="extension"></a><span data-ttu-id="cd667-153">Расширение</span><span class="sxs-lookup"><span data-stu-id="cd667-153">Extension</span></span>

* <span data-ttu-id="cd667-154">Включена поддержка автоматической установки расширения, если расширение команды не установлено.</span><span class="sxs-lookup"><span data-stu-id="cd667-154">Support automatically installing an extension if the extension of a command is not installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="cd667-155">HDInsight</span><span class="sxs-lookup"><span data-stu-id="cd667-155">HDInsight</span></span>

* <span data-ttu-id="cd667-156">Добавлены три параметра в команду `az hdinsight create` для включения поддержки Приватного канала и шифрования в функции передачи:</span><span class="sxs-lookup"><span data-stu-id="cd667-156">Add 3 parameters to the command `az hdinsight create` to support private link and encryption in transit feature:</span></span>

### <a name="iot-hub"></a><span data-ttu-id="cd667-157">Центр Интернета вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-157">Iot Hub</span></span>

* <span data-ttu-id="cd667-158">Исправление № 7792: создание Центра Интернета вещей не является идемпотентным.</span><span class="sxs-lookup"><span data-stu-id="cd667-158">Fix #7792: IoT Hub Create is not idempotent</span></span>

### <a name="iot-central"></a><span data-ttu-id="cd667-159">IoT Central</span><span class="sxs-lookup"><span data-stu-id="cd667-159">IoT Central</span></span>

* <span data-ttu-id="cd667-160">Добавлен список вариантов параметра для IoT Central.</span><span class="sxs-lookup"><span data-stu-id="cd667-160">Add paramater option list for iot central</span></span>

### <a name="keyvault"></a><span data-ttu-id="cd667-161">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="cd667-161">KeyVault</span></span>

* <span data-ttu-id="cd667-162">`az keyvault key encrypt/decrypt`: добавлен параметр `--data-type` для явного определения типа исходных данных.</span><span class="sxs-lookup"><span data-stu-id="cd667-162">`az keyvault key encrypt/decrypt`: add parameter `--data-type` for explicitly specifing the type of original data</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-163">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-163">Monitor</span></span>

* <span data-ttu-id="cd667-164">`az monitor log-analytics workspace data-export`: включена поддержка пространства имен концентратора событий в качестве назначения.</span><span class="sxs-lookup"><span data-stu-id="cd667-164">`az monitor log-analytics workspace data-export`: support event hub namespace as the destination.</span></span>
* <span data-ttu-id="cd667-165">`az monitor autoscale`: включена поддержка пространства имен и измерений для --condition.</span><span class="sxs-lookup"><span data-stu-id="cd667-165">`az monitor autoscale`: support namespace and dimensions for --condition</span></span>

### <a name="netappfiles"></a><span data-ttu-id="cd667-166">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="cd667-166">NetAppFiles</span></span>

* <span data-ttu-id="cd667-167">`az volume revert`:  включена поддержка возврата тома к одному из его моментальных снимков.</span><span class="sxs-lookup"><span data-stu-id="cd667-167">`az volume revert`:  Add Volume Revert to revert a volume to one of its snapshots.</span></span>
* <span data-ttu-id="cd667-168">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален командлет `az netappfiles mount-target`.</span><span class="sxs-lookup"><span data-stu-id="cd667-168">[BREAKING CHANGE] Remove `az netappfiles mount-target`.</span></span>
* <span data-ttu-id="cd667-169">`az volume show`: добавлен сайт в свойства Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cd667-169">`az volume show`: Add site to Active Directory Properties</span></span>

### <a name="network"></a><span data-ttu-id="cd667-170">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-170">Network</span></span>

* <span data-ttu-id="cd667-171">`az application-gateway private-link add`: включена поддержка определение существующей подсети по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="cd667-171">`az application-gateway private-link add`: support to specify an existing subnet by ID</span></span>
* <span data-ttu-id="cd667-172">`az network application-gateway waf-policy create`: включена поддержка версии и типа.</span><span class="sxs-lookup"><span data-stu-id="cd667-172">`az network application-gateway waf-policy create`: support version and type</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-173">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-173">Storage</span></span>

* <span data-ttu-id="cd667-174">Исправление № 10302: включена поддержка подбора типа содержимого при синхронизации файлов.</span><span class="sxs-lookup"><span data-stu-id="cd667-174">Fix #10302: Support guess content-type when synchronizing files</span></span>
* <span data-ttu-id="cd667-175">`az storage blob lease`: добавлена возможность применить новую версию API для операций аренды BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="cd667-175">`az storage blob lease`: Apply new api version for blob lease operations</span></span>
* <span data-ttu-id="cd667-176">`az storage fs access`: включена поддержка учетных данных AAD при управлении доступом для учетной записи ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="cd667-176">`az storage fs access`: Support AAD credential in managing access control for ADLS Gen2 account</span></span>
* <span data-ttu-id="cd667-177">`az storage share-rm create/update`: добавлен аргумент --access-tier для включения поддержки уровня доступа.</span><span class="sxs-lookup"><span data-stu-id="cd667-177">`az storage share-rm create/update`: add --access-tier to support access tier</span></span>

## <a name="july-16-2020"></a><span data-ttu-id="cd667-178">16 июля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-178">July 16, 2020</span></span>

<span data-ttu-id="cd667-179">Версия 2.9.1</span><span class="sxs-lookup"><span data-stu-id="cd667-179">Version 2.9.1</span></span>

### <a name="aks"></a><span data-ttu-id="cd667-180">AKS</span><span class="sxs-lookup"><span data-stu-id="cd667-180">AKS</span></span>

* <span data-ttu-id="cd667-181">Явный параметр VMSS в примере команды для Windows удален, так как он теперь используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-181">Remove explicit setting of VMSS in Windows example command since it is now default</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-182">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-182">IoT</span></span>

* <span data-ttu-id="cd667-183">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az iot pnp`: удаление предварительной версии команд IoT PNP из основной версии CLI.</span><span class="sxs-lookup"><span data-stu-id="cd667-183">[BREAKING CHANGE] `az iot pnp`: Remove IoT PNP preview commands from core CLI</span></span>

### <a name="rest"></a><span data-ttu-id="cd667-184">REST</span><span class="sxs-lookup"><span data-stu-id="cd667-184">REST</span></span>

* <span data-ttu-id="cd667-185">Исправлена ошибка № 14152. `az rest`: URL-адреса ARM принимаются без идентификатора подписки.</span><span class="sxs-lookup"><span data-stu-id="cd667-185">Fix #14152: `az rest`: Accept ARM URLs without subscription ID</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-186">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-186">Storage</span></span>

* <span data-ttu-id="cd667-187">Исправлена ошибка № 14138. Некоторые разрешения стали необязательными.</span><span class="sxs-lookup"><span data-stu-id="cd667-187">Fix #14138: Make some permissions optional</span></span>

## <a name="july-14-2020"></a><span data-ttu-id="cd667-188">14 июля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-188">July 14, 2020</span></span>

<span data-ttu-id="cd667-189">Версия 2.9.0</span><span class="sxs-lookup"><span data-stu-id="cd667-189">Version 2.9.0</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-190">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-190">ACR</span></span>

* <span data-ttu-id="cd667-191">Обработка ссылки на артефакт журнала из реестра для потоковой передачи журналов.</span><span class="sxs-lookup"><span data-stu-id="cd667-191">Handle log artifact link from Registry to stream logs</span></span>
* <span data-ttu-id="cd667-192">Устарели команды helm2.</span><span class="sxs-lookup"><span data-stu-id="cd667-192">Deprecate helm2 commands</span></span>

### <a name="aks"></a><span data-ttu-id="cd667-193">AKS</span><span class="sxs-lookup"><span data-stu-id="cd667-193">AKS</span></span>

* <span data-ttu-id="cd667-194">`az aks create`: добавлен аргумент --enable-aad.</span><span class="sxs-lookup"><span data-stu-id="cd667-194">`az aks create`: add --enable-aad argument</span></span>
* <span data-ttu-id="cd667-195">`az aks update`: добавлен аргумент --enable-aad.</span><span class="sxs-lookup"><span data-stu-id="cd667-195">`az aks update`: add --enable-aad argument</span></span>

### <a name="apim"></a><span data-ttu-id="cd667-196">APIM</span><span class="sxs-lookup"><span data-stu-id="cd667-196">APIM</span></span>

* <span data-ttu-id="cd667-197">Добавлены общие команды az apim api.</span><span class="sxs-lookup"><span data-stu-id="cd667-197">Added general az apim api commands</span></span>

### <a name="appconfig"></a><span data-ttu-id="cd667-198">AppConfig</span><span class="sxs-lookup"><span data-stu-id="cd667-198">AppConfig</span></span>

* <span data-ttu-id="cd667-199">Добавлен пример для использования --fields в appconfig revision.</span><span class="sxs-lookup"><span data-stu-id="cd667-199">Add example for using --fields in appconfig revision</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-200">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-200">AppService</span></span>

* <span data-ttu-id="cd667-201">`az functionapp create`: включена поддержка Java 11 и PowerShell 7.</span><span class="sxs-lookup"><span data-stu-id="cd667-201">`az functionapp create`: Added support for Java 11 and Powershell 7.</span></span> <span data-ttu-id="cd667-202">Включена поддержка API стеков.</span><span class="sxs-lookup"><span data-stu-id="cd667-202">Added Stacks API Support.</span></span>
* <span data-ttu-id="cd667-203">Исправлена ошибка № 14208, из-за которой создание многоконтейнерного приложения завершается сбоем.</span><span class="sxs-lookup"><span data-stu-id="cd667-203">Fix #14208 multi-container app creation fails</span></span>
* <span data-ttu-id="cd667-204">Исправлена ошибка с az webapp create, связанная с использованием вписанных в код стеков среды выполнения.</span><span class="sxs-lookup"><span data-stu-id="cd667-204">Fix az webapp create - use hardcoded runtime stacks</span></span>

### <a name="arm"></a><span data-ttu-id="cd667-205">ARM</span><span class="sxs-lookup"><span data-stu-id="cd667-205">ARM</span></span>

* <span data-ttu-id="cd667-206">`az resource tag`: исправлена ошибка, связанная с добавлением тегов к ресурсам с помощью типа ресурса `Microsoft.ContainerInstance/containerGroups`.</span><span class="sxs-lookup"><span data-stu-id="cd667-206">`az resource tag`: Fix the problem of tagging resources with resource type `Microsoft.ContainerInstance/containerGroups`</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-207">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="cd667-207">Compute</span></span>

* <span data-ttu-id="cd667-208">Выполнено обновление версии дисков до 2020-05-01 и вычислительных ресурсов до 2020-06-01.</span><span class="sxs-lookup"><span data-stu-id="cd667-208">Bump version disks 2020-05-01, compute 2020-06-01</span></span>
* <span data-ttu-id="cd667-209">Включено двойное шифрование набора шифрования диска.</span><span class="sxs-lookup"><span data-stu-id="cd667-209">Double encryption of disk encryption set</span></span>
* <span data-ttu-id="cd667-210">`az vmss update`: включена поддержка определения межклиентского образа.</span><span class="sxs-lookup"><span data-stu-id="cd667-210">`az vmss update`: support specify cross tenant image.</span></span>
* <span data-ttu-id="cd667-211">`az sig image-version create`: включена поддержка определения межклиентского образа.</span><span class="sxs-lookup"><span data-stu-id="cd667-211">`az sig image-version create`: support specify cross tenant image.</span></span>
* <span data-ttu-id="cd667-212">vm/vmss create. Включено шифрование кэша и передаваемых данных для дисков ОС и данных и временных дисков для виртуальных машин и Масштабируемых наборов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="cd667-212">vm/vmss create: Encryption of cache & data-in-transit for OS/Data disks and temp disks for VM & VMSS</span></span>
* <span data-ttu-id="cd667-213">Добавлена операция имитации удаления для виртуальных машин и Масштабируемых наборов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="cd667-213">Add simulate-eviction operation for VM and VMSS</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="cd667-214">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-214">CosmosDB</span></span>

* <span data-ttu-id="cd667-215">Последние компоненты: Autoscale, IpRules, EnableFreeTier и EnableAnalyticalStorage.</span><span class="sxs-lookup"><span data-stu-id="cd667-215">Recent features: Autoscale, IpRules, EnableFreeTier and EnableAnalyticalStorage</span></span>

### <a name="eventgrid"></a><span data-ttu-id="cd667-216">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="cd667-216">EventGrid</span></span>

* <span data-ttu-id="cd667-217">Включена поддержка CLI для 2020-04-01-preview и отмечены предварительные версии функций как is_Preview=true.</span><span class="sxs-lookup"><span data-stu-id="cd667-217">Add CLI support for 2020-04-01-preview and mark preview features with is_Preview=True</span></span>

### <a name="find"></a><span data-ttu-id="cd667-218">Поиск</span><span class="sxs-lookup"><span data-stu-id="cd667-218">Find</span></span>

* <span data-ttu-id="cd667-219">Исправлена ошибка № 14094, связанная с az find. Исправлена ошибка, из-за которой не удается войти при отключенной телеметрии.</span><span class="sxs-lookup"><span data-stu-id="cd667-219">Fix #14094 az find Fix Queries failing when not logged in and when telemetry is disabled</span></span>

### <a name="hdinsight"></a><span data-ttu-id="cd667-220">HDInsight</span><span class="sxs-lookup"><span data-stu-id="cd667-220">HDInsight</span></span>

* <span data-ttu-id="cd667-221">Добавлены две команды для перезагрузки узла HDInsight.</span><span class="sxs-lookup"><span data-stu-id="cd667-221">Add two commands to support hdinsight node reboot feature</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-222">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-222">Monitor</span></span>

* <span data-ttu-id="cd667-223">Удален флаг предварительной версии для команд в рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="cd667-223">Remove preview flag for commands under Log Analytics workspace</span></span>
* <span data-ttu-id="cd667-224">`az monitor diagnostic-settings subscription`: включена поддержка параметров диагностики для подписки.</span><span class="sxs-lookup"><span data-stu-id="cd667-224">`az monitor diagnostic-settings subscription`: Support diagnositc settings for subscription</span></span>
* <span data-ttu-id="cd667-225">`az monitor metrics`: включена поддержка символов "," и "|" в именах метрик.</span><span class="sxs-lookup"><span data-stu-id="cd667-225">`az monitor metrics`: support ',' and '|' in metric name</span></span>
* <span data-ttu-id="cd667-226">`az monitor log-analytics workspace data-export`: включена поддержка экспорта данных аналитики журнала.</span><span class="sxs-lookup"><span data-stu-id="cd667-226">`az monitor log-analytics workspace data-export`: support log analytics data export</span></span>

### <a name="network"></a><span data-ttu-id="cd667-227">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-227">Network</span></span>

* <span data-ttu-id="cd667-228">`az network application-gateway frontend-ip update`: Устарел параметр --public-ip-address.</span><span class="sxs-lookup"><span data-stu-id="cd667-228">`az network application-gateway frontend-ip update`: Deprecating the --public-ip-address parameter</span></span>
* <span data-ttu-id="cd667-229">Выполнено обновление azure-mgmt-network до 11.0.0.</span><span class="sxs-lookup"><span data-stu-id="cd667-229">Bump azure-mgmt-network to 11.0.0</span></span>
* <span data-ttu-id="cd667-230">`az network express-route gateway connection`: включена конфигурация маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="cd667-230">`az network express-route gateway connection`: support routing configuration</span></span>
* <span data-ttu-id="cd667-231">`az network virtual-appliance`: Включена поддержка сетевого виртуального устройства Azure.</span><span class="sxs-lookup"><span data-stu-id="cd667-231">`az network virtual-appliance`: Support Azure network virtual appliance.</span></span>
* <span data-ttu-id="cd667-232">Включена поддержка компонента Приватного канала в Шлюзе приложений.</span><span class="sxs-lookup"><span data-stu-id="cd667-232">Application Gateway support private link feature</span></span>

### <a name="policyinsights"></a><span data-ttu-id="cd667-233">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="cd667-233">PolicyInsights</span></span>

* <span data-ttu-id="cd667-234">`az policy state`: добавлена команда trigger-scan для активации оценки соответствия политикам.</span><span class="sxs-lookup"><span data-stu-id="cd667-234">`az policy state`: add trigger-scan command to trigger policy compliance evaluations</span></span>
* <span data-ttu-id="cd667-235">`az policy state list`: предоставлены версии сущностей политики в каждой записи соответствия.</span><span class="sxs-lookup"><span data-stu-id="cd667-235">`az policy state list`: expose versions of policy entities in each compliance record</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-236">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-236">Profile</span></span>

* <span data-ttu-id="cd667-237">`az account get-access-token`: включено отображение expiresOn для управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="cd667-237">`az account get-access-token`: Show expiresOn for Managed Identity</span></span>

### <a name="rdbms"></a><span data-ttu-id="cd667-238">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="cd667-238">RDBMS</span></span>

* <span data-ttu-id="cd667-239">Включена поддержка минимальной версии TLS.</span><span class="sxs-lookup"><span data-stu-id="cd667-239">Support Minimum TLS version</span></span>
* <span data-ttu-id="cd667-240">Включено шифрование инфраструктуры для Azure Postgres и MySQL</span><span class="sxs-lookup"><span data-stu-id="cd667-240">Add Infrastructure Encryption for Azure Postgres and MySQL</span></span>

### <a name="security"></a><span data-ttu-id="cd667-241">Безопасность</span><span class="sxs-lookup"><span data-stu-id="cd667-241">Security</span></span>

* <span data-ttu-id="cd667-242">Добавлены команды allowed_connections.</span><span class="sxs-lookup"><span data-stu-id="cd667-242">Add allowed_connections commands</span></span>
* <span data-ttu-id="cd667-243">Добавлены команды адаптивного усиления защиты сети.</span><span class="sxs-lookup"><span data-stu-id="cd667-243">Add Adaptive network hardeningss commands</span></span>
* <span data-ttu-id="cd667-244">Добавлены команды adaptive_application_controls.</span><span class="sxs-lookup"><span data-stu-id="cd667-244">Add adaptive_application_controls commands</span></span>
* <span data-ttu-id="cd667-245">Добавлены команды REST az security iot-solution/iot-alerts/iot-recommendations/iot-analytics в Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="cd667-245">Addition of az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST to Azure CLI</span></span>
* <span data-ttu-id="cd667-246">Добавлен интерфейс командной строки для обеспечения соответствия нормативным требованиям.</span><span class="sxs-lookup"><span data-stu-id="cd667-246">Add regulatory compliance CLI</span></span>

### <a name="signalr"></a><span data-ttu-id="cd667-247">SignalR</span><span class="sxs-lookup"><span data-stu-id="cd667-247">SignalR</span></span>

* <span data-ttu-id="cd667-248">Добавлены возможности, включая управление подключениями к частным конечным точкам, сетевыми правилами и вышестоящими компонентами.</span><span class="sxs-lookup"><span data-stu-id="cd667-248">Add features including managing private endpoint connections, network rules and upstream</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-249">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-249">SQL</span></span>

* <span data-ttu-id="cd667-250">`az sql mi create`, `az sql mi update`: добавлен параметр `--tags` для поддержки тегов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd667-250">`az sql mi create`, `az sql mi update`: Add `--tags` parameter to support resource tagging</span></span>
* <span data-ttu-id="cd667-251">`az sql mi failover`: включена поддержка отработки отказа с основного сайта на дополнительный.</span><span class="sxs-lookup"><span data-stu-id="cd667-251">`az sql mi failover`: Support failover from primary or secondary point</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-252">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-252">Storage</span></span>

* <span data-ttu-id="cd667-253">`az storage account create/update`: добавлен параметр --allow-blob-public-access для включения и отключения общего доступа к большим двоичным объектам и контейнерам.</span><span class="sxs-lookup"><span data-stu-id="cd667-253">`az storage account create/update`: Add --allow-blob-public-access to allow or disallow public access for blob and containers</span></span>
* <span data-ttu-id="cd667-254">`az storage account create/update`: добавлен параметр `--min-tls-version` для настройки минимальной версии TLS, используемой при выполнении запросов к хранилищу.</span><span class="sxs-lookup"><span data-stu-id="cd667-254">`az storage account create/update`: Add `--min-tls-version` to support setting the minimum TLS version to be permitted on requests to storage.</span></span>
* <span data-ttu-id="cd667-255">Удален возврат учетных данных маркера.</span><span class="sxs-lookup"><span data-stu-id="cd667-255">Remove check in token credential</span></span>
* <span data-ttu-id="cd667-256">Исправлено имя учетной записи хранения в примерах.</span><span class="sxs-lookup"><span data-stu-id="cd667-256">Fix the storage account name in examples</span></span>

### <a name="webapp"></a><span data-ttu-id="cd667-257">Веб-приложения</span><span class="sxs-lookup"><span data-stu-id="cd667-257">Webapp</span></span>

* <span data-ttu-id="cd667-258">Исправление. az webapp log deployment show: возврат журналов развертывания вместо метаданных журнала.</span><span class="sxs-lookup"><span data-stu-id="cd667-258">Bugfix: az webapp log deployment show - return deployment logs instead of log metadata</span></span>
* <span data-ttu-id="cd667-259">Исправление. az webapp vnet-integration add: исправлена обработка ошибок при неправильном имени виртуальной сети и включена поддержка идентификатора ресурса виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="cd667-259">Bugfix: az webapp vnet-integration add - fix error handling if bad vnet name, support vnet resource ID</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="cd667-260">23 июня 2020 года</span><span class="sxs-lookup"><span data-stu-id="cd667-260">June 23, 2020</span></span>

<span data-ttu-id="cd667-261">Версия 2.8.0</span><span class="sxs-lookup"><span data-stu-id="cd667-261">Version 2.8.0</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-262">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-262">ACR</span></span>

* <span data-ttu-id="cd667-263">Добавлена поддержка отключения конечных точек региона и отключения маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="cd667-263">Add support for region endpoint disable / routing disable</span></span>
* <span data-ttu-id="cd667-264">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.]  `az acr login --expose-token` не принимает имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="cd667-264">[BREAKING CHANGE] `az acr login --expose-token` does not accept username and password</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-265">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-265">ACS</span></span>

* <span data-ttu-id="cd667-266">Удален частный кластер и API 2019-10-27-preview.</span><span class="sxs-lookup"><span data-stu-id="cd667-266">Remove private cluster and 2019-10-27-preview API</span></span>

### <a name="aks"></a><span data-ttu-id="cd667-267">AKS</span><span class="sxs-lookup"><span data-stu-id="cd667-267">AKS</span></span>

* <span data-ttu-id="cd667-268">Включена поддержка параметра --yes для команды az aks upgrade.</span><span class="sxs-lookup"><span data-stu-id="cd667-268">Support --yes for az aks upgrade</span></span>
* <span data-ttu-id="cd667-269">Отменено изменение SKU виртуальной машины по умолчанию на Standard_D2s_v3 (№ 13541).</span><span class="sxs-lookup"><span data-stu-id="cd667-269">Revert "change default vm sku to Standard_D2s_v3 (#13541)"</span></span>
* <span data-ttu-id="cd667-270">Добавлена команда az aks update --uptime-sla.</span><span class="sxs-lookup"><span data-stu-id="cd667-270">Add "az aks update --uptime-sla"</span></span>
* <span data-ttu-id="cd667-271">Исправлена опечатка в команде az aks update.</span><span class="sxs-lookup"><span data-stu-id="cd667-271">Fix typo in az aks update command</span></span>
* <span data-ttu-id="cd667-272">Включена поддержка пула агентов узла 0 и блокировка ручного масштабирования для пула с поддержкой CAS.</span><span class="sxs-lookup"><span data-stu-id="cd667-272">Change to support 0 node agent pool and block manual scale for CAS enabled pool</span></span>
* <span data-ttu-id="cd667-273">Исправлена опечатка в VirtualMachineScaleSets и обновлены ссылки на версии Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="cd667-273">Fix typo on VirtualMachineScaleSets and update references to Kubernetes versions</span></span>

### <a name="ams"></a><span data-ttu-id="cd667-274">AMS</span><span class="sxs-lookup"><span data-stu-id="cd667-274">AMS</span></span>

* <span data-ttu-id="cd667-275">Изменен текст справки по параметру --expires.</span><span class="sxs-lookup"><span data-stu-id="cd667-275">CHANGE help text for "--expiry" parameter.</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-276">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-276">AppService</span></span>

* <span data-ttu-id="cd667-277">`az webapp log deployment show`: включено отображение журнала последнего развертывания или журналов конкретного развертывания, если указан идентификатор развертывания.</span><span class="sxs-lookup"><span data-stu-id="cd667-277">`az webapp log deployment show`: Show the latest deployment log, or the deployment logs of a specific deployment if deployment-id is specified</span></span>
* <span data-ttu-id="cd667-278">`az webapp log deployment list`: список доступных журналов развертывания.</span><span class="sxs-lookup"><span data-stu-id="cd667-278">`az webapp log deployment list`: List of deployment logs available</span></span>
* <span data-ttu-id="cd667-279">Исправление: ошибка поверхности при указании недопустимого имени веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="cd667-279">Fix: Surface error when invalid webapp name provided</span></span>
* <span data-ttu-id="cd667-280">Исправлена ошибка № 13261, и-за которой az webapp list-runtimes использует статический список до появления новых доступных API стеков.</span><span class="sxs-lookup"><span data-stu-id="cd667-280">Fix #13261 az webapp list-runtimes use static list until new Available Stacks API is available</span></span>
* <span data-ttu-id="cd667-281">`az appservice ase create`: исправлена ошибка создания № 13361.</span><span class="sxs-lookup"><span data-stu-id="cd667-281">`az appservice ase create`: Fix create issue #13361</span></span>
* <span data-ttu-id="cd667-282">`az appservice ase list-addresses`: исправлена ошибка изменения SDK № 13140.</span><span class="sxs-lookup"><span data-stu-id="cd667-282">`az appservice ase list-addresses`: Fix change of SDK #13140.</span></span>
* <span data-ttu-id="cd667-283">Исправлена ошибка создания слота или веб-приложения для контейнеров Windows.</span><span class="sxs-lookup"><span data-stu-id="cd667-283">Fix webapp/slot creation for Windows Containers</span></span>
* <span data-ttu-id="cd667-284">`az webapp auth update`: добавлен необязательный параметр для обновления версии среды выполнения.</span><span class="sxs-lookup"><span data-stu-id="cd667-284">`az webapp auth update`: Add optional parameter to update runtime-version</span></span>
* <span data-ttu-id="cd667-285">Включена поддержка перечисления, удаления, утверждения и отклонения подключения к частной конечной точке для веб-приложения в интерфейсе командной строки.</span><span class="sxs-lookup"><span data-stu-id="cd667-285">Support list, delete, approve and reject private endpoint connection for webapp in CLI</span></span>
* <span data-ttu-id="cd667-286">Исправлена ошибка № 13888: включена поддержка команд get, list, create для статических веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="cd667-286">Fix #13888 : Add support for Static WebApps: get, list, create commands</span></span>
* <span data-ttu-id="cd667-287">Улучшены сообщения об ошибках для подключения туннеля SSH.</span><span class="sxs-lookup"><span data-stu-id="cd667-287">Improved error messages for SSH Tunnel Connection</span></span>

### <a name="arm"></a><span data-ttu-id="cd667-288">ARM</span><span class="sxs-lookup"><span data-stu-id="cd667-288">ARM</span></span>

* <span data-ttu-id="cd667-289">`az tag`: добавлены примеры для параметра -h.</span><span class="sxs-lookup"><span data-stu-id="cd667-289">`az tag`: Add examples for -h</span></span>
* <span data-ttu-id="cd667-290">`az deployment group/sub what-if`: добавлен параметр --exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="cd667-290">`az deployment group/sub what-if`: Add --exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="cd667-291">`az deployment group/sub/mg/tenant create`: добавлен параметр --what-if-exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="cd667-291">`az deployment group/sub/mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="cd667-292">`az deployment group/sub/mg/tenant validate`: улучшен формат отображения сообщений об ошибках.</span><span class="sxs-lookup"><span data-stu-id="cd667-292">`az deployment group/sub/mg/tenant validate`: Show error messages in a better format.</span></span>
* <span data-ttu-id="cd667-293">`az group export`: добавлены новые параметры `--skip-resource-name-params` и `--skip-all-params` для включения поддержки параметризации с целью пропуска.</span><span class="sxs-lookup"><span data-stu-id="cd667-293">`az group export`: Add new parameters `--skip-resource-name-params` and `--skip-all-params` to support skip parameterization</span></span>
* <span data-ttu-id="cd667-294">Добавлена команда az feature unregister api.</span><span class="sxs-lookup"><span data-stu-id="cd667-294">Add az feature unregister api</span></span>

### <a name="aro"></a><span data-ttu-id="cd667-295">ARO</span><span class="sxs-lookup"><span data-stu-id="cd667-295">ARO</span></span>

* <span data-ttu-id="cd667-296">Добавлены атрибуты Public и Private в параметры для получения справки по видимости входящего трафика или сервера API.</span><span class="sxs-lookup"><span data-stu-id="cd667-296">Add Public, Private to params for help with ingress/apiserver visibility</span></span>

### <a name="batch"></a><span data-ttu-id="cd667-297">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-297">Batch</span></span>

* <span data-ttu-id="cd667-298">`az batch account create`: добавлен новый параметр `--public-network-access`.</span><span class="sxs-lookup"><span data-stu-id="cd667-298">`az batch account create`: Add new parameter `--public-network-access`</span></span>
* <span data-ttu-id="cd667-299">`az batch account create`: добавлен новый параметр `--identity-type`.</span><span class="sxs-lookup"><span data-stu-id="cd667-299">`az batch account create`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="cd667-300">`az batch account set`: добавлен новый параметр `--identity-type`.</span><span class="sxs-lookup"><span data-stu-id="cd667-300">`az batch account set`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="cd667-301">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az batch pool create. При создании пула с помощью пользовательского образа свойство --image теперь может ссылаться только на образ Общей коллекции образов.</span><span class="sxs-lookup"><span data-stu-id="cd667-301">[BREAKING CHANGE] az batch pool create: When creating a pool using a custom image, the --image property of can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="cd667-302">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az batch pool create. При создании пула с параметром --json-file и указании networkConfiguration свойство publicIPs было перемещено в новое свойство publicIPAddressConfiguration.</span><span class="sxs-lookup"><span data-stu-id="cd667-302">[BREAKING CHANGE] az batch pool create: When creating a pool with --json-file option and specifying a networkConfiguration, the publicIPs property has moved in to a new property publicIPAddressConfiguration.</span></span> <span data-ttu-id="cd667-303">Это новое свойство также поддерживает новое свойство ipAddressProvisioningType, которое определяет, как пул должен выделять IP-адреса, и свойство publicIPs, которое позволяет настроить список ресурсов PublicIP для использования, когда для ipAddressProvisioningType указано значение UserManaged.</span><span class="sxs-lookup"><span data-stu-id="cd667-303">This new property also supports a new ipAddressProvisioningType property which specifies how the pool should allocate IP's and a publicIPs property which allows for configuration of a list of PublicIP resources to use in the case ipAddressProvisioningType is set to UserManaged</span></span>
* <span data-ttu-id="cd667-304">`az network private-link-resource`: включена поддержка ресурса Microsoft.Batch batchAccount.</span><span class="sxs-lookup"><span data-stu-id="cd667-304">`az network private-link-resource`: Add support for the Microsoft.Batch batchAccount resource</span></span>
* <span data-ttu-id="cd667-305">`az network private-endpoint-connection`: включена поддержка ресурса Microsoft.Batch batchAccount.</span><span class="sxs-lookup"><span data-stu-id="cd667-305">`az network private-endpoint-connection`: Add support for the Microsoft.Batch batchAccount resource</span></span>

### <a name="cdn"></a><span data-ttu-id="cd667-306">CDN</span><span class="sxs-lookup"><span data-stu-id="cd667-306">CDN</span></span>

* <span data-ttu-id="cd667-307">`az cdn custom-domain enable-https`: включена поддержка BYOC.</span><span class="sxs-lookup"><span data-stu-id="cd667-307">`az cdn custom-domain enable-https`: Add BYOC support.</span></span>
* <span data-ttu-id="cd667-308">`az cdn custom-domain enable-https`: исправлена ошибка включения пользовательского HTTPS с использованием управляемых CDN сертификатов для SKU Standard_Verizon и Standard_Microsoft.</span><span class="sxs-lookup"><span data-stu-id="cd667-308">`az cdn custom-domain enable-https`: Fix enabling custom HTTPS with CDN managed certificates for Standard_Verizon and Standard_Microsoft SKUs.</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="cd667-309">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="cd667-309">Cognitive Services</span></span>

* <span data-ttu-id="cd667-310">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.]  `az cognitiveservices account` теперь имеет единую структуру для всех команд.</span><span class="sxs-lookup"><span data-stu-id="cd667-310">[BREAKING CHANGE] `az cognitiveservices account` now have a unified structure for all commands.</span></span>
* <span data-ttu-id="cd667-311">`az cognitiveservices account identity`: добавлена возможность управления удостоверениями для Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="cd667-311">`az cognitiveservices account identity`: Add identity management for Cognitive Services.</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-312">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="cd667-312">Compute</span></span>

* <span data-ttu-id="cd667-313">`az image builder`: обновлена версия API до 2020-02-14.</span><span class="sxs-lookup"><span data-stu-id="cd667-313">`az image builder`: Upgrade API version to 2020-02-14</span></span>
* <span data-ttu-id="cd667-314">`az image builder create`: добавлен параметр `--identity` для включения поддержки конфигурации удостоверений.</span><span class="sxs-lookup"><span data-stu-id="cd667-314">`az image builder create`: Add `--identity` to support identity configuration</span></span>
* <span data-ttu-id="cd667-315">`az image builder customizer add`: включена поддержка настройщика Центра обновления Windows.</span><span class="sxs-lookup"><span data-stu-id="cd667-315">`az image builder customizer add`: Support Windows update customizer</span></span>
* <span data-ttu-id="cd667-316">Новая команда `az image builder cancel`.</span><span class="sxs-lookup"><span data-stu-id="cd667-316">New command `az image builder cancel`</span></span>
* <span data-ttu-id="cd667-317">Включено отображение предупреждения, когда пользователь развертывает VMSS, прикрепленные к конкретной версии образа, а не к последней.</span><span class="sxs-lookup"><span data-stu-id="cd667-317">Show a warning when a user deploys a VMSS pinned to a specific image version rather than latest</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="cd667-318">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-318">Cosmos DB</span></span>

* <span data-ttu-id="cd667-319">`az cosmosdb`: добавлена команда exists в базу данных и группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="cd667-319">`az cosmosdb`: Add exists command to database and container groups</span></span>
* <span data-ttu-id="cd667-320">Разрешено создание фиксированных коллекций.</span><span class="sxs-lookup"><span data-stu-id="cd667-320">Allow creating fixed collections</span></span>

### <a name="eventhub"></a><span data-ttu-id="cd667-321">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="cd667-321">EventHub</span></span>

* <span data-ttu-id="cd667-322">`az eventhubs namespace create` : добавлены параметры управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="cd667-322">`az eventhubs namespace create` : Add managed identity parameters</span></span>

### <a name="extension"></a><span data-ttu-id="cd667-323">Расширение</span><span class="sxs-lookup"><span data-stu-id="cd667-323">Extension</span></span>

* <span data-ttu-id="cd667-324">Добавлен параметр --version для включения поддержки установки из конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="cd667-324">Add --version to support to install from a specific version</span></span>
* <span data-ttu-id="cd667-325">Включены расширения CLI для включения пакетов в пространство имен Azure.</span><span class="sxs-lookup"><span data-stu-id="cd667-325">Enable CLI extensions to include packages in the 'azure' namespace</span></span>

### <a name="iot-hub"></a><span data-ttu-id="cd667-326">Центр Интернета вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-326">Iot Hub</span></span>

* <span data-ttu-id="cd667-327">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az iot hub job: удалены устаревшие команды заданий.</span><span class="sxs-lookup"><span data-stu-id="cd667-327">[BREAKING CHANGE] az iot hub job: Remove deprecated job commands</span></span>

### <a name="keyvault"></a><span data-ttu-id="cd667-328">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="cd667-328">KeyVault</span></span>

* <span data-ttu-id="cd667-329">`az keyvault key import`: включена поддержка импорта из строк с помощью двух новых параметров.</span><span class="sxs-lookup"><span data-stu-id="cd667-329">`az keyvault key import`: Supports importing from strings via two new parameters.</span></span>
* <span data-ttu-id="cd667-330">Включена поддержка шифрования и расшифровки строк или байтов с помощью хранимых ключей.</span><span class="sxs-lookup"><span data-stu-id="cd667-330">Support string/bytes encryption and decryption with stored keys</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-331">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-331">Monitor</span></span>

* <span data-ttu-id="cd667-332">Включена поддержка возможности не дожидаться создания кластера.</span><span class="sxs-lookup"><span data-stu-id="cd667-332">Support no wait for cluster creation</span></span>
* <span data-ttu-id="cd667-333">`az monitor log-analytics workspace saved-search`: включена поддержка новых команд для сохраненного поиска.</span><span class="sxs-lookup"><span data-stu-id="cd667-333">`az monitor log-analytics workspace saved-search`: Support new commands for saved search</span></span>

### <a name="network"></a><span data-ttu-id="cd667-334">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-334">Network</span></span>

* <span data-ttu-id="cd667-335">`az network application-gateway address-pool update`: уточнено справочное сообщение и добавлены примеры.</span><span class="sxs-lookup"><span data-stu-id="cd667-335">`az network application-gateway address-pool update`: Refine help message and add examples.</span></span>
* <span data-ttu-id="cd667-336">`az network vnet create`: включена поддержка аргумента --nsg.</span><span class="sxs-lookup"><span data-stu-id="cd667-336">`az network vnet create`: Support --nsg argument</span></span>
* <span data-ttu-id="cd667-337">`az network lb address-pool`: включена поддержка создания внутреннего пула балансировки нагрузки с внутренним адресом.</span><span class="sxs-lookup"><span data-stu-id="cd667-337">`az network lb address-pool`: Support create lb backend pool with backend address.</span></span>
* <span data-ttu-id="cd667-338">`az network application-gateway address-pool`: исправлена ошибка с аргументом --add.</span><span class="sxs-lookup"><span data-stu-id="cd667-338">`az network application-gateway address-pool`: Fix for --add argument</span></span>

### <a name="rbac"></a><span data-ttu-id="cd667-339">RBAC</span><span class="sxs-lookup"><span data-stu-id="cd667-339">RBAC</span></span>

* <span data-ttu-id="cd667-340">`az ad sp create-for-rabc`: включена поддержка имен с пробелом, косой чертой и обратной косой чертой.</span><span class="sxs-lookup"><span data-stu-id="cd667-340">`az ad sp create-for-rabc`: Support name with space, slash and back slash</span></span>
* <span data-ttu-id="cd667-341">`az ad sp create-for-rbac`: уточнено сообщение об ошибке при указании недопустимой области пользователем.</span><span class="sxs-lookup"><span data-stu-id="cd667-341">`az ad sp create-for-rbac`: Refine error message when user specify an invalid scope</span></span>

### <a name="security"></a><span data-ttu-id="cd667-342">Безопасность</span><span class="sxs-lookup"><span data-stu-id="cd667-342">Security</span></span>

* <span data-ttu-id="cd667-343">Добавлены команды оценки безопасности.</span><span class="sxs-lookup"><span data-stu-id="cd667-343">Add security assessment commands</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-344">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-344">SQL</span></span>

* <span data-ttu-id="cd667-345">`az sql db ltr-policy/ltr-backup`: обновление и отображение политик долгосрочного хранения, отображение и удаление долгосрочных резервных копий, восстановление долгосрочных резервных копий.</span><span class="sxs-lookup"><span data-stu-id="cd667-345">`az sql db ltr-policy/ltr-backup`: update/show long term retention policy, show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-346">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-346">Storage</span></span>

* <span data-ttu-id="cd667-347">Исправлена проблема с проверкой подлинности для включения поддержки получения токена для параметра --subscription.</span><span class="sxs-lookup"><span data-stu-id="cd667-347">Fix authentication issue to support get token for --subscription</span></span>
* <span data-ttu-id="cd667-348">`az storage remove`: исправлена ошибка № 13459 с возникновением исключения при сбое операции.</span><span class="sxs-lookup"><span data-stu-id="cd667-348">`az storage remove`: Fix issue #13459 to raise exception for operation failure</span></span>
* <span data-ttu-id="cd667-349">Устранены ошибки № 13012, 13632 и 13657 для удаления неиспользуемых аргументов для команд, связанных с generate-sas.</span><span class="sxs-lookup"><span data-stu-id="cd667-349">Fix issues #13012, #13632 and #13657 to remove unused arguments for generate-sas related commands</span></span>
* <span data-ttu-id="cd667-350">`az storage logging update`: добавлена проверка версии ведения журнала.</span><span class="sxs-lookup"><span data-stu-id="cd667-350">`az storage logging update`: Add check for logging version</span></span>
* <span data-ttu-id="cd667-351">`az storage blob show`: добавлены дополнительные свойства для большого двоичного объекта с использованием пакета SDK для Track 2.</span><span class="sxs-lookup"><span data-stu-id="cd667-351">`az storage blob show`: Add more properties for blob with track 2 SDK</span></span>
* <span data-ttu-id="cd667-352">Исправление № 13708: уточнены предупреждающие сообщения об учетных данных.</span><span class="sxs-lookup"><span data-stu-id="cd667-352">Fix #13708: Refine warning message for credential</span></span>
* <span data-ttu-id="cd667-353">`az storage share-rm create/update`: включена поддержка протокола NFS и корневого сжатия.</span><span class="sxs-lookup"><span data-stu-id="cd667-353">`az storage share-rm create/update`: Add NFS protocol and root squash support</span></span>
* <span data-ttu-id="cd667-354">`az storage account create`: включена поддержка двойного шифрования.</span><span class="sxs-lookup"><span data-stu-id="cd667-354">`az storage account create`: Add support for double encryption</span></span>
* <span data-ttu-id="cd667-355">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.]  `az storage blob/container/file/share/table/queue generate-sas`: параметры --expiry и --permissions являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="cd667-355">[BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: make --expiry and --permissions required</span></span>
* <span data-ttu-id="cd667-356">`az storage blob set-tier`: миграция на Track 2 для включения поддержки настройки приоритета восстановления.</span><span class="sxs-lookup"><span data-stu-id="cd667-356">`az storage blob set-tier`: Migrate to Track 2 to support setting rehydrate priority</span></span>

## <a name="june-02-2020"></a><span data-ttu-id="cd667-357">02 июня 2020 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-357">June 02, 2020</span></span>

<span data-ttu-id="cd667-358">Версия 2.7.0</span><span class="sxs-lookup"><span data-stu-id="cd667-358">Version 2.7.0</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-359">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-359">ACR</span></span>

* <span data-ttu-id="cd667-360">Исправлена опечатка в сообщении об ошибке, возникающем при создании токена.</span><span class="sxs-lookup"><span data-stu-id="cd667-360">Fix a typo in an error message of token creation</span></span>

### <a name="aks"></a><span data-ttu-id="cd667-361">AKS</span><span class="sxs-lookup"><span data-stu-id="cd667-361">AKS</span></span>

* <span data-ttu-id="cd667-362">Номер SKU виртуальной машины по умолчанию изменен на Standard_D2s_v3.</span><span class="sxs-lookup"><span data-stu-id="cd667-362">Change default vm sku to Standard_D2s_v3</span></span>
* <span data-ttu-id="cd667-363">Исправлен процесс создания назначения ролей для кластера MSI и настраиваемой подсети.</span><span class="sxs-lookup"><span data-stu-id="cd667-363">Fix creating role assignment for MSI clsuter plus custom subnet</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-364">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-364">AppService</span></span>

* <span data-ttu-id="cd667-365">Исправлена ошибка 12739, из-за которой команда az appservice list-locations возвращает недопустимые расположения.</span><span class="sxs-lookup"><span data-stu-id="cd667-365">Fix #12739 az appservice list-locations returns some invalid locations</span></span>

### <a name="arm"></a><span data-ttu-id="cd667-366">ARM</span><span class="sxs-lookup"><span data-stu-id="cd667-366">ARM</span></span>

* <span data-ttu-id="cd667-367">`az deployment`: Исправлена ошибка 13159, из-за которой отображается неправильное сообщение JSON после удаления комментариев и сжатия.</span><span class="sxs-lookup"><span data-stu-id="cd667-367">`az deployment`: Fix issue #13159 of incorrect message of JSON after removing comments and compressing</span></span>
* <span data-ttu-id="cd667-368">`az resource tag`: Исправлена ошибка 13255, связанная с добавлением тегов к ресурсам с помощью типа ресурса `Microsoft.ContainerRegistry/registries/webhooks`.</span><span class="sxs-lookup"><span data-stu-id="cd667-368">`az resource tag`: Fix issue #13255 of tagging resources with resource type `Microsoft.ContainerRegistry/registries/webhooks`</span></span>
* <span data-ttu-id="cd667-369">Улучшены примеры для модуля ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd667-369">Improve the examples for the resource module</span></span>

### <a name="aro"></a><span data-ttu-id="cd667-370">ARO</span><span class="sxs-lookup"><span data-stu-id="cd667-370">ARO</span></span>

* <span data-ttu-id="cd667-371">Исправлена ошибка CLIError, связанная с неправильным флагом для --worker-vm-disk-size-gb.</span><span class="sxs-lookup"><span data-stu-id="cd667-371">Change CLIError to correct flag for --worker-vm-disk-size-gb</span></span>

### <a name="eventhub"></a><span data-ttu-id="cd667-372">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="cd667-372">EventHub</span></span>

* <span data-ttu-id="cd667-373">Исправлена ошибка 12406, из-за которой аргумент --capture-interval не обновляет intervalInSeconds.</span><span class="sxs-lookup"><span data-stu-id="cd667-373">Fix for issue #12406 Argument --capture-interval does not update the "intervalInSeconds"</span></span>

### <a name="hdinsight"></a><span data-ttu-id="cd667-374">HDInsight</span><span class="sxs-lookup"><span data-stu-id="cd667-374">HDInsight</span></span>

* <span data-ttu-id="cd667-375">Объект get_json_object изменен на shell_safe_json_parse.</span><span class="sxs-lookup"><span data-stu-id="cd667-375">Change get_json_object to shell_safe_json_parse</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-376">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-376">Monitor</span></span>

* <span data-ttu-id="cd667-377">`az monitor metrics alert`: уточнены нескольких справочных сообщений.</span><span class="sxs-lookup"><span data-stu-id="cd667-377">`az monitor metrics alert`: refine several help messages</span></span>
* <span data-ttu-id="cd667-378">`az monitor diagnostic-settings create`: включена поддержка аргумента --export-to-resource-specific.</span><span class="sxs-lookup"><span data-stu-id="cd667-378">`az monitor diagnostic-settings create`: support --export-to-resource-specific argument</span></span>
* <span data-ttu-id="cd667-379">Включена поддержка восстановления рабочей области LA.</span><span class="sxs-lookup"><span data-stu-id="cd667-379">Support LA workspace recover</span></span>

### <a name="network"></a><span data-ttu-id="cd667-380">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-380">Network</span></span>

* <span data-ttu-id="cd667-381">`az network dns zone`: включена поддержка символа -.</span><span class="sxs-lookup"><span data-stu-id="cd667-381">`az network dns zone`: support - character</span></span>
* <span data-ttu-id="cd667-382">`az network vpn-connection ipsec-policy`: изменены значения --sa-lifetime и --sa-max-size на более крупные в примере.</span><span class="sxs-lookup"><span data-stu-id="cd667-382">`az network vpn-connection ipsec-policy`: change the --sa-lifetime and --sa-max-size to larger values in example</span></span>
* <span data-ttu-id="cd667-383">Обновление сети до версии 2020-04-01</span><span class="sxs-lookup"><span data-stu-id="cd667-383">Bump network to 2020-04-01</span></span>
* <span data-ttu-id="cd667-384">`az network private-endpoint-connection`: включена поддержка Сетки событий.</span><span class="sxs-lookup"><span data-stu-id="cd667-384">`az network private-endpoint-connection`: support event grid</span></span>
* <span data-ttu-id="cd667-385">`az network express-route list-route-tables`: исправлена ошибка, из-за которой нельзя было перечислять маршруты в виде таблицы.</span><span class="sxs-lookup"><span data-stu-id="cd667-385">`az network express-route list-route-tables`: fix bug that cannot list routes as table</span></span>

### <a name="packaging"></a><span data-ttu-id="cd667-386">Упаковка</span><span class="sxs-lookup"><span data-stu-id="cd667-386">Packaging</span></span>

* <span data-ttu-id="cd667-387">Добавлен пакет Ubuntu Focal.</span><span class="sxs-lookup"><span data-stu-id="cd667-387">Add Ubuntu Focal Package</span></span>

### <a name="rbac"></a><span data-ttu-id="cd667-388">RBAC</span><span class="sxs-lookup"><span data-stu-id="cd667-388">RBAC</span></span>

* <span data-ttu-id="cd667-389">`az ad sp credential reset`: изменен процесс создания учетных данных, чтобы не использовать проблемные специальные символы.</span><span class="sxs-lookup"><span data-stu-id="cd667-389">`az ad sp credential reset`: modify credential generation to avoid troublesome special characters</span></span>

### <a name="redis"></a><span data-ttu-id="cd667-390">Redis</span><span class="sxs-lookup"><span data-stu-id="cd667-390">Redis</span></span>

* <span data-ttu-id="cd667-391">Исправление 13529: изменена документация по параметру enable_non_ssl_port.</span><span class="sxs-lookup"><span data-stu-id="cd667-391">Fix #13529: Change documentation of parameter enable_non_ssl_port</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-392">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-392">Storage</span></span>

* <span data-ttu-id="cd667-393">`az storage copy`: Добавлен параметр `--follow-symlinks` для включения поддержки символических ссылок.</span><span class="sxs-lookup"><span data-stu-id="cd667-393">`az storage copy`: Add parameter `--follow-symlinks` to support symlinks</span></span>
* <span data-ttu-id="cd667-394">Включен локальный контекст для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="cd667-394">Enable local context for storage account</span></span>
* <span data-ttu-id="cd667-395">`az storage logging`: Исправление 11969: уточнено сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="cd667-395">`az storage logging`: Fix issue #11969 to refine error message</span></span>

## <a name="may-19-2020"></a><span data-ttu-id="cd667-396">19 мая 2020 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-396">May 19, 2020</span></span>

<span data-ttu-id="cd667-397">Версия 2.6.0</span><span class="sxs-lookup"><span data-stu-id="cd667-397">Version 2.6.0</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-398">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-398">ACR</span></span>

* <span data-ttu-id="cd667-399">Добавлено время ожидания по умолчанию (5 минут) для любых запросов ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-399">Add default timeout of 5 minutes for any requests to ACR</span></span>
* <span data-ttu-id="cd667-400">Добавлена поддержка отключения доступа к общедоступной сети</span><span class="sxs-lookup"><span data-stu-id="cd667-400">Support disable public network access</span></span>
* <span data-ttu-id="cd667-401">`az acr token create`: предоставляет аргумент --days</span><span class="sxs-lookup"><span data-stu-id="cd667-401">`az acr token create`: expose --days argument</span></span>
* <span data-ttu-id="cd667-402">`az acr import`: принимает значения аргумента --source, которые содержат имя для входа в имени сервера, добавленное путем исправления на стороне клиента</span><span class="sxs-lookup"><span data-stu-id="cd667-402">`az acr import`: accept --source argument values which contain login in server name through client end correction</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-403">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-403">ACS</span></span>

* <span data-ttu-id="cd667-404">Исправление ошибки: удаление больше не существующих полей</span><span class="sxs-lookup"><span data-stu-id="cd667-404">Bug fix: remove fields cleanup for fields that no longer exist</span></span>

### <a name="aks"></a><span data-ttu-id="cd667-405">AKS</span><span class="sxs-lookup"><span data-stu-id="cd667-405">AKS</span></span>

* <span data-ttu-id="cd667-406">Обновлен контекст справки команды uptime-sla</span><span class="sxs-lookup"><span data-stu-id="cd667-406">Update uptime-sla command help context</span></span>
* <span data-ttu-id="cd667-407">Удалена проверка диапазона для обновления числа минут для автомасштабирования</span><span class="sxs-lookup"><span data-stu-id="cd667-407">Remove range check for updating min count for autoscaler</span></span>
* <span data-ttu-id="cd667-408">Исправлена ошибка, из-за которой CLI не выдает ошибку, когда пользователь указывает только пароль Windows</span><span class="sxs-lookup"><span data-stu-id="cd667-408">Fix that cli doe not fail when user only specifies Windows password</span></span>

### <a name="ams"></a><span data-ttu-id="cd667-409">AMS</span><span class="sxs-lookup"><span data-stu-id="cd667-409">AMS</span></span>

* <span data-ttu-id="cd667-410">`az ams transform create`: добавлена возможность создания преобразования с предустановкой FaceDetector</span><span class="sxs-lookup"><span data-stu-id="cd667-410">`az ams transform create`: Add ability to create a transform with a FaceDetector preset</span></span>
* <span data-ttu-id="cd667-411">`az ams content-key-policy create` : добавлена возможность создания политики ключа содержимого FairPlay с конфигурацией автономной аренды</span><span class="sxs-lookup"><span data-stu-id="cd667-411">`az ams content-key-policy create` : Add ability to create a FairPlay content key policy with an offline rental configuration</span></span>

### <a name="appconfig"></a><span data-ttu-id="cd667-412">AppConfig</span><span class="sxs-lookup"><span data-stu-id="cd667-412">AppConfig</span></span>

* <span data-ttu-id="cd667-413">Исправлена ошибка при отображении значений ключей с полями</span><span class="sxs-lookup"><span data-stu-id="cd667-413">Bug fix for list key values with fields</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-414">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-414">AppService</span></span>

* <span data-ttu-id="cd667-415">`az functionapp create`: параметр AzureWebJobsDashboard будет задан только в случае отключения AppInsights</span><span class="sxs-lookup"><span data-stu-id="cd667-415">`az functionapp create`: AzureWebJobsDashboard will only be set if AppInsights is disabled</span></span>
* <span data-ttu-id="cd667-416">Исправление № 10664 — интеграция виртуальной сети — проблема проверки расположения и исправление № 13257 — сбой веб-приложения az в случае необходимости создания группы ресурсов</span><span class="sxs-lookup"><span data-stu-id="cd667-416">Fix #10664- VNet Integration - Location Check Issue & fix #13257- az webapp up failing when RG needs to be created</span></span>
* <span data-ttu-id="cd667-417">`az webapp|functionapp config ssl import`: добавлен поиск хранилища ключей в группах ресурсов в подписке и улучшены справка и примеры.</span><span class="sxs-lookup"><span data-stu-id="cd667-417">`az webapp|functionapp config ssl import`: Lookup key vault across resources groups in subscription and improve help and examples.</span></span>
* <span data-ttu-id="cd667-418">Подключен локальный контекст для службы приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-418">Onboard local context for app service</span></span>

### <a name="arm"></a><span data-ttu-id="cd667-419">ARM</span><span class="sxs-lookup"><span data-stu-id="cd667-419">ARM</span></span>

* <span data-ttu-id="cd667-420">`az deployment`: устранена проблема, из-за которой templateLink не возвращается при развертывании или проверке template-uri</span><span class="sxs-lookup"><span data-stu-id="cd667-420">`az deployment`: Fix the problem that the templateLink will not be returned when deploying or validating template-uri</span></span>
* <span data-ttu-id="cd667-421">`az deployment`: устранена проблема, из-за которой развертывание или проверка не поддерживает специально закодированный символ</span><span class="sxs-lookup"><span data-stu-id="cd667-421">`az deployment`: Fix the problem that deployment/validate does not support specially encoded character</span></span>
* <span data-ttu-id="cd667-422">`az deployment sub/group what-if`: исправлены выравнивание массива и обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="cd667-422">`az deployment sub/group what-if`: Fix array alignment and error handling</span></span>
* <span data-ttu-id="cd667-423">`az deployment operation`: изменение сведений об устаревании</span><span class="sxs-lookup"><span data-stu-id="cd667-423">`az deployment operation`: Modify the deprecate information</span></span>

### <a name="aro"></a><span data-ttu-id="cd667-424">ARO</span><span class="sxs-lookup"><span data-stu-id="cd667-424">ARO</span></span>

* <span data-ttu-id="cd667-425">Добавлены примеры в az aro create, list, list-credentials, show, delete</span><span class="sxs-lookup"><span data-stu-id="cd667-425">Add examples to az aro create, list, list-credentials, show, delete</span></span>
* <span data-ttu-id="cd667-426">Добавлена функция generate_random_id</span><span class="sxs-lookup"><span data-stu-id="cd667-426">Add generate_random_id function</span></span>

### <a name="backup"></a><span data-ttu-id="cd667-427">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="cd667-427">Backup</span></span>

* <span data-ttu-id="cd667-428">Разрешен параметр FriendlyName при включении защиты для команды AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="cd667-428">Allow FriendlyName in enable protection for AzureFileShare command</span></span>
* <span data-ttu-id="cd667-429">Исправлена restore-disks в IaasVM</span><span class="sxs-lookup"><span data-stu-id="cd667-429">Fix in IaasVM restore-disks Command</span></span>
* <span data-ttu-id="cd667-430">Добавлен тип BackupManagementType "MAB" в команду item list</span><span class="sxs-lookup"><span data-stu-id="cd667-430">Add "MAB" BackupManagementType to item list command</span></span>
* <span data-ttu-id="cd667-431">Добавлена поддержка повторного обновления политики для элементов с ошибками.</span><span class="sxs-lookup"><span data-stu-id="cd667-431">Add support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="cd667-432">Добавлена функция защиты от возобновления для виртуальной машины Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-432">Add Resume Protection functionality for Azure Virtual Machine</span></span>
* <span data-ttu-id="cd667-433">Добавлена поддержка возможности указывать группу ресурсов для хранения instantRP во время создания или изменения политики</span><span class="sxs-lookup"><span data-stu-id="cd667-433">Add support to specify ResourceGroup for storing instantRP during Create or Modify Policy</span></span>

### <a name="ci"></a><span data-ttu-id="cd667-434">CI</span><span class="sxs-lookup"><span data-stu-id="cd667-434">CI</span></span>

* <span data-ttu-id="cd667-435">Поддержка flake8 3.8.0</span><span class="sxs-lookup"><span data-stu-id="cd667-435">Support flake8 3.8.0</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-436">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="cd667-436">Compute</span></span>

* <span data-ttu-id="cd667-437">Новая команда az vm auto-shutdown</span><span class="sxs-lookup"><span data-stu-id="cd667-437">New command az vm auto-shutdown</span></span>
* <span data-ttu-id="cd667-438">`az vm list-skus`: обновлено поведение для параметра --zone — теперь он возвращает все номера SKU типов</span><span class="sxs-lookup"><span data-stu-id="cd667-438">`az vm list-skus`: Update --zone behavior, return all type skus now</span></span>

### <a name="core"></a><span data-ttu-id="cd667-439">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-439">Core</span></span>

* <span data-ttu-id="cd667-440">Обновлено состояние включения и выключения локального контекста на уровне глобального пользователя</span><span class="sxs-lookup"><span data-stu-id="cd667-440">Update local context on/off status to global user level</span></span>

### <a name="extension"></a><span data-ttu-id="cd667-441">Расширение</span><span class="sxs-lookup"><span data-stu-id="cd667-441">Extension</span></span>

* <span data-ttu-id="cd667-442">`az extension add`: добавлен параметр --system для включения установки расширений по системному пути</span><span class="sxs-lookup"><span data-stu-id="cd667-442">`az extension add`: Add --system to enable installing extensions in a system path</span></span>
* <span data-ttu-id="cd667-443">Реализована поддержка .egg-info для хранения метаданных расширения типа wheel</span><span class="sxs-lookup"><span data-stu-id="cd667-443">Support .egg-info to store wheel type extension metadata</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-444">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-444">IoT</span></span>

* <span data-ttu-id="cd667-445">`az iot`: теперь в сообщении для информирования о первом запуске модуля команд Интернета вещей используется точный и современный идентификатор `azure-iot`, который не считается нерекомендуемым.</span><span class="sxs-lookup"><span data-stu-id="cd667-445">`az iot`: Update the IoT command module first run extension awareness message to the accurate, non-deprecated modern Id `azure-iot`.</span></span>

### <a name="iot-hub"></a><span data-ttu-id="cd667-446">Центр Интернета вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-446">IoT Hub</span></span>

* <span data-ttu-id="cd667-447">Добавлена поддержка API 2020-03-01 и команд сетевой изоляции</span><span class="sxs-lookup"><span data-stu-id="cd667-447">Support for 2020-03-01 API and Network Isolation commands</span></span>

### <a name="netappfiles"></a><span data-ttu-id="cd667-448">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="cd667-448">NetAppFiles</span></span>

* <span data-ttu-id="cd667-449">`az volume create`: добавлен параметр snapshot-id для создания тома. Это позволит пользователям создавать тома из существующего моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="cd667-449">`az volume create`: Adds snapshot-id as a parameter to create volume this will allow users to create a volume from existing snapshot.</span></span>

### <a name="network"></a><span data-ttu-id="cd667-450">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-450">Network</span></span>

* <span data-ttu-id="cd667-451">Исправлена ошибка, из-за которой значение ttl изменялось непредвиденным образом для add-record для dns</span><span class="sxs-lookup"><span data-stu-id="cd667-451">Fix ttl value changed unintended for dns add-record</span></span>
* <span data-ttu-id="cd667-452">`az network public-ip create`: информирование клиентов о выпуске критического изменения</span><span class="sxs-lookup"><span data-stu-id="cd667-452">`az network public-ip create`: Inform customers of a coming breaking change</span></span>
* <span data-ttu-id="cd667-453">Поддержка универсальных команд для сценария Приватного канала</span><span class="sxs-lookup"><span data-stu-id="cd667-453">Support generic commands for private link scenario</span></span>
* <span data-ttu-id="cd667-454">`az network private-endpoint-connection`: поддержка типов mysql, postgre и mariadb</span><span class="sxs-lookup"><span data-stu-id="cd667-454">`az network private-endpoint-connection`: Support mysql, postgre and mariadb types</span></span>
* <span data-ttu-id="cd667-455">`az network private-endpoint-connection`: поддержка типов cosmosdb</span><span class="sxs-lookup"><span data-stu-id="cd667-455">`az network private-endpoint-connection`: Support cosmosdb types</span></span>
* <span data-ttu-id="cd667-456">`az network private-endpoint`: параметр --group-ids теперь является нерекомендуемым и перенаправляется на --group-id</span><span class="sxs-lookup"><span data-stu-id="cd667-456">`az network private-endpoint`: deprecate --group-ids and redirect to --group-id</span></span>

### <a name="output"></a><span data-ttu-id="cd667-457">Выходные данные</span><span class="sxs-lookup"><span data-stu-id="cd667-457">Output</span></span>

* <span data-ttu-id="cd667-458">Отображение обновленной инструкции для find, feedback и --help</span><span class="sxs-lookup"><span data-stu-id="cd667-458">Show update instruction in find, feedback and --help</span></span>

### <a name="packaging"></a><span data-ttu-id="cd667-459">Упаковка</span><span class="sxs-lookup"><span data-stu-id="cd667-459">Packaging</span></span>

* <span data-ttu-id="cd667-460">Создание пакетов MSI/Homebrew с зависимостями, разрешенным из requirements.txt</span><span class="sxs-lookup"><span data-stu-id="cd667-460">Build MSI/Homebrew packages with dependecies resolved from requirements.txt</span></span>

### <a name="rbac"></a><span data-ttu-id="cd667-461">RBAC</span><span class="sxs-lookup"><span data-stu-id="cd667-461">RBAC</span></span>

* <span data-ttu-id="cd667-462">`az ad sp credential reset`: устранена возможность создания слабых учетных данных</span><span class="sxs-lookup"><span data-stu-id="cd667-462">`az ad sp credential reset`: fix weak credential generation</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-463">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-463">Storage</span></span>

* <span data-ttu-id="cd667-464">`az storage account file-service-properties update/show`: добавлена поддержка свойств файлов для учетной записи хранения</span><span class="sxs-lookup"><span data-stu-id="cd667-464">`az storage account file-service-properties update/show`: Add File Properties Support for Storage Account</span></span>
* <span data-ttu-id="cd667-465">`az storage container create`: исправление № 13373 путем добавления проверяющего элемента управления для общего доступа</span><span class="sxs-lookup"><span data-stu-id="cd667-465">`az storage container create`: Fix #13373 by adding validator for public access</span></span>
* <span data-ttu-id="cd667-466">Добавлена поддержка track2 для ADLS 2-го поколения</span><span class="sxs-lookup"><span data-stu-id="cd667-466">Add ADLS Gen2 track2 support</span></span>
* <span data-ttu-id="cd667-467">`az storage blob sync`: Включена поддержка `--connection-string`.</span><span class="sxs-lookup"><span data-stu-id="cd667-467">`az storage blob sync`: Support `--connection-string`</span></span>
* <span data-ttu-id="cd667-468">`az storage blob sync`: исправлено неверное сообщение об ошибке, которое отображается, когда azcopy не удается найти расположение установки</span><span class="sxs-lookup"><span data-stu-id="cd667-468">`az storage blob sync`: Fix the incorrect error message when azcopy cannot find the installation location</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="cd667-469">30 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-469">April 30, 2020</span></span>

<span data-ttu-id="cd667-470">Версия 2.5.1</span><span class="sxs-lookup"><span data-stu-id="cd667-470">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-471">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-471">ACR</span></span>

* <span data-ttu-id="cd667-472">`az acr check-health`: исправлена ошибка DOCKER_PULL_ERROR в Windows.</span><span class="sxs-lookup"><span data-stu-id="cd667-472">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-473">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="cd667-473">Compute</span></span>

* <span data-ttu-id="cd667-474">`az vm list-ip-addresses`: Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="cd667-474">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="cd667-475">Исправлена ошибка создания виртуальной машины, которая возникает, если в профиле облака не задано значение endpoint_vm_image_alias_doc.</span><span class="sxs-lookup"><span data-stu-id="cd667-475">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="cd667-476">`az vmss create`: добавлен параметр --os-disk-size-gb.</span><span class="sxs-lookup"><span data-stu-id="cd667-476">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="cd667-477">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-477">Cosmos DB</span></span>

* <span data-ttu-id="cd667-478">`az cosmosdb create/update`: добавлена поддержка --enable-public-network.</span><span class="sxs-lookup"><span data-stu-id="cd667-478">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="cd667-479">Расширение</span><span class="sxs-lookup"><span data-stu-id="cd667-479">Extension</span></span>

* <span data-ttu-id="cd667-480">Исправлена загрузка неправильных метаданных для расширения типа колеса.</span><span class="sxs-lookup"><span data-stu-id="cd667-480">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="cd667-481">Упаковка</span><span class="sxs-lookup"><span data-stu-id="cd667-481">Packaging</span></span>

* <span data-ttu-id="cd667-482">Добавлен скрипт az для Git Bash/Cygwin в Windows.</span><span class="sxs-lookup"><span data-stu-id="cd667-482">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-483">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-483">SQL</span></span>

* <span data-ttu-id="cd667-484">`az sql instance-pool`: добавлена группа команд для пулов экземпляров.</span><span class="sxs-lookup"><span data-stu-id="cd667-484">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-485">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-485">Storage</span></span>

* <span data-ttu-id="cd667-486">Пакет azure-multiapi-storage обновлен до версии 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="cd667-486">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="cd667-487">Добавлена поддержка GZRS при создании и обновлении учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="cd667-487">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="cd667-488">`az storage account failover`: добавлена поддержка отработки отказа учетной записи хранения GRS или GZRS.</span><span class="sxs-lookup"><span data-stu-id="cd667-488">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="cd667-489">`az storage blob upload`: добавлен параметр --encryption-scope для указания сведений об области шифрования.</span><span class="sxs-lookup"><span data-stu-id="cd667-489">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="cd667-490">28 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-490">April 28, 2020</span></span>

<span data-ttu-id="cd667-491">Версия 2.5.0</span><span class="sxs-lookup"><span data-stu-id="cd667-491">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-492">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-492">ACS</span></span>

* <span data-ttu-id="cd667-493">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az openshift create: удален параметр --vnet-peer.</span><span class="sxs-lookup"><span data-stu-id="cd667-493">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="cd667-494">`az openshift create`: добавлены флаги для поддержки частного кластера.</span><span class="sxs-lookup"><span data-stu-id="cd667-494">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="cd667-495">`az openshift`: обновление до версии API `2019-10-27-preview`.</span><span class="sxs-lookup"><span data-stu-id="cd667-495">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="cd667-496">`az openshift`: добавлена команда `update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-496">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="cd667-497">AKS</span><span class="sxs-lookup"><span data-stu-id="cd667-497">AKS</span></span>

* <span data-ttu-id="cd667-498">`az aks create`: включена поддержка Windows.</span><span class="sxs-lookup"><span data-stu-id="cd667-498">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-499">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-499">AppService</span></span>

* <span data-ttu-id="cd667-500">`az webapp deployment source config-zip`: удалена функция перевода в спящий режим после выполнения request.get().</span><span class="sxs-lookup"><span data-stu-id="cd667-500">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="cd667-501">ARM</span><span class="sxs-lookup"><span data-stu-id="cd667-501">ARM</span></span>

* <span data-ttu-id="cd667-502">Добавлены команды What-If развертывания шаблона.</span><span class="sxs-lookup"><span data-stu-id="cd667-502">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="cd667-503">ARO</span><span class="sxs-lookup"><span data-stu-id="cd667-503">ARO</span></span>

* <span data-ttu-id="cd667-504">`az aro`: исправлены выходные данные таблицы.</span><span class="sxs-lookup"><span data-stu-id="cd667-504">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="cd667-505">CI</span><span class="sxs-lookup"><span data-stu-id="cd667-505">CI</span></span>

* <span data-ttu-id="cd667-506">Включена поддержка PyTest и прекращена поддержка Nose для автотестов.</span><span class="sxs-lookup"><span data-stu-id="cd667-506">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-507">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="cd667-507">Compute</span></span>

* <span data-ttu-id="cd667-508">`az vmss disk detach`: устранена проблема с NoneType для диска данных.</span><span class="sxs-lookup"><span data-stu-id="cd667-508">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="cd667-509">`az vm availability-set list`: включена поддержка отображения списка виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="cd667-509">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="cd667-510">`az vm list-skus`: исправлена проблема с отображением формата таблицы.</span><span class="sxs-lookup"><span data-stu-id="cd667-510">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="cd667-511">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="cd667-511">KeyVault</span></span>

* <span data-ttu-id="cd667-512">Добавлен новый параметр `--enable-rbac-authorization` для использования во время создания или обновления.</span><span class="sxs-lookup"><span data-stu-id="cd667-512">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-513">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-513">Monitor</span></span>

* <span data-ttu-id="cd667-514">Включена поддержка компонентов CMK в кластере LA.</span><span class="sxs-lookup"><span data-stu-id="cd667-514">Support LA cluster CMK features</span></span>
* <span data-ttu-id="cd667-515">`az monitor log-analytics workspace linked-storage`: включена поддержка функций BYOS.</span><span class="sxs-lookup"><span data-stu-id="cd667-515">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="cd667-516">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-516">Network</span></span>

* <span data-ttu-id="cd667-517">`az network security-partner`: включена поддержка поставщика партнера по безопасности.</span><span class="sxs-lookup"><span data-stu-id="cd667-517">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="cd667-518">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="cd667-518">Privatedns</span></span>

* <span data-ttu-id="cd667-519">Добавлена функция в частной зоне DNS для импорта и экспорта файла зоны.</span><span class="sxs-lookup"><span data-stu-id="cd667-519">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="cd667-520">21 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-520">April 21, 2020</span></span>

<span data-ttu-id="cd667-521">Версия 2.4.0</span><span class="sxs-lookup"><span data-stu-id="cd667-521">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-522">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-522">ACR</span></span>

* <span data-ttu-id="cd667-523">`az acr run --cmd`: отключает переопределение рабочего каталога.</span><span class="sxs-lookup"><span data-stu-id="cd667-523">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="cd667-524">Включена поддержка выделенной конечной точки данных.</span><span class="sxs-lookup"><span data-stu-id="cd667-524">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="cd667-525">AKS</span><span class="sxs-lookup"><span data-stu-id="cd667-525">AKS</span></span>

* <span data-ttu-id="cd667-526">`az aks list -o table` теперь показывает privateFqdn как FQDN для частных кластеров.</span><span class="sxs-lookup"><span data-stu-id="cd667-526">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="cd667-527">Добавлен параметр --uptime-sla.</span><span class="sxs-lookup"><span data-stu-id="cd667-527">Add --uptime-sla</span></span>
* <span data-ttu-id="cd667-528">Обновлен пакет containerservice.</span><span class="sxs-lookup"><span data-stu-id="cd667-528">Update containerservice package</span></span>
* <span data-ttu-id="cd667-529">Включена поддержка общедоступных IP-адресов узлов.</span><span class="sxs-lookup"><span data-stu-id="cd667-529">Add node public IP support</span></span>
* <span data-ttu-id="cd667-530">Исправлена опечатка в команде справки.</span><span class="sxs-lookup"><span data-stu-id="cd667-530">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="cd667-531">AppConfig</span><span class="sxs-lookup"><span data-stu-id="cd667-531">AppConfig</span></span>

* <span data-ttu-id="cd667-532">Разрешена ссылка на хранилище ключей для команд kv list и export.</span><span class="sxs-lookup"><span data-stu-id="cd667-532">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="cd667-533">Исправлена ошибка при отображении значений ключей.</span><span class="sxs-lookup"><span data-stu-id="cd667-533">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-534">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-534">AppService</span></span>

* <span data-ttu-id="cd667-535">`az functionapp create`: изменен способ настройки linuxFxVersion для приложений-функций dotnet в Linux.</span><span class="sxs-lookup"><span data-stu-id="cd667-535">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="cd667-536">Это должно исправить ошибку, препятствующую созданию приложений dotnet для использования в Linux.</span><span class="sxs-lookup"><span data-stu-id="cd667-536">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="cd667-537">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az webapp create` Исправлена ошибка для сохранения существующих параметров AppSettings с помощью az webapp create.</span><span class="sxs-lookup"><span data-stu-id="cd667-537">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="cd667-538">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az webapp up` Исправлена ошибка для создания группы ресурсов для команды az webapp up при использовании флага -g.</span><span class="sxs-lookup"><span data-stu-id="cd667-538">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="cd667-539">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az webapp config` Исправлена ошибка для отображения значений для выходных данных не в формате JSON с помощью команды az webapp config connection-string list.</span><span class="sxs-lookup"><span data-stu-id="cd667-539">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="cd667-540">ARM</span><span class="sxs-lookup"><span data-stu-id="cd667-540">ARM</span></span>

* <span data-ttu-id="cd667-541">`az deployment create/validate`: добавлен параметр `--no-prompt` для пропуска запроса отсутствующих параметров для шаблона ARM.</span><span class="sxs-lookup"><span data-stu-id="cd667-541">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="cd667-542">`az deployment group/mg/sub/tenant validate`: включена поддержка комментариев в файле параметров развертывания.</span><span class="sxs-lookup"><span data-stu-id="cd667-542">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="cd667-543">`az deployment`: удалено значение `is_preview` для параметра `--handle-extended-json-format`.</span><span class="sxs-lookup"><span data-stu-id="cd667-543">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="cd667-544">`az deployment group/mg/sub/tenant cancel`: включена поддержка отмены развертывания для шаблона ARM.</span><span class="sxs-lookup"><span data-stu-id="cd667-544">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="cd667-545">`az deployment group/mg/sub/tenant validate`: улучшено отображение сообщения об ошибке при сбое проверки развертывания.</span><span class="sxs-lookup"><span data-stu-id="cd667-545">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="cd667-546">`az deployment-scripts`: добавлена новая команда для DeploymentScripts.</span><span class="sxs-lookup"><span data-stu-id="cd667-546">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="cd667-547">`az resource tag`: добавлен параметр `--is-incremental` для инкрементного добавления тегов к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="cd667-547">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="cd667-548">ARO</span><span class="sxs-lookup"><span data-stu-id="cd667-548">ARO</span></span>

* <span data-ttu-id="cd667-549">`az aro`:  добавлен модуль команды aro Azure RedHat OpenShift версии 4.</span><span class="sxs-lookup"><span data-stu-id="cd667-549">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="cd667-550">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-550">Batch</span></span>

* <span data-ttu-id="cd667-551">Обновлен API пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="cd667-551">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-552">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="cd667-552">Compute</span></span>

* <span data-ttu-id="cd667-553">`az sig image-version create`: добавлен тип учетной записи хранения Premium_LRS.</span><span class="sxs-lookup"><span data-stu-id="cd667-553">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="cd667-554">`az vmss update`: устранена проблема с обновлением уведомления о завершении.</span><span class="sxs-lookup"><span data-stu-id="cd667-554">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="cd667-555">`az vm/vmss create`: включена поддержка версии специализированного образа.</span><span class="sxs-lookup"><span data-stu-id="cd667-555">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="cd667-556">API SIG версии 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="cd667-556">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="cd667-557">`az sig image-version create`: добавлен параметр --target-region-encryption.</span><span class="sxs-lookup"><span data-stu-id="cd667-557">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="cd667-558">Исправлена ошибка, из-за которой тесты завершались сбоем при последовательном выполнении из-за дублирования имени хранилища ключей в глобальном кэше в памяти.</span><span class="sxs-lookup"><span data-stu-id="cd667-558">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="cd667-559">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-559">CosmosDB</span></span>

* <span data-ttu-id="cd667-560">Включена поддержка `az cosmosdb private-link-resource/private-endpoint-connection`.</span><span class="sxs-lookup"><span data-stu-id="cd667-560">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="cd667-561">IoT Central</span><span class="sxs-lookup"><span data-stu-id="cd667-561">IoT Central</span></span>

* <span data-ttu-id="cd667-562">Прекращена поддержка `az iotcentral`.</span><span class="sxs-lookup"><span data-stu-id="cd667-562">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="cd667-563">Добавлен модуль команды `az iot central`.</span><span class="sxs-lookup"><span data-stu-id="cd667-563">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-564">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-564">Monitor</span></span>

* <span data-ttu-id="cd667-565">Включена поддержка сценария приватного канала для монитора.</span><span class="sxs-lookup"><span data-stu-id="cd667-565">Support private link scenario for monitor</span></span>
* <span data-ttu-id="cd667-566">Исправлен неправильный способ имитации в test_monitor_general_operations.py.</span><span class="sxs-lookup"><span data-stu-id="cd667-566">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="cd667-567">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-567">Network</span></span>

* <span data-ttu-id="cd667-568">Прекращена поддержка SKU для команды public ip update.</span><span class="sxs-lookup"><span data-stu-id="cd667-568">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="cd667-569">`az network private-endpoint`: включена поддержка закрытой группы зон DNS.</span><span class="sxs-lookup"><span data-stu-id="cd667-569">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="cd667-570">Включена функция локального контекста для параметра vnet/subnet.</span><span class="sxs-lookup"><span data-stu-id="cd667-570">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="cd667-571">Исправлен неправильный пример использования в test_nw_flow_log_delete.</span><span class="sxs-lookup"><span data-stu-id="cd667-571">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="cd667-572">Упаковка</span><span class="sxs-lookup"><span data-stu-id="cd667-572">Packaging</span></span>

* <span data-ttu-id="cd667-573">Прекращена поддержка пакета Ubuntu/Disco.</span><span class="sxs-lookup"><span data-stu-id="cd667-573">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="cd667-574">RBAC</span><span class="sxs-lookup"><span data-stu-id="cd667-574">RBAC</span></span>

* <span data-ttu-id="cd667-575">`az ad app create/update`: включена поддержка параметра --optional-claims.</span><span class="sxs-lookup"><span data-stu-id="cd667-575">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="cd667-576">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="cd667-576">RDBMS</span></span>

* <span data-ttu-id="cd667-577">Добавлены команды администратора Azure Active Directory для PostgreSQL и MySQL.</span><span class="sxs-lookup"><span data-stu-id="cd667-577">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="cd667-578">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="cd667-578">Service Fabric</span></span>

* <span data-ttu-id="cd667-579">Исправление 12891: `az sf application update --application-parameters` удаляет старые параметры, отсутствующие в запросе.</span><span class="sxs-lookup"><span data-stu-id="cd667-579">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="cd667-580">Исправление 12470: включена поддержка az sf create cluster, исправлены ошибки, связанные с устойчивостью и надежностью обновления, поиск VMSS выполняется корректно в коде при указании имени типа узла.</span><span class="sxs-lookup"><span data-stu-id="cd667-580">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-581">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-581">SQL</span></span>

* <span data-ttu-id="cd667-582">Добавлены команды `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`.</span><span class="sxs-lookup"><span data-stu-id="cd667-582">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="cd667-583">`az sql midb`: обновление и отображение политик долгосрочного хранения, отображение и удаление долгосрочных резервных копий, восстановление долгосрочных резервных копий.</span><span class="sxs-lookup"><span data-stu-id="cd667-583">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-584">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-584">Storage</span></span>

* <span data-ttu-id="cd667-585">Обновлена версия azure-mgmt-storage до 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="cd667-585">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="cd667-586">`az storage logging off`: включено отключение ведения журналов для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="cd667-586">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="cd667-587">`az storage account update`: включена автоматическая смена ключа для CMK.</span><span class="sxs-lookup"><span data-stu-id="cd667-587">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="cd667-588">`az storage account encryption-scope create/update/list/show`: включена настройка области шифрования.</span><span class="sxs-lookup"><span data-stu-id="cd667-588">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="cd667-589">`az storage container create`: добавлены параметры --default-encryption-scope и --deny-encryption-scope-override для настройки области шифрования на уровне контейнера.</span><span class="sxs-lookup"><span data-stu-id="cd667-589">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="cd667-590">Опрос</span><span class="sxs-lookup"><span data-stu-id="cd667-590">Survey</span></span>

* <span data-ttu-id="cd667-591">Добавлен параметр для отключения ссылки опроса.</span><span class="sxs-lookup"><span data-stu-id="cd667-591">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="cd667-592">01 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-592">April 01, 2020</span></span>

<span data-ttu-id="cd667-593">Версия 2.3.1</span><span class="sxs-lookup"><span data-stu-id="cd667-593">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-594">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-594">ACR</span></span>

* <span data-ttu-id="cd667-595">Исправлена неправильная версия azure-mgmt-containerregistry для Linux.</span><span class="sxs-lookup"><span data-stu-id="cd667-595">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-596">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-596">Profile</span></span>

* <span data-ttu-id="cd667-597">az login: Исправлена ошибка входа в облачных профилях, отличающихся от `latest`.</span><span class="sxs-lookup"><span data-stu-id="cd667-597">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="cd667-598">31 марта 2020 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-598">March 31, 2020</span></span>

<span data-ttu-id="cd667-599">Версия 2.3.0</span><span class="sxs-lookup"><span data-stu-id="cd667-599">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-600">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-600">ACR</span></span>

* <span data-ttu-id="cd667-601">az acr task update: исключение пустого указателя.</span><span class="sxs-lookup"><span data-stu-id="cd667-601">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="cd667-602">`az acr import`: Отредактировано справочное сообщение и сообщение об ошибке для уточнения того, как использовать параметры --source и --registry.</span><span class="sxs-lookup"><span data-stu-id="cd667-602">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="cd667-603">Добавлено средство проверки для аргумента registry_name.</span><span class="sxs-lookup"><span data-stu-id="cd667-603">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="cd667-604">`az acr login`: удален флаг предпросмотра для --expose-token.</span><span class="sxs-lookup"><span data-stu-id="cd667-604">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="cd667-605">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр ветви az acr task create/update.</span><span class="sxs-lookup"><span data-stu-id="cd667-605">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="cd667-606">Клиент az acr task update теперь может независимо обновлять контекст, токен GitHub и триггеры.</span><span class="sxs-lookup"><span data-stu-id="cd667-606">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="cd667-607">az acr agentpool: новая функция.</span><span class="sxs-lookup"><span data-stu-id="cd667-607">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="cd667-608">AKS</span><span class="sxs-lookup"><span data-stu-id="cd667-608">AKS</span></span>

* <span data-ttu-id="cd667-609">Исправлена ошибка с apiServerAccessProfile при обновлении --api-server-authorized-ip-ranges.</span><span class="sxs-lookup"><span data-stu-id="cd667-609">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="cd667-610">Обновление AKS: при обновлении исходящие IP-адреса переопределяются с помощью входных значений.</span><span class="sxs-lookup"><span data-stu-id="cd667-610">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="cd667-611">Не создаются имена субъектов-служб для кластеров MSI и реализована поддержка присоединение ACR к кластерам MSI.</span><span class="sxs-lookup"><span data-stu-id="cd667-611">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="cd667-612">AMS</span><span class="sxs-lookup"><span data-stu-id="cd667-612">AMS</span></span>

* <span data-ttu-id="cd667-613">Исправление 12469: не удается добавить content-key-policy для FairPlay из-за проблем с параметром ask.</span><span class="sxs-lookup"><span data-stu-id="cd667-613">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="cd667-614">AppConfig</span><span class="sxs-lookup"><span data-stu-id="cd667-614">AppConfig</span></span>

* <span data-ttu-id="cd667-615">Добавлен параметр --skip-keyvault для экспорта kv.</span><span class="sxs-lookup"><span data-stu-id="cd667-615">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-616">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-616">AppService</span></span>

* <span data-ttu-id="cd667-617">Исправление 12509: удален тег, добавлявшийся по умолчанию при создании приложения с помощью az webapp up.</span><span class="sxs-lookup"><span data-stu-id="cd667-617">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="cd667-618">az functionapp create: обновлено меню справки для --runtime-version и добавлено предупреждение, когда пользователь указывает параметр --runtime-version для DotNet.</span><span class="sxs-lookup"><span data-stu-id="cd667-618">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="cd667-619">az functionapp create: изменен способ установки JavaVersion для приложений-функций Windows.</span><span class="sxs-lookup"><span data-stu-id="cd667-619">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="cd667-620">ARM</span><span class="sxs-lookup"><span data-stu-id="cd667-620">ARM</span></span>

* <span data-ttu-id="cd667-621">az deployment create/validate: по умолчанию используется параметр --handle-extended-json-format.</span><span class="sxs-lookup"><span data-stu-id="cd667-621">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="cd667-622">az lock create: в справочную документацию добавлены примеры создания подресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd667-622">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="cd667-623">Список az deployment {group/mg/sub/tenant}: реализована поддержка фильтрации ProvisioningState.</span><span class="sxs-lookup"><span data-stu-id="cd667-623">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="cd667-624">az deployment: исправлена ошибка синтаксического анализа комментария в последнем аргументе.</span><span class="sxs-lookup"><span data-stu-id="cd667-624">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="cd667-625">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="cd667-625">Backup</span></span>

* <span data-ttu-id="cd667-626">Добавлена возможность восстановления нескольких файлов.</span><span class="sxs-lookup"><span data-stu-id="cd667-626">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="cd667-627">Добавлена возможность резервного копирования только дисков с ОС.</span><span class="sxs-lookup"><span data-stu-id="cd667-627">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="cd667-628">Добавлен параметр restore-as-unmanaged-disk, позволяющий задать неуправляемое восстановление.</span><span class="sxs-lookup"><span data-stu-id="cd667-628">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-629">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="cd667-629">Compute</span></span>

* <span data-ttu-id="cd667-630">az vm create: для --nsg-rule добавлен вариант NONE.</span><span class="sxs-lookup"><span data-stu-id="cd667-630">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="cd667-631">az vmss create/update: удален тег предпросмотра для автоматического восстановления VMSS.</span><span class="sxs-lookup"><span data-stu-id="cd667-631">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="cd667-632">az vm update: реализована поддержка --workspace.</span><span class="sxs-lookup"><span data-stu-id="cd667-632">az vm update: Support --workspace</span></span>
* <span data-ttu-id="cd667-633">Исправлена ошибка в коде инициализации VirtualMachineScaleSetExtension.</span><span class="sxs-lookup"><span data-stu-id="cd667-633">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="cd667-634">Версия VMAccessAgent обновлена до 2.4.</span><span class="sxs-lookup"><span data-stu-id="cd667-634">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="cd667-635">az vmss set-orchestration-service-state: реализована поддержка состояния службы оркестрации наборов VMSS.</span><span class="sxs-lookup"><span data-stu-id="cd667-635">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="cd667-636">Версия API диска обновлена до 2019-11-01.</span><span class="sxs-lookup"><span data-stu-id="cd667-636">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="cd667-637">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun.</span><span class="sxs-lookup"><span data-stu-id="cd667-637">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="cd667-638">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-638">Cosmos DB</span></span>

* <span data-ttu-id="cd667-639">Добавлен отсутствовавший параметр --type для перенаправления в связи с устареванием.</span><span class="sxs-lookup"><span data-stu-id="cd667-639">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="cd667-640">Docker</span><span class="sxs-lookup"><span data-stu-id="cd667-640">Docker</span></span>

* <span data-ttu-id="cd667-641">Обновление до Alpine 3.11 и Python 3.6.10.</span><span class="sxs-lookup"><span data-stu-id="cd667-641">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="cd667-642">Расширение</span><span class="sxs-lookup"><span data-stu-id="cd667-642">Extension</span></span>

* <span data-ttu-id="cd667-643">Добавлена возможность загрузки расширений в системный путь через пакеты.</span><span class="sxs-lookup"><span data-stu-id="cd667-643">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="cd667-644">HDInsight</span><span class="sxs-lookup"><span data-stu-id="cd667-644">HDInsight</span></span>

* <span data-ttu-id="cd667-645">(az hdinsight create:) Добавлена возможность указания клиентами минимальной поддерживаемой версии TLS с помощью параметра `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="cd667-645">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="cd667-646">Допустимые значения: 1.0,1.1,1.2.</span><span class="sxs-lookup"><span data-stu-id="cd667-646">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-647">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-647">IoT</span></span>

* <span data-ttu-id="cd667-648">Добавлен параметр codeowner.</span><span class="sxs-lookup"><span data-stu-id="cd667-648">Add codeowner</span></span>
* <span data-ttu-id="cd667-649">az iot hub create: номер SKU по умолчанию изменен с F1 на S1.</span><span class="sxs-lookup"><span data-stu-id="cd667-649">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="cd667-650">iot hub: реализована поддержка IotHub в профиле 2019-03-01-hybrid.</span><span class="sxs-lookup"><span data-stu-id="cd667-650">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="cd667-651">IoT Central</span><span class="sxs-lookup"><span data-stu-id="cd667-651">IoTCentral</span></span>

* <span data-ttu-id="cd667-652">Обновлены сведения об ошибках, шаблон приложения по умолчанию и сообщение с подсказкой.</span><span class="sxs-lookup"><span data-stu-id="cd667-652">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="cd667-653">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="cd667-653">KeyVault</span></span>

* <span data-ttu-id="cd667-654">Реализована поддержка резервного копирования и восстановления сертификатов.</span><span class="sxs-lookup"><span data-stu-id="cd667-654">Support certificate backup/restore</span></span>
* <span data-ttu-id="cd667-655">keyvault create/update: добавлена поддержка параметра --retention-days.</span><span class="sxs-lookup"><span data-stu-id="cd667-655">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="cd667-656">При перечислении больше не показываются управляемые ключи и секреты.</span><span class="sxs-lookup"><span data-stu-id="cd667-656">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="cd667-657">az keyvault create: реализована поддержка `--network-acls`, `--network-acls-ips` и `--network-acls-vnets` для указания сетевых правил при создании хранилища.</span><span class="sxs-lookup"><span data-stu-id="cd667-657">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="cd667-658">Блокировка</span><span class="sxs-lookup"><span data-stu-id="cd667-658">Lock</span></span>

* <span data-ttu-id="cd667-659">Исправлена ошибка с командой az lock delete, не работавшей с Microsoft.DocumentDB.</span><span class="sxs-lookup"><span data-stu-id="cd667-659">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-660">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-660">Monitor</span></span>

* <span data-ttu-id="cd667-661">az monitor clone: добавлена возможность клонирования правил метрики из одного ресурса в другой.</span><span class="sxs-lookup"><span data-stu-id="cd667-661">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="cd667-662">Исправлена ошибка IcM179210086: не удается создать настраиваемое оповещение для метрики Application Insights.</span><span class="sxs-lookup"><span data-stu-id="cd667-662">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="cd667-663">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="cd667-663">NetAppFiles</span></span>

* <span data-ttu-id="cd667-664">az volume create: для томов защиты данных добавлены операции репликации (approve, suspend, resume, status, remove).</span><span class="sxs-lookup"><span data-stu-id="cd667-664">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="cd667-665">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-665">Network</span></span>

* <span data-ttu-id="cd667-666">az network application-gateway waf-policy managed-rule rule-set add: добавлена поддержка Microsoft_BotManagerRuleSet.</span><span class="sxs-lookup"><span data-stu-id="cd667-666">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="cd667-667">Журнал потоков наблюдателя за сетями: исправлены неправильные сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="cd667-667">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="cd667-668">Добавлена поддержка имен узлов в прослушивателе шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="cd667-668">support host names in application gateway listener</span></span>
* <span data-ttu-id="cd667-669">az network nat gateway: добавлена возможность создания пустого ресурса без общедоступного IP-адреса или общедоступного IP-префикса.</span><span class="sxs-lookup"><span data-stu-id="cd667-669">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="cd667-670">Добавлена возможность создания VPN-шлюза.</span><span class="sxs-lookup"><span data-stu-id="cd667-670">Support vpn gateway generation</span></span>
* <span data-ttu-id="cd667-671">Реализована поддержка `--if-none-match` для `az network dns record-set {} add-record`.</span><span class="sxs-lookup"><span data-stu-id="cd667-671">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="cd667-672">Упаковка</span><span class="sxs-lookup"><span data-stu-id="cd667-672">Packaging</span></span>

* <span data-ttu-id="cd667-673">Прекращена поддержка Python 3.5.</span><span class="sxs-lookup"><span data-stu-id="cd667-673">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-674">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-674">Profile</span></span>

* <span data-ttu-id="cd667-675">az login: добавлен показ предупреждений об ошибках MFA.</span><span class="sxs-lookup"><span data-stu-id="cd667-675">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="cd667-676">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="cd667-676">RDBMS</span></span>

* <span data-ttu-id="cd667-677">Добавлены команды управления ключами шифрования данных сервера для PostgreSQL и MySQL.</span><span class="sxs-lookup"><span data-stu-id="cd667-677">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="cd667-678">10 марта 2020 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-678">March 10, 2020</span></span>

<span data-ttu-id="cd667-679">Версия 2.2.0</span><span class="sxs-lookup"><span data-stu-id="cd667-679">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-680">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-680">ACR</span></span>

* <span data-ttu-id="cd667-681">Исправлена команда `az acr login`, которая неправильно вызывала ошибку.</span><span class="sxs-lookup"><span data-stu-id="cd667-681">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="cd667-682">Добавлена новая команда `az acr helm install-cli`.</span><span class="sxs-lookup"><span data-stu-id="cd667-682">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="cd667-683">Добавлена частная ссылка и включена поддержка CMK.</span><span class="sxs-lookup"><span data-stu-id="cd667-683">Add private link and CMK support</span></span>
* <span data-ttu-id="cd667-684">Добавлена команда private-link-resource list.</span><span class="sxs-lookup"><span data-stu-id="cd667-684">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="cd667-685">AKS</span><span class="sxs-lookup"><span data-stu-id="cd667-685">AKS</span></span>

* <span data-ttu-id="cd667-686">Исправлена функция поиска AKS в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="cd667-686">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="cd667-687">az aks: устранены ошибки NoneType при мониторинге надстроек и пула агентов.</span><span class="sxs-lookup"><span data-stu-id="cd667-687">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="cd667-688">Добавлен параметр --nodepool-tags в пуле узлов при создании кластера Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="cd667-688">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="cd667-689">Добавлен параметр --tags при добавлении пула узлов в кластер или его обновлении.</span><span class="sxs-lookup"><span data-stu-id="cd667-689">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="cd667-690">aks create: добавлен параметр `--enable-private-cluster`.</span><span class="sxs-lookup"><span data-stu-id="cd667-690">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="cd667-691">Добавлен параметр --nodepool-labels в пуле узлов при создании кластера Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="cd667-691">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="cd667-692">Добавлен параметр --labels при добавлении нового пула узлов в кластер Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="cd667-692">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="cd667-693">Добавлен отсутствующий символ / в URL-адрес панели мониторинга.</span><span class="sxs-lookup"><span data-stu-id="cd667-693">add missing / in the dashboard url</span></span>
* <span data-ttu-id="cd667-694">Включена поддержка создания кластеров AKS для управляемых удостоверений</span><span class="sxs-lookup"><span data-stu-id="cd667-694">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="cd667-695">az aks: включена проверка состояния сетевого подключаемого модуля: Azure или Kubenet.</span><span class="sxs-lookup"><span data-stu-id="cd667-695">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="cd667-696">az aks: включена поддержка ключа сеанса AAD.</span><span class="sxs-lookup"><span data-stu-id="cd667-696">az aks: Add aad session key support</span></span>
* <span data-ttu-id="cd667-697">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az aks: включена поддержка изменений MSI для GF и BF для omsagent (мониторинг контейнеров) (1)</span><span class="sxs-lookup"><span data-stu-id="cd667-697">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="cd667-698">az aks use-dev-spaces: добавлен параметр типа конечной точки в команду use-dev-spaces для настройки конечной точки, созданной в контроллере Azure Dev Spaces.</span><span class="sxs-lookup"><span data-stu-id="cd667-698">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="cd667-699">AppConfig</span><span class="sxs-lookup"><span data-stu-id="cd667-699">AppConfig</span></span>

* <span data-ttu-id="cd667-700">Включена разблокировка с использованием kv set для добавления функции и ссылки на хранилище ключей.</span><span class="sxs-lookup"><span data-stu-id="cd667-700">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-701">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-701">AppService</span></span>

* <span data-ttu-id="cd667-702">az webapp create: устранена проблема с выполнением команды с параметром --runtime.</span><span class="sxs-lookup"><span data-stu-id="cd667-702">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="cd667-703">az functionapp deployment source config-zip: добавлено сообщение об ошибке, если группа ресурсов или имя функции недействительны или не существуют.</span><span class="sxs-lookup"><span data-stu-id="cd667-703">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="cd667-704">functionapp create: исправлено сообщение с предупреждением, которое появляется с `functionapp create` и в котором указан флаг `--functions_version`, но в имени флага ошибочно используется `_` вместо `-`.</span><span class="sxs-lookup"><span data-stu-id="cd667-704">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="cd667-705">az functionapp create: обновлен способ настройки linuxFxVersion и имени образа контейнера для приложений с функциями Linux.</span><span class="sxs-lookup"><span data-stu-id="cd667-705">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="cd667-706">az functionapp deployment source config-zip: устранена проблема, вызванная изменением параметров приложения во время развертывания ZIP, что приводит к ошибкам 5xx во время развертывания.</span><span class="sxs-lookup"><span data-stu-id="cd667-706">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="cd667-707">Исправление 5720946: не удается задать имя с помощью az webapp backup.</span><span class="sxs-lookup"><span data-stu-id="cd667-707">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="cd667-708">ARM</span><span class="sxs-lookup"><span data-stu-id="cd667-708">ARM</span></span>

* <span data-ttu-id="cd667-709">az resource: улучшены примеры для модуля ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd667-709">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="cd667-710">az policy assignment list: Включена поддержка списков назначений политик в области группы управления.</span><span class="sxs-lookup"><span data-stu-id="cd667-710">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="cd667-711">Добавлены команды `az deployment group` и `az deployment operation group` для развертывания шаблонов в группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd667-711">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="cd667-712">Это дубликат `az group deployment` и `az group deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="cd667-712">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="cd667-713">Добавлены команды `az deployment sub` и `az deployment operation sub` для развертывания шаблонов в области подписки.</span><span class="sxs-lookup"><span data-stu-id="cd667-713">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="cd667-714">Это дубликат `az deployment` и `az deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="cd667-714">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="cd667-715">Добавлены команды `az deployment mg` и `az deployment operation mg` для развертывания шаблонов в группах управления.</span><span class="sxs-lookup"><span data-stu-id="cd667-715">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="cd667-716">Добавлены команды `az deployment tenant` и `az deployment operation tenant` для развертывания шаблонов в области арендатора.</span><span class="sxs-lookup"><span data-stu-id="cd667-716">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="cd667-717">az policy assignment create: добавлено описание параметра `--location`.</span><span class="sxs-lookup"><span data-stu-id="cd667-717">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="cd667-718">az group deployment create: добавлен параметр `--aux-tenants` для включения поддержки перекрестных арендаторов.</span><span class="sxs-lookup"><span data-stu-id="cd667-718">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="cd667-719">CDN</span><span class="sxs-lookup"><span data-stu-id="cd667-719">CDN</span></span>

* <span data-ttu-id="cd667-720">Добавлены команды WAF CDN.</span><span class="sxs-lookup"><span data-stu-id="cd667-720">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-721">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="cd667-721">Compute</span></span>

* <span data-ttu-id="cd667-722">az sig image-version: добавлен параметр --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="cd667-722">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="cd667-723">az ppg show: добавлен параметр --colocation-status, чтобы включить выборку состояния совместного размещения всех ресурсов в группе размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="cd667-723">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="cd667-724">az vmss create/update: включена поддержка автоматического исправления.</span><span class="sxs-lookup"><span data-stu-id="cd667-724">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="cd667-725">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az image template: шаблон переименован в построитель.</span><span class="sxs-lookup"><span data-stu-id="cd667-725">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="cd667-726">az image builder create: добавлен параметр --image-template.</span><span class="sxs-lookup"><span data-stu-id="cd667-726">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="cd667-727">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-727">Cosmos DB</span></span>

* <span data-ttu-id="cd667-728">Добавлены командлеты хранимой процедуры SQL, определяемых пользователем функций и триггеров.</span><span class="sxs-lookup"><span data-stu-id="cd667-728">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="cd667-729">az cosmosdb create: добавлен параметр --key-uri для добавления сведений о шифровании хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="cd667-729">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="cd667-730">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="cd667-730">KeyVault</span></span>

* <span data-ttu-id="cd667-731">keyvault create: включена функция обратимого удаления по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-731">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-732">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-732">Monitor</span></span>

* <span data-ttu-id="cd667-733">az monitor metrics alert create: включена поддержка `~` в `--condition`.</span><span class="sxs-lookup"><span data-stu-id="cd667-733">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="cd667-734">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-734">Network</span></span>

* <span data-ttu-id="cd667-735">az network application-gateway rewrite-rule create: включена поддержка конфигурации URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="cd667-735">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="cd667-736">az network dns zone import: для параметра --zone-name в будущем можно будет не учитывать регистр.</span><span class="sxs-lookup"><span data-stu-id="cd667-736">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="cd667-737">az network private-endpoint/private-link-service: удалена метка предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="cd667-737">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="cd667-738">az network bastion: включена поддержка бастиона.</span><span class="sxs-lookup"><span data-stu-id="cd667-738">az network bastion: support bastion</span></span>
* <span data-ttu-id="cd667-739">az network vnet list-available-ips: включена поддержка списка доступных IP-адресов в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="cd667-739">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="cd667-740">az network watcher flow-log create/list/delete/update: добавлены новые команды для управления журналами потоков Наблюдателя и предоставлен параметр --location для явного определения Наблюдателя.</span><span class="sxs-lookup"><span data-stu-id="cd667-740">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="cd667-741">az network watcher flow-log configure: поддержка прекращена.</span><span class="sxs-lookup"><span data-stu-id="cd667-741">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="cd667-742">az network watcher flow-log show: включена поддержка параметров --location и --name для получения результатов в формате ARM; поддержка предыдущего форматированного вывода прекращена.</span><span class="sxs-lookup"><span data-stu-id="cd667-742">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="cd667-743">Политика</span><span class="sxs-lookup"><span data-stu-id="cd667-743">Policy</span></span>

* <span data-ttu-id="cd667-744">az policy assignment create: исправлена ошибка, из-за которой автоматически генерируемое имя назначения политики превышало предельное значение.</span><span class="sxs-lookup"><span data-stu-id="cd667-744">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="cd667-745">RBAC</span><span class="sxs-lookup"><span data-stu-id="cd667-745">RBAC</span></span>

* <span data-ttu-id="cd667-746">az ad group show: исправлено значение --group, обрабатываемое как проблема с регулярными выражениями.</span><span class="sxs-lookup"><span data-stu-id="cd667-746">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="cd667-747">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="cd667-747">RDBMS</span></span>

* <span data-ttu-id="cd667-748">Обновлена версия пакета SDK azure-mgmt-rdbms до 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="cd667-748">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="cd667-749">az postgres private-endpoint-connection: включено управление подключениями частных конечных точек Postgres.</span><span class="sxs-lookup"><span data-stu-id="cd667-749">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="cd667-750">az postgres private-link-resource: включено управление ресурсами частных ссылок Postgres.</span><span class="sxs-lookup"><span data-stu-id="cd667-750">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="cd667-751">az mysql private-endpoint-connection: включено управление подключениями частных конечных точек MySQL.</span><span class="sxs-lookup"><span data-stu-id="cd667-751">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="cd667-752">az mysql private-link-resource: включено управление ресурсами частных ссылок MySQL.</span><span class="sxs-lookup"><span data-stu-id="cd667-752">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="cd667-753">az mariadb private-endpoint-connection: включено управление подключениями частных конечных точек MariaDB.</span><span class="sxs-lookup"><span data-stu-id="cd667-753">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="cd667-754">az mariadb private-link-resource: включено управление ресурсами частных ссылок MariaDB.</span><span class="sxs-lookup"><span data-stu-id="cd667-754">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="cd667-755">Обновление тестов частной конечной точки RDBMS</span><span class="sxs-lookup"><span data-stu-id="cd667-755">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-756">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-756">SQL</span></span>

* <span data-ttu-id="cd667-757">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention.</span><span class="sxs-lookup"><span data-stu-id="cd667-757">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="cd667-758">(sql server create:) добавлен необязательный флаг включения и отключения доступа к общедоступным сетям в команду создания SQL Server.</span><span class="sxs-lookup"><span data-stu-id="cd667-758">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="cd667-759">(sql server update:) внесены некоторые изменения для клиентов.</span><span class="sxs-lookup"><span data-stu-id="cd667-759">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="cd667-760">Добавлено свойство minimal_tls_version для MI и SQL DB.</span><span class="sxs-lookup"><span data-stu-id="cd667-760">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-761">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-761">Storage</span></span>

* <span data-ttu-id="cd667-762">az storage blob delete-batch: исправлено неправильное поведение флага `--dryrun`.</span><span class="sxs-lookup"><span data-stu-id="cd667-762">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="cd667-763">az storage account network-rule add (исправление): добавлено требование того, чтобы операция была идемпотентной.</span><span class="sxs-lookup"><span data-stu-id="cd667-763">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="cd667-764">az storage account create/update: включена поддержка предпочтения маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="cd667-764">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="cd667-765">Обновлена версия azure-mgmt-storage до 8.0.0.</span><span class="sxs-lookup"><span data-stu-id="cd667-765">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="cd667-766">az storage container immutability create: добавлен параметр --allow-protected-append-write.</span><span class="sxs-lookup"><span data-stu-id="cd667-766">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="cd667-767">az storage account private-link-resource list: включена поддержка вывода списка ресурсов частной ссылки для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="cd667-767">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="cd667-768">az storage account private-endpoint-connection approve/reject/show/delete: включена поддержка управления подключениями к частным конечным точкам.</span><span class="sxs-lookup"><span data-stu-id="cd667-768">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="cd667-769">az storage account blob-service-properties update: добавлены параметры --enable-restore-policy и --restore-days.</span><span class="sxs-lookup"><span data-stu-id="cd667-769">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="cd667-770">az storage blob restore: включена поддержка восстановления диапазонов BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="cd667-770">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="cd667-771">18 февраля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-771">February 18, 2020</span></span>

<span data-ttu-id="cd667-772">Версия 2.1.0</span><span class="sxs-lookup"><span data-stu-id="cd667-772">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-773">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-773">ACR</span></span>

* <span data-ttu-id="cd667-774">Добавлен новый аргумент `--expose-token` для `az acr login`.</span><span class="sxs-lookup"><span data-stu-id="cd667-774">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="cd667-775">Исправлены неправильные выходные данные `az acr task identity show -n Name -r Registry -o table`.</span><span class="sxs-lookup"><span data-stu-id="cd667-775">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="cd667-776">az acr login: отображение CLIError при наличии ошибок, возвращаемых командой docker.</span><span class="sxs-lookup"><span data-stu-id="cd667-776">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-777">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-777">ACS</span></span>

* <span data-ttu-id="cd667-778">aks create/update: добавление проверки `--vnet-subnet-id`.</span><span class="sxs-lookup"><span data-stu-id="cd667-778">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="cd667-779">Aladdin</span><span class="sxs-lookup"><span data-stu-id="cd667-779">Aladdin</span></span>

* <span data-ttu-id="cd667-780">Выполнение синтаксического анализа созданных примеров в _help.py для команд.</span><span class="sxs-lookup"><span data-stu-id="cd667-780">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="cd667-781">AMS</span><span class="sxs-lookup"><span data-stu-id="cd667-781">AMS</span></span>

* <span data-ttu-id="cd667-782">az ams теперь предоставляется в общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="cd667-782">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="cd667-783">AppConfig</span><span class="sxs-lookup"><span data-stu-id="cd667-783">AppConfig</span></span>

* <span data-ttu-id="cd667-784">Исправлено справочное сообщение, чтобы исключить неподдерживаемый фильтр ключей или меток.</span><span class="sxs-lookup"><span data-stu-id="cd667-784">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="cd667-785">Удален тег preview для большинства команд, кроме управляемого удостоверения и флагов функций.</span><span class="sxs-lookup"><span data-stu-id="cd667-785">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="cd667-786">Добавлен управляемый ключ клиента при обновлении магазинов.</span><span class="sxs-lookup"><span data-stu-id="cd667-786">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-787">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-787">AppService</span></span>

* <span data-ttu-id="cd667-788">az webapp list-runtimes: исправлена ошибка для list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="cd667-788">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="cd667-789">Добавлена команда az webapp|functionapp config ssl create.</span><span class="sxs-lookup"><span data-stu-id="cd667-789">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="cd667-790">Включена поддержка приложений-функций версии 3 и Node 12.</span><span class="sxs-lookup"><span data-stu-id="cd667-790">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="cd667-791">ARM</span><span class="sxs-lookup"><span data-stu-id="cd667-791">ARM</span></span>

* <span data-ttu-id="cd667-792">az policy assignment create: исправлено сообщение об ошибке, если параметр `--policy` является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="cd667-792">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="cd667-793">az group deployment create: Устранена ошибка stat: path too long for Windows при использовании большого файла parameters.json.</span><span class="sxs-lookup"><span data-stu-id="cd667-793">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="cd667-794">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="cd667-794">Backup</span></span>

* <span data-ttu-id="cd667-795">Исправлен поток восстановления на уровне элемента в OLR.</span><span class="sxs-lookup"><span data-stu-id="cd667-795">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="cd667-796">Включена поддержка восстановления в виде файлов для баз данных SQL и SAP.</span><span class="sxs-lookup"><span data-stu-id="cd667-796">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-797">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="cd667-797">Compute</span></span>

* <span data-ttu-id="cd667-798">vm/vmss/availability-set update: add --ppg: разрешено обновление ProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="cd667-798">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="cd667-799">vmss create: add --data-disk-iops and --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="cd667-799">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="cd667-800">az vm host: удален тег preview для `vm host` и `vm host group`.</span><span class="sxs-lookup"><span data-stu-id="cd667-800">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="cd667-801">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправление 10728. `az vm create`: автоматическое создание подсети, если указанные виртуальная сеть и подсеть не существуют.</span><span class="sxs-lookup"><span data-stu-id="cd667-801">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="cd667-802">Повышена надежность списка образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="cd667-802">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="cd667-803">Eventhub</span><span class="sxs-lookup"><span data-stu-id="cd667-803">Eventhub</span></span>

* <span data-ttu-id="cd667-804">Включена поддержка Azure Stack для профиля 2019-03-01-hybrid.</span><span class="sxs-lookup"><span data-stu-id="cd667-804">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="cd667-805">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="cd667-805">KeyVault</span></span>

* <span data-ttu-id="cd667-806">az keyvault key create: добавлено новое значение `import` для параметра `--ops`.</span><span class="sxs-lookup"><span data-stu-id="cd667-806">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="cd667-807">az keyvault key list-versions: включена поддержка параметров `--id` для определения ключей.</span><span class="sxs-lookup"><span data-stu-id="cd667-807">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="cd667-808">Включена поддержка подключений к частным конечным точкам.</span><span class="sxs-lookup"><span data-stu-id="cd667-808">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="cd667-809">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-809">Network</span></span>

* <span data-ttu-id="cd667-810">Выполнена активация azure-mgmt-network 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="cd667-810">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="cd667-811">az network private-link-service update/create: включена поддержка --enable-proxy-protocol.</span><span class="sxs-lookup"><span data-stu-id="cd667-811">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="cd667-812">Добавлена функция монитора подключения версии 2.</span><span class="sxs-lookup"><span data-stu-id="cd667-812">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="cd667-813">Упаковка</span><span class="sxs-lookup"><span data-stu-id="cd667-813">Packaging</span></span>

* <span data-ttu-id="cd667-814">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка Python 2.7.</span><span class="sxs-lookup"><span data-stu-id="cd667-814">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-815">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-815">Profile</span></span>

* <span data-ttu-id="cd667-816">Предварительный просмотр: В учетные записи подписок добавлены новые атрибуты `homeTenantId` и `managedByTenants`.</span><span class="sxs-lookup"><span data-stu-id="cd667-816">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="cd667-817">Чтобы изменения вступили в силу, повторно выполните команду `az login`.</span><span class="sxs-lookup"><span data-stu-id="cd667-817">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="cd667-818">az login: отображение предупреждения, если подписка связана с несколькими клиентами, но по умолчанию используется с первым из них</span><span class="sxs-lookup"><span data-stu-id="cd667-818">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="cd667-819">(чтобы выбрать определенный клиент при доступе к этой подписке, включите `--tenant` в `az login`).</span><span class="sxs-lookup"><span data-stu-id="cd667-819">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="cd667-820">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-820">Role</span></span>

* <span data-ttu-id="cd667-821">az role assignment create: исправлена ошибка с кодом HTTP 400, возникающая при присвоении роли субъекту-службе по отображаемому имени.</span><span class="sxs-lookup"><span data-stu-id="cd667-821">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-822">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-822">SQL</span></span>

* <span data-ttu-id="cd667-823">Обновлен командлет `az sql mi update` Управляемого экземпляра SQL (добавлены два новых параметра: tier и family).</span><span class="sxs-lookup"><span data-stu-id="cd667-823">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-824">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-824">Storage</span></span>

* <span data-ttu-id="cd667-825">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az storage account create`: Тип учетной записи хранения по умолчанию изменен на StorageV2.</span><span class="sxs-lookup"><span data-stu-id="cd667-825">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="cd667-826">4 февраля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-826">February 04, 2020</span></span>

<span data-ttu-id="cd667-827">Версия 2.0.81</span><span class="sxs-lookup"><span data-stu-id="cd667-827">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-828">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-828">ACS</span></span>

* <span data-ttu-id="cd667-829">Добавлена возможность задания выделенных исходящих портов и времени ожидания подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="cd667-829">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="cd667-830">Выполнено обновление до API версии 2019-11-01.</span><span class="sxs-lookup"><span data-stu-id="cd667-830">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-831">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-831">ACR</span></span>

* <span data-ttu-id="cd667-832">[Критическое изменение] `az acr delete` будет выводить запрос.</span><span class="sxs-lookup"><span data-stu-id="cd667-832">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="cd667-833">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда az acr task delete будет выводить запрос.</span><span class="sxs-lookup"><span data-stu-id="cd667-833">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="cd667-834">Добавлена новая группа команд az acr taskrun show/list/delete для управления выполнением задач.</span><span class="sxs-lookup"><span data-stu-id="cd667-834">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="cd667-835">AKS</span><span class="sxs-lookup"><span data-stu-id="cd667-835">AKS</span></span>

* <span data-ttu-id="cd667-836">Каждый кластер получает отдельный субъект-службу для улучшения изоляции.</span><span class="sxs-lookup"><span data-stu-id="cd667-836">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="cd667-837">AppConfig</span><span class="sxs-lookup"><span data-stu-id="cd667-837">AppConfig</span></span>

* <span data-ttu-id="cd667-838">Поддержка импорта ссылок на хранилище ключей из службы приложений и их экспорта в нее.</span><span class="sxs-lookup"><span data-stu-id="cd667-838">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="cd667-839">Поддержка импорта и экспорта всех меток между файлами appconfig.</span><span class="sxs-lookup"><span data-stu-id="cd667-839">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="cd667-840">Проверка имен ключей и функций перед настройкой и импортом.</span><span class="sxs-lookup"><span data-stu-id="cd667-840">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="cd667-841">Предоставление изменений номера SKU в хранилище конфигураций.</span><span class="sxs-lookup"><span data-stu-id="cd667-841">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="cd667-842">Новая группа команд для управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="cd667-842">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-843">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-843">AppService</span></span>

* <span data-ttu-id="cd667-844">Azure Stack: команды поверхности в профиле 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="cd667-844">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="cd667-845">functionapp: добавлена возможность создавать приложения-функции Java в Linux.</span><span class="sxs-lookup"><span data-stu-id="cd667-845">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="cd667-846">ARM</span><span class="sxs-lookup"><span data-stu-id="cd667-846">ARM</span></span>

* <span data-ttu-id="cd667-847">Исправление ошибки 10246: аварийное завершение `az resource tag` в случае, если переданный параметр `--ids` являлся идентификатором группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd667-847">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="cd667-848">Исправление ошибки 11658: команда `az group export` не поддерживала параметры `--query` и `--output`.</span><span class="sxs-lookup"><span data-stu-id="cd667-848">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="cd667-849">Исправление ошибки 10279: код выхода `az group deployment validate` был равен 0, если проверка не пройдена.</span><span class="sxs-lookup"><span data-stu-id="cd667-849">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="cd667-850">Исправление ошибки 9916: улучшено сообщение об ошибке из-за конфликта между тегом и другими условиями фильтра для команды `az resource list`.</span><span class="sxs-lookup"><span data-stu-id="cd667-850">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="cd667-851">Добавлен новый параметр `--managed-by` для добавления данных managedBy для команды `az group create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-851">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="cd667-852">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="cd667-852">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="cd667-853">Добавлена подгруппа `monitor` для управления мониторингом Log Analytics в кластере Azure Red Hat OpensShift.</span><span class="sxs-lookup"><span data-stu-id="cd667-853">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="cd667-854">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="cd667-854">BotService</span></span>

* <span data-ttu-id="cd667-855">Исправление ошибки 11697: команда `az bot create` не являлась идемпотентной.</span><span class="sxs-lookup"><span data-stu-id="cd667-855">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="cd667-856">Проверки исправления имен изменены для выполнения только в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="cd667-856">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="cd667-857">CDN</span><span class="sxs-lookup"><span data-stu-id="cd667-857">CDN</span></span>

* <span data-ttu-id="cd667-858">Добавлена поддержка функции rulesEngine.</span><span class="sxs-lookup"><span data-stu-id="cd667-858">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="cd667-859">Добавлена новая группа команд cdn endpoint rule для управления правилами.</span><span class="sxs-lookup"><span data-stu-id="cd667-859">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="cd667-860">Пакет azure-mgmt-cdn обновлен до версии 4.0.0 для использования API версии 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="cd667-860">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="cd667-861">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="cd667-861">Deployment Manager</span></span>

* <span data-ttu-id="cd667-862">Добавлена операция вывода списка всех ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd667-862">Add list operation for all resources.</span></span>
* <span data-ttu-id="cd667-863">Улучшен ресурс шага для нового типа шага.</span><span class="sxs-lookup"><span data-stu-id="cd667-863">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="cd667-864">Пакет azure-mgmt-deploymentmanager обновлен для использования версии 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="cd667-864">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-865">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-865">IoT</span></span>

* <span data-ttu-id="cd667-866">Команды IoT hub Job объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="cd667-866">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="cd667-867">IoT Central</span><span class="sxs-lookup"><span data-stu-id="cd667-867">IoT Central</span></span>

* <span data-ttu-id="cd667-868">Добавлена поддержка создания и обновления приложений с новыми SKU: ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="cd667-868">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="cd667-869">Key Vault</span><span class="sxs-lookup"><span data-stu-id="cd667-869">Key Vault</span></span>

* <span data-ttu-id="cd667-870">Добавлена новая команда `az keyvault key download` для скачивания ключей.</span><span class="sxs-lookup"><span data-stu-id="cd667-870">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="cd667-871">Разное</span><span class="sxs-lookup"><span data-stu-id="cd667-871">Misc</span></span>

* <span data-ttu-id="cd667-872">Исправление ошибки 6371: поддержка завершения имен файлов и переменных среды в Bash.</span><span class="sxs-lookup"><span data-stu-id="cd667-872">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="cd667-873">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-873">Network</span></span>

* <span data-ttu-id="cd667-874">Исправление ошибки 2092: для команды az network dns record-set add/remove добавлено предупреждение, отображаемое, если набор записей не найден.</span><span class="sxs-lookup"><span data-stu-id="cd667-874">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="cd667-875">В будущем для подтверждения этого автоматического создания будет добавлен дополнительный аргумент.</span><span class="sxs-lookup"><span data-stu-id="cd667-875">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="cd667-876">Политика</span><span class="sxs-lookup"><span data-stu-id="cd667-876">Policy</span></span>

* <span data-ttu-id="cd667-877">Добавлена новая команда `az policy metadata` для получения ресурсов метаданных расширенной политики.</span><span class="sxs-lookup"><span data-stu-id="cd667-877">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="cd667-878">`az policy remediation create`: С помощью параметра `--resource-discovery-mode` можно указать, следует ли повторно оценить соответствие перед исправлением.</span><span class="sxs-lookup"><span data-stu-id="cd667-878">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-879">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-879">Profile</span></span>

* <span data-ttu-id="cd667-880">`az account get-access-token`: Добавлен параметр `--tenant` для получения маркера для арендатора напрямую, без необходимости указывать подписку.</span><span class="sxs-lookup"><span data-stu-id="cd667-880">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="cd667-881">RBAC</span><span class="sxs-lookup"><span data-stu-id="cd667-881">RBAC</span></span>

* <span data-ttu-id="cd667-882">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправление ошибки 11883: `az role assignment create`: пустая область приведет к ошибке.</span><span class="sxs-lookup"><span data-stu-id="cd667-882">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="cd667-883">Безопасность</span><span class="sxs-lookup"><span data-stu-id="cd667-883">Security</span></span>

* <span data-ttu-id="cd667-884">Добавлены новые команды `az atp show` и `az atp update` для просмотра и настройки дополнительных параметров защиты от угроз для учетных записей хранения.</span><span class="sxs-lookup"><span data-stu-id="cd667-884">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-885">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-885">SQL</span></span>

* <span data-ttu-id="cd667-886">`sql dw create`: параметры `--zone-redundant` и `--read-replica-count` объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="cd667-886">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="cd667-887">Эти параметры не применяются к хранилищу данных.</span><span class="sxs-lookup"><span data-stu-id="cd667-887">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="cd667-888">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql db create`: Значения WideWorldImportersStd и WideWorldImportersFull больше не являются задокументированным допустимыми значениями для команды az sql db create --sample-name.</span><span class="sxs-lookup"><span data-stu-id="cd667-888">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="cd667-889">Эти примеры базы данных всегда будут приводить к сбою создания.</span><span class="sxs-lookup"><span data-stu-id="cd667-889">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="cd667-890">Добавлены новые команды `sql db classification show/list/update/delete` и `sql db classification recommendation list/enable/disable` для управления классификациями конфиденциальности баз данных SQL.</span><span class="sxs-lookup"><span data-stu-id="cd667-890">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="cd667-891">`az sql db audit-policy`: устранены пустые действия аудита и группы.</span><span class="sxs-lookup"><span data-stu-id="cd667-891">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-892">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-892">Storage</span></span>

* <span data-ttu-id="cd667-893">Добавлена новая группа команд `az storage share-rm` для использования поставщика ресурсов Microsoft.Storage в операциях управления файловыми ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="cd667-893">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="cd667-894">Исправление ошибки 11415: ошибка разрешения для `az storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-894">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="cd667-895">Добавлены интеграция AzCopy 10.3.3 и поддержка Win32.</span><span class="sxs-lookup"><span data-stu-id="cd667-895">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="cd667-896">`az storage copy`: добавлены параметры `--include-path`, `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="cd667-896">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="cd667-897">`az storage remove`: параметры `--inlcude` и `--exclude` заменены параметрами `--include-path`, `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="cd667-897">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="cd667-898">`az storage sync`: добавлены параметры `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="cd667-898">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="cd667-899">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="cd667-899">ServiceFabric</span></span>

* <span data-ttu-id="cd667-900">Добавлены новые команды для управления приложениями и службами.</span><span class="sxs-lookup"><span data-stu-id="cd667-900">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="cd667-901">13 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-901">January 13, 2020</span></span>

<span data-ttu-id="cd667-902">Версия 2.0.80</span><span class="sxs-lookup"><span data-stu-id="cd667-902">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-903">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="cd667-903">Compute</span></span>

* <span data-ttu-id="cd667-904">Обновление диска: добавлены параметры --disk-encryption-set и --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="cd667-904">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="cd667-905">Создание и обновление моментального снимка: добавлены параметры --disk-encryption-set и --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="cd667-905">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-906">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-906">Storage</span></span>

* <span data-ttu-id="cd667-907">Обновление azure-mgmt-storage до версии 7.1.0</span><span class="sxs-lookup"><span data-stu-id="cd667-907">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="cd667-908">`az storage account create`: добавлены параметры `--encryption-key-type-for-table` и `--encryption-key-type-for-queue` для включения поддержки службы шифрования таблиц и очередей.</span><span class="sxs-lookup"><span data-stu-id="cd667-908">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="cd667-909">7 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-909">January 07, 2020</span></span>

<span data-ttu-id="cd667-910">Версия 2.0.79</span><span class="sxs-lookup"><span data-stu-id="cd667-910">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-911">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-911">ACR</span></span>

* <span data-ttu-id="cd667-912">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --os для команд acr build, acr task create/update, acr run и acr pack.</span><span class="sxs-lookup"><span data-stu-id="cd667-912">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="cd667-913">Вместо этого используется параметр --platform.</span><span class="sxs-lookup"><span data-stu-id="cd667-913">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="cd667-914">AppConfig</span><span class="sxs-lookup"><span data-stu-id="cd667-914">AppConfig</span></span>

* <span data-ttu-id="cd667-915">Добавлена поддержка импорта и экспорта флагов функций.</span><span class="sxs-lookup"><span data-stu-id="cd667-915">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="cd667-916">Добавлена новая команда az appconfig kv set-keyvault для создания ссылки на хранилище ключей.</span><span class="sxs-lookup"><span data-stu-id="cd667-916">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="cd667-917">Добавлена поддержка различных соглашений об именовании при экспорте флагов функций в файл.</span><span class="sxs-lookup"><span data-stu-id="cd667-917">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-918">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-918">AppService</span></span>

* <span data-ttu-id="cd667-919">Устранена проблема № 7154: обновлена документация по команде <> — теперь в ней используются обратные, а не одинарные кавычки.</span><span class="sxs-lookup"><span data-stu-id="cd667-919">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="cd667-920">Устранена проблема № 11287 (webapp up): по умолчанию для приложения, созданного с использованием этого флага, должен быть включен SSL.</span><span class="sxs-lookup"><span data-stu-id="cd667-920">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="cd667-921">Устранена проблема № 11592: добавлен флаг az webapp up для статических сайтов HTML.</span><span class="sxs-lookup"><span data-stu-id="cd667-921">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="cd667-922">ARM</span><span class="sxs-lookup"><span data-stu-id="cd667-922">ARM</span></span>

* <span data-ttu-id="cd667-923">Исправлена ошибка с командой `az resource tag`: невозможно было обновить теги хранилища Служб восстановления.</span><span class="sxs-lookup"><span data-stu-id="cd667-923">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="cd667-924">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="cd667-924">Backup</span></span>

* <span data-ttu-id="cd667-925">Добавлена новая команда backup protection undelete для включения функции обратимого удаления рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="cd667-925">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="cd667-926">Добавлен новый параметр --soft-delete-feature-state для команды set backup-properties.</span><span class="sxs-lookup"><span data-stu-id="cd667-926">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="cd667-927">Добавлена поддержка исключения диска для рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="cd667-927">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-928">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="cd667-928">Compute</span></span>

* <span data-ttu-id="cd667-929">Исправлен сбой `vm create` в профиле Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="cd667-929">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="cd667-930">Добавлена поддержка определений списков и метрик запросов для виртуальной машины (vm monitor metrics tail/list-definitions).</span><span class="sxs-lookup"><span data-stu-id="cd667-930">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="cd667-931">Добавлено новое действия повторного применения команды az vm</span><span class="sxs-lookup"><span data-stu-id="cd667-931">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="cd667-932">HDInsight</span><span class="sxs-lookup"><span data-stu-id="cd667-932">HDInsight</span></span>

* <span data-ttu-id="cd667-933">Включена поддержка создания кластера Kafka с помощью прокси-сервера Kafka RESTful.</span><span class="sxs-lookup"><span data-stu-id="cd667-933">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="cd667-934">Обновление azure-mgmt-hdinsight до версии 1.3.0</span><span class="sxs-lookup"><span data-stu-id="cd667-934">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="cd667-935">Прочее</span><span class="sxs-lookup"><span data-stu-id="cd667-935">Misc.</span></span>

* <span data-ttu-id="cd667-936">Добавлена команда `az version show` предварительного просмотра для отображения версий модулей и расширений Azure CLI в формате JSON по умолчанию или в формате, настроенном с помощью параметра --output</span><span class="sxs-lookup"><span data-stu-id="cd667-936">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="cd667-937">Центры событий</span><span class="sxs-lookup"><span data-stu-id="cd667-937">Event Hubs</span></span>

* <span data-ttu-id="cd667-938">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az eventhubs eventhub update и az eventhubs eventhub create.</span><span class="sxs-lookup"><span data-stu-id="cd667-938">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="cd667-939">Данный параметр недопустим для сущностей концентратора событий.</span><span class="sxs-lookup"><span data-stu-id="cd667-939">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="cd667-940">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="cd667-940">Service Bus</span></span>

* <span data-ttu-id="cd667-941">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az servicebus topic create, az servicebus topic update, az servicebus queue create и az servicebus queue update.</span><span class="sxs-lookup"><span data-stu-id="cd667-941">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="cd667-942">Этот параметр является недопустимым для разделов и очередей служебной шины.</span><span class="sxs-lookup"><span data-stu-id="cd667-942">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="cd667-943">RBAC</span><span class="sxs-lookup"><span data-stu-id="cd667-943">RBAC</span></span>

* <span data-ttu-id="cd667-944">Устранена проблема № 11712: команда `az ad app/sp show` не возвращала код выхода 3, если приложение или субъект-служба не существует.</span><span class="sxs-lookup"><span data-stu-id="cd667-944">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-945">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-945">Storage</span></span>

* <span data-ttu-id="cd667-946">`az storage account create`: удален флаг предварительного просмотра для параметра --enable-hierarchical-namespace.</span><span class="sxs-lookup"><span data-stu-id="cd667-946">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="cd667-947">Хранилище azure-mgmt-storage обновлено до версии 7.0.0 для использования API версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="cd667-947">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="cd667-948">Добавлены новые параметры (`--enable-delete-retention` и `--delete-retention-days`) для поддержки управления политикой хранения удаленных свойств службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="cd667-948">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="cd667-949">17 декабря 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-949">December 17, 2019</span></span>

<span data-ttu-id="cd667-950">2.0.78</span><span class="sxs-lookup"><span data-stu-id="cd667-950">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-951">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-951">ACR</span></span>

* <span data-ttu-id="cd667-952">Добавлена поддержка локального контекста во время выполнения задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="cd667-952">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-953">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-953">ACS</span></span>

* <span data-ttu-id="cd667-954">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде az openshift create параметр `--workspace-resource-id` переименован на `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="cd667-954">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="cd667-955">AMS</span><span class="sxs-lookup"><span data-stu-id="cd667-955">AMS</span></span>

* <span data-ttu-id="cd667-956">Команды show обновлены для возвращения ответа 3, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="cd667-956">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="cd667-957">AppConfig</span><span class="sxs-lookup"><span data-stu-id="cd667-957">AppConfig</span></span>

* <span data-ttu-id="cd667-958">Исправлена ошибка, возникающая при добавлении api-version в URL-адрес запроса.</span><span class="sxs-lookup"><span data-stu-id="cd667-958">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="cd667-959">Имеющееся решение не работает с разбивкой на страницы.</span><span class="sxs-lookup"><span data-stu-id="cd667-959">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="cd667-960">Добавлена поддержка отображения языков, кроме английского, так как наша внутренняя служба поддерживает Юникод для глобализации.</span><span class="sxs-lookup"><span data-stu-id="cd667-960">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-961">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-961">AppService</span></span>

* <span data-ttu-id="cd667-962">Устранена проблема № 11217 (webapp): теперь команда az webapp config ssl upload поддерживает параметр слота.</span><span class="sxs-lookup"><span data-stu-id="cd667-962">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="cd667-963">Устранена проблема № 10965. Ошибка: Имя не может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="cd667-963">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="cd667-964">Разрешено удаление по IP-адресу и подсети.</span><span class="sxs-lookup"><span data-stu-id="cd667-964">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="cd667-965">Добавлена поддержка импорта сертификатов из хранилища ключей: `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="cd667-965">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="cd667-966">ARM</span><span class="sxs-lookup"><span data-stu-id="cd667-966">ARM</span></span>

* <span data-ttu-id="cd667-967">Обновлен пакет ресурсов azure-mgmt-resource для использования версии 6.0.0</span><span class="sxs-lookup"><span data-stu-id="cd667-967">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="cd667-968">Добавлена межклиентская поддержка команды `az group deployment create` путем добавления нового параметра `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="cd667-968">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="cd667-969">Добавлен новый параметр `--metadata` для поддержки добавления метаданных определений наборов политик.</span><span class="sxs-lookup"><span data-stu-id="cd667-969">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="cd667-970">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="cd667-970">Backup</span></span>

* <span data-ttu-id="cd667-971">Добавлена поддержка резервного копирования для рабочей нагрузки SQL и SAP HANA.</span><span class="sxs-lookup"><span data-stu-id="cd667-971">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="cd667-972">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="cd667-972">BotService</span></span>

* <span data-ttu-id="cd667-973">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг --version из предварительной версии команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="cd667-973">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="cd667-974">Поддерживаются только боты пакетов SDK версии 4.</span><span class="sxs-lookup"><span data-stu-id="cd667-974">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="cd667-975">Добавлена проверка доступности имени для команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="cd667-975">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="cd667-976">Добавлена поддержка обновления URL-адреса значка для бота с помощью команды az bot update.</span><span class="sxs-lookup"><span data-stu-id="cd667-976">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="cd667-977">Добавлена поддержка обновления канала Direct Line с помощью команды az bot directline update.</span><span class="sxs-lookup"><span data-stu-id="cd667-977">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="cd667-978">Добавлена поддержка флага --enable-enhanced-auth в команде az bot directline create.</span><span class="sxs-lookup"><span data-stu-id="cd667-978">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="cd667-979">Следующие группы команд предоставляются в общедоступной, а не в предварительной версии: az bot authsetting.</span><span class="sxs-lookup"><span data-stu-id="cd667-979">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="cd667-980">Следующие команды в az bot предоставляются в общедоступной, а не в предварительной версии: create, prepare-deploy, show, delete и update.</span><span class="sxs-lookup"><span data-stu-id="cd667-980">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="cd667-981">Устранена проблема с командой az bot prepare-deploy, которая изменяла значение параметра --proj-file-path на нижний регистр (например, с Test.csproj на test.csproj).</span><span class="sxs-lookup"><span data-stu-id="cd667-981">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-982">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="cd667-982">Compute</span></span>

* <span data-ttu-id="cd667-983">vmss create/update: добавлен параметр --scale-on-policy, который определяет, какие виртуальные машины выбираются для удаления при масштабировании VMSS.</span><span class="sxs-lookup"><span data-stu-id="cd667-983">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="cd667-984">vm/vmss update: добавлен параметр --priority.</span><span class="sxs-lookup"><span data-stu-id="cd667-984">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="cd667-985">vm/vmss update: добавлен параметр --max-price.</span><span class="sxs-lookup"><span data-stu-id="cd667-985">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="cd667-986">Добавлена группа команд для шифрования дисков (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="cd667-986">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="cd667-987">disk create: добавлены параметры --encryption-type и --disk-encryption-set.</span><span class="sxs-lookup"><span data-stu-id="cd667-987">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="cd667-988">vm/vmss create. Добавлены параметры --os-disk-encryption-set и --data-disk-encryption-sets.</span><span class="sxs-lookup"><span data-stu-id="cd667-988">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="cd667-989">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-989">Core</span></span>

* <span data-ttu-id="cd667-990">Удалена поддержка Python версии 3.4.</span><span class="sxs-lookup"><span data-stu-id="cd667-990">Removed support for Python 3.4</span></span>
* <span data-ttu-id="cd667-991">Подключение к опросу HaTS в нескольких командах.</span><span class="sxs-lookup"><span data-stu-id="cd667-991">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="cd667-992">DLS</span><span class="sxs-lookup"><span data-stu-id="cd667-992">DLS</span></span>

* <span data-ttu-id="cd667-993">Обновлена версия пакета SDK для ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="cd667-993">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="cd667-994">Установка</span><span class="sxs-lookup"><span data-stu-id="cd667-994">Install</span></span>

* <span data-ttu-id="cd667-995">Добавлена поддержка установки скриптов Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="cd667-995">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-996">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-996">IOT</span></span>

* <span data-ttu-id="cd667-997">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --failover-region из команды manual-failover.</span><span class="sxs-lookup"><span data-stu-id="cd667-997">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="cd667-998">Теперь она будет выполнять отработку отказа в назначенный геопарный дополнительный регион.</span><span class="sxs-lookup"><span data-stu-id="cd667-998">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="cd667-999">Key Vault</span><span class="sxs-lookup"><span data-stu-id="cd667-999">Key Vault</span></span>

* <span data-ttu-id="cd667-1000">Устранена проблема № 8095: (`az keyvault storage remove`): улучшено справочное сообщение.</span><span class="sxs-lookup"><span data-stu-id="cd667-1000">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="cd667-1001">Устранена проблема № 8921 (`az keyvault key/secret/certificate list/list-deleted/list-versions`): исправлена ошибка проверки в параметре `--maxresults`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1001">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="cd667-1002">Устранена проблема № 10512 (`az keyvault set-policy`): улучшено сообщение об ошибке, возвращаемое, если не указан ни один из параметров `--object-id`, `--spn` или `--upn`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1002">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="cd667-1003">Устранена проблема № 10846 (`az keyvault secret show-deleted`): при указании значения `--id` значение `--name/-n` не требовалось.</span><span class="sxs-lookup"><span data-stu-id="cd667-1003">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="cd667-1004">Устранена проблема № 11084: (`az keyvault secret download`): улучшено справочное сообщение параметра `--encoding`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1004">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="cd667-1005">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-1005">Network</span></span>

* <span data-ttu-id="cd667-1006">az network application-gateway probe: добавлена поддержка параметра --port, позволяющего указать порт, который используется для проверки внутренних серверов при создании и обновлении.</span><span class="sxs-lookup"><span data-stu-id="cd667-1006">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="cd667-1007">az network application-gateway url-path-map create/update: исправлена ошибка с `--waf-policy`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1007">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="cd667-1008">az network application-gateway: добавлена поддержка параметра `--rewrite-rule-set`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1008">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="cd667-1009">az network list-service-aliases: добавлена поддержка перечисления псевдонимов служб, которые можно использовать для политик конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="cd667-1009">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="cd667-1010">az network dns zone import: добавлена поддержка символа .@ в имени записи.</span><span class="sxs-lookup"><span data-stu-id="cd667-1010">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="cd667-1011">Упаковка</span><span class="sxs-lookup"><span data-stu-id="cd667-1011">Packaging</span></span>

* <span data-ttu-id="cd667-1012">Снова добавлены сборки Edge для установки PIP.</span><span class="sxs-lookup"><span data-stu-id="cd667-1012">Added back edge builds for pip install</span></span>
* <span data-ttu-id="cd667-1013">Добавлен пакет Ubuntu eoan.</span><span class="sxs-lookup"><span data-stu-id="cd667-1013">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="cd667-1014">Политика</span><span class="sxs-lookup"><span data-stu-id="cd667-1014">Policy</span></span>

* <span data-ttu-id="cd667-1015">Добавлена поддержка API Политики версии 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="cd667-1015">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="cd667-1016">az policy set-definition: добавлена поддержка группирования в определениях наборов политик с помощью параметра `--definition-groups`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1016">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="cd667-1017">Redis</span><span class="sxs-lookup"><span data-stu-id="cd667-1017">Redis</span></span>

* <span data-ttu-id="cd667-1018">В команду `az redis create` добавлена предварительная версия параметра `--replicas-per-master`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1018">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="cd667-1019">Обновлена версия azure-mgmt-redis с 6.0.0 на 7.0.0 RC1.</span><span class="sxs-lookup"><span data-stu-id="cd667-1019">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="cd667-1020">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="cd667-1020">ServiceFabric</span></span>

* <span data-ttu-id="cd667-1021">Исправлена логика добавления типа узла, а также устранена проблема № 10963: при добавлении нового типа узла с уровнем устойчивости Gold возникала ошибка CLI.</span><span class="sxs-lookup"><span data-stu-id="cd667-1021">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="cd667-1022">Обновлена версия параметра ServiceFabricNodeVmExt до 1.1 в шаблоне создания.</span><span class="sxs-lookup"><span data-stu-id="cd667-1022">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-1023">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-1023">SQL</span></span>

* <span data-ttu-id="cd667-1024">В команды create и update базы данных SQL добавлены параметры --read-scale и --read-replicas для поддержки управления масштабированием операций чтения.</span><span class="sxs-lookup"><span data-stu-id="cd667-1024">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-1025">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-1025">Storage</span></span>

* <span data-ttu-id="cd667-1026">Выпущена общедоступная версия больших файловых ресурсов для команды создания и обновления учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="cd667-1026">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="cd667-1027">Выпущена общедоступная версия поддержки маркера SAS для делегирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd667-1027">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="cd667-1028">Добавлены новые команды (`az storage account blob-service-properties show` и `az storage account blob-service-properties update --enable-change-feed`) для управления свойствами службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="cd667-1028">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="cd667-1029">[ОЖИДАЕТСЯ КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] `az storage copy`: символ `*` больше не поддерживается в качестве подстановочного знака в URL-адресе. Тем не менее новые параметры--include-pattern и--exclude-pattern будут добавлены с поддержкой подстановочных знаков `*`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1029">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="cd667-1030">Устранена проблема № 11043: добавлена поддержка удаления всего контейнера или общего ресурса в команде `az storage remove`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1030">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="cd667-1031">26 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1031">November 26, 2019</span></span>

<span data-ttu-id="cd667-1032">Версия 2.0.77</span><span class="sxs-lookup"><span data-stu-id="cd667-1032">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-1033">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-1033">ACR</span></span>

* <span data-ttu-id="cd667-1034">Параметр `--branch`, используемый при обновлении или создании задачи ACR, объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="cd667-1034">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="cd667-1035">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="cd667-1035">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="cd667-1036">Добавлен флаг `--workspace-resource-id` для создания кластера Azure Red Hat Openshift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="cd667-1036">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="cd667-1037">Добавлен флаг `monitor_profile` для создания кластера Azure Red Hat OpenShift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="cd667-1037">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="cd667-1038">AKS</span><span class="sxs-lookup"><span data-stu-id="cd667-1038">AKS</span></span>

* <span data-ttu-id="cd667-1039">Включена поддержка операции смены сертификата кластера с использованием команды az aks rotate-certs.</span><span class="sxs-lookup"><span data-stu-id="cd667-1039">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="cd667-1040">AppConfig</span><span class="sxs-lookup"><span data-stu-id="cd667-1040">AppConfig</span></span>

* <span data-ttu-id="cd667-1041">Включена поддержка использования символа ":" для разделителя `as az appconfig kv import`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1041">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="cd667-1042">Исправлена проблема с перечислением значений ключей с несколькими метками, включая метку NULL.</span><span class="sxs-lookup"><span data-stu-id="cd667-1042">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="cd667-1043">Обновлен пакет SDK для плоскости управления, azure-mgmt-appconfiguration, до версии 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="cd667-1043">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="cd667-1044">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-1044">AppService</span></span>

* <span data-ttu-id="cd667-1045">Исправлена ошибка № 11100. Использование AttributeError для az webapp up при создании плана службы.</span><span class="sxs-lookup"><span data-stu-id="cd667-1045">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="cd667-1046">az webapp up. При принудительном создании или развертывании сайта для поддерживаемых языков значения по умолчанию не используются.</span><span class="sxs-lookup"><span data-stu-id="cd667-1046">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="cd667-1047">Включена поддержка Среды службы приложений: az appservice ase show | list | list-addresses | list-plans | create | update | delete.</span><span class="sxs-lookup"><span data-stu-id="cd667-1047">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="cd667-1048">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="cd667-1048">Backup</span></span>

* <span data-ttu-id="cd667-1049">Исправлена проблема в команде az backup policy list-associated-items.</span><span class="sxs-lookup"><span data-stu-id="cd667-1049">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="cd667-1050">Добавлен необязательный параметр BackupManagementType.</span><span class="sxs-lookup"><span data-stu-id="cd667-1050">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-1051">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="cd667-1051">Compute</span></span>

* <span data-ttu-id="cd667-1052">Обновлена версия API вычислений, дисков, моментальных снимков до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="cd667-1052">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="cd667-1053">vmss create. Улучшение для --orchestration-mode.</span><span class="sxs-lookup"><span data-stu-id="cd667-1053">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="cd667-1054">sig image-definition create. Добавлен параметр --os-state для указания того, являются ли виртуальные машины, созданные в этом образе, универсальными или специализированными.</span><span class="sxs-lookup"><span data-stu-id="cd667-1054">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="cd667-1055">sig image-definition create. Добавлен параметр --hyper-v-generation для указания создания гипервизора.</span><span class="sxs-lookup"><span data-stu-id="cd667-1055">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="cd667-1056">sig image-version create. Включена поддержка параметров --os-snapshot и --data-snapshots.</span><span class="sxs-lookup"><span data-stu-id="cd667-1056">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="cd667-1057">image create. Включена поддержка параметра --data-disk-caching для указания параметра кэширования для дисков данных.</span><span class="sxs-lookup"><span data-stu-id="cd667-1057">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="cd667-1058">Обновлена версия пакета SDK для вычислений Python до 10.0.0.</span><span class="sxs-lookup"><span data-stu-id="cd667-1058">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="cd667-1059">vm/vmss create. Добавлен фрагмент Spot в свойство перечисления Priority.</span><span class="sxs-lookup"><span data-stu-id="cd667-1059">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="cd667-1060">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименование параметра --max-billing в --max-price для виртуальных машин и Масштабируемых наборов виртуальных машин в соответствии с командлетами Swagger и PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cd667-1060">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="cd667-1061">vm monitor log show. Включена поддержка запроса журналов в связанной рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="cd667-1061">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-1062">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-1062">IOT</span></span>

* <span data-ttu-id="cd667-1063">Исправление № 2531. Добавлены вспомогательные аргументы для обновления концентратора.</span><span class="sxs-lookup"><span data-stu-id="cd667-1063">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="cd667-1064">Исправление № 8323. Добавлены недостающие параметры для создания пользовательской конечной точки хранилища.</span><span class="sxs-lookup"><span data-stu-id="cd667-1064">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="cd667-1065">Исправлена ошибка регрессии. Отменены изменения, переопределяющие конечную точку хранилища по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-1065">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="cd667-1066">Key Vault</span><span class="sxs-lookup"><span data-stu-id="cd667-1066">Key Vault</span></span>

* <span data-ttu-id="cd667-1067">Исправление № 11121. При использовании `az keyvault certificate list` для передачи `--include-pending` теперь не требуется значение `true` или `false`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1067">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="cd667-1068">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="cd667-1068">NetAppFiles</span></span>

* <span data-ttu-id="cd667-1069">Обновлена версия azure-mgmt-netapp до 0.7.0, которая включает некоторые дополнительные свойства тома, связанные с предстоящими операциями репликации.</span><span class="sxs-lookup"><span data-stu-id="cd667-1069">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="cd667-1070">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-1070">Network</span></span>

* <span data-ttu-id="cd667-1071">application-gateway waf-config. Не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="cd667-1071">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="cd667-1072">application-gateway waf-policy. Добавлены управляемые правила подгрупп для контроля управляемых наборов правил и правил исключения.</span><span class="sxs-lookup"><span data-stu-id="cd667-1072">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="cd667-1073">application-gateway waf-policy. Добавлен параметр политики подгруппы для управления глобальной конфигурацией политики WAF.</span><span class="sxs-lookup"><span data-stu-id="cd667-1073">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="cd667-1074">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] application-gateway waf-policy. Переименовано правило подгруппы в пользовательское правило.</span><span class="sxs-lookup"><span data-stu-id="cd667-1074">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="cd667-1075">application-gateway http-listener. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="cd667-1075">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="cd667-1076">application-gateway url-path-map rule. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="cd667-1076">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="cd667-1077">Упаковка</span><span class="sxs-lookup"><span data-stu-id="cd667-1077">Packaging</span></span>

* <span data-ttu-id="cd667-1078">Удалена команда az wrapper в Python.</span><span class="sxs-lookup"><span data-stu-id="cd667-1078">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="cd667-1079">Включена поддержка Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="cd667-1079">Added support for Python 3.8</span></span>
* <span data-ttu-id="cd667-1080">Изменена версия на Python 3 для пакета RPM.</span><span class="sxs-lookup"><span data-stu-id="cd667-1080">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-1081">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-1081">Profile</span></span>

* <span data-ttu-id="cd667-1082">Исправлена ошибка при выполнении `az login -u {} -p {}` с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="cd667-1082">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="cd667-1083">Исправлена ошибка с `SSLError` при выполнении `az login` за прокси-сервером с самозаверяющим корневым сертификатом.</span><span class="sxs-lookup"><span data-stu-id="cd667-1083">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="cd667-1084">Исправлена ошибка № 10578. `az login` зависает при одновременном запуске нескольких экземпляров в Windows или WSL.</span><span class="sxs-lookup"><span data-stu-id="cd667-1084">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="cd667-1085">Исправлена ошибка № 11059. Сбой выполнения `az login --allow-no-subscriptions`, если в клиенте есть подписки.</span><span class="sxs-lookup"><span data-stu-id="cd667-1085">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="cd667-1086">Исправлена ошибка № 11238. После переименования подписки вход с помощью MSI приведет к тому, что одна и та же подписка появится дважды.</span><span class="sxs-lookup"><span data-stu-id="cd667-1086">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="cd667-1087">RBAC</span><span class="sxs-lookup"><span data-stu-id="cd667-1087">RBAC</span></span>

* <span data-ttu-id="cd667-1088">Исправлена ошибка № 10996. Исправлена ошибка с `--force-change-password-next-login` в `az ad user update`, если `--password` не указывается.</span><span class="sxs-lookup"><span data-stu-id="cd667-1088">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="cd667-1089">Redis</span><span class="sxs-lookup"><span data-stu-id="cd667-1089">Redis</span></span>

* <span data-ttu-id="cd667-1090">Исправлена ошибка № 2902. Предотвращена настройка конфигураций памяти при обновлении кэша с номером SKU "Базовый".</span><span class="sxs-lookup"><span data-stu-id="cd667-1090">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="cd667-1091">Резервирование</span><span class="sxs-lookup"><span data-stu-id="cd667-1091">Reservations</span></span>

* <span data-ttu-id="cd667-1092">Обновлена версия пакета SDK до 0.6.0</span><span class="sxs-lookup"><span data-stu-id="cd667-1092">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="cd667-1093">Добавлены сведения о плане выставления счетов после вызова Get-Catalogs.</span><span class="sxs-lookup"><span data-stu-id="cd667-1093">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="cd667-1094">Добавлена новая команда `az reservations reservation-order calculate` для вычисления стоимости резервирования.</span><span class="sxs-lookup"><span data-stu-id="cd667-1094">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="cd667-1095">Добавлена новая команда `az reservations reservation-order purchase` для приобретения нового резервирования.</span><span class="sxs-lookup"><span data-stu-id="cd667-1095">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="cd667-1096">Rest</span><span class="sxs-lookup"><span data-stu-id="cd667-1096">Rest</span></span>
* <span data-ttu-id="cd667-1097">Изменена версия `az rest` на общедоступную.</span><span class="sxs-lookup"><span data-stu-id="cd667-1097">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-1098">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-1098">SQL</span></span>

* <span data-ttu-id="cd667-1099">Обновлена версия azure-mgmt-sql до 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="cd667-1099">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-1100">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-1100">Storage</span></span>

* <span data-ttu-id="cd667-1101">storage account create. Добавлен параметр --enable-hierarchical-namespace для включения поддержки семантики файловой системы в службе больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="cd667-1101">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="cd667-1102">Удалено несвязанное исключение из сообщения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="cd667-1102">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="cd667-1103">Исправлены проблемы, из-за которых появлялось неверное сообщение об отсутствии нужных разрешений на выполнение требуемой операции</span><span class="sxs-lookup"><span data-stu-id="cd667-1103">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="cd667-1104">при блокировке правилами сети (AuthenticationFailed).</span><span class="sxs-lookup"><span data-stu-id="cd667-1104">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="cd667-1105">4 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1105">November 4, 2019</span></span>

<span data-ttu-id="cd667-1106">Версия 2.0.76</span><span class="sxs-lookup"><span data-stu-id="cd667-1106">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-1107">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-1107">ACR</span></span>

* <span data-ttu-id="cd667-1108">В команду `az acr pack build` добавлен параметр предварительной версии `--pack-image-tag`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1108">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="cd667-1109">Добавлена поддержка включения аудита при создании реестра.</span><span class="sxs-lookup"><span data-stu-id="cd667-1109">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="cd667-1110">Включена поддержка функции RBAC, распространяющаяся на репозиторий.</span><span class="sxs-lookup"><span data-stu-id="cd667-1110">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="cd667-1111">AKS</span><span class="sxs-lookup"><span data-stu-id="cd667-1111">AKS</span></span>

* <span data-ttu-id="cd667-1112">В команду `az aks create` добавлены `--enable-cluster-autoscaler`, `--min-count` и `--max-count`, что позволяет автоматически масштабировать кластер для пула узлов.</span><span class="sxs-lookup"><span data-stu-id="cd667-1112">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="cd667-1113">Добавлены указанные выше флаги, а также `--update-cluster-autoscaler` и `--disable-cluster-autoscaler` в команду `az aks update`, что позволяет обновлять средство автоматического масштабирования кластера.</span><span class="sxs-lookup"><span data-stu-id="cd667-1113">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="cd667-1114">AppConfig</span><span class="sxs-lookup"><span data-stu-id="cd667-1114">AppConfig</span></span>

* <span data-ttu-id="cd667-1115">Добавлена группа команд функции appconfig для управления флагами функций, хранимыми в Конфигурации приложений.</span><span class="sxs-lookup"><span data-stu-id="cd667-1115">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="cd667-1116">Исправлена незначительная ошибка команды экспорта в файл appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="cd667-1116">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="cd667-1117">Прерывание чтения содержимого конечного файла во время экспорта.</span><span class="sxs-lookup"><span data-stu-id="cd667-1117">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-1118">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-1118">AppService</span></span>

* <span data-ttu-id="cd667-1119">`az appservice plan create`: Добавлена поддержка определения persitescaling при создании плана appservice.</span><span class="sxs-lookup"><span data-stu-id="cd667-1119">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="cd667-1120">Исправлена проблема, из-за которой операция webapp config ssl bind удаляла существующие теги из ресурса.</span><span class="sxs-lookup"><span data-stu-id="cd667-1120">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="cd667-1121">Добавлен флаг `--build-remote` для `az functionapp deployment source config-zip` для включения поддержки действия удаленной сборки во время развертывания приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="cd667-1121">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="cd667-1122">Изменена версия узла по умолчанию для приложений-функций на ~10 для Windows</span><span class="sxs-lookup"><span data-stu-id="cd667-1122">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="cd667-1123">В `az functionapp create` добавлено свойство `--runtime-version`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1123">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="cd667-1124">ARM</span><span class="sxs-lookup"><span data-stu-id="cd667-1124">ARM</span></span>

* <span data-ttu-id="cd667-1125">`az deployment/group deployment validate`: В `--handle-extended-json-format` добавлен параметр для включения поддержки многострочности и комментариев в шаблоне JSON при развертывании.</span><span class="sxs-lookup"><span data-stu-id="cd667-1125">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="cd667-1126">Версия azure-mgmt-resource обновлена до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="cd667-1126">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="cd667-1127">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="cd667-1127">Backup</span></span>

* <span data-ttu-id="cd667-1128">Добавлена поддержка резервного копирования AzureFiles.</span><span class="sxs-lookup"><span data-stu-id="cd667-1128">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-1129">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="cd667-1129">Compute</span></span>

* <span data-ttu-id="cd667-1130">`az vm create`: Добавлено предупреждение при одновременном определении ускоренной сети и существующей сетевой карты.</span><span class="sxs-lookup"><span data-stu-id="cd667-1130">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="cd667-1131">`az vm create`: Добавлен параметр `--vmss` для определения существующего масштабируемого набора виртуальных машин, которому должна быть назначена виртуальная машина.</span><span class="sxs-lookup"><span data-stu-id="cd667-1131">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="cd667-1132">`az vm/vmss create`: Добавлена локальная копия файла псевдонима изображения, к которой можно получить доступ в ограниченной сетевой среде.</span><span class="sxs-lookup"><span data-stu-id="cd667-1132">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="cd667-1133">`az vmss create`: Добавлен параметр `--orchestration-mode` для определения того, как виртуальные машины управляются масштабируемым набором.</span><span class="sxs-lookup"><span data-stu-id="cd667-1133">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="cd667-1134">`az vm/vmss update`: Добавлен параметр `--ultra-ssd-enabled`, чтобы разрешить обновление параметра Ultra SSD.</span><span class="sxs-lookup"><span data-stu-id="cd667-1134">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="cd667-1135">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az vm extension set`: Исправлена ошибка, из-за которой пользователям не удавалось определять расширение на виртуальной машине с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1135">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="cd667-1136">Добавлены новые команды `az vm image terms accept/cancel/show` для управления условиями использования образов Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="cd667-1136">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="cd667-1137">Расширение VMAccessForLinux обновлено до версии 1.5.</span><span class="sxs-lookup"><span data-stu-id="cd667-1137">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="cd667-1138">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-1138">CosmosDB</span></span>

* <span data-ttu-id="cd667-1139">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql container create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="cd667-1139">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="cd667-1140">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az gremlin graph create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="cd667-1140">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="cd667-1141">`az sql container create`: Добавлены команды `--unique-key-policy` и `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1141">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="cd667-1142">`az sql container create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-1142">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="cd667-1143">`gremlin graph create`: Добавлена команда `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1143">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="cd667-1144">`gremlin graph create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-1144">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="cd667-1145">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="cd667-1145">Fixed typo in help message</span></span>
* <span data-ttu-id="cd667-1146">База данных: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="cd667-1146">database: Added deprecation information</span></span>
* <span data-ttu-id="cd667-1147">Коллекция: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="cd667-1147">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-1148">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-1148">IoT</span></span>

* <span data-ttu-id="cd667-1149">Добавлен новый тип источника маршрутизации: DigitalTwinChangeEvents.</span><span class="sxs-lookup"><span data-stu-id="cd667-1149">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="cd667-1150">Добавлены отсутствующие компоненты в `az iot hub create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1150">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="cd667-1151">Key Vault</span><span class="sxs-lookup"><span data-stu-id="cd667-1151">Key Vault</span></span>

* <span data-ttu-id="cd667-1152">Исправлена непредвиденная ошибка с отсутствием файла сертификата.</span><span class="sxs-lookup"><span data-stu-id="cd667-1152">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="cd667-1153">Исправлена ошибка с неработающей командой `az keyvault recover/purge`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1153">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="cd667-1154">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="cd667-1154">NetAppFiles</span></span>

* <span data-ttu-id="cd667-1155">Пакет azure-mgmt-netapp обновлен до версии 0.6.0 для включения поддержки API версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="cd667-1155">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="cd667-1156">Эта новая версия API включает:</span><span class="sxs-lookup"><span data-stu-id="cd667-1156">This new API version includes:</span></span>

    - <span data-ttu-id="cd667-1157">При создании тома с использованием `--protocol-types` допускается NFSv4.1 вместо NFSv4.</span><span class="sxs-lookup"><span data-stu-id="cd667-1157">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="cd667-1158">Свойство политики экспорта томов теперь называется nfsv41, а не nfsv4.</span><span class="sxs-lookup"><span data-stu-id="cd667-1158">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="cd667-1159">Параметр `--creation-token` для тома переименован в `--file-path`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1159">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="cd667-1160">Дата создания моментального снимка теперь имеет значение Created.</span><span class="sxs-lookup"><span data-stu-id="cd667-1160">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="cd667-1161">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-1161">Network</span></span>

* <span data-ttu-id="cd667-1162">`az network private-dns link vnet create/update`: Добавлена поддержка связывания виртуальных сетей между клиентами.</span><span class="sxs-lookup"><span data-stu-id="cd667-1162">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="cd667-1163">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az network vnet subnet list`: Параметры `--resource-group` и `--vnet-name` теперь являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="cd667-1163">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="cd667-1164">`az network public-ip prefix create`: Включена поддержка определения версии IP-адреса (IPv4, IPv6) при создании.</span><span class="sxs-lookup"><span data-stu-id="cd667-1164">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="cd667-1165">Версия azure-mgmt-network обновлена до 7.0.0 и версия api-version до 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="cd667-1165">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="cd667-1166">`az network vrouter`: Включена поддержка нового виртуального маршрутизатора службы и пиринга виртуальных маршрутизаторов.</span><span class="sxs-lookup"><span data-stu-id="cd667-1166">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="cd667-1167">`az network express-route gateway connection`: Добавлена поддержка параметра `--internet-security`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1167">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-1168">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-1168">Profile</span></span>

* <span data-ttu-id="cd667-1169">Исправлена ошибка с неработающей командой `az account get-access-token --resource-type ms-graph`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1169">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="cd667-1170">Удалено предупреждение из `az login`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1170">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="cd667-1171">RBAC</span><span class="sxs-lookup"><span data-stu-id="cd667-1171">RBAC</span></span>

* <span data-ttu-id="cd667-1172">Исправление `az ad app update --id {} --display-name {}` не работает.</span><span class="sxs-lookup"><span data-stu-id="cd667-1172">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="cd667-1173">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="cd667-1173">ServiceFabric</span></span>

* <span data-ttu-id="cd667-1174">`az sf cluster create`: Исправлена проблема путем изменения VMSS для вычислений с использованием файла template.json для Service Fabric Linux и Windows со стандартных дисков на управляемые.</span><span class="sxs-lookup"><span data-stu-id="cd667-1174">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-1175">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-1175">SQL</span></span>

* <span data-ttu-id="cd667-1176">Добавлены параметры `--compute-model`, `--auto-pause-delay` и `--min-capacity` для включения поддержки операций CRUD для нового предложения Базы данных SQL: Модель бессерверных вычислений.</span><span class="sxs-lookup"><span data-stu-id="cd667-1176">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-1177">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-1177">Storage</span></span>

* <span data-ttu-id="cd667-1178">`az storage account create/update`: Добавлен параметр --enable-files-adds и группа аргументов свойств Azure Active Directory для включения поддержки аутентификации доменных служб Azure Active Directory для Файлов Azure.</span><span class="sxs-lookup"><span data-stu-id="cd667-1178">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="cd667-1179">Расширена команда `az storage account keys list/renew` для включения поддержки перечисления или повторного создания ключей Kerberos для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="cd667-1179">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="cd667-1180">15 октября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1180">October 15, 2019</span></span>

<span data-ttu-id="cd667-1181">Версия 2.0.75</span><span class="sxs-lookup"><span data-stu-id="cd667-1181">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="cd667-1182">AKS</span><span class="sxs-lookup"><span data-stu-id="cd667-1182">AKS</span></span>

* <span data-ttu-id="cd667-1183">Для параметра `--load-balancer-sku` изменено значение по умолчанию на `standard`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="cd667-1183">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="cd667-1184">Для параметра `--vm-set-type` изменено значение по умолчанию на `virtualmachinescalesets`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="cd667-1184">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="cd667-1185">AMS</span><span class="sxs-lookup"><span data-stu-id="cd667-1185">AMS</span></span>

* <span data-ttu-id="cd667-1186">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя `job start` изменено на `job create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1186">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="cd667-1187">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В параметре `--ask` команды `content-key-policy create` вместо кодировки UTF8 теперь используется шестнадцатеричная строка из 32 символов.</span><span class="sxs-lookup"><span data-stu-id="cd667-1187">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-1188">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-1188">AppService</span></span>

* <span data-ttu-id="cd667-1189">Добавлены команды `webapp config access-restriction show|set|add|remove`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1189">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="cd667-1190">Улучшена обработка ошибок в `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1190">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="cd667-1191">Для `appservice plan update` добавлена поддержка номера SKU `Isolated`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1191">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="cd667-1192">ARM</span><span class="sxs-lookup"><span data-stu-id="cd667-1192">ARM</span></span>

* <span data-ttu-id="cd667-1193">В `deployment create` добавлен параметр `--handle-extended-json-format` для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="cd667-1193">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-1194">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="cd667-1194">Compute</span></span>

* <span data-ttu-id="cd667-1195">Добавлен параметр `--enable-agent` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1195">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="cd667-1196">Внесены изменения в `vm create`, позволяющие автоматически использовать номер SKU "Стандартный" для общедоступных IP-адресов при использовании зон.</span><span class="sxs-lookup"><span data-stu-id="cd667-1196">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="cd667-1197">Внесены изменения в `vm create`, позволяющие автоматически создавать допустимое имя для виртуальной машины, если оно не задано.</span><span class="sxs-lookup"><span data-stu-id="cd667-1197">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="cd667-1198">В `vmss create` добавлен параметр `--computer-name-prefix` для поддержки пользовательского префикса имени для виртуальных машин в VMSS.</span><span class="sxs-lookup"><span data-stu-id="cd667-1198">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="cd667-1199">В `vm create` добавлен параметр `--workspace` для автоматического включения рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="cd667-1199">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="cd667-1200">API коллекций обновлен до версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="cd667-1200">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="cd667-1201">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-1201">Core</span></span>

* <span data-ttu-id="cd667-1202">Добавлена проверка синтаксиса для параметра `--set` в универсальной команде обновления.</span><span class="sxs-lookup"><span data-stu-id="cd667-1202">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-1203">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-1203">IoT</span></span>

* <span data-ttu-id="cd667-1204">Исправлена проблема, при которой `iot hub show` неправильно выдавал ошибку "Ресурс не найден".</span><span class="sxs-lookup"><span data-stu-id="cd667-1204">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-1205">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-1205">Monitor</span></span>

* <span data-ttu-id="cd667-1206">В `monitor log-analytics workspace` добавлена поддержка CRUD.</span><span class="sxs-lookup"><span data-stu-id="cd667-1206">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="cd667-1207">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-1207">Network</span></span>

* <span data-ttu-id="cd667-1208">В `network private-dns link vnet [create|update]` добавлена поддержка виртуального канала для клиентов.</span><span class="sxs-lookup"><span data-stu-id="cd667-1208">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="cd667-1209">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для `network vnet subnet list` теперь требуются параметры `--resource-group` и `--vnet-name`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1209">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-1210">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-1210">SQL</span></span>

* <span data-ttu-id="cd667-1211">В `sql mi ad-admin` добавлены команды, которые поддерживают назначение администратора AAD в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="cd667-1211">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-1212">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-1212">Storage</span></span>

* <span data-ttu-id="cd667-1213">В `storage copy` добавлен параметр `--preserve-s2s-access-tier`, позволяющий сохранить уровень доступа во время копирования между службами.</span><span class="sxs-lookup"><span data-stu-id="cd667-1213">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="cd667-1214">В `storage account [create|update]` добавлен параметр `--enable-large-file-share` для поддержки общих папок большого размера в учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="cd667-1214">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="cd667-1215">24 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1215">September 24, 2019</span></span>

<span data-ttu-id="cd667-1216">Версия 2.0.74</span><span class="sxs-lookup"><span data-stu-id="cd667-1216">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-1217">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-1217">ACR</span></span>

* <span data-ttu-id="cd667-1218">В `acr config retention update` добавлен обязательный параметр `--type`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1218">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="cd667-1219">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованный параметр `--name -n` изменен на `--registry -r ` для группы команд `acr config`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1219">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="cd667-1220">AKS</span><span class="sxs-lookup"><span data-stu-id="cd667-1220">AKS</span></span>

* <span data-ttu-id="cd667-1221">В команду `aks create` добавлен параметр `--load-balancer-sku`, позволяющий создать кластер AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="cd667-1221">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="cd667-1222">В команды `aks [create|update]` добавлены параметры `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` и `--load-balancer-outbound-ip-prefixes`, позволяющие обновлять профиль подсистемы балансировки нагрузки у кластера AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="cd667-1222">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="cd667-1223">В команду `aks create` добавлен параметр `--vm-set-type`, позволяющий указывать типы виртуальных машин в кластере AKS.</span><span class="sxs-lookup"><span data-stu-id="cd667-1223">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="cd667-1224">ARM</span><span class="sxs-lookup"><span data-stu-id="cd667-1224">ARM</span></span>

* <span data-ttu-id="cd667-1225">В команду `group deployment create` добавлен параметр `--handle-extended-json-format`, для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="cd667-1225">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-1226">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="cd667-1226">Compute</span></span>

* <span data-ttu-id="cd667-1227">В команды `vmss [create|update]` добавлен параметр `--terminate-notification-time`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="cd667-1227">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="cd667-1228">В команду `vmss update` добавлен параметр `--enable-terminate-notification`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="cd667-1228">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="cd667-1229">В команды `[vm|vmss] create` добавлены параметры `--priority,`, `--eviction-policy,` и `--max-billing`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1229">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="cd667-1230">Изменена команда `disk create`, которая теперь позволяет указать точный размер отправки на диск.</span><span class="sxs-lookup"><span data-stu-id="cd667-1230">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="cd667-1231">В `snapshot create` добавлена поддержка добавочных моментальных снимков для управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="cd667-1231">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="cd667-1232">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-1232">Cosmos DB</span></span>

* <span data-ttu-id="cd667-1233">В команду `cosmosdb keys list` добавлен параметр `--type <key-type>` для отображения ключей, ключей только для чтения или строк подключения.</span><span class="sxs-lookup"><span data-stu-id="cd667-1233">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="cd667-1234">Добавлена команда `cosmosdb keys regenerate`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1234">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="cd667-1235">[УСТАРЕЛО] Команды `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` и `cosmosdb list-read-only-keys` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="cd667-1235">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="cd667-1236">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="cd667-1236">EventGrid</span></span>

* <span data-ttu-id="cd667-1237">Исправлен текст справки по конечной точке — дана ссылка на правильный параметр.</span><span class="sxs-lookup"><span data-stu-id="cd667-1237">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="cd667-1238">Key Vault</span><span class="sxs-lookup"><span data-stu-id="cd667-1238">Key Vault</span></span>

* <span data-ttu-id="cd667-1239">Исправлена проблема, из-за которой вход с помощью клиента (`login -t`) мог приводить к сбою `keyvault create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1239">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-1240">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-1240">Monitor</span></span>

* <span data-ttu-id="cd667-1241">Исправлена проблема с тем, что символ `:` являлся недопустимым в аргументе `--condition` для `monitor metrics alert create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1241">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="cd667-1242">Политика</span><span class="sxs-lookup"><span data-stu-id="cd667-1242">Policy</span></span>

* <span data-ttu-id="cd667-1243">Добавлена поддержка API Политики версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="cd667-1243">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="cd667-1244">В команду `policy assignment create` добавлен параметр `--enforcement-mode`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1244">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-1245">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-1245">Storage</span></span>

* <span data-ttu-id="cd667-1246">В команду `az storage copy` добавлен параметр `--blob-type`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1246">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="cd667-1247">10 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1247">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-1248">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-1248">ACR</span></span>

* <span data-ttu-id="cd667-1249">Добавлена группа команд `acr config retention` для настройки политики хранения.</span><span class="sxs-lookup"><span data-stu-id="cd667-1249">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="cd667-1250">AKS</span><span class="sxs-lookup"><span data-stu-id="cd667-1250">AKS</span></span>

* <span data-ttu-id="cd667-1251">Добавлена возможность интеграции ACR с помощью следующих команд:</span><span class="sxs-lookup"><span data-stu-id="cd667-1251">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="cd667-1252">В `aks [create|update]` добавлен параметр `--attach-acr` для подключения ACR к кластеру AKS.</span><span class="sxs-lookup"><span data-stu-id="cd667-1252">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="cd667-1253">В `aks update` добавлен параметр `--detach-acr` для отключения ACR от кластера AKS.</span><span class="sxs-lookup"><span data-stu-id="cd667-1253">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="cd667-1254">ARM</span><span class="sxs-lookup"><span data-stu-id="cd667-1254">ARM</span></span>

* <span data-ttu-id="cd667-1255">Добавлена возможность использования API версии 2019-05-10.</span><span class="sxs-lookup"><span data-stu-id="cd667-1255">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="cd667-1256">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-1256">Batch</span></span>

* <span data-ttu-id="cd667-1257">Добавлены новые параметры конфигурации JSON в `--json-file` для `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="cd667-1257">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="cd667-1258">Добавлен параметр `MountConfigurations` для подключений файловой системы (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="cd667-1258">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="cd667-1259">Добавлено необязательное свойство `publicIPs` в `NetworkConfiguration` для общедоступных IP-адресов в пулах (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="cd667-1259">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="cd667-1260">В `--image` добавлена поддержка коллекций общих образов.</span><span class="sxs-lookup"><span data-stu-id="cd667-1260">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="cd667-1261">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `--start-task-wait-for-success` в `batch pool create` изменено на `true`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1261">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="cd667-1262">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `Scope` в `AutoUserSpecification` задано как Pool (ранее `Task` на узлах Windows и `Pool` на узлах Linux).</span><span class="sxs-lookup"><span data-stu-id="cd667-1262">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="cd667-1263">Этот аргумент можно задать только в конфигурации JSON с помощью `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1263">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="cd667-1264">HDInsight</span><span class="sxs-lookup"><span data-stu-id="cd667-1264">HDInsight</span></span>

* <span data-ttu-id="cd667-1265">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="cd667-1265">GA release</span></span>
* <span data-ttu-id="cd667-1266">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--workernode-count/-c` в `az hdinsight resize` теперь является обязательным.</span><span class="sxs-lookup"><span data-stu-id="cd667-1266">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="cd667-1267">Key Vault</span><span class="sxs-lookup"><span data-stu-id="cd667-1267">Key Vault</span></span>

* <span data-ttu-id="cd667-1268">Исправлена проблема, когда подсети не удавалось удалить из сетевых правил.</span><span class="sxs-lookup"><span data-stu-id="cd667-1268">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="cd667-1269">Исправлена проблема, когда дублированные подсети и IP-адреса могли быть добавлены к сетевым правилам.</span><span class="sxs-lookup"><span data-stu-id="cd667-1269">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="cd667-1270">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-1270">Network</span></span>

* <span data-ttu-id="cd667-1271">Добавлен параметр `--interval` в `network watcher flow-log` для выбора значения интервала анализа трафика.</span><span class="sxs-lookup"><span data-stu-id="cd667-1271">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="cd667-1272">Добавлена команда `network application-gateway identity` для управления удостоверением шлюза.</span><span class="sxs-lookup"><span data-stu-id="cd667-1272">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="cd667-1273">Добавлена возможность указать идентификатор Key Vault в команде `network application-gateway ssl-cert`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1273">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="cd667-1274">Добавлена команда `network express-route peering peer-connection [show|list]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1274">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="cd667-1275">Политика</span><span class="sxs-lookup"><span data-stu-id="cd667-1275">Policy</span></span>

* <span data-ttu-id="cd667-1276">Добавлена возможность использования API версии 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="cd667-1276">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="cd667-1277">27 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1277">August 27, 2019</span></span>

<span data-ttu-id="cd667-1278">Версия 2.0.72</span><span class="sxs-lookup"><span data-stu-id="cd667-1278">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-1279">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-1279">ACR</span></span>

* <span data-ttu-id="cd667-1280">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка SKU `classic`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1280">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="cd667-1281">Управление API</span><span class="sxs-lookup"><span data-stu-id="cd667-1281">API Management</span></span>

* <span data-ttu-id="cd667-1282">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена группа команд `apim`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1282">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-1283">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-1283">AppService</span></span>

* <span data-ttu-id="cd667-1284">Исправлена проблема с командой `webapp webjob continuous start` при указании слота.</span><span class="sxs-lookup"><span data-stu-id="cd667-1284">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="cd667-1285">Изменена команда `webapp up` для обнаружения и удаления папки `env` из файла, используемого для развертывания.</span><span class="sxs-lookup"><span data-stu-id="cd667-1285">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="cd667-1286">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="cd667-1286">Keyvault</span></span>

* <span data-ttu-id="cd667-1287">Исправлена ошибка в команде `keyvault secret set`, которая игнорировала аргумент `--expires`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1287">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="cd667-1288">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-1288">Network</span></span>

* <span data-ttu-id="cd667-1289">Добавлена поддержка IPv6-адресов для аргументов `--private-ip-address-version`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1289">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="cd667-1290">Добавлены новые команды `network private-endpoint [create|update|list-types]` для управления закрытыми конечными точками.</span><span class="sxs-lookup"><span data-stu-id="cd667-1290">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="cd667-1291">Добавлена группа команд для `network private-link-service`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1291">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="cd667-1292">Добавлены аргументы `--private-endpoint-network-policies` и `--private-link-service-network-policies` для команды `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="cd667-1292">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="cd667-1293">RBAC</span><span class="sxs-lookup"><span data-stu-id="cd667-1293">RBAC</span></span>

* <span data-ttu-id="cd667-1294">Исправлена проблема с `ad app update --homepage`, когда домашнюю страницу нельзя было обновить.</span><span class="sxs-lookup"><span data-stu-id="cd667-1294">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="cd667-1295">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="cd667-1295">ServiceFabric</span></span>

* <span data-ttu-id="cd667-1296">Добавлена поддержка имен Key Vault в смешанном регистре.</span><span class="sxs-lookup"><span data-stu-id="cd667-1296">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="cd667-1297">Исправлена проблема с использованием сертификатов в Key Vault.</span><span class="sxs-lookup"><span data-stu-id="cd667-1297">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="cd667-1298">Исправлена проблема с использованием файлов сертификатов PFX.</span><span class="sxs-lookup"><span data-stu-id="cd667-1298">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="cd667-1299">Исправлена проблема с `sf cluster certificate add`, когда группа ресурсов Key Vault не была указана.</span><span class="sxs-lookup"><span data-stu-id="cd667-1299">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="cd667-1300">Исправлена проблема с неработающей командой `sf cluster set`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1300">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="cd667-1301">SignalR</span><span class="sxs-lookup"><span data-stu-id="cd667-1301">SignalR</span></span>

* <span data-ttu-id="cd667-1302">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="cd667-1302">Added new commands:</span></span>
  * <span data-ttu-id="cd667-1303">`signalr cors`: Управление CORS SignalR</span><span class="sxs-lookup"><span data-stu-id="cd667-1303">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="cd667-1304">`signalr restart`: Перезапуск службы SignalR</span><span class="sxs-lookup"><span data-stu-id="cd667-1304">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="cd667-1305">`signalr update`: Обновление службы SignalR</span><span class="sxs-lookup"><span data-stu-id="cd667-1305">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="cd667-1306">Добавлен аргумент `--service-mode` для команды `signalr create`</span><span class="sxs-lookup"><span data-stu-id="cd667-1306">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-1307">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-1307">Storage</span></span>

* <span data-ttu-id="cd667-1308">Добавлена команда `storage account revoke-delegation-keys`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1308">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="cd667-1309">13 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1309">August 13, 2019</span></span>

<span data-ttu-id="cd667-1310">Версия 2.0.71</span><span class="sxs-lookup"><span data-stu-id="cd667-1310">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-1311">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-1311">AppService</span></span>

* <span data-ttu-id="cd667-1312">Исправлена проблема, из-за которой выполнение команд `webapp webjob continuous` для слотов завершалось сбоем.</span><span class="sxs-lookup"><span data-stu-id="cd667-1312">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="cd667-1313">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="cd667-1313">BotService</span></span>

* <span data-ttu-id="cd667-1314">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка создания ботов на основе пакета SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="cd667-1314">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="cd667-1315">Cognitive Services:</span><span class="sxs-lookup"><span data-stu-id="cd667-1315">CognitiveServices</span></span>

* <span data-ttu-id="cd667-1316">Добавлены команды `cognitiveservices account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1316">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="cd667-1317">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-1317">Cosmos DB</span></span>

* <span data-ttu-id="cd667-1318">Удалено предупреждение при обновлении нескольких расположений для записи.</span><span class="sxs-lookup"><span data-stu-id="cd667-1318">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="cd667-1319">Добавлены команды CRUD для ресурсов CosmosDB SQL, MongoDB, Cassandra, Gremlin и ресурсов таблиц, а также пропускной способности ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd667-1319">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="cd667-1320">HDInsight</span><span class="sxs-lookup"><span data-stu-id="cd667-1320">HDInsight</span></span>

<span data-ttu-id="cd667-1321">Этот выпуск содержит большое число критических изменений.</span><span class="sxs-lookup"><span data-stu-id="cd667-1321">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="cd667-1322">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="cd667-1322">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="cd667-1323">Переименование `--storage-default-container` в `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="cd667-1323">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="cd667-1324">Переименование `--storage-default-filesystem` в `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="cd667-1324">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="cd667-1325">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--name` для `application create`, чтобы представлять имя приложения вместо имени кластера.</span><span class="sxs-lookup"><span data-stu-id="cd667-1325">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="cd667-1326">Добавлен аргумент `--cluster-name` для `application create`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1326">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="cd667-1327">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="cd667-1327">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="cd667-1328">Переименование `--application-type` в `--type`</span><span class="sxs-lookup"><span data-stu-id="cd667-1328">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="cd667-1329">Переименование `--marketplace-identifier` в `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="cd667-1329">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="cd667-1330">Переименование `--https-endpoint-access-mode` в `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="cd667-1330">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="cd667-1331">Переименован аргумент `--https-endpoint-destination-port` на `--destination-port`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1331">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="cd667-1332">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="cd667-1332">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="cd667-1333">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Переименован аргумент `--target-instance-count` на `--workernode-count` для `hdinsight resize`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1333">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="cd667-1334">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены все команды в группе `hdinsight script-action`, чтобы использовать параметр `--name` в качестве имени действия скрипта.</span><span class="sxs-lookup"><span data-stu-id="cd667-1334">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="cd667-1335">Добавлен аргумент `--cluster-name` для всех команд `hdinsight script-action`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1335">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="cd667-1336">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименован аргумент `--script-execution-id` на `--execution-id`для всех команд `hdinsight script-action`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1336">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="cd667-1337">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `hdinsight script-action show` переименована в `hdinsight script-action show-execution-details`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1337">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="cd667-1338">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Изменены параметры для `hdinsight script-action execute --roles`, чтобы они разделялись пробелами, а не запятыми.</span><span class="sxs-lookup"><span data-stu-id="cd667-1338">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="cd667-1339">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--persisted` для `hdinsight script-action list`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1339">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="cd667-1340">Изменен параметр `hdinsight create --cluster-configurations`, чтобы принимать путь к локальному файлу JSON или строке JSON.</span><span class="sxs-lookup"><span data-stu-id="cd667-1340">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="cd667-1341">Добавлена команда `hdinsight script-action list-execution-history`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1341">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="cd667-1342">Изменен параметр `hdinsight monitor enable --workspace`, чтобы принимать идентификатор или имя рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="cd667-1342">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="cd667-1343">Добавлен аргумент `hdinsight monitor enable --primary-key`, который требуется, если в качестве параметра указан идентификатор рабочей области.</span><span class="sxs-lookup"><span data-stu-id="cd667-1343">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="cd667-1344">Добавлены дополнительные примеры и обновленные описания для справочных сообщений.</span><span class="sxs-lookup"><span data-stu-id="cd667-1344">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="cd667-1345">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="cd667-1345">Interactive</span></span>

* <span data-ttu-id="cd667-1346">Исправлена ошибка загрузки.</span><span class="sxs-lookup"><span data-stu-id="cd667-1346">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="cd667-1347">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="cd667-1347">Kubernetes</span></span>

* <span data-ttu-id="cd667-1348">Теперь используется `https`, если порт контейнера панели мониторинга использует `https`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1348">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="cd667-1349">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-1349">Network</span></span>

* <span data-ttu-id="cd667-1350">Добавлен аргумент `--yes` для `network dns record-set cname delete`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1350">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-1351">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-1351">Profile</span></span>

* <span data-ttu-id="cd667-1352">Добавлен аргумент `--resource-type` для `account get-access-token`, чтобы получать маркеры доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="cd667-1352">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="cd667-1353">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="cd667-1353">ServiceFabric</span></span>

* <span data-ttu-id="cd667-1354">Добавлены все поддерживаемые версии ОС для команды sf cluster create.</span><span class="sxs-lookup"><span data-stu-id="cd667-1354">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="cd667-1355">Исправлена ошибка проверки основного сертификата.</span><span class="sxs-lookup"><span data-stu-id="cd667-1355">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-1356">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-1356">Storage</span></span>

* <span data-ttu-id="cd667-1357">Добавлена команда `storage copy`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1357">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="cd667-1358">30 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1358">July 30, 2019</span></span>

<span data-ttu-id="cd667-1359">Версия 2.0.70</span><span class="sxs-lookup"><span data-stu-id="cd667-1359">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-1360">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-1360">ACR</span></span>

* <span data-ttu-id="cd667-1361">Исправлена проблема № 9952 (регрессия в команде `acr pack build`).</span><span class="sxs-lookup"><span data-stu-id="cd667-1361">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="cd667-1362">Удалено имя образа построителя по умолчанию в `acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1362">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-1363">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-1363">Appservice</span></span>

* <span data-ttu-id="cd667-1364">Команда `webapp config ssl` изменена для отображения сообщения, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="cd667-1364">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="cd667-1365">Исправлена проблема, когда команда `functionapp create` не принимала тип учетной записи хранения `Standard_RAGRS`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1365">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="cd667-1366">Исправлена проблема, когда команда `webapp up` завершала работу со сбоем в случае выполнения со старой версией Python.</span><span class="sxs-lookup"><span data-stu-id="cd667-1366">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="cd667-1367">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-1367">Network</span></span>

* <span data-ttu-id="cd667-1368">Удален недопустимый параметр `--ids` из `network nic ip-config add` (исправление проблемы № 9861).</span><span class="sxs-lookup"><span data-stu-id="cd667-1368">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="cd667-1369">Исправлена проблема № 9604.</span><span class="sxs-lookup"><span data-stu-id="cd667-1369">Fixes #9604.</span></span> <span data-ttu-id="cd667-1370">Добавлен параметр `--root-certs` в `network application-gateway http-settings [create|update]` для поддержки связанных с пользователем доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="cd667-1370">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="cd667-1371">Исправлен аргумент `--subscription` для `network dns record-set ns create` (проблема № 9965).</span><span class="sxs-lookup"><span data-stu-id="cd667-1371">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="cd667-1372">RBAC</span><span class="sxs-lookup"><span data-stu-id="cd667-1372">RBAC</span></span>

* <span data-ttu-id="cd667-1373">Добавлена команда `user update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1373">Added `user update` command</span></span>
* <span data-ttu-id="cd667-1374">[УСТАРЕЛО]`--upn-or-object-id` не рекомендуется использовать в связанных с пользователями командах.</span><span class="sxs-lookup"><span data-stu-id="cd667-1374">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="cd667-1375">Вместо этого применяйте аргумент `--id`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1375">Use replacement argument `--id`</span></span>
* <span data-ttu-id="cd667-1376">Добавлен аргумент `--id` в связанные с пользователями команды.</span><span class="sxs-lookup"><span data-stu-id="cd667-1376">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-1377">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-1377">SQL</span></span>

* <span data-ttu-id="cd667-1378">Добавлены команды управления для ключей и предохранителя TDE управляемого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="cd667-1378">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-1379">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-1379">Storage</span></span>

* <span data-ttu-id="cd667-1380">Добавлена команда `storage remove`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1380">Added `storage remove` command</span></span>
* <span data-ttu-id="cd667-1381">Исправлена проблема с `storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1381">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-1382">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-1382">VM</span></span>

* <span data-ttu-id="cd667-1383">Изменена команда `list-skus` для использования новой версии API для вывода сведений о зонах.</span><span class="sxs-lookup"><span data-stu-id="cd667-1383">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="cd667-1384">Изменено значение по умолчанию параметра `--single-placement-group` на `false` для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1384">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="cd667-1385">Добавлена возможность выбирать номера SKU хранилища ZRS для `[snapshot|disk] create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1385">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="cd667-1386">Добавлена новая группа команд `vm host` для поддержки выделенных узлов.</span><span class="sxs-lookup"><span data-stu-id="cd667-1386">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="cd667-1387">Добавлены параметры `--host` и `--host-group` в команде `vm create` для указания выделенного узла виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="cd667-1387">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="cd667-1388">16 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1388">July 16, 2019</span></span>

<span data-ttu-id="cd667-1389">Версия 2.0.69</span><span class="sxs-lookup"><span data-stu-id="cd667-1389">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-1390">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-1390">Appservice</span></span>

* <span data-ttu-id="cd667-1391">Изменены команды `webapp identity`. Теперь они возвращают правильное сообщение об ошибке, если параметр ResourceGroupName или имя приложения недопустимы.</span><span class="sxs-lookup"><span data-stu-id="cd667-1391">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="cd667-1392">Исправлена команда `webapp list`. Теперь она возвращает правильное значение для параметра numberOfSites, если не указан параметр ResourceGroup.</span><span class="sxs-lookup"><span data-stu-id="cd667-1392">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="cd667-1393">Исправлены побочные эффекты для команд `appservice plan create` и `webapp create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1393">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="cd667-1394">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-1394">Core</span></span>

* <span data-ttu-id="cd667-1395">Исправлена ошибка, при которой отображался параметр `--subscription`, хотя он был неприменим.</span><span class="sxs-lookup"><span data-stu-id="cd667-1395">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="cd667-1396">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-1396">Batch</span></span>

* <span data-ttu-id="cd667-1397">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `batch pool node-agent-skus list` заменена на `batch pool supported-images list`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1397">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="cd667-1398">Добавлена поддержка правил безопасности, которые блокируют сетевой доступ к пулу на основе исходного порта трафика при использовании параметра `--json-file` команды `batch pool create network`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1398">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="cd667-1399">Добавлена поддержка выполнения задачи в рабочей папке контейнера или рабочей папке задачи пакета при использовании параметра `--json-file` команды `batch task create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1399">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="cd667-1400">Исправлена ошибка в параметре `--application-package-references` команды `batch pool create`, которая позволяла работать только со значениями по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-1400">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="cd667-1401">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="cd667-1401">Eventhubs</span></span>

* <span data-ttu-id="cd667-1402">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1402">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="cd667-1403">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="cd667-1403">RDBMS</span></span>

* <span data-ttu-id="cd667-1404">Добавлен необязательный параметр для указания номера SKU реплики в команде создания реплики.</span><span class="sxs-lookup"><span data-stu-id="cd667-1404">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="cd667-1405">Исправлена ошибка теста CI при создании реплики MySQL.</span><span class="sxs-lookup"><span data-stu-id="cd667-1405">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="cd667-1406">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="cd667-1406">Relay</span></span>

* <span data-ttu-id="cd667-1407">Исправлена проблема с гибридным подключением при выключенной авторизации клиента ([8775](https://github.com/azure/azure-cli/issues/8775)).</span><span class="sxs-lookup"><span data-stu-id="cd667-1407">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="cd667-1408">Добавлен параметр `--requires-transport-security` для команды `relay wcfrelay create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1408">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="cd667-1409">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="cd667-1409">Servicebus</span></span>

* <span data-ttu-id="cd667-1410">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1410">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-1411">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-1411">Storage</span></span>

* <span data-ttu-id="cd667-1412">Добавлена возможность обновления учетной записи хранения для AADDS в службе "Файлы".</span><span class="sxs-lookup"><span data-stu-id="cd667-1412">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="cd667-1413">Устранена проблема, описанная здесь: `storage blob service-properties update --set`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1413">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="cd667-1414">2 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1414">July 2, 2019</span></span>

<span data-ttu-id="cd667-1415">Версия 2.0.68</span><span class="sxs-lookup"><span data-stu-id="cd667-1415">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="cd667-1416">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-1416">Core</span></span>

* <span data-ttu-id="cd667-1417">Командные модули теперь объединены в один распространяемый пакет Python.</span><span class="sxs-lookup"><span data-stu-id="cd667-1417">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="cd667-1418">В результате этого прекращается непосредственное использование множества пакетов `azure-cli-` в PyPI.</span><span class="sxs-lookup"><span data-stu-id="cd667-1418">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="cd667-1419">Это также должно уменьшить размер установки и повлияет только на пользователей, которые выполняли установку непосредственно через `pip`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1419">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-1420">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-1420">ACR</span></span>

* <span data-ttu-id="cd667-1421">В заданиях добавлена поддержка триггеров таймера.</span><span class="sxs-lookup"><span data-stu-id="cd667-1421">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-1422">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-1422">Appservice</span></span>

* <span data-ttu-id="cd667-1423">Внесены изменения в `functionapp create` для включения Application Insights по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-1423">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="cd667-1424">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена устаревшая команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1424">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="cd667-1425">Вместо нее используйте новую команду `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1425">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="cd667-1426">В `functionapp deployment config-zip` добавлена поддержка плана потребления приложения-функции Linux.</span><span class="sxs-lookup"><span data-stu-id="cd667-1426">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="cd667-1427">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-1427">Cosmos DB</span></span>

* <span data-ttu-id="cd667-1428">Добавлена возможность отключения TTL.</span><span class="sxs-lookup"><span data-stu-id="cd667-1428">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="cd667-1429">DLS</span><span class="sxs-lookup"><span data-stu-id="cd667-1429">DLS</span></span>

* <span data-ttu-id="cd667-1430">Обновленная версия ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="cd667-1430">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="cd667-1431">Отзывы</span><span class="sxs-lookup"><span data-stu-id="cd667-1431">Feedback</span></span>

* <span data-ttu-id="cd667-1432">При сообщении о сбое при выполнении команды расширения `az feedback` теперь пытается открыть браузер по URL-адресу репозитория или проекта расширения из индекса.</span><span class="sxs-lookup"><span data-stu-id="cd667-1432">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="cd667-1433">HDInsight</span><span class="sxs-lookup"><span data-stu-id="cd667-1433">HDInsight</span></span>

* <span data-ttu-id="cd667-1434">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя группы команд `oms` изменилось на `monitor`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1434">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="cd667-1435">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--http-password/-p` стал обязательным.</span><span class="sxs-lookup"><span data-stu-id="cd667-1435">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="cd667-1436">Добавлены средства заполнения для `--cluster-admin-account` и средство заполнения для параметров `cluster-users-group-dns`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1436">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="cd667-1437">Параметр `cluster-users-group-dns` стал обязательным, если присутствует `—esp`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1437">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="cd667-1438">Добавлено время ожидания для всех существующих средств автоматического заполнения аргументов.</span><span class="sxs-lookup"><span data-stu-id="cd667-1438">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="cd667-1439">Добавлено время ожидания для преобразования имени ресурса в идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="cd667-1439">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="cd667-1440">Внесены изменения в средства автоматического заполнения для выбора ресурсов из любой группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd667-1440">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="cd667-1441">Это может быть группа ресурсов, отличная от той, которая указана с помощью `-g`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1441">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="cd667-1442">Добавлена поддержка параметров `--sub-domain-suffix` и `--disable_gateway_auth` в команде `hdinsight application create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1442">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="cd667-1443">Управляемые службы</span><span class="sxs-lookup"><span data-stu-id="cd667-1443">Managed Services</span></span>

* <span data-ttu-id="cd667-1444">Командный модуль управляемых служб выпущен в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="cd667-1444">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-1445">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-1445">Profile</span></span>
* <span data-ttu-id="cd667-1446">Аргумент `--subscription` подавляется для команды выхода.</span><span class="sxs-lookup"><span data-stu-id="cd667-1446">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="cd667-1447">RBAC</span><span class="sxs-lookup"><span data-stu-id="cd667-1447">RBAC</span></span>

* <span data-ttu-id="cd667-1448">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален аргумент `--password` для `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1448">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="cd667-1449">В команду `create` добавлен параметр `--assignee-principal-type` для устранения периодических сбоев из-за задержки репликации сервера AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="cd667-1449">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="cd667-1450">Исправлен сбой в `ad signed-in-user` при перечислении собственных объектов.</span><span class="sxs-lookup"><span data-stu-id="cd667-1450">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="cd667-1451">Исправлена проблема, при которой `ad sp` не удавалось найти нужное приложение в субъекте-службе.</span><span class="sxs-lookup"><span data-stu-id="cd667-1451">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="cd667-1452">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="cd667-1452">RDBMS</span></span>

* <span data-ttu-id="cd667-1453">Добавлена поддержка репликации MariaDB.</span><span class="sxs-lookup"><span data-stu-id="cd667-1453">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-1454">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-1454">SQL</span></span>

* <span data-ttu-id="cd667-1455">Описаны допустимые значения для `sql db create --sample-name`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1455">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-1456">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-1456">Storage</span></span>

* <span data-ttu-id="cd667-1457">В `storage blob generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1457">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="cd667-1458">В `storage container generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1458">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="cd667-1459">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-1459">VM</span></span>

* <span data-ttu-id="cd667-1460">Исправлена ошибка, при которой команда `vmss create` возвращала сообщение об ошибке при выполнении с `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1460">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="cd667-1461">Прекращена проверка `vmss create --single-placement-group` на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="cd667-1461">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="cd667-1462">Команда не завершается сбоем, если для `--single-placement-group` задано значение `true`, а значение `--instance-count` больше 100 или указаны зоны доступности. Сама проверка теперь выполняется службой вычислений.</span><span class="sxs-lookup"><span data-stu-id="cd667-1462">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="cd667-1463">Исправлена ошибка, при которой команда `[vm|vmss] extension image list` завершалась сбоем при указании `--latest`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1463">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="cd667-1464">18 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1464">June 18, 2019</span></span>

<span data-ttu-id="cd667-1465">Версия 2.0.67</span><span class="sxs-lookup"><span data-stu-id="cd667-1465">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="cd667-1466">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-1466">Core</span></span>

<span data-ttu-id="cd667-1467">В этом выпуске добавлен новый тег [Предварительная версия], который яснее дает понять, что группа команд, команда или аргумент находятся в состоянии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="cd667-1467">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="cd667-1468">Ранее это указывалось в тексте справки или подразумевалось в номере версии командного модуля.</span><span class="sxs-lookup"><span data-stu-id="cd667-1468">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="cd667-1469">В будущем в интерфейсе командной строки номера версий отдельных пакетов не будут указываться.</span><span class="sxs-lookup"><span data-stu-id="cd667-1469">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="cd667-1470">Если команда доступна в предварительной версии, это также касается и всех ее аргументов.</span><span class="sxs-lookup"><span data-stu-id="cd667-1470">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="cd667-1471">Если группа команд помечается как находящаяся в предварительной версии, значит все команды и аргументы также считаются доступными в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="cd667-1471">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="cd667-1472">В результате этого изменения несколько групп команд могут "внезапно" оказаться в состоянии предварительной версии в этом выпуске.</span><span class="sxs-lookup"><span data-stu-id="cd667-1472">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="cd667-1473">В действительности большинство пакетов, которые находились в состоянии предварительной версии, в этом выпуске будут считаться общедоступными.</span><span class="sxs-lookup"><span data-stu-id="cd667-1473">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-1474">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-1474">ACR</span></span>
* <span data-ttu-id="cd667-1475">Добавлена команда acr check-health.</span><span class="sxs-lookup"><span data-stu-id="cd667-1475">Added 'acr check-health' command</span></span>
* <span data-ttu-id="cd667-1476">Улучшена обработка ошибок с маркерами безопасности AAD и ошибок при получении внешних команд.</span><span class="sxs-lookup"><span data-stu-id="cd667-1476">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-1477">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-1477">ACS</span></span>
* <span data-ttu-id="cd667-1478">Устаревшие команды ACS теперь скрыты в тексте справки.</span><span class="sxs-lookup"><span data-stu-id="cd667-1478">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="cd667-1479">AMS</span><span class="sxs-lookup"><span data-stu-id="cd667-1479">AMS</span></span>
* <span data-ttu-id="cd667-1480">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в возврате строк времени ISO 8601 для archive-window-length и key-frame-interval-duration.</span><span class="sxs-lookup"><span data-stu-id="cd667-1480">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-1481">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-1481">AppService</span></span>
* <span data-ttu-id="cd667-1482">Добавлена маршрутизация на основе расположение для `webapp deleted list` и `webapp deleted restore`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1482">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="cd667-1483">Исправлена проблема, при которой целевой URL-адрес веб-приложения ("Вы можете запустить приложение в...") не был активным в Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="cd667-1483">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="cd667-1484">Устранена проблема, при которой создание приложений в некоторых SKU завершалось сбоем с ошибкой AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="cd667-1484">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="cd667-1485">Добавлена предварительная проверка в `[appservice|webapp] create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1485">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="cd667-1486">Исправлено `[webapp|functionapp] traffic-routing` для использования правильного actionHostName.</span><span class="sxs-lookup"><span data-stu-id="cd667-1486">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="cd667-1487">Добавлена поддержка слотов для команд `functionapp`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1487">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="cd667-1488">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-1488">Batch</span></span>
* <span data-ttu-id="cd667-1489">Исправлена регрессия проверки подлинности AAD, которую вызывал чрезмерный поток уведомлений об авторизации с помощью общего ключа.</span><span class="sxs-lookup"><span data-stu-id="cd667-1489">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="cd667-1490">Batch AI</span><span class="sxs-lookup"><span data-stu-id="cd667-1490">BatchAI</span></span>
* <span data-ttu-id="cd667-1491">Команды BatchAI теперь признаны устаревшими и скрыты.</span><span class="sxs-lookup"><span data-stu-id="cd667-1491">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="cd667-1492">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="cd667-1492">BotService</span></span>
* <span data-ttu-id="cd667-1493">Добавлены предупреждающие сообщения о прекращении поддержки и режиме обслуживания для команд, которые поддерживают пакет SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="cd667-1493">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="cd667-1494">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-1494">CosmosDB</span></span>
* <span data-ttu-id="cd667-1495">[УСТАРЕЛО] использовать команду `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1495">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="cd667-1496">Добавлена команда `cosmosdb keys list`, заменяющая `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1496">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="cd667-1497">`cosmsodb create/update`: Добавлен новый формат для --location, который позволяет задавать свойство isZoneRedundant.</span><span class="sxs-lookup"><span data-stu-id="cd667-1497">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="cd667-1498">Нерекомендуемый старый формат.</span><span class="sxs-lookup"><span data-stu-id="cd667-1498">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="cd667-1499">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="cd667-1499">EventGrid</span></span>
* <span data-ttu-id="cd667-1500">Добавлены команды `eventgrid domain` для операций CRUD домена.</span><span class="sxs-lookup"><span data-stu-id="cd667-1500">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="cd667-1501">Добавлены команды `eventgrid domain topic` для операций CRUD разделов домена.</span><span class="sxs-lookup"><span data-stu-id="cd667-1501">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="cd667-1502">В `eventgrid [topic|event-subscription] list` добавлен аргумент `--odata-query` для фильтрации результатов с использованием синтаксиса OData.</span><span class="sxs-lookup"><span data-stu-id="cd667-1502">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="cd667-1503">`event-subscription create/update`: Добавлена ServiceBusQueue в качестве новых значений для параметра `--endpoint-type`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1503">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="cd667-1504">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в прекращении поддержки `--included-event-types All` с `eventgrid event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1504">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="cd667-1505">HDInsight</span><span class="sxs-lookup"><span data-stu-id="cd667-1505">HDInsight</span></span>
* <span data-ttu-id="cd667-1506">Добавлена поддержка параметра `--ssh-public-key` в команде `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1506">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-1507">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-1507">IoT</span></span>
* <span data-ttu-id="cd667-1508">Добавлена поддержка для повторного создания ключей политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="cd667-1508">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="cd667-1509">Добавлен пакет SDK и поддержка для службы подготовки репозитория DigitalTwin.</span><span class="sxs-lookup"><span data-stu-id="cd667-1509">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="cd667-1510">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-1510">Network</span></span>
* <span data-ttu-id="cd667-1511">Добавлена поддержка зон для Шлюза NAT.</span><span class="sxs-lookup"><span data-stu-id="cd667-1511">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="cd667-1512">Добавлена команда `network list-service-tags`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1512">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="cd667-1513">Исправлена проблема с `dns zone import`, при которой пользователям не удавалось импортировать записи А с подстановочным знаком.</span><span class="sxs-lookup"><span data-stu-id="cd667-1513">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="cd667-1514">Исправлена проблема с `watcher flow-log configure`, при которой не удавалось включить ведение журнала потоков в определенных регионах.</span><span class="sxs-lookup"><span data-stu-id="cd667-1514">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-1515">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-1515">Resource</span></span>
* <span data-ttu-id="cd667-1516">Добавлена команда `az rest` для вызовов REST.</span><span class="sxs-lookup"><span data-stu-id="cd667-1516">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="cd667-1517">Исправлена ошибка, возникавшая при использовании `policy assignment list` с группой ресурсов или уровнем подписки `--scope`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1517">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="cd667-1518">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="cd667-1518">ServiceBus</span></span>
* <span data-ttu-id="cd667-1519">Устранена проблема № [9319](https://github.com/azure/azure-cli/issues/9319) с `servicebus topic create --max-size`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1519">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-1520">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-1520">SQL</span></span>
* <span data-ttu-id="cd667-1521">Параметр `--location` стал необязательным для `sql [server|mi] create`. Если он не указан, используется расположение группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd667-1521">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="cd667-1522">Исправлена ошибка "Объект NoneType не подлежит итерации" с `sql db list-editions --available`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1522">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="cd667-1523">SQLVm</span><span class="sxs-lookup"><span data-stu-id="cd667-1523">SQLVm</span></span>
* <span data-ttu-id="cd667-1524">Критическое изменение. Для `sql vm create` теперь требуется параметр `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1524">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="cd667-1525">Внесены изменения, позволяющие задавать SKU образа SQL при создании или обновлении виртуальной машины SQL.</span><span class="sxs-lookup"><span data-stu-id="cd667-1525">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-1526">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-1526">Storage</span></span>
* <span data-ttu-id="cd667-1527">Исправлена проблема с отсутствующим ключом учетной записи для `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1527">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="cd667-1528">Исправлена проблема с `storage blob sync` на платформе Linux.</span><span class="sxs-lookup"><span data-stu-id="cd667-1528">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-1529">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-1529">VM</span></span>
* <span data-ttu-id="cd667-1530">[Предварительная версия] Добавлены команды `vm image template` для создания образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="cd667-1530">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="cd667-1531">4 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1531">June 4, 2019</span></span>

<span data-ttu-id="cd667-1532">Версия 2.0.66</span><span class="sxs-lookup"><span data-stu-id="cd667-1532">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="cd667-1533">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-1533">Core</span></span>
* <span data-ttu-id="cd667-1534">Исправлена ошибка, из-за которой выполнение команды завершалось со сбоем, если параметр `--output yaml` использовался с параметром `--query`</span><span class="sxs-lookup"><span data-stu-id="cd667-1534">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-1535">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-1535">ACR</span></span>
* <span data-ttu-id="cd667-1536">Добавлена группа команд acr pack для создания заданий быстрой сборки с помощью пакетов сборок.</span><span class="sxs-lookup"><span data-stu-id="cd667-1536">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-1537">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-1537">ACS</span></span>
* <span data-ttu-id="cd667-1538">Разрешено включение и отключение надстройки панели мониторинга Kubernetes для AKS.</span><span class="sxs-lookup"><span data-stu-id="cd667-1538">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="cd667-1539">Если подписку нельзя использовать с Azure Red Hat OpenShift, будет отображаться соответствующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="cd667-1539">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="cd667-1540">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-1540">Batch</span></span>
* <span data-ttu-id="cd667-1541">Улучшена обработка ошибок, если не выполнен вход в учетную запись \[[№ 9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[№ 8978](https://github.com/Azure/azure-cli/issues/8978)\].</span><span class="sxs-lookup"><span data-stu-id="cd667-1541">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-1542">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-1542">IoT</span></span>
* <span data-ttu-id="cd667-1543">Добавлена поддержка для перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="cd667-1543">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="cd667-1544">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-1544">Network</span></span>
* <span data-ttu-id="cd667-1545">Добавлены команды `network application-gateway waf-policy` для поддержки настраиваемых правил WAF.</span><span class="sxs-lookup"><span data-stu-id="cd667-1545">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="cd667-1546">Добавлены аргументы `--waf-policy` и `--max-capacity` для команды `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="cd667-1546">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="cd667-1547">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-1547">Resource</span></span>
* <span data-ttu-id="cd667-1548">Улучшен вывод сообщения команды `deployment create` при отсутствии TTY.</span><span class="sxs-lookup"><span data-stu-id="cd667-1548">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="cd667-1549">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-1549">Role</span></span>
* <span data-ttu-id="cd667-1550">Обновлен текст справки.</span><span class="sxs-lookup"><span data-stu-id="cd667-1550">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-1551">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="cd667-1551">Compute</span></span>
* <span data-ttu-id="cd667-1552">Добавлена поддержка команды `vm create` для создания виртуальных машин из управляемого образа с номерами LUN дисков данных, которые не начинаются с 0 или для которых пропущены номера.</span><span class="sxs-lookup"><span data-stu-id="cd667-1552">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="cd667-1553">21 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1553">May 21, 2019</span></span>

<span data-ttu-id="cd667-1554">Версия 2.0.65</span><span class="sxs-lookup"><span data-stu-id="cd667-1554">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="cd667-1555">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-1555">Core</span></span>
* <span data-ttu-id="cd667-1556">Улучшена функция обратной связи при ошибках аутентификации.</span><span class="sxs-lookup"><span data-stu-id="cd667-1556">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="cd667-1557">Исправлена проблема, из-за которой интерфейс командной строки загружал расширения, которые не были совместимы с его базовой версией.</span><span class="sxs-lookup"><span data-stu-id="cd667-1557">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="cd667-1558">Исправлена проблема с запуском и неисправностью `clouds.config`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1558">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-1559">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-1559">ACR</span></span>
* <span data-ttu-id="cd667-1560">Добавлена поддержка управляемых удостоверений в Задачи.</span><span class="sxs-lookup"><span data-stu-id="cd667-1560">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-1561">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-1561">ACS</span></span>
* <span data-ttu-id="cd667-1562">Исправлена команда `openshift create`, используемая с пользовательским клиентом AAD.</span><span class="sxs-lookup"><span data-stu-id="cd667-1562">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-1563">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-1563">AppService</span></span>
* <span data-ttu-id="cd667-1564">[УСТАРЕЛО] Команда `functionapp devops-build` устарела и будет удалена в следующем выпуске.</span><span class="sxs-lookup"><span data-stu-id="cd667-1564">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="cd667-1565">Внесено изменение в `functionapp devops-pipeline` для получения журнала сборки из Azure DevOps в режиме подробного протоколирования.</span><span class="sxs-lookup"><span data-stu-id="cd667-1565">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="cd667-1566">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален неподдерживаемый флаг `--use_local_settings` из команды `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1566">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="cd667-1567">Внесено изменение в `webapp up` для возврата выходных данных JSON, если `--logs` не используется.</span><span class="sxs-lookup"><span data-stu-id="cd667-1567">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="cd667-1568">Добавлена поддержка записи ресурсов по умолчанию в локальную конфигурацию для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1568">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="cd667-1569">Добавлена поддержка `webapp up` для повторного развертывания приложения без использования аргумента `--location`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1569">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="cd667-1570">Устранена проблема, из-за которой нельзя было создать для Linux номер SKU с планом службы приложений "Бесплатный".</span><span class="sxs-lookup"><span data-stu-id="cd667-1570">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="cd667-1571">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="cd667-1571">BotService</span></span>
* <span data-ttu-id="cd667-1572">Внесено изменение для включения поддержки всех регистров в параметрах `--lang` для команд.</span><span class="sxs-lookup"><span data-stu-id="cd667-1572">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="cd667-1573">Обновлено описание модуля команды.</span><span class="sxs-lookup"><span data-stu-id="cd667-1573">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="cd667-1574">Потребление</span><span class="sxs-lookup"><span data-stu-id="cd667-1574">Consumption</span></span>
* <span data-ttu-id="cd667-1575">Добавлен отсутствующий обязательный параметр при выполнении `consumption usage list --billing-period-name`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1575">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-1576">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-1576">IoT</span></span>
* <span data-ttu-id="cd667-1577">Добавлена поддержка перечисления всех ключей.</span><span class="sxs-lookup"><span data-stu-id="cd667-1577">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="cd667-1578">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-1578">Network</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="cd667-1580">Добавлен аргумент `--nat-gateway` для `network vnet subnet [create|update]` для подключения к шлюзу NAT.</span><span class="sxs-lookup"><span data-stu-id="cd667-1580">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="cd667-1581">Исправлена проблема с `dns zone import`, из-за которой имена записей не сопоставлялись с типом записей.</span><span class="sxs-lookup"><span data-stu-id="cd667-1581">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="cd667-1582">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="cd667-1582">RDBMS</span></span>
* <span data-ttu-id="cd667-1583">Добавлена поддержка Postgres и MySQL для георепликации.</span><span class="sxs-lookup"><span data-stu-id="cd667-1583">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="cd667-1584">RBAC</span><span class="sxs-lookup"><span data-stu-id="cd667-1584">RBAC</span></span>
* <span data-ttu-id="cd667-1585">Добавлена поддержка области группы управления для `role assignment`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1585">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-1586">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-1586">Storage</span></span>
* <span data-ttu-id="cd667-1587">`storage blob sync`: добавьте команду синхронизации для хранилища BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="cd667-1587">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="cd667-1588">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="cd667-1588">Compute</span></span>
* <span data-ttu-id="cd667-1589">Добавлен параметр `--computer-name` для `vm create` для установки имени виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="cd667-1589">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="cd667-1590">Переименован параметр `--ssh-key-value` в `--ssh-key-values` для `[vm|vmss] create` для приема нескольких значений пути или открытого ключа SSH.</span><span class="sxs-lookup"><span data-stu-id="cd667-1590">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="cd667-1591">__Примечание.__ Это **не** критическое изменение, благодаря которому `--ssh-key-value` будет правильно анализироваться, так как соответствует только `--ssh-key-values`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1591">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="cd667-1592">Внесено изменение в аргумент `ppg create` для `--type` — теперь он необязательный.</span><span class="sxs-lookup"><span data-stu-id="cd667-1592">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="cd667-1593">6 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1593">May 6, 2019</span></span>

<span data-ttu-id="cd667-1594">Версия 2.0.64</span><span class="sxs-lookup"><span data-stu-id="cd667-1594">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-1595">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-1595">ACS</span></span>
* <span data-ttu-id="cd667-1596">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--fqdn` из команд `openshift`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1596">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="cd667-1597">Внесено изменение для использования общедоступной версии API для Azure Red Hat Openshift.</span><span class="sxs-lookup"><span data-stu-id="cd667-1597">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="cd667-1598">Добавлен флаг `customer-admin-group-id` в `openshift create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1598">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="cd667-1599">[Общедоступная версия.] `(PREVIEW)` больше не используется для `aks create` в параметре `--network-policy`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1599">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-1600">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-1600">Appservice</span></span>
* <span data-ttu-id="cd667-1601">[УСТАРЕЛО] Команда `functionapp devops-build` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="cd667-1601">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="cd667-1602">Команда переименована в `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1602">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="cd667-1603">Исправлен процесс получения правильного имени пользователя для Cloud Shell, приводивший к ошибке выполнения `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1603">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="cd667-1604">Обновлена документация по `appservice plan --sku` в соответствии с поддерживаемыми планами службы приложений.</span><span class="sxs-lookup"><span data-stu-id="cd667-1604">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="cd667-1605">Добавлены необязательные аргументы для группы ресурсов и план для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1605">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="cd667-1606">Добавлена поддержка `webapp ssh` в соответствии с переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1606">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="cd667-1607">Добавлена поддержка `appserviceplan create` для ценовой категории "Бесплатный" в Linux.</span><span class="sxs-lookup"><span data-stu-id="cd667-1607">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="cd667-1608">Внесено изменение в `webapp up` для перевода в спящий режим на 30 с после установки параметра приложения `SCM_DO_BUILD_DURING_DEPLOYMENT=true` для обработки холодного запуска Kudu.</span><span class="sxs-lookup"><span data-stu-id="cd667-1608">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="cd667-1609">Добавлена поддержка среды выполнения `powershell` для `functionapp create` в Windows.</span><span class="sxs-lookup"><span data-stu-id="cd667-1609">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="cd667-1610">Добавлена команда `create-remote-connection`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1610">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="cd667-1611">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-1611">Batch</span></span>
* <span data-ttu-id="cd667-1612">Исправлена ошибка в проверяющем элементе управления для параметров `--application-package-references`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1612">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="cd667-1613">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="cd667-1613">Botservice</span></span>
* <span data-ttu-id="cd667-1614">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` для создания пустого бота веб-приложения по умолчанию (т. е. бот не развертывается в Службе приложений).</span><span class="sxs-lookup"><span data-stu-id="cd667-1614">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="cd667-1615">Добавлен флаг `--echo` в `bot create` для использования старого поведения с `-v v4`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1615">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="cd667-1616">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено значение по умолчанию `--version` на `v4`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1616">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="cd667-1617">__ПРИМЕЧАНИЕ.__ `bot prepare-publish` по-прежнему использует старое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-1617">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="cd667-1618">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `--lang` — значение `Csharp` больше не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-1618">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="cd667-1619">Если команда требует `--lang`, который не указан, команда завершит работу с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="cd667-1619">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="cd667-1620">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в аргументы `--appid` и `--password` для `bot create` — теперь они являются обязательными и их можно создать с помощью `ad app create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1620">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="cd667-1621">Добавлена проверка `--appid` и `--password`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1621">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="cd667-1622">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4`, чтобы не создавать или не использовать учетную запись хранения или Application Insights.</span><span class="sxs-lookup"><span data-stu-id="cd667-1622">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="cd667-1623">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v3`, чтобы требовать регион, где доступна служба Application Insights.</span><span class="sxs-lookup"><span data-stu-id="cd667-1623">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="cd667-1624">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot update`, чтобы влиять только на определенные свойства бота.</span><span class="sxs-lookup"><span data-stu-id="cd667-1624">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="cd667-1625">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в флаг `--lang` для принятия `Javascript` вместо `Node`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1625">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="cd667-1626">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`Node` больше не используется как допустимое значение `--lang`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1626">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="cd667-1627">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` — значение `SCM_DO_BUILD_DURING_DEPLOYMENT` больше не равно true.</span><span class="sxs-lookup"><span data-stu-id="cd667-1627">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="cd667-1628">Все развертывания через Kudu будут работать в соответствии с поведением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-1628">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="cd667-1629">Внесено изменение в `bot download` для ботов без файлов `.bot`, чтобы создавать файл конфигурации для определенного языка со значениями из параметров приложения для бота.</span><span class="sxs-lookup"><span data-stu-id="cd667-1629">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="cd667-1630">В команду `bot prepare-deploy` добавлена поддержка параметра `Typescript`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1630">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="cd667-1631">Добавлено предупреждающее сообщение в `bot prepare-deploy` для ботов `Javascript` и `Typescript`, когда `--code-dir` не содержит `package.json`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1631">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="cd667-1632">Внесено изменение в `bot prepare-deploy` для возврата `true` при успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="cd667-1632">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="cd667-1633">Включено ведение подробного журнала для `bot prepare-deploy`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1633">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="cd667-1634">Добавлены более доступные регионы Application Insights для `az bot create -v v3`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1634">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="cd667-1635">Configure</span><span class="sxs-lookup"><span data-stu-id="cd667-1635">Configure</span></span>
* <span data-ttu-id="cd667-1636">Добавлена поддержка конфигурации по умолчанию для аргумента на основе папки.</span><span class="sxs-lookup"><span data-stu-id="cd667-1636">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="cd667-1637">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="cd667-1637">Eventhubs</span></span>
* <span data-ttu-id="cd667-1638">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1638">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="cd667-1639">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1639">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="cd667-1640">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-1640">Network</span></span>
* <span data-ttu-id="cd667-1641">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--cache` на `--defer` для `vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1641">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="cd667-1642">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="cd667-1642">Policy Insights</span></span>
* <span data-ttu-id="cd667-1643">Добавлена поддержка `--expand PolicyEvaluationDetails` для результатов оценки политики запросов для ресурса.</span><span class="sxs-lookup"><span data-stu-id="cd667-1643">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="cd667-1644">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-1644">Role</span></span>
* <span data-ttu-id="cd667-1645">[УСТАРЕЛО] Внесено изменение в `create-for-rbac` для скрытия аргумента --password (поддержка прекращается в мае 2019 г.).</span><span class="sxs-lookup"><span data-stu-id="cd667-1645">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="cd667-1646">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="cd667-1646">Service Bus</span></span>
* <span data-ttu-id="cd667-1647">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1647">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="cd667-1648">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1648">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="cd667-1649">Внесено исправление в `topic [create|update]` — теперь `--max-size` поддерживает значения 10, 20, 40 и 80 ГБ для номера SKU ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="cd667-1649">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-1650">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-1650">SQL</span></span>
* <span data-ttu-id="cd667-1651">Добавлены команды `sql virtual-cluster [list|show|delete]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1651">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-1652">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-1652">VM</span></span>
* <span data-ttu-id="cd667-1653">Добавлены параметры `--protect-from-scale-in` и `--protect-from-scale-set-actions` для `vmss update`, чтобы включать обновления политики защиты для экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="cd667-1653">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="cd667-1654">Добавлены параметры `--instance-id` для `vmss update` для включения общего обновления экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="cd667-1654">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="cd667-1655">Добавлен параметр `--instance-id` для команды `vmss wait`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1655">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="cd667-1656">Добавлена новая группа команд `ppg` для управления группами размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="cd667-1656">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="cd667-1657">Добавлен параметр `--ppg` для `[vm|vmss] create` и `vm availability-set create` для управления PPG.</span><span class="sxs-lookup"><span data-stu-id="cd667-1657">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="cd667-1658">Добавлен параметр `--hyper-v-generation` для команды `image create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1658">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="cd667-1659">23 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1659">April 23, 2019</span></span>

<span data-ttu-id="cd667-1660">Версия 2.0.63</span><span class="sxs-lookup"><span data-stu-id="cd667-1660">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-1661">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-1661">ACS</span></span>
* <span data-ttu-id="cd667-1662">Внесено изменение в `aks get-credentials` для запроса на перезапись повторяющихся значений.</span><span class="sxs-lookup"><span data-stu-id="cd667-1662">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="cd667-1663">Удалено описание `(PREVIEW)` из команд Dev Spaces aks use-dev-spaces и aks remove-dev-spaces.</span><span class="sxs-lookup"><span data-stu-id="cd667-1663">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="cd667-1664">AMS</span><span class="sxs-lookup"><span data-stu-id="cd667-1664">AMS</span></span>
* <span data-ttu-id="cd667-1665">Исправлена ошибка с обновлением фильтров ресурсов и учетных записей.</span><span class="sxs-lookup"><span data-stu-id="cd667-1665">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-1666">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-1666">AppService</span></span>
* <span data-ttu-id="cd667-1667">Добавлена поддержка ASE и времени ожидания для `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1667">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="cd667-1668">Добавлена возможность настройки непрерывной интеграции и развертывания в конвейере Azure DevOps из репозитория Github для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="cd667-1668">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="cd667-1669">Добавлен аргумент `--github-pat` для `functionapp devops-build create` для получения личного маркера доступа Github.</span><span class="sxs-lookup"><span data-stu-id="cd667-1669">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="cd667-1670">Добавлен аргумент `--github-repository` для `functionapp devops-build create` для подключения репозитория Github, который содержит исходный код приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="cd667-1670">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="cd667-1671">Исправлена проблема со сбоем `az webapp up --logs` и обновлением .Net Core до версии 2.1 по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-1671">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="cd667-1672">Удалены ненужные параметры приложения-функции при создании приложения-функции с помощью плана потребления.</span><span class="sxs-lookup"><span data-stu-id="cd667-1672">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="cd667-1673">Внесены изменения в `webapp up`, чтобы строка ASP по умолчанию добавляла номера в конец для создания плана службы приложений на основе параметров SKU.</span><span class="sxs-lookup"><span data-stu-id="cd667-1673">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="cd667-1674">Добавлен параметр `-b` для `webapp up` для запуска приложения в браузере.</span><span class="sxs-lookup"><span data-stu-id="cd667-1674">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="cd667-1675">Внесены изменения в `webapp deployment source config zip` для обработки переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1675">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="cd667-1676">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="cd667-1676">Deployment Manager</span></span>
* <span data-ttu-id="cd667-1677">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Создание и администрирование артефактов, которые поддерживают развертывания</span><span class="sxs-lookup"><span data-stu-id="cd667-1677">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="cd667-1678">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="cd667-1678">Lab</span></span>
* <span data-ttu-id="cd667-1679">Исправлена ошибка, которая приводила к неожиданному завершению работы.</span><span class="sxs-lookup"><span data-stu-id="cd667-1679">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="cd667-1680">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-1680">Network</span></span>
* <span data-ttu-id="cd667-1681">Добавлено автоматическое делегирование сервера имен для `dns zone create` в родительском объекте во время создания дочерней зоны.</span><span class="sxs-lookup"><span data-stu-id="cd667-1681">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-1682">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-1682">Resource</span></span>
* <span data-ttu-id="cd667-1683">[УСТАРЕЛО] Не рекомендуются к использованию аргументы `--link-id`, `--target-id` и `--filter-string` для `resource link`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1683">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="cd667-1684">Используйте вместо них аргументы `--link`, `--target` и `--filter`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1684">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="cd667-1685">Исправлена проблема, из-за которой команды `resource link [create|update]` не работали.</span><span class="sxs-lookup"><span data-stu-id="cd667-1685">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="cd667-1686">Исправлена проблема, из-за которой удаление с помощью идентификатора ресурса приводило к сбою или ошибке.</span><span class="sxs-lookup"><span data-stu-id="cd667-1686">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-1687">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-1687">SQL</span></span>
* <span data-ttu-id="cd667-1688">Добавлена поддержка пользовательского часового пояса в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="cd667-1688">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="cd667-1689">Внесено изменение, чтобы разрешить использовать имя эластичного пула с `sql db update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1689">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="cd667-1690">В команду `sql server [create|update]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1690">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="cd667-1691">Добавлена команда `sql server wait`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1691">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-1692">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-1692">Storage</span></span>
* <span data-ttu-id="cd667-1693">Устранена проблема с двойной кодировкой маркеров SAS в `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1693">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-1694">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-1694">VM</span></span>
* <span data-ttu-id="cd667-1695">Добавлен флаг `--skip-shutdown` для `vm|vmss stop` для выключения виртуальных машин без завершения работы.</span><span class="sxs-lookup"><span data-stu-id="cd667-1695">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="cd667-1696">Добавлен аргумент `--storage-account-type` для `sig image-version create` настройки типа учетной записи профиля публикации.</span><span class="sxs-lookup"><span data-stu-id="cd667-1696">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="cd667-1697">Добавлен аргумент `--target-regions` для `sig image-version create` для указания типов учетных записей хранения, связанных с регионами.</span><span class="sxs-lookup"><span data-stu-id="cd667-1697">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="cd667-1698">9 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1698">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="cd667-1699">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-1699">Core</span></span>
* <span data-ttu-id="cd667-1700">Исправлена проблема, из-за которой для некоторых расширений отображалась версия `Unknown` и ее невозможно было обновить.</span><span class="sxs-lookup"><span data-stu-id="cd667-1700">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-1701">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-1701">ACR</span></span>
* <span data-ttu-id="cd667-1702">Добавлена поддержка запуска образа без контекста.</span><span class="sxs-lookup"><span data-stu-id="cd667-1702">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="cd667-1703">AMS</span><span class="sxs-lookup"><span data-stu-id="cd667-1703">AMS</span></span>
* [УСТАРЕЛО]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="cd667-1706">Добавлена поддержка новых параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1706">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="cd667-1707">Добавлен новый параметр `--filters` для `ams streaming-locator create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1707">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-1708">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-1708">AppService</span></span>
* <span data-ttu-id="cd667-1709">В команду `webapp up` добавлена поддержка параметра `--logs`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1709">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="cd667-1710">Исправлены ошибки в команде `functionapp devops-build create` при создании файла `azure-pipelines.yml`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1710">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="cd667-1711">Улучшена обработка и индикаторы ошибок с `unctionapp devops-build create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1711">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="cd667-1712">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--local-git` для команды `devops-build`. Обнаружение и обработка локального репозитория Git являются обязательными для создания конвейеров DevOps в Azure.</span><span class="sxs-lookup"><span data-stu-id="cd667-1712">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="cd667-1713">Добавлена поддержка создания плана функций Linux.</span><span class="sxs-lookup"><span data-stu-id="cd667-1713">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="cd667-1714">Добавлена возможность менять план для приложения-функции с помощью `functionapp update --plan`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1714">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="cd667-1715">Добавлена поддержка параметров горизонтального увеличения масштаба плана "Премиум" для Функций Azure.</span><span class="sxs-lookup"><span data-stu-id="cd667-1715">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="cd667-1716">CDN</span><span class="sxs-lookup"><span data-stu-id="cd667-1716">CDN</span></span>
* <span data-ttu-id="cd667-1717">Добавлена поддержка `Microsoft_Standard` и `Standard_ChinaCdn`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1717">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="cd667-1718">Отзывы</span><span class="sxs-lookup"><span data-stu-id="cd667-1718">Feedback</span></span>
* <span data-ttu-id="cd667-1719">Внесены изменения в `feedback` для отображения метаданных недавно выполненных команд.</span><span class="sxs-lookup"><span data-stu-id="cd667-1719">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="cd667-1720">Внесены изменения в `feedback`. Теперь при регистрации проблемы отображается запрос, в соответствии с которым пользователь должен открыть браузер и воспользоваться шаблоном проблемы.</span><span class="sxs-lookup"><span data-stu-id="cd667-1720">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="cd667-1721">Внесены изменения в `feedback`. Теперь текст проблемы выводится при запуске с параметром --verbose.</span><span class="sxs-lookup"><span data-stu-id="cd667-1721">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-1722">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-1722">Monitor</span></span>
* <span data-ttu-id="cd667-1723">Исправлена проблема, из-за которой у параметра count было недопустимое значение в `metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1723">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="cd667-1724">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-1724">Network</span></span>
* <span data-ttu-id="cd667-1725">Исправлен формат таблицы, которая не отображалась с помощью `vnet-gateway list-bgp-peer-status`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1725">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="cd667-1726">Добавлены команды `list-request-headers` и `list-response-headers` для `application-gateway rewrite-rule`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1726">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="cd667-1727">Добавлена команда `list-server-variables` для `application-gateway rewrite-rule condition`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1727">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="cd667-1728">Исправлена проблема, из-за которой обновление состояния соединения на порту ExpressRoute вызывало неизвестное исключение атрибута `express-route port update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1728">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="cd667-1729">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="cd667-1729">PrivateDNS</span></span>
* <span data-ttu-id="cd667-1730">Добавлена команда `network private-dns` для частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="cd667-1730">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-1731">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-1731">Resource</span></span>
* <span data-ttu-id="cd667-1732">Исправлена проблема с `deployment create` и `group deployment create`, из-за которой файл параметров с пустым набором параметров не работал.</span><span class="sxs-lookup"><span data-stu-id="cd667-1732">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="cd667-1733">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-1733">Role</span></span>
* <span data-ttu-id="cd667-1734">Внесены исправления в `create-for-rbac`. Теперь `--years` обрабатывается правильно.</span><span class="sxs-lookup"><span data-stu-id="cd667-1734">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="cd667-1735">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `role assignment delete`. Теперь появляется запрос при удалении всех назначений в рамках подписки без дополнительных условий.</span><span class="sxs-lookup"><span data-stu-id="cd667-1735">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-1736">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-1736">SQL</span></span>
* <span data-ttu-id="cd667-1737">Команда `sql mi [create|update]` обновлена с помощью свойств proxyOverride и publicDataEndpointEnabled.</span><span class="sxs-lookup"><span data-stu-id="cd667-1737">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-1738">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-1738">Storage</span></span>
* <span data-ttu-id="cd667-1739">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален результат выполнения `storage blob delete`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1739">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="cd667-1740">В команду `storage blob generate-sas` добавлен параметр `--full-uri` для создания полного URI большого двоичного объекта с помощью SAS.</span><span class="sxs-lookup"><span data-stu-id="cd667-1740">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="cd667-1741">В команду `storage file copy start` добавлен параметр `--file-snapshot` для копирования файла из моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="cd667-1741">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="cd667-1742">Внесены изменения в `storage blob copy cancel`. Теперь вместо исключения для NoPendingCopyOperation отображается только сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="cd667-1742">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="cd667-1743">26 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1743">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="cd667-1744">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-1744">Core</span></span>
* <span data-ttu-id="cd667-1745">Устранены проблемы с несовместимостью расширений для разработки.</span><span class="sxs-lookup"><span data-stu-id="cd667-1745">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="cd667-1746">Функция обработки ошибок теперь указывает клиентам на страницу проблем.</span><span class="sxs-lookup"><span data-stu-id="cd667-1746">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="cd667-1747">Cloud</span><span class="sxs-lookup"><span data-stu-id="cd667-1747">Cloud</span></span>
* <span data-ttu-id="cd667-1748">Исправлена ошибка с сообщением о не найденной подписке в `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1748">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-1749">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-1749">ACR</span></span>
* <span data-ttu-id="cd667-1750">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="cd667-1750">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="cd667-1751">Добавлено `--auth-mode` в команды `acr build`, `acr run`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1751">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="cd667-1752">Добавлена команда acr task credential для управления учетными данными для задачи.</span><span class="sxs-lookup"><span data-stu-id="cd667-1752">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="cd667-1753">Добавлено --no-wait в команду `acr build`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1753">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-1754">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-1754">AppService</span></span>
* <span data-ttu-id="cd667-1755">Исправлена ошибка с `webapp up`, из-за которой нельзя было правильно выполнить запуск из пустого каталога или скрипта неизвестного кода.</span><span class="sxs-lookup"><span data-stu-id="cd667-1755">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="cd667-1756">Исправлена ошибка, из-за которой не работали слоты для `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1756">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="cd667-1757">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="cd667-1757">BOT Service</span></span>
* <span data-ttu-id="cd667-1758">Добавлено `bot prepare-deploy` для подготовки к развертыванию ботов с помощью `webapp`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1758">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="cd667-1759">Изменено `bot create --kind registration` для отображения пароля, если пароль не указан.</span><span class="sxs-lookup"><span data-stu-id="cd667-1759">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="cd667-1760">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--endpoint` в `bot create --kind registration` на пустую строку (по умолчанию) вместо запрашиваемой.</span><span class="sxs-lookup"><span data-stu-id="cd667-1760">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="cd667-1761">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="cd667-1761">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="cd667-1762">CDN</span><span class="sxs-lookup"><span data-stu-id="cd667-1762">CDN</span></span>
* <span data-ttu-id="cd667-1763">Добавлена поддержка параметра `--no-wait` в команде `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1763">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="cd667-1764">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено поведение кэширования строки запроса `cdn endpoint create` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-1764">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="cd667-1765">IgnoreQueryString больше не используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-1765">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="cd667-1766">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="cd667-1766">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="cd667-1767">Сosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-1767">Cosmosdb</span></span>
* <span data-ttu-id="cd667-1768">Добавлена поддержка `--enable-multiple-write-locations` для обновления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="cd667-1768">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="cd667-1769">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="cd667-1769">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="cd667-1770">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="cd667-1770">Interactive</span></span>
* <span data-ttu-id="cd667-1771">Исправлена несовместимость с интерактивным расширением, установленным с помощью azdev.</span><span class="sxs-lookup"><span data-stu-id="cd667-1771">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-1772">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-1772">Monitor</span></span>
* <span data-ttu-id="cd667-1773">Внесено изменение, разрешающее использовать значение измерения `*` для `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1773">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="cd667-1774">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-1774">Network</span></span>
* <span data-ttu-id="cd667-1775">Добавлена группа команд `rewrite-rule` для `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1775">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-1776">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-1776">Profile</span></span>
* <span data-ttu-id="cd667-1777">Включена поддержка учетной записи уровня клиентов для управляемого удостоверения службы для `login`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1777">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="cd667-1778">Postgres</span><span class="sxs-lookup"><span data-stu-id="cd667-1778">Postgres</span></span> 
* <span data-ttu-id="cd667-1779">Добавлены команды postgresql `replica` и команда `restart server`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1779">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="cd667-1780">Внесены изменения для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="cd667-1780">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-1781">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-1781">Resource</span></span>
* <span data-ttu-id="cd667-1782">Улучшены табличные выходные данные для `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1782">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="cd667-1783">Исправлена проблема с `deployment [create|validate]`, из-за которой secureObject типа не распознавался.</span><span class="sxs-lookup"><span data-stu-id="cd667-1783">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="cd667-1784">График</span><span class="sxs-lookup"><span data-stu-id="cd667-1784">Graph</span></span>
* <span data-ttu-id="cd667-1785">Добавлена поддержка параметра `--end-date` в команде `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1785">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="cd667-1786">Добавлена поддержка разрешений для `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1786">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="cd667-1787">Исправлена проблема с `ad app permission list`, из-за которой отсутствовали разрешения.</span><span class="sxs-lookup"><span data-stu-id="cd667-1787">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="cd667-1788">Изменено `ad sp delete` для пропуска удаления назначения роли, если текущая учетная запись не содержит подписок.</span><span class="sxs-lookup"><span data-stu-id="cd667-1788">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="cd667-1789">Изменено `ad app create` для использования `--identifier-uris` пустого списка (по умолчанию), если список не указан.</span><span class="sxs-lookup"><span data-stu-id="cd667-1789">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-1790">носителей.</span><span class="sxs-lookup"><span data-stu-id="cd667-1790">storage</span></span>
* <span data-ttu-id="cd667-1791">Добавлено `--snapshot` для `storage file download-batch` для скачивания из моментального снимка общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="cd667-1791">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="cd667-1792">Изменен индикатор выполнения `storage blob [download-batch|upload-batch]`, чтобы обобщить сведения и указать текущий большой двоичный объект.</span><span class="sxs-lookup"><span data-stu-id="cd667-1792">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="cd667-1793">Исправлена проблема с `storage account update` при обновлении параметров шифрования.</span><span class="sxs-lookup"><span data-stu-id="cd667-1793">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="cd667-1794">Исправлена проблема со сбоем `storage blob show` при использовании OAuth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="cd667-1794">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-1795">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-1795">VM</span></span>
* <span data-ttu-id="cd667-1796">Добавлена команда `image update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1796">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="cd667-1797">12 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1797">March 12, 2019</span></span>

<span data-ttu-id="cd667-1798">Версия 2.0.60</span><span class="sxs-lookup"><span data-stu-id="cd667-1798">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="cd667-1799">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-1799">Core</span></span>

* <span data-ttu-id="cd667-1800">Исправлена недопустимая ошибка в `cloud set` о том, что подписка не найдена.</span><span class="sxs-lookup"><span data-stu-id="cd667-1800">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-1801">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-1801">ACR</span></span>

* <span data-ttu-id="cd667-1802">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="cd667-1802">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-1803">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-1803">ACS</span></span>

* <span data-ttu-id="cd667-1804">Внесены изменения, в соответствии с которыми параметр `--listen-address` для `aks browse` игнорируется, если он не поддерживается kubectl.</span><span class="sxs-lookup"><span data-stu-id="cd667-1804">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="cd667-1805">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-1805">AppService</span></span>

* <span data-ttu-id="cd667-1806">Добавлено `[webapp|functionapp] deployment list-publishing-credentials` для получения URL-адреса публикации Kudu и связанных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="cd667-1806">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="cd667-1807">Удалена ошибочная инструкция печати для `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1807">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="cd667-1808">Исправлено `functionapp` для настройки правильного образа для среды выполнения в планах службы приложений Linux.</span><span class="sxs-lookup"><span data-stu-id="cd667-1808">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="cd667-1809">Удален тег предварительной версии для `webapp up` и добавлены усовершенствования в команду.</span><span class="sxs-lookup"><span data-stu-id="cd667-1809">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="cd667-1810">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="cd667-1810">Botservice</span></span>

* <span data-ttu-id="cd667-1811">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="cd667-1811">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="cd667-1812">Добавлено `Microsoft-BotFramework-AppId` и `Microsoft-BotFramework-AppPassword` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="cd667-1812">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="cd667-1813">Удалены одинарные кавычки из выходных данных команды `bot publish` в конце `bot create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1813">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="cd667-1814">Изменено `bot publish` для включения поддержки асинхронных операций.</span><span class="sxs-lookup"><span data-stu-id="cd667-1814">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="cd667-1815">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-1815">Container</span></span>

* <span data-ttu-id="cd667-1816">Добавлен аргумент `--no-wait` для команды `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="cd667-1816">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="cd667-1817">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="cd667-1817">EventHub</span></span>

* <span data-ttu-id="cd667-1818">Добавлен флаг `--skip-empty-archives` для `eventhub create|update` для включения поддержки пустых архивов при записи.</span><span class="sxs-lookup"><span data-stu-id="cd667-1818">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="cd667-1819">Поиск</span><span class="sxs-lookup"><span data-stu-id="cd667-1819">Find</span></span>

* <span data-ttu-id="cd667-1820">Основные обновления функций</span><span class="sxs-lookup"><span data-stu-id="cd667-1820">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="cd667-1821">HDInsight</span><span class="sxs-lookup"><span data-stu-id="cd667-1821">HDInsight</span></span>

* <span data-ttu-id="cd667-1822">Добавлен параметр `--storage-account-managed-identity` для `hdinsight create` для включения поддержки MSI ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="cd667-1822">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="cd667-1823">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-1823">Network</span></span>

* <span data-ttu-id="cd667-1824">Исправлена проблема с `vpn-connection update`, когда обновление VPN-подключения между шлюзами в разных подписках завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="cd667-1824">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="cd667-1825">Rdbms</span><span class="sxs-lookup"><span data-stu-id="cd667-1825">Rdbms</span></span>

* <span data-ttu-id="cd667-1826">Незначительные исправления для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="cd667-1826">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="cd667-1827">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-1827">Role</span></span>

* <span data-ttu-id="cd667-1828">Исправлено `role definition update` для использования идентификатора для правильного разрешения определения.</span><span class="sxs-lookup"><span data-stu-id="cd667-1828">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="cd667-1829">Изменено `ad app credential reset` для исключения предположения о том, что субъект-служба приложения всегда существует.</span><span class="sxs-lookup"><span data-stu-id="cd667-1829">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="cd667-1830">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="cd667-1830">Service Fabric</span></span>

* <span data-ttu-id="cd667-1831">Исправлена проблема с `sf cluster list` и невозможностью итерации.</span><span class="sxs-lookup"><span data-stu-id="cd667-1831">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="cd667-1832">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1832">February 26, 2019</span></span>

<span data-ttu-id="cd667-1833">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="cd667-1833">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="cd667-1834">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-1834">Core</span></span>

* <span data-ttu-id="cd667-1835">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="cd667-1835">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-1836">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-1836">ACR</span></span>

* <span data-ttu-id="cd667-1837">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1837">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="cd667-1838">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="cd667-1838">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-1839">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-1839">ACS</span></span>

* <span data-ttu-id="cd667-1840">Добавлен параметр `--listen-address` для команды `aks port-forward`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1840">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-1841">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-1841">AppService</span></span>

* <span data-ttu-id="cd667-1842">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1842">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="cd667-1843">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-1843">Batch</span></span>
* <span data-ttu-id="cd667-1844">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1844">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="cd667-1845">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1845">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="cd667-1846">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="cd667-1846">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="cd667-1847">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1847">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="cd667-1848">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="cd667-1848">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="cd667-1849">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cd667-1849">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="cd667-1850">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-1850">CosmosDB</span></span>

* <span data-ttu-id="cd667-1851">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="cd667-1851">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="cd667-1852">Kusto</span><span class="sxs-lookup"><span data-stu-id="cd667-1852">Kusto</span></span>

* <span data-ttu-id="cd667-1853">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="cd667-1853">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="cd667-1854">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-1854">Network</span></span>

* <span data-ttu-id="cd667-1855">Добавлен аргумент `--express-route-gateway-bypass` для команды `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="cd667-1855">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="cd667-1856">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1856">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="cd667-1857">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1857">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="cd667-1858">Добавлен аргумент `--legacy-mode` в команду `express-route peering [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1858">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="cd667-1859">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1859">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="cd667-1860">Добавлен аргумент `--gateway-default-site` для команды `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="cd667-1860">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="cd667-1861">Добавлены команды `ipsec-policy` для `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1861">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-1862">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-1862">Resource</span></span>

* <span data-ttu-id="cd667-1863">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="cd667-1863">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="cd667-1864">Добавлена поддержка файла параметров на основе URI для `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1864">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="cd667-1865">Добавлена поддержка определений и параметров на основе URI для `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1865">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="cd667-1866">Исправлена обработка параметров и правил для `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1866">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="cd667-1867">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="cd667-1867">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="cd667-1868">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-1868">Role</span></span>

* <span data-ttu-id="cd667-1869">Добавлена поддержка ролей приложений для `ad app [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1869">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-1870">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-1870">VM</span></span>

* <span data-ttu-id="cd667-1871">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="cd667-1871">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="cd667-1872">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1872">February 12, 2019</span></span>

<span data-ttu-id="cd667-1873">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="cd667-1873">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="cd667-1874">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-1874">Core</span></span>

* <span data-ttu-id="cd667-1875">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="cd667-1875">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="cd667-1876">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="cd667-1876">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-1877">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-1877">ACR</span></span>
* <span data-ttu-id="cd667-1878">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1878">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="cd667-1879">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1879">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-1880">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-1880">ACS</span></span>
* <span data-ttu-id="cd667-1881">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="cd667-1881">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="cd667-1882">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1882">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="cd667-1883">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="cd667-1883">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="cd667-1884">AMS</span><span class="sxs-lookup"><span data-stu-id="cd667-1884">AMS</span></span>
* <span data-ttu-id="cd667-1885">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1885">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="cd667-1886">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1886">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-1887">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-1887">Appservice</span></span>
* <span data-ttu-id="cd667-1888">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="cd667-1888">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="cd667-1889">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="cd667-1889">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="cd667-1890">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1890">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="cd667-1891">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="cd667-1891">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="cd667-1892">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="cd667-1892">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="cd667-1893">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="cd667-1893">Botservice</span></span>
* <span data-ttu-id="cd667-1894">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1894">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="cd667-1895">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1895">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="cd667-1896">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1896">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="cd667-1897">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="cd667-1897">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="cd667-1898">[УСТАРЕЛО] Аргумент `--proj-name` не рекомендуется к использованию. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1898">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="cd667-1899">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="cd667-1899">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="cd667-1900">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="cd667-1900">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="cd667-1901">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="cd667-1901">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="cd667-1902">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="cd667-1902">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="cd667-1903">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="cd667-1903">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="cd667-1904">Key Vault</span><span class="sxs-lookup"><span data-stu-id="cd667-1904">Key Vault</span></span>
* <span data-ttu-id="cd667-1905">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1905">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-1906">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-1906">Monitor</span></span>
* <span data-ttu-id="cd667-1907">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1907">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="cd667-1908">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-1908">Network</span></span>
* <span data-ttu-id="cd667-1909">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="cd667-1909">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="cd667-1910">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="cd667-1910">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="cd667-1911">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="cd667-1911">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="cd667-1912">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1912">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="cd667-1913">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="cd667-1913">Policy Insights</span></span>
* <span data-ttu-id="cd667-1914">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd667-1914">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="cd667-1915">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="cd667-1915">RDBMS</span></span>
* <span data-ttu-id="cd667-1916">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="cd667-1916">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="cd667-1917">Redis</span><span class="sxs-lookup"><span data-stu-id="cd667-1917">Redis</span></span>
* <span data-ttu-id="cd667-1918">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="cd667-1918">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="cd667-1919">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="cd667-1919">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="cd667-1920">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="cd667-1920">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="cd667-1921">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="cd667-1921">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="cd667-1922">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1922">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="cd667-1923">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="cd667-1923">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="cd667-1924">[УСТАРЕЛО] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd667-1924">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="cd667-1925">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-1925">Role</span></span>
* <span data-ttu-id="cd667-1926">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1926">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="cd667-1927">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-1927">SQL VM</span></span>
* <span data-ttu-id="cd667-1928">[УСТАРЕЛО] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="cd667-1928">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-1929">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-1929">VM</span></span>
* <span data-ttu-id="cd667-1930">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1930">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="cd667-1931">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1931">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="cd667-1932">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="cd667-1932">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="cd667-1933">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1933">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="cd667-1934">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1934">January 31, 2019</span></span>

<span data-ttu-id="cd667-1935">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="cd667-1935">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="cd667-1936">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-1936">Core</span></span>

* <span data-ttu-id="cd667-1937">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="cd667-1937">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="cd667-1938">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1938">January 28, 2019</span></span>

<span data-ttu-id="cd667-1939">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="cd667-1939">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-1940">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-1940">ACR</span></span>
* <span data-ttu-id="cd667-1941">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="cd667-1941">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-1942">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-1942">ACS</span></span>
* <span data-ttu-id="cd667-1943">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="cd667-1943">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="cd667-1944">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="cd667-1944">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="cd667-1945">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1945">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="cd667-1946">AMS</span><span class="sxs-lookup"><span data-stu-id="cd667-1946">AMS</span></span>
* <span data-ttu-id="cd667-1947">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1947">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="cd667-1948">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1948">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-1949">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-1949">Appservice</span></span>
* <span data-ttu-id="cd667-1950">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1950">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="cd667-1951">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="cd667-1951">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="cd667-1952">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="cd667-1952">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="cd667-1953">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-1953">Container</span></span>
* <span data-ttu-id="cd667-1954">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1954">Added `container start` command</span></span>
* <span data-ttu-id="cd667-1955">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="cd667-1955">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="cd667-1956">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="cd667-1956">EventGrid</span></span>
* <span data-ttu-id="cd667-1957">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1957">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="cd667-1958">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1958">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="cd667-1959">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="cd667-1959">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="cd667-1960">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="cd667-1960">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="cd667-1961">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="cd667-1961">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="cd667-1962">HDInsight</span><span class="sxs-lookup"><span data-stu-id="cd667-1962">HDInsight</span></span>
* <span data-ttu-id="cd667-1963">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1963">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="cd667-1964">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="cd667-1964">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="cd667-1965">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1965">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="cd667-1966">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="cd667-1966">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="cd667-1967">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1967">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="cd667-1968">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1968">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-1969">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-1969">IoT</span></span>
* <span data-ttu-id="cd667-1970">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="cd667-1970">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="cd667-1971">Kusto</span><span class="sxs-lookup"><span data-stu-id="cd667-1971">Kusto</span></span>
* <span data-ttu-id="cd667-1972">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="cd667-1972">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-1973">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-1973">Monitor</span></span>
* <span data-ttu-id="cd667-1974">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="cd667-1974">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-1975">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-1975">Profile</span></span>
* <span data-ttu-id="cd667-1976">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="cd667-1976">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="cd667-1977">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-1977">Network</span></span>
* <span data-ttu-id="cd667-1978">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1978">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="cd667-1979">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="cd667-1979">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-1980">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-1980">Resource</span></span>
* <span data-ttu-id="cd667-1981">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1981">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="cd667-1982">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1982">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="cd667-1983">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-1983">SQL Virtual Machine</span></span>
* <span data-ttu-id="cd667-1984">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="cd667-1984">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-1985">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-1985">Storage</span></span>
* <span data-ttu-id="cd667-1986">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="cd667-1986">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="cd667-1987">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="cd667-1987">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-1988">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-1988">VM</span></span>
* <span data-ttu-id="cd667-1989">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="cd667-1989">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="cd667-1990">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="cd667-1990">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="cd667-1991">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-1991">January 15, 2019</span></span>

<span data-ttu-id="cd667-1992">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="cd667-1992">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-1993">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-1993">ACR</span></span>
* <span data-ttu-id="cd667-1994">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="cd667-1994">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="cd667-1995">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="cd667-1995">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="cd667-1996">[УСТАРЕЛО] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="cd667-1996">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="cd667-1997">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-1997">ACS</span></span>
* <span data-ttu-id="cd667-1998">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="cd667-1998">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-1999">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-1999">Appservice</span></span>
* <span data-ttu-id="cd667-2000">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="cd667-2000">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="cd667-2001">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="cd667-2001">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="cd667-2002">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="cd667-2002">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="cd667-2003">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2003">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="cd667-2004">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="cd667-2004">Botservice</span></span>
* <span data-ttu-id="cd667-2005">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2005">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="cd667-2006">Configure</span><span class="sxs-lookup"><span data-stu-id="cd667-2006">Configure</span></span>
* <span data-ttu-id="cd667-2007">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2007">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="cd667-2008">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-2008">CosmosDB</span></span>
* <span data-ttu-id="cd667-2009">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="cd667-2009">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="cd667-2010">HDInsight</span><span class="sxs-lookup"><span data-stu-id="cd667-2010">HDInsight</span></span>
* <span data-ttu-id="cd667-2011">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="cd667-2011">Added commands for managing applications</span></span>
* <span data-ttu-id="cd667-2012">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2012">Added commands for managing script actions</span></span>
* <span data-ttu-id="cd667-2013">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="cd667-2013">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="cd667-2014">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2014">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="cd667-2015">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-2015">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="cd667-2016">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-2016">Network</span></span>
* <span data-ttu-id="cd667-2017">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="cd667-2017">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="cd667-2018">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="cd667-2018">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="cd667-2019">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="cd667-2019">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="cd667-2020">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2020">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="cd667-2021">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-2021">Role</span></span>
* <span data-ttu-id="cd667-2022">[УСТАРЕЛО] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd667-2022">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="cd667-2023">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="cd667-2023">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="cd667-2024">Безопасность</span><span class="sxs-lookup"><span data-stu-id="cd667-2024">Security</span></span>
* <span data-ttu-id="cd667-2025">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="cd667-2025">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-2026">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-2026">Storage</span></span>
* <span data-ttu-id="cd667-2027">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="cd667-2027">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="cd667-2028">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2028">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="cd667-2029">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2029">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="cd667-2030">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2030">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="cd667-2031">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2031">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2032">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2032">VM</span></span>
* <span data-ttu-id="cd667-2033">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="cd667-2033">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="cd667-2034">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2034">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="cd667-2035">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2035">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="cd667-2036">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="cd667-2036">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="cd667-2037">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-2037">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="cd667-2038">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="cd667-2038">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="cd667-2039">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2039">December 20, 2018</span></span>

<span data-ttu-id="cd667-2040">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="cd667-2040">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="cd667-2041">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-2041">Appservice</span></span>
* <span data-ttu-id="cd667-2042">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="cd667-2042">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="cd667-2043">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="cd667-2043">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="cd667-2044">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="cd667-2044">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="cd667-2045">IoT Central</span><span class="sxs-lookup"><span data-stu-id="cd667-2045">IoTCentral</span></span>
* <span data-ttu-id="cd667-2046">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="cd667-2046">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="cd667-2047">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-2047">Role</span></span>
* <span data-ttu-id="cd667-2048">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2048">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-2049">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-2049">SQL</span></span>
* <span data-ttu-id="cd667-2050">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="cd667-2050">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2051">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2051">VM</span></span>
* <span data-ttu-id="cd667-2052">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2052">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="cd667-2053">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2053">December 18, 2018</span></span>

<span data-ttu-id="cd667-2054">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="cd667-2054">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="cd667-2055">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-2055">ACR</span></span>
* <span data-ttu-id="cd667-2056">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="cd667-2056">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="cd667-2057">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="cd667-2057">Condensed the table layout for task list</span></span>
* <span data-ttu-id="cd667-2058">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="cd667-2058">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-2059">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-2059">ACS</span></span>
* <span data-ttu-id="cd667-2060">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2060">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="cd667-2061">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="cd667-2061">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="cd667-2062">[УСТАРЕЛО] Команды `az acs` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="cd667-2062">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="cd667-2063">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2063">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="cd667-2064">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="cd667-2064">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="cd667-2065">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2065">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-2066">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-2066">Appservice</span></span>
* <span data-ttu-id="cd667-2067">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2067">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="cd667-2068">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="cd667-2068">Botservice</span></span>
* <span data-ttu-id="cd667-2069">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2069">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="cd667-2070">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="cd667-2070">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="cd667-2071">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="cd667-2071">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="cd667-2072">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="cd667-2072">Reduced Kudu network calls</span></span>
* <span data-ttu-id="cd667-2073">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="cd667-2073">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="cd667-2074">Потребление</span><span class="sxs-lookup"><span data-stu-id="cd667-2074">Consumption</span></span>
* <span data-ttu-id="cd667-2075">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="cd667-2075">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="cd667-2076">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-2076">CosmosDB</span></span>
* <span data-ttu-id="cd667-2077">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="cd667-2077">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="cd667-2078">Maps</span><span class="sxs-lookup"><span data-stu-id="cd667-2078">Maps</span></span>
* <span data-ttu-id="cd667-2079">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="cd667-2079">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="cd667-2080">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-2080">Network</span></span>
* <span data-ttu-id="cd667-2081">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2081">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="cd667-2082">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="cd667-2082">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-2083">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-2083">Resource</span></span>
* <span data-ttu-id="cd667-2084">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2084">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="cd667-2085">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2085">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-2086">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-2086">Storage</span></span>
*  <span data-ttu-id="cd667-2087">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="cd667-2087">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2088">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2088">VM</span></span>
* <span data-ttu-id="cd667-2089">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="cd667-2089">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="cd667-2090">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2090">December 4, 2018</span></span>

<span data-ttu-id="cd667-2091">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="cd667-2091">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="cd667-2092">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-2092">Core</span></span>
* <span data-ttu-id="cd667-2093">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="cd667-2093">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="cd667-2094">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="cd667-2094">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-2095">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-2095">Appservice</span></span>
* <span data-ttu-id="cd667-2096">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="cd667-2096">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="cd667-2097">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="cd667-2097">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="cd667-2098">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-2098">Network</span></span>
* <span data-ttu-id="cd667-2099">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="cd667-2099">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="cd667-2100">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-2100">Role</span></span>
* <span data-ttu-id="cd667-2101">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="cd667-2101">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="cd667-2102">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2102">VM</span></span>
* <span data-ttu-id="cd667-2103">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd667-2103">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="cd667-2104">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="cd667-2104">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="cd667-2105">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="cd667-2105">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="cd667-2106">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="cd667-2106">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="cd667-2107">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2107">November 20, 2018</span></span>

<span data-ttu-id="cd667-2108">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="cd667-2108">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="cd667-2109">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-2109">Core</span></span>
* <span data-ttu-id="cd667-2110">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="cd667-2110">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-2111">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-2111">ACR</span></span>
* <span data-ttu-id="cd667-2112">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="cd667-2112">Added context token to task step</span></span>
* <span data-ttu-id="cd667-2113">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="cd667-2113">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="cd667-2114">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2114">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-2115">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-2115">Appservice</span></span>
* <span data-ttu-id="cd667-2116">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="cd667-2116">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="cd667-2117">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-2117">Updated the default `node_version`.</span></span> <span data-ttu-id="cd667-2118">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="cd667-2118">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="cd667-2119">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="cd667-2119">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="cd667-2120">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="cd667-2120">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="cd667-2121">IotCentral</span><span class="sxs-lookup"><span data-stu-id="cd667-2121">IotCentral</span></span>
* <span data-ttu-id="cd667-2122">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="cd667-2122">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="cd667-2123">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="cd667-2123">KeyVault</span></span>
* <span data-ttu-id="cd667-2124">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="cd667-2124">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="cd667-2125">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-2125">Network</span></span>
* <span data-ttu-id="cd667-2126">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2126">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="cd667-2127">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2127">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="cd667-2128">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="cd667-2128">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="cd667-2129">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2129">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="cd667-2130">Rdbms</span><span class="sxs-lookup"><span data-stu-id="cd667-2130">Rdbms</span></span>
* <span data-ttu-id="cd667-2131">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="cd667-2131">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="cd667-2132">RBAC:</span><span class="sxs-lookup"><span data-stu-id="cd667-2132">Rbac</span></span>
* <span data-ttu-id="cd667-2133">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2133">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="cd667-2134">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="cd667-2134">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="cd667-2135">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-2135">Storage</span></span>
* <span data-ttu-id="cd667-2136">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="cd667-2136">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="cd667-2137">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2137">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="cd667-2138">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="cd667-2138">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="cd667-2139">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2139">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2140">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2140">VM</span></span>
* <span data-ttu-id="cd667-2141">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="cd667-2141">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="cd667-2142">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2142">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="cd667-2143">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2143">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="cd667-2144">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="cd667-2144">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="cd667-2145">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2145">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="cd667-2146">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2146">Added `snapshot wait` command</span></span>
* <span data-ttu-id="cd667-2147">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2147">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="cd667-2148">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2148">November 6, 2018</span></span>

<span data-ttu-id="cd667-2149">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="cd667-2149">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="cd667-2150">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-2150">Core</span></span>
* <span data-ttu-id="cd667-2151">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="cd667-2151">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-2152">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-2152">ACR</span></span>
* <span data-ttu-id="cd667-2153">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="cd667-2153">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="cd667-2154">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="cd667-2154">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-2155">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-2155">ACS</span></span>
* <span data-ttu-id="cd667-2156">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-2156">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="cd667-2157">Помощник</span><span class="sxs-lookup"><span data-stu-id="cd667-2157">Advisor</span></span>
* <span data-ttu-id="cd667-2158">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="cd667-2158">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="cd667-2159">AMS</span><span class="sxs-lookup"><span data-stu-id="cd667-2159">AMS</span></span>
* <span data-ttu-id="cd667-2160">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="cd667-2160">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="cd667-2161">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="cd667-2161">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="cd667-2162">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2162">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="cd667-2163">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="cd667-2163">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="cd667-2164">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2164">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="cd667-2165">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2165">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="cd667-2166">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2166">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="cd667-2167">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2167">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="cd667-2168">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2168">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="cd667-2169">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2169">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="cd667-2170">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2170">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="cd667-2171">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2171">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="cd667-2172">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="cd667-2172">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="cd667-2173">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="cd667-2173">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="cd667-2174">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2174">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="cd667-2175">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="cd667-2175">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="cd667-2176">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="cd667-2176">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-2177">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-2177">AppService</span></span>
* <span data-ttu-id="cd667-2178">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="cd667-2178">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="cd667-2179">Configure</span><span class="sxs-lookup"><span data-stu-id="cd667-2179">Configure</span></span>
* <span data-ttu-id="cd667-2180">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="cd667-2180">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="cd667-2181">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-2181">Container</span></span>
* <span data-ttu-id="cd667-2182">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="cd667-2182">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="cd667-2183">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="cd667-2183">EventHub</span></span>
* <span data-ttu-id="cd667-2184">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2184">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="cd667-2185">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="cd667-2185">Interactive</span></span>
* <span data-ttu-id="cd667-2186">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="cd667-2186">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-2187">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-2187">Monitor</span></span>
* <span data-ttu-id="cd667-2188">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2188">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="cd667-2189">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-2189">Network</span></span>
* <span data-ttu-id="cd667-2190">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2190">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="cd667-2191">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="cd667-2191">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="cd667-2192">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2192">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="cd667-2193">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-2193">Profile</span></span>
* <span data-ttu-id="cd667-2194">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2194">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="cd667-2195">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="cd667-2195">RDBMS</span></span>
* <span data-ttu-id="cd667-2196">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="cd667-2196">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-2197">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-2197">Resource</span></span>
* <span data-ttu-id="cd667-2198">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2198">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="cd667-2199">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-2199">Role</span></span>
* <span data-ttu-id="cd667-2200">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="cd667-2200">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="cd667-2201">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="cd667-2201">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="cd667-2202">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="cd667-2202">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-2203">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-2203">Storage</span></span>
* <span data-ttu-id="cd667-2204">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2204">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2205">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2205">VM</span></span>
* <span data-ttu-id="cd667-2206">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="cd667-2206">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="cd667-2207">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="cd667-2207">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="cd667-2208">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="cd667-2208">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="cd667-2209">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="cd667-2209">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="cd667-2210">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="cd667-2210">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="cd667-2211">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2211">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="cd667-2212">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2212">October 23, 2018</span></span>

<span data-ttu-id="cd667-2213">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="cd667-2213">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="cd667-2214">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-2214">Core</span></span>
* <span data-ttu-id="cd667-2215">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2215">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="cd667-2216">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2216">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-2217">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-2217">ACR</span></span>
* <span data-ttu-id="cd667-2218">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="cd667-2218">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="cd667-2219">CDN</span><span class="sxs-lookup"><span data-stu-id="cd667-2219">CDN</span></span>
* <span data-ttu-id="cd667-2220">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-2220">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="cd667-2221">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="cd667-2221">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="cd667-2222">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-2222">Container</span></span>
* <span data-ttu-id="cd667-2223">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="cd667-2223">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="cd667-2224">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="cd667-2224">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="cd667-2225">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2225">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="cd667-2226">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="cd667-2226">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="cd667-2227">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="cd667-2227">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="cd667-2228">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="cd667-2228">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="cd667-2229">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2229">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="cd667-2230">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-2230">CosmosDB</span></span>
* <span data-ttu-id="cd667-2231">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2231">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="cd667-2232">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="cd667-2232">Interactive</span></span>
* <span data-ttu-id="cd667-2233">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="cd667-2233">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="cd667-2234">IoT Central</span><span class="sxs-lookup"><span data-stu-id="cd667-2234">IoT Central</span></span>
* <span data-ttu-id="cd667-2235">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="cd667-2235">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="cd667-2236">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="cd667-2236">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-2237">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-2237">Monitor</span></span>
* <span data-ttu-id="cd667-2238">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="cd667-2238">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="cd667-2239">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="cd667-2239">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="cd667-2240">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="cd667-2240">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="cd667-2241">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="cd667-2241">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="cd667-2242">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2242">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="cd667-2243">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="cd667-2243">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="cd667-2244">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="cd667-2244">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="cd667-2245">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="cd667-2245">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="cd667-2246">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="cd667-2246">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="cd667-2247">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2247">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="cd667-2248">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-2248">Network</span></span>
* <span data-ttu-id="cd667-2249">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="cd667-2249">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="cd667-2250">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="cd667-2250">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="cd667-2251">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="cd667-2251">ServiceBus</span></span>
* <span data-ttu-id="cd667-2252">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="cd667-2252">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-2253">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-2253">SQL</span></span>
* <span data-ttu-id="cd667-2254">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="cd667-2254">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-2255">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-2255">Storage</span></span>
* <span data-ttu-id="cd667-2256">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="cd667-2256">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="cd667-2257">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="cd667-2257">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2258">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2258">VM</span></span>
* <span data-ttu-id="cd667-2259">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="cd667-2259">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="cd667-2260">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="cd667-2260">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="cd667-2261">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="cd667-2261">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="cd667-2262">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2262">October 16, 2018</span></span>

<span data-ttu-id="cd667-2263">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="cd667-2263">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2264">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2264">VM</span></span>
* <span data-ttu-id="cd667-2265">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="cd667-2265">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="cd667-2266">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2266">October 9, 2018</span></span>

<span data-ttu-id="cd667-2267">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="cd667-2267">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="cd667-2268">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-2268">Core</span></span>
* <span data-ttu-id="cd667-2269">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="cd667-2269">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-2270">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-2270">ACR</span></span>
* <span data-ttu-id="cd667-2271">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="cd667-2271">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-2272">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-2272">ACS</span></span>
* <span data-ttu-id="cd667-2273">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="cd667-2273">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="cd667-2274">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="cd667-2274">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="cd667-2275">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2275">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="cd667-2276">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="cd667-2276">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="cd667-2277">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-2277">Container</span></span>
* <span data-ttu-id="cd667-2278">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="cd667-2278">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="cd667-2279">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="cd667-2279">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="cd667-2280">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="cd667-2280">Event Hub</span></span>
* <span data-ttu-id="cd667-2281">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2281">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="cd667-2282">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="cd667-2282">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="cd667-2283">Модули</span><span class="sxs-lookup"><span data-stu-id="cd667-2283">Extensions</span></span>
* <span data-ttu-id="cd667-2284">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="cd667-2284">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="cd667-2285">HDInsight</span><span class="sxs-lookup"><span data-stu-id="cd667-2285">HDInsight</span></span>
* <span data-ttu-id="cd667-2286">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="cd667-2286">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-2287">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-2287">IoT</span></span>
* <span data-ttu-id="cd667-2288">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="cd667-2288">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="cd667-2289">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="cd667-2289">KeyVault</span></span>
* <span data-ttu-id="cd667-2290">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="cd667-2290">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="cd667-2291">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-2291">Network</span></span>
* <span data-ttu-id="cd667-2292">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-2292">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="cd667-2293">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="cd667-2293">See #6052</span></span>
* <span data-ttu-id="cd667-2294">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2294">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="cd667-2295">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="cd667-2295">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="cd667-2296">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2296">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="cd667-2297">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2297">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="cd667-2298">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2298">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="cd667-2299">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2299">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="cd667-2300">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-2300">Role</span></span>
* <span data-ttu-id="cd667-2301">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2301">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="cd667-2302">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2302">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="cd667-2303">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="cd667-2303">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="cd667-2304">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="cd667-2304">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="cd667-2305">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="cd667-2305">Service Bus</span></span>
* <span data-ttu-id="cd667-2306">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="cd667-2306">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2307">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2307">VM</span></span>
* <span data-ttu-id="cd667-2308">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2308">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="cd667-2309">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="cd667-2309">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="cd667-2310">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2310">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="cd667-2311">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2311">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="cd667-2312">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="cd667-2312">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="cd667-2313">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="cd667-2313">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="cd667-2314">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2314">September 21, 2018</span></span>

<span data-ttu-id="cd667-2315">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="cd667-2315">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-2316">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-2316">ACR</span></span>
* <span data-ttu-id="cd667-2317">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="cd667-2317">Added ACR Task commands</span></span>
* <span data-ttu-id="cd667-2318">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="cd667-2318">Added quick run command</span></span>
* <span data-ttu-id="cd667-2319">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="cd667-2319">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="cd667-2320">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="cd667-2320">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="cd667-2321">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="cd667-2321">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="cd667-2322">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="cd667-2322">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-2323">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-2323">ACS</span></span>
* <span data-ttu-id="cd667-2324">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="cd667-2324">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="cd667-2325">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="cd667-2325">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-2326">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-2326">AppService</span></span>

* <span data-ttu-id="cd667-2327">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="cd667-2327">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="cd667-2328">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="cd667-2328">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="cd667-2329">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="cd667-2329">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="cd667-2330">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="cd667-2330">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="cd667-2331">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-2331">Batch</span></span>
* <span data-ttu-id="cd667-2332">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="cd667-2332">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="cd667-2333">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2333">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="cd667-2334">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2334">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="cd667-2335">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="cd667-2335">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="cd667-2336">Batch AI</span><span class="sxs-lookup"><span data-stu-id="cd667-2336">Batch AI</span></span> 
* <span data-ttu-id="cd667-2337">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2337">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="cd667-2338">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="cd667-2338">Cognitive Services</span></span>
* <span data-ttu-id="cd667-2339">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2339">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="cd667-2340">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2340">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="cd667-2341">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2341">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="cd667-2342">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2342">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="cd667-2343">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="cd667-2343">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="cd667-2344">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2344">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="cd667-2345">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-2345">Container</span></span>
* <span data-ttu-id="cd667-2346">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="cd667-2346">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="cd667-2347">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="cd667-2347">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="cd667-2348">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="cd667-2348">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="cd667-2349">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="cd667-2349">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="cd667-2350">Data Lake</span><span class="sxs-lookup"><span data-stu-id="cd667-2350">Datalake</span></span>
* <span data-ttu-id="cd667-2351">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="cd667-2351">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="cd667-2352">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="cd667-2352">Interactive Shell</span></span>
* <span data-ttu-id="cd667-2353">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="cd667-2353">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="cd667-2354">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2354">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-2355">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-2355">IoT</span></span>
* <span data-ttu-id="cd667-2356">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="cd667-2356">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="cd667-2357">Key Vault</span><span class="sxs-lookup"><span data-stu-id="cd667-2357">Key Vault</span></span>
* <span data-ttu-id="cd667-2358">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="cd667-2358">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="cd667-2359">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-2359">Network</span></span>
* <span data-ttu-id="cd667-2360">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2360">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="cd667-2361">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="cd667-2361">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="cd667-2362">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="cd667-2362">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="cd667-2363">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2363">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="cd667-2364">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2364">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="cd667-2365">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2365">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="cd667-2366">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="cd667-2366">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="cd667-2367">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2367">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="cd667-2368">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2368">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="cd667-2369">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2369">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="cd667-2370">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2370">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="cd667-2371">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2371">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="cd667-2372">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2372">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="cd667-2373">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="cd667-2373">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="cd667-2374">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2374">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="cd667-2375">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="cd667-2375">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="cd667-2376">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="cd667-2376">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="cd667-2377">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="cd667-2377">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="cd667-2378">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="cd667-2378">RDBMS</span></span>
* <span data-ttu-id="cd667-2379">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="cd667-2379">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="cd667-2380">резервирование.</span><span class="sxs-lookup"><span data-stu-id="cd667-2380">Reservation</span></span>
* <span data-ttu-id="cd667-2381">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2381">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="cd667-2382">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="cd667-2382">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="cd667-2383">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="cd667-2383">Manage App</span></span>
* <span data-ttu-id="cd667-2384">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="cd667-2384">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="cd667-2385">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="cd667-2385">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="cd667-2386">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-2386">Role</span></span>
* <span data-ttu-id="cd667-2387">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="cd667-2387">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="cd667-2388">SignalR</span><span class="sxs-lookup"><span data-stu-id="cd667-2388">SignalR</span></span>
* <span data-ttu-id="cd667-2389">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="cd667-2389">First release</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-2390">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-2390">Storage</span></span>
* <span data-ttu-id="cd667-2391">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="cd667-2391">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="cd667-2392">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="cd667-2392">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2393">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2393">VM</span></span>
* <span data-ttu-id="cd667-2394">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="cd667-2394">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="cd667-2395">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2395">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="cd667-2396">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2396">August 28, 2018</span></span>

<span data-ttu-id="cd667-2397">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="cd667-2397">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="cd667-2398">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-2398">Core</span></span>

* <span data-ttu-id="cd667-2399">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="cd667-2399">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="cd667-2400">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="cd667-2400">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-2401">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-2401">ACR</span></span>

* <span data-ttu-id="cd667-2402">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="cd667-2402">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="cd667-2403">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2403">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-2404">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-2404">ACS</span></span>

* <span data-ttu-id="cd667-2405">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2405">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="cd667-2406">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="cd667-2406">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-2407">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-2407">AppService</span></span>

* <span data-ttu-id="cd667-2408">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="cd667-2408">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="cd667-2409">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="cd667-2409">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="cd667-2410">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="cd667-2410">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="cd667-2411">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="cd667-2411">Backup</span></span>

* <span data-ttu-id="cd667-2412">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="cd667-2412">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="cd667-2413">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="cd667-2413">Bot Service</span></span>

* <span data-ttu-id="cd667-2414">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="cd667-2414">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="cd667-2415">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="cd667-2415">Cognitive Services</span></span>

* <span data-ttu-id="cd667-2416">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="cd667-2416">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-2417">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-2417">IoT</span></span>

* <span data-ttu-id="cd667-2418">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="cd667-2418">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-2419">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-2419">Monitor</span></span>

* <span data-ttu-id="cd667-2420">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="cd667-2420">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="cd667-2421">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="cd667-2421">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="cd667-2422">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-2422">Network</span></span>

* <span data-ttu-id="cd667-2423">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="cd667-2423">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-2424">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-2424">Resource</span></span>

* <span data-ttu-id="cd667-2425">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="cd667-2425">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-2426">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-2426">Storage</span></span>

* <span data-ttu-id="cd667-2427">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="cd667-2427">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2428">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2428">VM</span></span>

* <span data-ttu-id="cd667-2429">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="cd667-2429">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="cd667-2430">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2430">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="cd667-2431">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2431">Auguest 14, 2018</span></span>

<span data-ttu-id="cd667-2432">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="cd667-2432">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="cd667-2433">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-2433">Core</span></span>

* <span data-ttu-id="cd667-2434">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2434">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="cd667-2435">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="cd667-2435">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="cd667-2436">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="cd667-2436">Telemetry</span></span>

* <span data-ttu-id="cd667-2437">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="cd667-2437">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-2438">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-2438">ACR</span></span>

* <span data-ttu-id="cd667-2439">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2439">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="cd667-2440">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2440">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-2441">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-2441">ACS</span></span>

* <span data-ttu-id="cd667-2442">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="cd667-2442">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="cd667-2443">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="cd667-2443">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="cd667-2444">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="cd667-2444">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="cd667-2445">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="cd667-2445">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="cd667-2446">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="cd667-2446">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="cd667-2447">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-2447">AppService</span></span>

* <span data-ttu-id="cd667-2448">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2448">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="cd667-2449">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="cd667-2449">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="cd667-2450">Batch AI</span><span class="sxs-lookup"><span data-stu-id="cd667-2450">BatchAI</span></span>

* <span data-ttu-id="cd667-2451">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="cd667-2451">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="cd667-2452">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-2452">Container</span></span>

* <span data-ttu-id="cd667-2453">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="cd667-2453">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="cd667-2454">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-2454">IoT</span></span>

* <span data-ttu-id="cd667-2455">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="cd667-2455">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="cd667-2456">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2456">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="cd667-2457">IoT Central</span><span class="sxs-lookup"><span data-stu-id="cd667-2457">Iot Central</span></span>

* <span data-ttu-id="cd667-2458">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="cd667-2458">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="cd667-2459">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="cd667-2459">KeyVault</span></span>


* <span data-ttu-id="cd667-2460">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="cd667-2460">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="cd667-2461">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="cd667-2461">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="cd667-2462">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="cd667-2462">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="cd667-2463">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="cd667-2463">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="cd667-2464">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="cd667-2464">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="cd667-2465">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="cd667-2465">Relay</span></span>

* <span data-ttu-id="cd667-2466">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="cd667-2466">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-2467">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-2467">Sql</span></span>

* <span data-ttu-id="cd667-2468">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2468">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-2469">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-2469">Storage</span></span>

* <span data-ttu-id="cd667-2470">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="cd667-2470">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="cd667-2471">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="cd667-2471">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="cd667-2472">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="cd667-2472">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="cd667-2473">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="cd667-2473">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="cd667-2474">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="cd667-2474">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2475">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2475">VM</span></span>

* <span data-ttu-id="cd667-2476">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="cd667-2476">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="cd667-2477">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2477">July 31, 2018</span></span>

<span data-ttu-id="cd667-2478">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="cd667-2478">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-2479">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-2479">ACR</span></span>

* <span data-ttu-id="cd667-2480">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2480">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="cd667-2481">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2481">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-2482">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-2482">ACS</span></span>

* <span data-ttu-id="cd667-2483">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="cd667-2483">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="cd667-2484">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-2484">Batch</span></span>

* <span data-ttu-id="cd667-2485">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="cd667-2485">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="cd667-2486">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-2486">Container</span></span>

* <span data-ttu-id="cd667-2487">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="cd667-2487">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="cd667-2488">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-2488">Network</span></span>

* <span data-ttu-id="cd667-2489">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="cd667-2489">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="cd667-2490">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-2490">Resource</span></span>

* <span data-ttu-id="cd667-2491">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="cd667-2491">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="cd667-2492">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="cd667-2492">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="cd667-2493">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-2493">Role</span></span>

* <span data-ttu-id="cd667-2494">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="cd667-2494">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="cd667-2495">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="cd667-2495">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="cd667-2496">Поиск</span><span class="sxs-lookup"><span data-stu-id="cd667-2496">Search</span></span>

* <span data-ttu-id="cd667-2497">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="cd667-2497">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="cd667-2498">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="cd667-2498">Service Bus</span></span>

* <span data-ttu-id="cd667-2499">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="cd667-2499">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="cd667-2500">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="cd667-2500">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="cd667-2501">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="cd667-2501">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="cd667-2502">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2502">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-2503">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-2503">Storage</span></span>

* <span data-ttu-id="cd667-2504">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="cd667-2504">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="cd667-2505">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="cd667-2505">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2506">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2506">VM</span></span>

* <span data-ttu-id="cd667-2507">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="cd667-2507">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="cd667-2508">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2508">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="cd667-2509">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="cd667-2509">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="cd667-2510">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="cd667-2510">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="cd667-2511">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2511">July 18, 2018</span></span>

<span data-ttu-id="cd667-2512">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="cd667-2512">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="cd667-2513">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-2513">Core</span></span>

* <span data-ttu-id="cd667-2514">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="cd667-2514">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="cd667-2515">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="cd667-2515">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="cd667-2516">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="cd667-2516">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-2517">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-2517">ACR</span></span>

* <span data-ttu-id="cd667-2518">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="cd667-2518">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="cd667-2519">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2519">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="cd667-2520">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="cd667-2520">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="cd667-2521">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="cd667-2521">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-2522">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-2522">ACS</span></span>

* <span data-ttu-id="cd667-2523">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="cd667-2523">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-2524">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-2524">AppService</span></span>

* <span data-ttu-id="cd667-2525">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="cd667-2525">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="cd667-2526">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-2526">Batch</span></span>

* <span data-ttu-id="cd667-2527">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="cd667-2527">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="cd667-2528">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="cd667-2528">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="cd667-2529">Batch AI</span><span class="sxs-lookup"><span data-stu-id="cd667-2529">Batch AI</span></span>

* <span data-ttu-id="cd667-2530">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2530">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="cd667-2531">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-2531">Container</span></span>

* <span data-ttu-id="cd667-2532">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="cd667-2532">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="cd667-2533">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="cd667-2533">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="cd667-2534">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-2534">Network</span></span>

* <span data-ttu-id="cd667-2535">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2535">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="cd667-2536">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2536">Added `network nic wait`</span></span>
* <span data-ttu-id="cd667-2537">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="cd667-2537">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="cd667-2538">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="cd667-2538">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="cd667-2539">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-2539">Resource</span></span>

* <span data-ttu-id="cd667-2540">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2540">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="cd667-2541">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2541">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="cd667-2542">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2542">Added `deployment wait` command</span></span>
* <span data-ttu-id="cd667-2543">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="cd667-2543">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-2544">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-2544">SQL</span></span>

* <span data-ttu-id="cd667-2545">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2545">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="cd667-2546">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2546">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="cd667-2547">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2547">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-2548">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-2548">Storage</span></span>

* <span data-ttu-id="cd667-2549">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2549">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2550">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2550">VM</span></span>

* <span data-ttu-id="cd667-2551">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-2551">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="cd667-2552">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2552">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="cd667-2553">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2553">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="cd667-2554">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2554">July 3, 2018</span></span>

<span data-ttu-id="cd667-2555">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="cd667-2555">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="cd667-2556">AKS</span><span class="sxs-lookup"><span data-stu-id="cd667-2556">AKS</span></span>

* <span data-ttu-id="cd667-2557">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="cd667-2557">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="cd667-2558">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2558">July 3, 2018</span></span>

<span data-ttu-id="cd667-2559">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="cd667-2559">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="cd667-2560">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-2560">Core</span></span>

* <span data-ttu-id="cd667-2561">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="cd667-2561">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-2562">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-2562">ACR</span></span>

* <span data-ttu-id="cd667-2563">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="cd667-2563">Added polling build status</span></span>
* <span data-ttu-id="cd667-2564">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="cd667-2564">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="cd667-2565">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2565">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-2566">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-2566">ACS</span></span>

* <span data-ttu-id="cd667-2567">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-2567">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="cd667-2568">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-2568">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="cd667-2569">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2569">Updated options for `aks browse` command.</span></span> <span data-ttu-id="cd667-2570">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2570">Added `--listen-port` support</span></span>
* <span data-ttu-id="cd667-2571">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2571">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="cd667-2572">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="cd667-2572">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="cd667-2573">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2573">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-2574">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-2574">AppService</span></span>

* <span data-ttu-id="cd667-2575">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2575">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="cd667-2576">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="cd667-2576">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="cd667-2577">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="cd667-2577">Backup</span></span>

* <span data-ttu-id="cd667-2578">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="cd667-2578">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="cd667-2579">Batch AI</span><span class="sxs-lookup"><span data-stu-id="cd667-2579">BatchAI</span></span>

* <span data-ttu-id="cd667-2580">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2580">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="cd667-2581">Cloud</span><span class="sxs-lookup"><span data-stu-id="cd667-2581">Cloud</span></span>

* <span data-ttu-id="cd667-2582">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2582">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="cd667-2583">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-2583">Container</span></span>

* <span data-ttu-id="cd667-2584">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="cd667-2584">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="cd667-2585">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2585">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="cd667-2586">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="cd667-2586">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="cd667-2587">Расширение</span><span class="sxs-lookup"><span data-stu-id="cd667-2587">Extension</span></span>

* <span data-ttu-id="cd667-2588">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="cd667-2588">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="cd667-2589">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-2589">Network</span></span>

* <span data-ttu-id="cd667-2590">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="cd667-2590">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="cd667-2591">Rdbms</span><span class="sxs-lookup"><span data-stu-id="cd667-2591">Rdbms</span></span>

* <span data-ttu-id="cd667-2592">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2592">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-2593">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-2593">Resource</span></span>

* <span data-ttu-id="cd667-2594">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2594">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2595">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2595">VM</span></span>

* <span data-ttu-id="cd667-2596">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="cd667-2596">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="cd667-2597">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2597">June 25, 2018</span></span>

<span data-ttu-id="cd667-2598">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="cd667-2598">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="cd667-2599">CLI</span><span class="sxs-lookup"><span data-stu-id="cd667-2599">CLI</span></span>

* <span data-ttu-id="cd667-2600">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="cd667-2600">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="cd667-2601">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2601">June 19, 2018</span></span>

<span data-ttu-id="cd667-2602">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="cd667-2602">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="cd667-2603">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-2603">Core</span></span>

* <span data-ttu-id="cd667-2604">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="cd667-2604">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-2605">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-2605">ACR</span></span>

* <span data-ttu-id="cd667-2606">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2606">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="cd667-2607">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="cd667-2607">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-2608">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-2608">ACS</span></span>

* <span data-ttu-id="cd667-2609">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2609">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="cd667-2610">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2610">Added `--update` support</span></span>
* <span data-ttu-id="cd667-2611">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2611">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="cd667-2612">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2612">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="cd667-2613">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2613">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="cd667-2614">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2614">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="cd667-2615">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2615">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="cd667-2616">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2616">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-2617">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-2617">AppService</span></span>

* <span data-ttu-id="cd667-2618">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="cd667-2618">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="cd667-2619">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2619">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="cd667-2620">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-2620">Batch</span></span>

* <span data-ttu-id="cd667-2621">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2621">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="cd667-2622">Batch AI</span><span class="sxs-lookup"><span data-stu-id="cd667-2622">Batch AI</span></span>

* <span data-ttu-id="cd667-2623">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="cd667-2623">Added support for workspaces.</span></span> <span data-ttu-id="cd667-2624">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2624">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="cd667-2625">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2625">Added support for experiments.</span></span> <span data-ttu-id="cd667-2626">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="cd667-2626">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="cd667-2627">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="cd667-2627">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="cd667-2628">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2628">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="cd667-2629">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2629">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="cd667-2630">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2630">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="cd667-2631">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="cd667-2631">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="cd667-2632">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2632">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="cd667-2633">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2633">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="cd667-2634">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2634">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="cd667-2635">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2635">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="cd667-2636">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2636">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="cd667-2637">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2637">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="cd667-2638">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="cd667-2638">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="cd667-2639">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2639">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="cd667-2640">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="cd667-2640">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="cd667-2641">[`--config`, `-c`] переименовано в [`--config-file`, `-f`].</span><span class="sxs-lookup"><span data-stu-id="cd667-2641">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="cd667-2642">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="cd667-2642">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="cd667-2643">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="cd667-2643">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="cd667-2644">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="cd667-2644">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="cd667-2645">Maps</span><span class="sxs-lookup"><span data-stu-id="cd667-2645">Maps</span></span>

* <span data-ttu-id="cd667-2646">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2646">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="cd667-2647">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-2647">Network</span></span>

* <span data-ttu-id="cd667-2648">Добавлена поддержка `https` в `network lb probe create` ([№ 6571](https://github.com/Azure/azure-cli/issues/6571)).</span><span class="sxs-lookup"><span data-stu-id="cd667-2648">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="cd667-2649">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="cd667-2649">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="cd667-2650">#6502</span><span class="sxs-lookup"><span data-stu-id="cd667-2650">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="cd667-2651">Резервирование</span><span class="sxs-lookup"><span data-stu-id="cd667-2651">Reservations</span></span>

* <span data-ttu-id="cd667-2652">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2652">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="cd667-2653">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2653">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="cd667-2654">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2654">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="cd667-2655">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2655">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="cd667-2656">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2656">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="cd667-2657">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2657">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="cd667-2658">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-2658">Role</span></span>

* <span data-ttu-id="cd667-2659">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="cd667-2659">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-2660">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-2660">SQL</span></span>

* <span data-ttu-id="cd667-2661">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="cd667-2661">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-2662">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-2662">Storage</span></span>

* <span data-ttu-id="cd667-2663">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="cd667-2663">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2664">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2664">VM</span></span>

* <span data-ttu-id="cd667-2665">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2665">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="cd667-2666">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2666">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="cd667-2667">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="cd667-2667">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="cd667-2668">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2668">June 13, 2018</span></span>

<span data-ttu-id="cd667-2669">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="cd667-2669">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="cd667-2670">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-2670">Core</span></span>

* <span data-ttu-id="cd667-2671">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="cd667-2671">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="cd667-2672">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2672">June 13, 2018</span></span>

<span data-ttu-id="cd667-2673">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="cd667-2673">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="cd667-2674">AKS</span><span class="sxs-lookup"><span data-stu-id="cd667-2674">AKS</span></span>

* <span data-ttu-id="cd667-2675">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="cd667-2675">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="cd667-2676">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="cd667-2676">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="cd667-2677">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="cd667-2677">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="cd667-2678">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="cd667-2678">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="cd667-2679">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cd667-2679">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-2680">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-2680">AppService</span></span>

* <span data-ttu-id="cd667-2681">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="cd667-2681">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="cd667-2682">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2682">June 5, 2018</span></span>

<span data-ttu-id="cd667-2683">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="cd667-2683">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="cd667-2684">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="cd667-2684">Interactive</span></span>

* <span data-ttu-id="cd667-2685">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="cd667-2685">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="cd667-2686">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2686">June 5, 2018</span></span>

<span data-ttu-id="cd667-2687">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="cd667-2687">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="cd667-2688">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-2688">Core</span></span>

* <span data-ttu-id="cd667-2689">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="cd667-2689">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="cd667-2690">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="cd667-2690">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-2691">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-2691">ACR</span></span>

* <span data-ttu-id="cd667-2692">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="cd667-2692">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="cd667-2693">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2693">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="cd667-2694">AKS</span><span class="sxs-lookup"><span data-stu-id="cd667-2694">AKS</span></span>

* <span data-ttu-id="cd667-2695">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="cd667-2695">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="cd667-2696">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-2696">Batch</span></span>

* <span data-ttu-id="cd667-2697">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="cd667-2697">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-2698">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-2698">IOT</span></span>

* <span data-ttu-id="cd667-2699">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="cd667-2699">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="cd667-2700">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-2700">Network</span></span>

* <span data-ttu-id="cd667-2701">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2701">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="cd667-2702">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="cd667-2702">Policy Insights</span></span>

* <span data-ttu-id="cd667-2703">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="cd667-2703">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="cd667-2704">ARM</span><span class="sxs-lookup"><span data-stu-id="cd667-2704">ARM</span></span>

* <span data-ttu-id="cd667-2705">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2705">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-2706">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-2706">SQL</span></span>

* <span data-ttu-id="cd667-2707">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="cd667-2707">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="cd667-2708">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="cd667-2708">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="cd667-2709">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-2709">Storage</span></span>

* <span data-ttu-id="cd667-2710">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2710">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2711">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2711">VM</span></span>

* <span data-ttu-id="cd667-2712">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2712">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="cd667-2713">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2713">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="cd667-2714">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2714">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="cd667-2715">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2715">May 22, 2018</span></span>

<span data-ttu-id="cd667-2716">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="cd667-2716">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="cd667-2717">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-2717">Core</span></span>

* <span data-ttu-id="cd667-2718">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2718">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-2719">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-2719">ACS</span></span>

* <span data-ttu-id="cd667-2720">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2720">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="cd667-2721">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="cd667-2721">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-2722">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-2722">AppService</span></span>

* <span data-ttu-id="cd667-2723">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="cd667-2723">Improved generic update commands</span></span>
* <span data-ttu-id="cd667-2724">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2724">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="cd667-2725">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-2725">Container</span></span>

* <span data-ttu-id="cd667-2726">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="cd667-2726">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="cd667-2727">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="cd667-2727">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="cd667-2728">Расширение</span><span class="sxs-lookup"><span data-stu-id="cd667-2728">Extension</span></span>

* <span data-ttu-id="cd667-2729">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="cd667-2729">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="cd667-2730">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="cd667-2730">Interactive</span></span>

* <span data-ttu-id="cd667-2731">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="cd667-2731">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="cd667-2732">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="cd667-2732">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="cd667-2733">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="cd667-2733">KeyVault</span></span>

* <span data-ttu-id="cd667-2734">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="cd667-2734">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="cd667-2735">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-2735">Network</span></span>

* <span data-ttu-id="cd667-2736">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="cd667-2736">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="cd667-2737">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="cd667-2737">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-2738">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-2738">SQL</span></span>

* <span data-ttu-id="cd667-2739">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="cd667-2739">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="cd667-2740">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2740">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="cd667-2741">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2741">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="cd667-2742">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="cd667-2742">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="cd667-2743">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="cd667-2743">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="cd667-2744">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2744">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="cd667-2745">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2745">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="cd667-2746">`edition`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2746">`edition`.</span></span> <span data-ttu-id="cd667-2747">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2747">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="cd667-2748">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2748">`elasticPoolName`.</span></span> <span data-ttu-id="cd667-2749">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2749">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="cd667-2750">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="cd667-2750">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="cd667-2751">`edition`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2751">`edition`.</span></span> <span data-ttu-id="cd667-2752">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2752">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="cd667-2753">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2753">`dtu`.</span></span> <span data-ttu-id="cd667-2754">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2754">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="cd667-2755">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2755">`databaseDtuMin`.</span></span> <span data-ttu-id="cd667-2756">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2756">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="cd667-2757">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2757">`databaseDtuMax`.</span></span> <span data-ttu-id="cd667-2758">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2758">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="cd667-2759">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2759">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="cd667-2760">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2760">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-2761">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-2761">Storage</span></span>

* <span data-ttu-id="cd667-2762">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2762">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="cd667-2763">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2763">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2764">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2764">VM</span></span>

* <span data-ttu-id="cd667-2765">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2765">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="cd667-2766">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2766">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="cd667-2767">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2767">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="cd667-2768">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="cd667-2768">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="cd667-2769">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2769">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="cd667-2770">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2770">May 7, 2018</span></span>

<span data-ttu-id="cd667-2771">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="cd667-2771">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="cd667-2772">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-2772">Core</span></span>

* <span data-ttu-id="cd667-2773">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="cd667-2773">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="cd667-2774">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2774">Added limited support for positional arguments</span></span>
* <span data-ttu-id="cd667-2775">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2775">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="cd667-2776">#5591</span><span class="sxs-lookup"><span data-stu-id="cd667-2776">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="cd667-2777">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2777">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="cd667-2778">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="cd667-2778">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="cd667-2779">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="cd667-2779">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="cd667-2780">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2780">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="cd667-2781">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="cd667-2781">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-2782">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-2782">ACR</span></span>

* <span data-ttu-id="cd667-2783">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="cd667-2783">Added ACR Build commands</span></span>
* <span data-ttu-id="cd667-2784">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="cd667-2784">Improved resource not found error messages</span></span>
* <span data-ttu-id="cd667-2785">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="cd667-2785">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="cd667-2786">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="cd667-2786">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="cd667-2787">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="cd667-2787">Improved repository commands error messages</span></span>
* <span data-ttu-id="cd667-2788">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="cd667-2788">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-2789">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-2789">ACS</span></span>

* <span data-ttu-id="cd667-2790">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="cd667-2790">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="cd667-2791">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="cd667-2791">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="cd667-2792">AMS</span><span class="sxs-lookup"><span data-stu-id="cd667-2792">AMS</span></span>

* <span data-ttu-id="cd667-2793">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="cd667-2793">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-2794">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-2794">Appservice</span></span>

* <span data-ttu-id="cd667-2795">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="cd667-2795">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="cd667-2796">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2796">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="cd667-2797">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="cd667-2797">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="cd667-2798">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="cd667-2798">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="cd667-2799">Batch AI</span><span class="sxs-lookup"><span data-stu-id="cd667-2799">Batch AI</span></span>

* <span data-ttu-id="cd667-2800">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="cd667-2800">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="cd667-2801">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="cd667-2801">Cognitive Services</span></span>

* <span data-ttu-id="cd667-2802">Исправлена опечатка в примере для `cognitiveservices account create` ([№ 5603](https://github.com/Azure/azure-cli/issues/5603)).</span><span class="sxs-lookup"><span data-stu-id="cd667-2802">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="cd667-2803">Потребление</span><span class="sxs-lookup"><span data-stu-id="cd667-2803">Consumption</span></span>

* <span data-ttu-id="cd667-2804">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="cd667-2804">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="cd667-2805">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-2805">Container</span></span>

* <span data-ttu-id="cd667-2806">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="cd667-2806">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="cd667-2807">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-2807">Cosmos DB</span></span>

* <span data-ttu-id="cd667-2808">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-2808">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="cd667-2809">DMS</span><span class="sxs-lookup"><span data-stu-id="cd667-2809">DMS</span></span>

* <span data-ttu-id="cd667-2810">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="cd667-2810">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="cd667-2811">Расширение</span><span class="sxs-lookup"><span data-stu-id="cd667-2811">Extension</span></span>

* <span data-ttu-id="cd667-2812">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="cd667-2812">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="cd667-2813">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="cd667-2813">Interactive</span></span>

* <span data-ttu-id="cd667-2814">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="cd667-2814">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="cd667-2815">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="cd667-2815">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="cd667-2816">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="cd667-2816">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="cd667-2817">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="cd667-2817">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="cd667-2818">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="cd667-2818">Lab</span></span>

* <span data-ttu-id="cd667-2819">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="cd667-2819">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="cd667-2820">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-2820">Network</span></span>

* <span data-ttu-id="cd667-2821">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="cd667-2821">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="cd667-2822">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-2822">Profile</span></span>

* <span data-ttu-id="cd667-2823">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2823">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="cd667-2824">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="cd667-2824">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="cd667-2825">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2825">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="cd667-2826">Redis</span><span class="sxs-lookup"><span data-stu-id="cd667-2826">Redis</span></span>

* <span data-ttu-id="cd667-2827">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2827">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="cd667-2828">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="cd667-2828">Deprecated `redis list-all`.</span></span> <span data-ttu-id="cd667-2829">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2829">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="cd667-2830">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2830">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="cd667-2831">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="cd667-2831">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="cd667-2832">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-2832">Role</span></span>

* <span data-ttu-id="cd667-2833">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="cd667-2833">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-2834">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-2834">Storage</span></span>

* <span data-ttu-id="cd667-2835">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="cd667-2835">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="cd667-2836">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="cd667-2836">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="cd667-2837">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="cd667-2837">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="cd667-2838">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="cd667-2838">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="cd667-2839">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="cd667-2839">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2840">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2840">VM</span></span>

* <span data-ttu-id="cd667-2841">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="cd667-2841">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="cd667-2842">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="cd667-2842">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="cd667-2843">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="cd667-2843">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="cd667-2844">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2844">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="cd667-2845">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="cd667-2845">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="cd667-2846">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="cd667-2846">Added write accelerator support</span></span>
* <span data-ttu-id="cd667-2847">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2847">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="cd667-2848">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="cd667-2848">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="cd667-2849">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="cd667-2849">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="cd667-2850">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2850">April 10, 2018</span></span>

<span data-ttu-id="cd667-2851">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="cd667-2851">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-2852">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-2852">ACR</span></span>

* <span data-ttu-id="cd667-2853">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="cd667-2853">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-2854">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-2854">ACS</span></span>

* <span data-ttu-id="cd667-2855">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="cd667-2855">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-2856">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-2856">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="cd667-2858">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="cd667-2858">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="cd667-2859">Batch AI</span><span class="sxs-lookup"><span data-stu-id="cd667-2859">BatchAI</span></span>

* <span data-ttu-id="cd667-2860">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="cd667-2860">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="cd667-2861">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="cd667-2861">Job level mounting</span></span>
  - <span data-ttu-id="cd667-2862">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2862">Environment variables with secret values</span></span>
  - <span data-ttu-id="cd667-2863">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="cd667-2863">Performance counters settings</span></span>
  - <span data-ttu-id="cd667-2864">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="cd667-2864">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="cd667-2865">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2865">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="cd667-2866">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="cd667-2866">Usage and limits reporting</span></span>
  - <span data-ttu-id="cd667-2867">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2867">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="cd667-2868">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2868">Support for custom images</span></span>
  - <span data-ttu-id="cd667-2869">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="cd667-2869">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="cd667-2870">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="cd667-2870">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="cd667-2871">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="cd667-2871">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="cd667-2872">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="cd667-2872">National clouds are supported</span></span>
* <span data-ttu-id="cd667-2873">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="cd667-2873">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="cd667-2874">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="cd667-2874">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="cd667-2875">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="cd667-2875">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="cd667-2876">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="cd667-2876">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="cd667-2877">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="cd667-2877">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="cd667-2878">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="cd667-2878">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="cd667-2879">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2879">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="cd667-2880">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="cd667-2880">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="cd667-2881">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="cd667-2881">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="cd667-2882">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2882">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="cd667-2883">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="cd667-2883">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="cd667-2884">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2884">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="cd667-2885">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2885">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="cd667-2886">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="cd667-2886">Billing</span></span>

* <span data-ttu-id="cd667-2887">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="cd667-2887">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="cd667-2888">Потребление</span><span class="sxs-lookup"><span data-stu-id="cd667-2888">Consumption</span></span>

* <span data-ttu-id="cd667-2889">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2889">Added `marketplace` commands</span></span>
* <span data-ttu-id="cd667-2890">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2890">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="cd667-2891">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2891">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="cd667-2892">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2892">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="cd667-2893">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2893">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="cd667-2894">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2894">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="cd667-2895">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-2895">Container</span></span>

* <span data-ttu-id="cd667-2896">Добавлены параметры подключения тома репозитория Git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2896">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="cd667-2897">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="cd667-2897">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="cd667-2898">Расширение</span><span class="sxs-lookup"><span data-stu-id="cd667-2898">Extension</span></span>

* <span data-ttu-id="cd667-2899">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="cd667-2899">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="cd667-2900">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="cd667-2900">Interactive</span></span>

* <span data-ttu-id="cd667-2901">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="cd667-2901">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="cd667-2902">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="cd667-2902">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="cd667-2903">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2903">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="cd667-2904">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-2904">Network</span></span>

* <span data-ttu-id="cd667-2905">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2905">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="cd667-2906">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2906">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="cd667-2907">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="cd667-2907">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="cd667-2908">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="cd667-2908">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="cd667-2909">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="cd667-2909">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="cd667-2910">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2910">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="cd667-2911">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2911">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="cd667-2912">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="cd667-2912">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-2913">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-2913">Profile</span></span>

* <span data-ttu-id="cd667-2914">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2914">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="cd667-2915">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi` & `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2915">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="cd667-2916">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="cd667-2916">RDBMS</span></span>

* <span data-ttu-id="cd667-2917">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2917">Added `georestore` command</span></span>
* <span data-ttu-id="cd667-2918">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="cd667-2918">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-2919">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-2919">Resource</span></span>

* <span data-ttu-id="cd667-2920">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2920">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="cd667-2921">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2921">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-2922">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-2922">SQL</span></span>

* <span data-ttu-id="cd667-2923">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2923">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-2924">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-2924">Storage</span></span>

* <span data-ttu-id="cd667-2925">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="cd667-2925">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2926">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2926">VM</span></span>

* <span data-ttu-id="cd667-2927">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="cd667-2927">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="cd667-2928">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="cd667-2928">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="cd667-2930">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2930">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="cd667-2931">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="cd667-2931">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="cd667-2932">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="cd667-2932">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="cd667-2933">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="cd667-2933">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="cd667-2934">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2934">March 27, 2018</span></span>

<span data-ttu-id="cd667-2935">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="cd667-2935">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="cd667-2936">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-2936">Core</span></span>

* <span data-ttu-id="cd667-2937">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="cd667-2937">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-2938">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-2938">ACS</span></span>

* <span data-ttu-id="cd667-2939">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="cd667-2939">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-2940">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-2940">Appservice</span></span>

* <span data-ttu-id="cd667-2941">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2941">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="cd667-2942">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2942">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="cd667-2943">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="cd667-2943">Backup</span></span>

* <span data-ttu-id="cd667-2944">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2944">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="cd667-2945">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="cd667-2945">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="cd667-2946">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="cd667-2946">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="cd667-2947">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2947">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="cd667-2948">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-2948">Container</span></span>

* <span data-ttu-id="cd667-2949">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2949">Added `container exec` command.</span></span> <span data-ttu-id="cd667-2950">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="cd667-2950">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="cd667-2951">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="cd667-2951">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="cd667-2952">Расширение</span><span class="sxs-lookup"><span data-stu-id="cd667-2952">Extension</span></span>

* <span data-ttu-id="cd667-2953">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="cd667-2953">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="cd667-2954">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2954">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="cd667-2955">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-2955">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="cd667-2956">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="cd667-2956">Interactive</span></span>

* <span data-ttu-id="cd667-2957">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="cd667-2957">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="cd667-2958">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2958">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="cd667-2959">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="cd667-2959">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="cd667-2960">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="cd667-2960">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="cd667-2961">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="cd667-2961">Lab</span></span>

* <span data-ttu-id="cd667-2962">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2962">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-2963">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-2963">Monitor</span></span>

* <span data-ttu-id="cd667-2964">Добавлена поддержка аргументов `--top`, `--orderby` и `--namespace` для `metrics list` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="cd667-2964">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="cd667-2965">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="cd667-2965">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="cd667-2966">Добавлена поддержка `--namespace` для `metrics list-definitions` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="cd667-2966">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="cd667-2967">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-2967">Network</span></span>

* <span data-ttu-id="cd667-2968">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="cd667-2968">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-2969">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-2969">Profile</span></span>

* <span data-ttu-id="cd667-2970">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2970">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="cd667-2971">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="cd667-2971">RDBMS</span></span>

* <span data-ttu-id="cd667-2972">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="cd667-2972">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-2973">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-2973">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="cd667-2975">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-2975">Role</span></span>

* <span data-ttu-id="cd667-2976">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2976">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="cd667-2977">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="cd667-2977">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="cd667-2978">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="cd667-2978">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="cd667-2979">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2979">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="cd667-2980">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2980">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-2981">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-2981">Storage</span></span>

* <span data-ttu-id="cd667-2982">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="cd667-2982">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="cd667-2983">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="cd667-2983">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-2984">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-2984">VM</span></span>

* <span data-ttu-id="cd667-2985">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="cd667-2985">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="cd667-2986">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2986">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="cd667-2987">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="cd667-2987">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="cd667-2988">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="cd667-2988">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="cd667-2989">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-2989">March 13, 2018</span></span>

<span data-ttu-id="cd667-2990">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="cd667-2990">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-2991">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-2991">ACR</span></span>

* <span data-ttu-id="cd667-2992">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2992">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="cd667-2993">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="cd667-2993">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="cd667-2994">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="cd667-2994">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-2995">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-2995">ACS</span></span>

* <span data-ttu-id="cd667-2996">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="cd667-2996">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="cd667-2997">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="cd667-2997">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="cd667-2998">Помощник</span><span class="sxs-lookup"><span data-stu-id="cd667-2998">Advisor</span></span>

* <span data-ttu-id="cd667-2999">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="cd667-2999">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="cd667-3000">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3000">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="cd667-3001">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3001">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="cd667-3002">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3002">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="cd667-3003">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3003">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-3004">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-3004">Appservice</span></span>

* <span data-ttu-id="cd667-3005">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="cd667-3005">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="cd667-3006">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3006">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="cd667-3007">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="cd667-3007">Eventhubs</span></span>

* <span data-ttu-id="cd667-3008">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="cd667-3008">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="cd667-3009">Расширение</span><span class="sxs-lookup"><span data-stu-id="cd667-3009">Extension</span></span>

* <span data-ttu-id="cd667-3010">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="cd667-3010">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="cd667-3011">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="cd667-3011">Interactive</span></span>

* <span data-ttu-id="cd667-3012">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="cd667-3012">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="cd667-3013">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="cd667-3013">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="cd667-3014">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="cd667-3014">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="cd667-3015">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="cd667-3015">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-3016">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-3016">Monitor</span></span>

* <span data-ttu-id="cd667-3017">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="cd667-3017">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="cd667-3018">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3018">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="cd667-3019">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3019">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="cd667-3020">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3020">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="cd667-3021">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-3021">Network</span></span>

* <span data-ttu-id="cd667-3022">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3022">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="cd667-3023">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="cd667-3023">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="cd667-3024">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3024">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="cd667-3025">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3025">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-3026">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-3026">Profile</span></span>

* <span data-ttu-id="cd667-3027">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="cd667-3027">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="cd667-3028">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3028">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="cd667-3029">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="cd667-3029">RDBMS</span></span>

* <span data-ttu-id="cd667-3030">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="cd667-3030">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="cd667-3031">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="cd667-3031">Service Bus</span></span>

* <span data-ttu-id="cd667-3032">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="cd667-3032">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-3033">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-3033">Storage</span></span>

* <span data-ttu-id="cd667-3034">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="cd667-3034">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="cd667-3035">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="cd667-3035">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-3036">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-3036">VM</span></span>

* <span data-ttu-id="cd667-3037">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="cd667-3037">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="cd667-3038">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="cd667-3038">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="cd667-3039">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3039">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="cd667-3040">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="cd667-3040">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="cd667-3041">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="cd667-3041">February 27, 2018</span></span>

<span data-ttu-id="cd667-3042">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="cd667-3042">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="cd667-3043">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-3043">Core</span></span>

* <span data-ttu-id="cd667-3044">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="cd667-3044">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="cd667-3045">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="cd667-3045">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="cd667-3046">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3046">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-3047">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-3047">ACS</span></span>

* <span data-ttu-id="cd667-3048">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-3048">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="cd667-3049">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="cd667-3049">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="cd667-3050">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3050">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="cd667-3051">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3051">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-3052">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-3052">Appservice</span></span>

* <span data-ttu-id="cd667-3053">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="cd667-3053">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="cd667-3054">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="cd667-3054">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="cd667-3055">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="cd667-3055">Cognitive Services</span></span>

* <span data-ttu-id="cd667-3056">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="cd667-3056">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="cd667-3057">Потребление</span><span class="sxs-lookup"><span data-stu-id="cd667-3057">Consumption</span></span>

* <span data-ttu-id="cd667-3058">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="cd667-3058">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="cd667-3059">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="cd667-3059">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="cd667-3060">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-3060">Container</span></span>

* <span data-ttu-id="cd667-3061">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="cd667-3061">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="cd667-3062">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-3062">Network</span></span>

* <span data-ttu-id="cd667-3063">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3063">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-3064">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-3064">Resource</span></span>

* <span data-ttu-id="cd667-3065">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="cd667-3065">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="cd667-3066">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-3066">Role</span></span>

* <span data-ttu-id="cd667-3067">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="cd667-3067">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-3068">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-3068">SQL</span></span>

* <span data-ttu-id="cd667-3069">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="cd667-3069">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-3070">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-3070">Storage</span></span>

* <span data-ttu-id="cd667-3071">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3071">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-3072">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-3072">VM</span></span>

* <span data-ttu-id="cd667-3073">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="cd667-3073">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="cd667-3074">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-3074">February 13, 2018</span></span>

<span data-ttu-id="cd667-3075">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="cd667-3075">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="cd667-3076">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-3076">Core</span></span>

* <span data-ttu-id="cd667-3077">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="cd667-3077">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-3078">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-3078">ACS</span></span>

* <span data-ttu-id="cd667-3079">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="cd667-3079">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="cd667-3080">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3080">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="cd667-3081">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="cd667-3081">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="cd667-3082">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="cd667-3082">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="cd667-3083">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="cd667-3083">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="cd667-3084">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3084">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="cd667-3085">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="cd667-3085">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="cd667-3086">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3086">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-3087">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-3087">Appservice</span></span>

* <span data-ttu-id="cd667-3088">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="cd667-3088">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="cd667-3089">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3089">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="cd667-3090">CDN</span><span class="sxs-lookup"><span data-stu-id="cd667-3090">CDN</span></span>

* <span data-ttu-id="cd667-3091">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3091">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="cd667-3092">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-3092">Container</span></span>

* <span data-ttu-id="cd667-3093">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="cd667-3093">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="cd667-3094">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="cd667-3094">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="cd667-3095">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-3095">CosmosDB</span></span>

* <span data-ttu-id="cd667-3096">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="cd667-3096">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="cd667-3097">Расширение</span><span class="sxs-lookup"><span data-stu-id="cd667-3097">Extension</span></span>

* <span data-ttu-id="cd667-3098">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3098">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="cd667-3099">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3099">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="cd667-3100">Отзывы</span><span class="sxs-lookup"><span data-stu-id="cd667-3100">Feedback</span></span>

* <span data-ttu-id="cd667-3101">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="cd667-3101">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="cd667-3102">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="cd667-3102">Interactive</span></span>

* <span data-ttu-id="cd667-3103">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="cd667-3103">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="cd667-3104">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="cd667-3104">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-3105">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-3105">IoT</span></span>

* <span data-ttu-id="cd667-3106">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="cd667-3106">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="cd667-3107">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="cd667-3107">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="cd667-3108">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3108">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="cd667-3109">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="cd667-3109">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-3110">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-3110">Monitor</span></span>

* <span data-ttu-id="cd667-3111">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3111">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="cd667-3112">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-3112">Network</span></span>

* <span data-ttu-id="cd667-3113">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="cd667-3113">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="cd667-3114">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-3114">Profile</span></span>

* <span data-ttu-id="cd667-3115">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="cd667-3115">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-3116">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-3116">Resource</span></span>

* <span data-ttu-id="cd667-3117">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3117">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="cd667-3118">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-3118">Role</span></span>

* <span data-ttu-id="cd667-3119">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="cd667-3119">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-3120">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-3120">SQL</span></span>

* <span data-ttu-id="cd667-3121">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3121">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="cd667-3122">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3122">Added `sql db rename`</span></span>
* <span data-ttu-id="cd667-3123">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="cd667-3123">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-3124">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-3124">Storage</span></span>

* <span data-ttu-id="cd667-3125">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="cd667-3125">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-3126">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-3126">VM</span></span>

* <span data-ttu-id="cd667-3127">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="cd667-3127">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="cd667-3128">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="cd667-3128">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="cd667-3129">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="cd667-3129">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="cd667-3130">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-3130">January 31, 2018</span></span>

<span data-ttu-id="cd667-3131">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="cd667-3131">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="cd667-3132">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-3132">Core</span></span>

* <span data-ttu-id="cd667-3133">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="cd667-3133">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="cd667-3134">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="cd667-3134">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="cd667-3135">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="cd667-3135">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="cd667-3136">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="cd667-3136">Use `--verbose` to see</span></span>
* <span data-ttu-id="cd667-3137">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="cd667-3137">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-3138">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-3138">ACS</span></span>

* <span data-ttu-id="cd667-3139">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3139">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="cd667-3140">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3140">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-3141">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-3141">Appservice</span></span>

* <span data-ttu-id="cd667-3142">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="cd667-3142">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="cd667-3143">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="cd667-3143">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="cd667-3144">CDN</span><span class="sxs-lookup"><span data-stu-id="cd667-3144">CDN</span></span>

* <span data-ttu-id="cd667-3145">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3145">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="cd667-3146">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-3146">CosmosDB</span></span>

* <span data-ttu-id="cd667-3147">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="cd667-3147">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="cd667-3148">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="cd667-3148">Interactive</span></span>

* <span data-ttu-id="cd667-3149">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="cd667-3149">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="cd667-3150">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-3150">Network</span></span>

* <span data-ttu-id="cd667-3151">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3151">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="cd667-3152">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-3152">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="cd667-3153">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3153">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="cd667-3154">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3154">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="cd667-3155">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3155">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="cd667-3156">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="cd667-3156">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="cd667-3157">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="cd667-3157">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="cd667-3158">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="cd667-3158">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="cd667-3159">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3159">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="cd667-3160">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3160">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-3161">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-3161">Profile</span></span>

* <span data-ttu-id="cd667-3162">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="cd667-3162">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-3163">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-3163">Resource</span></span>

* <span data-ttu-id="cd667-3164">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="cd667-3164">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-3165">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-3165">Storage</span></span>

* <span data-ttu-id="cd667-3166">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="cd667-3166">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="cd667-3167">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="cd667-3167">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="cd667-3168">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3168">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="cd667-3169">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3169">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="cd667-3170">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="cd667-3170">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-3171">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-3171">VM</span></span>

* <span data-ttu-id="cd667-3172">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="cd667-3172">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="cd667-3173">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="cd667-3173">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="cd667-3174">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="cd667-3174">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="cd667-3175">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3175">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="cd667-3176">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-3176">January 17, 2018</span></span>

<span data-ttu-id="cd667-3177">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="cd667-3177">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-3178">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-3178">ACR</span></span>

* <span data-ttu-id="cd667-3179">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="cd667-3179">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="cd667-3180">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="cd667-3180">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-3181">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-3181">ACS</span></span>

* <span data-ttu-id="cd667-3182">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3182">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="cd667-3183">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="cd667-3183">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-3184">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-3184">Appservice</span></span>

* <span data-ttu-id="cd667-3185">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="cd667-3185">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="cd667-3186">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="cd667-3186">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="cd667-3187">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3187">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="cd667-3188">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="cd667-3188">Backup</span></span>

* <span data-ttu-id="cd667-3189">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="cd667-3189">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="cd667-3190">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="cd667-3190">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="cd667-3191">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="cd667-3191">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="cd667-3192">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="cd667-3192">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="cd667-3193">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="cd667-3193">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="cd667-3194">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-3194">Batch</span></span>

* <span data-ttu-id="cd667-3195">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="cd667-3195">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="cd667-3196">Cloud</span><span class="sxs-lookup"><span data-stu-id="cd667-3196">Cloud</span></span>

* <span data-ttu-id="cd667-3197">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="cd667-3197">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="cd667-3198">Потребление</span><span class="sxs-lookup"><span data-stu-id="cd667-3198">Consumption</span></span>

* <span data-ttu-id="cd667-3199">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3199">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="cd667-3200">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-3200">Event Grid</span></span>

* <span data-ttu-id="cd667-3201">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3201">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="cd667-3202">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3202">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="cd667-3203">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3203">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="cd667-3204">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3204">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="cd667-3205">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3205">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="cd667-3206">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3206">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="cd667-3207">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3207">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="cd667-3208">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="cd667-3208">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="cd667-3209">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="cd667-3209">Interactive</span></span>

* <span data-ttu-id="cd667-3210">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="cd667-3210">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="cd667-3211">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="cd667-3211">Fixed errors on startup</span></span>
* <span data-ttu-id="cd667-3212">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="cd667-3212">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-3213">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-3213">IoT</span></span>

* <span data-ttu-id="cd667-3214">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="cd667-3214">Added support for device provisioning service</span></span>
* <span data-ttu-id="cd667-3215">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="cd667-3215">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="cd667-3216">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="cd667-3216">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-3217">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-3217">Monitor</span></span>

* <span data-ttu-id="cd667-3218">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="cd667-3218">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="cd667-3219">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3219">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="cd667-3220">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="cd667-3220">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="cd667-3221">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-3221">Network</span></span>

* <span data-ttu-id="cd667-3222">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="cd667-3222">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="cd667-3223">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="cd667-3223">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-3224">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-3224">Profile</span></span>

* <span data-ttu-id="cd667-3225">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="cd667-3225">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="cd667-3226">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-3226">Role</span></span>

* <span data-ttu-id="cd667-3227">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="cd667-3227">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="cd667-3228">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="cd667-3228">Service Fabric</span></span>

* <span data-ttu-id="cd667-3229">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="cd667-3229">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="cd667-3230">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="cd667-3230">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-3231">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-3231">VM</span></span>

* <span data-ttu-id="cd667-3232">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3232">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="cd667-3233">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="cd667-3233">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="cd667-3234">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3234">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="cd667-3235">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="cd667-3235">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="cd667-3236">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="cd667-3236">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="cd667-3237">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3237">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="cd667-3238">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3238">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="cd667-3239">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3239">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="cd667-3240">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-3240">December 19, 2017</span></span>

<span data-ttu-id="cd667-3241">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="cd667-3241">Version 2.0.23</span></span>

* <span data-ttu-id="cd667-3242">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="cd667-3242">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="cd667-3243">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-3243">Container</span></span>

* <span data-ttu-id="cd667-3244">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="cd667-3244">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="cd667-3245">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-3245">Network</span></span>

* <span data-ttu-id="cd667-3246">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="cd667-3246">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="cd667-3247">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="cd667-3247">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-3248">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-3248">Storage</span></span>

* <span data-ttu-id="cd667-3249">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="cd667-3249">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-3250">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-3250">VM</span></span>

* <span data-ttu-id="cd667-3251">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="cd667-3251">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="cd667-3252">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-3252">December 5, 2017</span></span>

<span data-ttu-id="cd667-3253">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="cd667-3253">Version 2.0.22</span></span>

* <span data-ttu-id="cd667-3254">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3254">Removed `az component` commands.</span></span> <span data-ttu-id="cd667-3255">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3255">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="cd667-3256">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-3256">Core</span></span>
* <span data-ttu-id="cd667-3257">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="cd667-3257">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="cd667-3258">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="cd667-3258">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-3259">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-3259">ACS</span></span>

* <span data-ttu-id="cd667-3260">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3260">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="cd667-3261">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3261">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="cd667-3262">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="cd667-3262">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="cd667-3263">Помощник</span><span class="sxs-lookup"><span data-stu-id="cd667-3263">Advisor</span></span>

* <span data-ttu-id="cd667-3264">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="cd667-3264">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-3265">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-3265">Appservice</span></span>

* <span data-ttu-id="cd667-3266">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3266">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="cd667-3267">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="cd667-3267">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="cd667-3268">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3268">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="cd667-3269">Потребление</span><span class="sxs-lookup"><span data-stu-id="cd667-3269">Consumption</span></span>

* <span data-ttu-id="cd667-3270">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="cd667-3270">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="cd667-3271">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-3271">Container</span></span>

* <span data-ttu-id="cd667-3272">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="cd667-3272">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-3273">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-3273">Monitor</span></span>

* <span data-ttu-id="cd667-3274">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="cd667-3274">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-3275">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-3275">Resource</span></span>

* <span data-ttu-id="cd667-3276">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="cd667-3276">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="cd667-3277">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-3277">Role</span></span>

* <span data-ttu-id="cd667-3278">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3278">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="cd667-3279">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="cd667-3279">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="cd667-3280">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3280">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-3281">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-3281">SQL</span></span>

* <span data-ttu-id="cd667-3282">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3282">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="cd667-3283">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3283">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-3284">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-3284">VM</span></span>

* <span data-ttu-id="cd667-3285">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3285">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="cd667-3286">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-3286">November 14, 2017</span></span>

<span data-ttu-id="cd667-3287">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="cd667-3287">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-3288">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-3288">ACR</span></span>

* <span data-ttu-id="cd667-3289">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="cd667-3289">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="cd667-3290">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-3290">ACS</span></span>

* <span data-ttu-id="cd667-3291">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="cd667-3291">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="cd667-3292">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="cd667-3292">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="cd667-3293">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3293">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="cd667-3294">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="cd667-3294">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="cd667-3295">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="cd667-3295">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-3296">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-3296">Appservice</span></span>

* <span data-ttu-id="cd667-3297">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="cd667-3297">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="cd667-3298">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3298">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="cd667-3299">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3299">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="cd667-3300">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3300">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="cd667-3301">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="cd667-3301">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="cd667-3302">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="cd667-3302">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="cd667-3303">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-3303">Batch</span></span>

* <span data-ttu-id="cd667-3304">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3304">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="cd667-3305">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="cd667-3305">Batchai</span></span>

* <span data-ttu-id="cd667-3306">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3306">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="cd667-3307">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3307">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="cd667-3308">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3308">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="cd667-3309">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3309">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="cd667-3310">Cloud</span><span class="sxs-lookup"><span data-stu-id="cd667-3310">Cloud</span></span>

* <span data-ttu-id="cd667-3311">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="cd667-3311">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="cd667-3312">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-3312">Container</span></span>

* <span data-ttu-id="cd667-3313">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="cd667-3313">Added support to open multiple ports</span></span>
* <span data-ttu-id="cd667-3314">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="cd667-3314">Added container group restart policy</span></span>
* <span data-ttu-id="cd667-3315">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="cd667-3315">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="cd667-3316">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="cd667-3316">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="cd667-3317">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="cd667-3317">Data Lake Analytics</span></span>

* <span data-ttu-id="cd667-3318">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="cd667-3318">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="cd667-3319">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="cd667-3319">Data Lake Store</span></span>

* <span data-ttu-id="cd667-3320">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="cd667-3320">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="cd667-3321">Расширение</span><span class="sxs-lookup"><span data-stu-id="cd667-3321">Extension</span></span>

* <span data-ttu-id="cd667-3322">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="cd667-3322">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="cd667-3323">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="cd667-3323">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-3324">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-3324">IoT</span></span>

* <span data-ttu-id="cd667-3325">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="cd667-3325">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-3326">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-3326">Monitor</span></span>

* <span data-ttu-id="cd667-3327">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3327">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="cd667-3328">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-3328">Network</span></span>

* <span data-ttu-id="cd667-3329">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="cd667-3329">Added support for CAA DNS records</span></span>
* <span data-ttu-id="cd667-3330">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3330">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="cd667-3331">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="cd667-3331">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="cd667-3332">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3332">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="cd667-3333">Резервирование</span><span class="sxs-lookup"><span data-stu-id="cd667-3333">Reservations</span></span>

* <span data-ttu-id="cd667-3334">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="cd667-3334">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-3335">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-3335">Resource</span></span>

* <span data-ttu-id="cd667-3336">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3336">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-3337">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-3337">SQL</span></span>

* <span data-ttu-id="cd667-3338">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3338">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-3339">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-3339">Storage</span></span>

* <span data-ttu-id="cd667-3340">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-3340">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="cd667-3341">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="cd667-3341">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="cd667-3342">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3342">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="cd667-3343">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3343">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="cd667-3344">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3344">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="cd667-3345">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3345">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="cd667-3346">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3346">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-3347">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-3347">VM</span></span>

* <span data-ttu-id="cd667-3348">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3348">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="cd667-3349">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="cd667-3349">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="cd667-3350">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3350">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="cd667-3351">Переименование `vm format-secret` в `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="cd667-3351">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="cd667-3352">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="cd667-3352">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="cd667-3353">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-3353">October 24, 2017</span></span>

<span data-ttu-id="cd667-3354">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="cd667-3354">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="cd667-3355">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-3355">Core</span></span>

* <span data-ttu-id="cd667-3356">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="cd667-3356">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-3357">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-3357">ACR</span></span>

* <span data-ttu-id="cd667-3358">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="cd667-3358">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="cd667-3359">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="cd667-3359">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="cd667-3360">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="cd667-3360">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-3361">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-3361">ACS</span></span>

* <span data-ttu-id="cd667-3362">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="cd667-3362">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="cd667-3363">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="cd667-3363">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-3364">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-3364">Appservice</span></span>

* <span data-ttu-id="cd667-3365">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="cd667-3365">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="cd667-3366">Компонент</span><span class="sxs-lookup"><span data-stu-id="cd667-3366">Component</span></span>

* <span data-ttu-id="cd667-3367">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="cd667-3367">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-3368">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-3368">Monitor</span></span>

* <span data-ttu-id="cd667-3369">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3369">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-3370">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-3370">Resource</span></span>

* <span data-ttu-id="cd667-3371">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="cd667-3371">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="cd667-3372">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="cd667-3372">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-3373">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-3373">VM</span></span>

* <span data-ttu-id="cd667-3374">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="cd667-3374">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="cd667-3375">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-3375">October 9, 2017</span></span>

<span data-ttu-id="cd667-3376">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="cd667-3376">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="cd667-3377">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-3377">Core</span></span>

* <span data-ttu-id="cd667-3378">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="cd667-3378">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-3379">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-3379">Appservice</span></span>

* <span data-ttu-id="cd667-3380">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3380">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="cd667-3381">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-3381">Batch</span></span>

* <span data-ttu-id="cd667-3382">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="cd667-3382">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="cd667-3383">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="cd667-3383">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="cd667-3384">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="cd667-3384">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="cd667-3385">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="cd667-3385">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="cd667-3386">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="cd667-3386">Batchai</span></span>

* <span data-ttu-id="cd667-3387">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="cd667-3387">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="cd667-3388">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="cd667-3388">Keyvault</span></span>

* <span data-ttu-id="cd667-3389">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="cd667-3389">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="cd667-3390">(#4448)</span><span class="sxs-lookup"><span data-stu-id="cd667-3390">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="cd667-3391">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-3391">Network</span></span>

* <span data-ttu-id="cd667-3392">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="cd667-3392">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="cd667-3393">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="cd667-3393">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-3394">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-3394">Resource</span></span>

* <span data-ttu-id="cd667-3395">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3395">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="cd667-3396">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="cd667-3396">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="cd667-3397">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="cd667-3397">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="cd667-3398">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="cd667-3398">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-3399">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-3399">Sql</span></span>

* <span data-ttu-id="cd667-3400">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="cd667-3400">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="cd667-3401">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="cd667-3401">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="cd667-3402">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="cd667-3402">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-3403">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-3403">Storage</span></span>

* <span data-ttu-id="cd667-3404">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd667-3404">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-3405">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="cd667-3405">Vm</span></span>

* <span data-ttu-id="cd667-3406">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="cd667-3406">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="cd667-3407">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3407">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="cd667-3408">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3408">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="cd667-3409">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3409">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="cd667-3410">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="cd667-3410">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="cd667-3411">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-3411">September 22, 2017</span></span>

<span data-ttu-id="cd667-3412">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="cd667-3412">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-3413">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-3413">Resource</span></span>

* <span data-ttu-id="cd667-3414">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="cd667-3414">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="cd667-3415">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="cd667-3415">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="cd667-3416">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="cd667-3416">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="cd667-3417">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3417">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="cd667-3418">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-3418">Network</span></span>

* <span data-ttu-id="cd667-3419">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="cd667-3419">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="cd667-3420">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="cd667-3420">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="cd667-3421">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="cd667-3421">Added `asg` application security group commands</span></span>
* <span data-ttu-id="cd667-3422">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="cd667-3422">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="cd667-3423">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="cd667-3423">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="cd667-3424">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="cd667-3424">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="cd667-3425">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3425">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-3426">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-3426">Storage</span></span>

* <span data-ttu-id="cd667-3427">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="cd667-3427">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="cd667-3428">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="cd667-3428">Eventgrid</span></span>

* <span data-ttu-id="cd667-3429">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="cd667-3429">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-3430">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-3430">SQL</span></span>

* <span data-ttu-id="cd667-3431">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="cd667-3431">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="cd667-3432">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="cd667-3432">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="cd667-3433">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="cd667-3433">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="cd667-3434">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="cd667-3434">Keyvault</span></span>

* <span data-ttu-id="cd667-3435">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="cd667-3435">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-3436">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-3436">VM</span></span>

* <span data-ttu-id="cd667-3437">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="cd667-3437">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="cd667-3438">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="cd667-3438">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="cd667-3439">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="cd667-3439">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="cd667-3440">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="cd667-3440">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="cd667-3441">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="cd667-3441">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="cd667-3442">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="cd667-3442">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-3443">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-3443">ACS</span></span>

* <span data-ttu-id="cd667-3444">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="cd667-3444">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-3445">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-3445">Appservice</span></span>

* <span data-ttu-id="cd667-3446">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="cd667-3446">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="cd667-3447">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="cd667-3447">Backup</span></span>

* <span data-ttu-id="cd667-3448">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="cd667-3448">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="cd667-3449">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-3449">September 11, 2017</span></span>

<span data-ttu-id="cd667-3450">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="cd667-3450">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="cd667-3451">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-3451">Core</span></span>

* <span data-ttu-id="cd667-3452">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="cd667-3452">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="cd667-3453">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="cd667-3453">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-3454">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-3454">Acs</span></span>

* <span data-ttu-id="cd667-3455">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3455">Added `acs list-locations` command</span></span>
* <span data-ttu-id="cd667-3456">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-3456">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-3457">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-3457">Appservice</span></span>

* <span data-ttu-id="cd667-3458">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="cd667-3458">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="cd667-3459">CDN</span><span class="sxs-lookup"><span data-stu-id="cd667-3459">CDN</span></span>

* <span data-ttu-id="cd667-3460">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3460">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="cd667-3461">Расширение</span><span class="sxs-lookup"><span data-stu-id="cd667-3461">Extension</span></span>

* <span data-ttu-id="cd667-3462">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="cd667-3462">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="cd667-3463">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="cd667-3463">Keyvault</span></span>

* <span data-ttu-id="cd667-3464">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3464">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="cd667-3465">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-3465">Network</span></span>

* <span data-ttu-id="cd667-3466">Переименование `vnet list-private-access-services` в `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="cd667-3466">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="cd667-3467">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3467">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="cd667-3468">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3468">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="cd667-3469">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3469">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="cd667-3470">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3470">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-3471">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-3471">Resource</span></span>

* <span data-ttu-id="cd667-3472">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3472">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="cd667-3473">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3473">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="cd667-3474">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="cd667-3474">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="cd667-3475">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="cd667-3475">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-3476">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-3476">SQL</span></span>

* <span data-ttu-id="cd667-3477">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3477">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-3478">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-3478">VM</span></span>

* <span data-ttu-id="cd667-3479">Исправлено: Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="cd667-3479">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="cd667-3480">Исправлено: Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="cd667-3480">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="cd667-3481">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3481">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="cd667-3482">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="cd667-3482">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="cd667-3483">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="cd667-3483">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="cd667-3484">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-3484">August 31, 2017</span></span>

<span data-ttu-id="cd667-3485">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="cd667-3485">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="cd667-3486">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="cd667-3486">Keyvault</span></span>

* <span data-ttu-id="cd667-3487">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3487">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="cd667-3488">Sf</span><span class="sxs-lookup"><span data-stu-id="cd667-3488">Sf</span></span>

* <span data-ttu-id="cd667-3489">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="cd667-3489">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-3490">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-3490">Storage</span></span>

* <span data-ttu-id="cd667-3491">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="cd667-3491">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="cd667-3492">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="cd667-3492">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="cd667-3493">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-3493">August 28, 2017</span></span>

<span data-ttu-id="cd667-3494">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="cd667-3494">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="cd667-3495">CLI</span><span class="sxs-lookup"><span data-stu-id="cd667-3495">CLI</span></span>

* <span data-ttu-id="cd667-3496">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="cd667-3496">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-3497">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-3497">ACS</span></span>

* <span data-ttu-id="cd667-3498">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="cd667-3498">Corrected preview regions</span></span>
* <span data-ttu-id="cd667-3499">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3499">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="cd667-3500">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="cd667-3500">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-3501">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-3501">Appservice</span></span>

* <span data-ttu-id="cd667-3502">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3502">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="cd667-3503">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3503">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="cd667-3504">Предоставлен параметр `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3504">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="cd667-3505">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="cd667-3505">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="cd667-3506">Исправлено: Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="cd667-3506">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-3507">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-3507">IoT</span></span>

* <span data-ttu-id="cd667-3508">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="cd667-3508">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="cd667-3509">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-3509">Network</span></span>

* <span data-ttu-id="cd667-3510">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3510">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="cd667-3511">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3511">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="cd667-3512">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3512">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="cd667-3513">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3513">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="cd667-3514">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3514">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-3515">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-3515">Profile</span></span>

* <span data-ttu-id="cd667-3516">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="cd667-3516">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="cd667-3517">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="cd667-3517">Service Fabric</span></span>

* <span data-ttu-id="cd667-3518">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="cd667-3518">Preview release</span></span>
* <span data-ttu-id="cd667-3519">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="cd667-3519">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="cd667-3520">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="cd667-3520">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="cd667-3521">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3521">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-3522">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-3522">Storage</span></span>

* <span data-ttu-id="cd667-3523">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="cd667-3523">Enabled setting blob tier</span></span>
* <span data-ttu-id="cd667-3524">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="cd667-3524">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="cd667-3525">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3525">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="cd667-3526">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="cd667-3526">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="cd667-3527">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3527">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="cd667-3528">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3528">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-3529">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-3529">VM</span></span>

* <span data-ttu-id="cd667-3530">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3530">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="cd667-3531">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3531">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="cd667-3532">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="cd667-3532">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="cd667-3533">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="cd667-3533">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="cd667-3534">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="cd667-3534">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="cd667-3535">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3535">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="cd667-3536">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-3536">August 15, 2017</span></span>

<span data-ttu-id="cd667-3537">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="cd667-3537">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-3538">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-3538">ACS</span></span>

* <span data-ttu-id="cd667-3539">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="cd667-3539">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-3540">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-3540">Appservice</span></span>

* <span data-ttu-id="cd667-3541">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="cd667-3541">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="cd667-3542">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-3542">Event Grid</span></span>

* <span data-ttu-id="cd667-3543">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="cd667-3543">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="cd667-3544">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-3544">August 11, 2017</span></span>

<span data-ttu-id="cd667-3545">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="cd667-3545">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-3546">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-3546">ACS</span></span>

* <span data-ttu-id="cd667-3547">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="cd667-3547">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="cd667-3548">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-3548">Batch</span></span>

* <span data-ttu-id="cd667-3549">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="cd667-3549">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="cd667-3550">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="cd667-3550">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="cd667-3551">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd667-3551">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="cd667-3552">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="cd667-3552">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="cd667-3553">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="cd667-3553">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="cd667-3554">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="cd667-3554">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="cd667-3555">Компонент</span><span class="sxs-lookup"><span data-stu-id="cd667-3555">Component</span></span>

* <span data-ttu-id="cd667-3556">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="cd667-3556">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="cd667-3557">Контейнер</span><span class="sxs-lookup"><span data-stu-id="cd667-3557">Container</span></span>

* <span data-ttu-id="cd667-3558">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="cd667-3558">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="cd667-3559">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="cd667-3559">Data Lake Store</span></span>

* <span data-ttu-id="cd667-3560">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="cd667-3560">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="cd667-3561">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-3561">Event Grid</span></span>

* <span data-ttu-id="cd667-3562">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="cd667-3562">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="cd667-3563">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-3563">Network</span></span>

* <span data-ttu-id="cd667-3564">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="cd667-3564">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="cd667-3565">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3565">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="cd667-3566">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3566">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="cd667-3567">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3567">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-3568">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-3568">Profile</span></span>

* <span data-ttu-id="cd667-3569">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="cd667-3569">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-3570">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-3570">Storage</span></span>

* <span data-ttu-id="cd667-3571">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="cd667-3571">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-3572">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-3572">VM</span></span>

* <span data-ttu-id="cd667-3573">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="cd667-3573">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="cd667-3574">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3574">Exposed `list-skus` command</span></span>
* <span data-ttu-id="cd667-3575">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="cd667-3575">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="cd667-3576">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="cd667-3576">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="cd667-3577">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="cd667-3577">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="cd667-3578">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-3578">July 28, 2017</span></span>

<span data-ttu-id="cd667-3579">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="cd667-3579">Version 2.0.12</span></span>

* <span data-ttu-id="cd667-3580">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="cd667-3580">Added container commands</span></span>
* <span data-ttu-id="cd667-3581">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cd667-3581">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="cd667-3582">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-3582">Core</span></span>

* <span data-ttu-id="cd667-3583">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="cd667-3583">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="cd667-3584">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="cd667-3584">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="cd667-3585">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="cd667-3585">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="cd667-3586">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="cd667-3586">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="cd667-3587">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="cd667-3587">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="cd667-3588">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="cd667-3588">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="cd667-3589">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="cd667-3589">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="cd667-3590">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="cd667-3590">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="cd667-3591">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="cd667-3591">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="cd667-3592">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="cd667-3592">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="cd667-3593">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="cd667-3593">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="cd667-3594">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="cd667-3594">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="cd667-3595">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="cd667-3595">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="cd667-3596">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="cd667-3596">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="cd667-3597">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="cd667-3597">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="cd667-3598">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="cd667-3598">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="cd667-3599">ACR</span><span class="sxs-lookup"><span data-stu-id="cd667-3599">ACR</span></span>

* <span data-ttu-id="cd667-3600">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="cd667-3600">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="cd667-3601">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="cd667-3601">Support SKU update for managed registries</span></span>
* <span data-ttu-id="cd667-3602">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="cd667-3602">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="cd667-3603">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="cd667-3603">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="cd667-3604">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="cd667-3604">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="cd667-3605">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="cd667-3605">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-3606">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-3606">ACS</span></span>

* <span data-ttu-id="cd667-3607">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="cd667-3607">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-3608">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="cd667-3608">Appservice</span></span>

* <span data-ttu-id="cd667-3609">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="cd667-3609">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="cd667-3610">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="cd667-3610">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="cd667-3611">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3611">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="cd667-3612">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="cd667-3612">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="cd667-3613">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="cd667-3613">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="cd667-3614">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="cd667-3614">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="cd667-3615">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="cd667-3615">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="cd667-3616">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="cd667-3616">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="cd667-3617">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="cd667-3617">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="cd667-3618">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3618">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="cd667-3619">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="cd667-3619">Batch</span></span>

* <span data-ttu-id="cd667-3620">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="cd667-3620">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="cd667-3621">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3621">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="cd667-3622">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3622">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="cd667-3623">CDN</span><span class="sxs-lookup"><span data-stu-id="cd667-3623">CDN</span></span>

* <span data-ttu-id="cd667-3624">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="cd667-3624">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="cd667-3625">Cloud</span><span class="sxs-lookup"><span data-stu-id="cd667-3625">Cloud</span></span>

* <span data-ttu-id="cd667-3626">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="cd667-3626">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="cd667-3627">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="cd667-3627">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="cd667-3628">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="cd667-3628">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="cd667-3629">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="cd667-3629">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="cd667-3630">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3630">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="cd667-3631">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-3631">CosmosDB</span></span>

* <span data-ttu-id="cd667-3632">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="cd667-3632">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="cd667-3633">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="cd667-3633">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="cd667-3634">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="cd667-3634">Data Lake Analytics</span></span>

* <span data-ttu-id="cd667-3635">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3635">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="cd667-3636">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3636">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="cd667-3637">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3637">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="cd667-3638">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="cd667-3638">Data Lake Store</span></span>

* <span data-ttu-id="cd667-3639">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3639">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="cd667-3640">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="cd667-3640">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="cd667-3641">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3641">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="cd667-3642">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="cd667-3642">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="cd667-3643">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="cd667-3643">Interactive</span></span>

* <span data-ttu-id="cd667-3644">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="cd667-3644">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="cd667-3645">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="cd667-3645">Increased test coverage</span></span>
* <span data-ttu-id="cd667-3646">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="cd667-3646">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="cd667-3647">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="cd667-3647">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="cd667-3648">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="cd667-3648">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="cd667-3649">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="cd667-3649">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="cd667-3650">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="cd667-3650">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="cd667-3651">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3651">Added `--progress` flag</span></span>
* <span data-ttu-id="cd667-3652">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3652">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="cd667-3653">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="cd667-3653">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="cd667-3654">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="cd667-3654">IoT</span></span>

* <span data-ttu-id="cd667-3655">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="cd667-3655">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="cd667-3656">(3934).</span><span class="sxs-lookup"><span data-stu-id="cd667-3656">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="cd667-3657">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="cd667-3657">Key vault</span></span>

* <span data-ttu-id="cd667-3658">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="cd667-3658">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="cd667-3659">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3659">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="cd667-3660">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="cd667-3660">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="cd667-3661">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3661">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="cd667-3662">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3662">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="cd667-3663">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="cd667-3663">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="cd667-3664">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="cd667-3664">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="cd667-3665">(3307).</span><span class="sxs-lookup"><span data-stu-id="cd667-3665">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="cd667-3666">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="cd667-3666">Lab</span></span>

* <span data-ttu-id="cd667-3667">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3667">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="cd667-3668">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3668">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-3669">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-3669">Monitor</span></span>

* <span data-ttu-id="cd667-3670">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="cd667-3670">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="cd667-3671">Переименование `monitor alert-rule-incidents list` в `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="cd667-3671">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="cd667-3672">Переименование `monitor alert-rule-incidents show` в `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="cd667-3672">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="cd667-3673">Переименование `monitor metric-defintions list` в `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="cd667-3673">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="cd667-3674">Переименование `monitor alert-rules` в `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="cd667-3674">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="cd667-3675">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="cd667-3675">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="cd667-3676">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="cd667-3676">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="cd667-3677">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="cd667-3677">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="cd667-3678">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="cd667-3678">`location` no longer required</span></span>
  * <span data-ttu-id="cd667-3679">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="cd667-3679">Add name and ID support for target</span></span>
  * <span data-ttu-id="cd667-3680">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="cd667-3680">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="cd667-3681">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="cd667-3681">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="cd667-3682">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="cd667-3682">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="cd667-3683">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="cd667-3683">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="cd667-3684">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3684">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="cd667-3685">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3685">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="cd667-3686">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-3686">Network</span></span>

* <span data-ttu-id="cd667-3687">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3687">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="cd667-3688">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3688">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="cd667-3689">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="cd667-3689">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="cd667-3690">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3690">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="cd667-3691">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3691">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="cd667-3692">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3692">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="cd667-3693">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3693">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="cd667-3694">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3694">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="cd667-3695">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3695">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="cd667-3696">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3696">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="cd667-3697">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3697">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="cd667-3698">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3698">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="cd667-3699">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3699">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="cd667-3700">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3700">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="cd667-3701">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3701">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="cd667-3702">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3702">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="cd667-3703">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="cd667-3703">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="cd667-3704">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3704">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="cd667-3705">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3705">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="cd667-3706">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3706">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="cd667-3707">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3707">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="cd667-3708">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3708">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="cd667-3709">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3709">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="cd667-3710">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="cd667-3710">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="cd667-3711">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="cd667-3711">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="cd667-3712">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="cd667-3712">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="cd667-3713">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="cd667-3713">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-3714">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-3714">Profile</span></span>

* <span data-ttu-id="cd667-3715">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="cd667-3715">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="cd667-3716">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="cd667-3716">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="cd667-3717">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="cd667-3717">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="cd667-3718">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="cd667-3718">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="cd667-3719">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="cd667-3719">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="cd667-3720">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="cd667-3720">RDBMS</span></span>

* <span data-ttu-id="cd667-3721">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="cd667-3721">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="cd667-3722">Исправлена проблема с обработкой `%s` из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="cd667-3722">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="cd667-3723">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="cd667-3723">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="cd667-3724">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="cd667-3724">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-3725">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-3725">Resource</span></span>

* <span data-ttu-id="cd667-3726">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3726">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="cd667-3727">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3727">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="cd667-3728">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3728">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="cd667-3729">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3729">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="cd667-3730">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="cd667-3730">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="cd667-3731">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3731">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="cd667-3732">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="cd667-3732">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="cd667-3733">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3733">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="cd667-3734">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-3734">Role</span></span>

* <span data-ttu-id="cd667-3735">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="cd667-3735">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="cd667-3736">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="cd667-3736">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="cd667-3737">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="cd667-3737">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="cd667-3738">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="cd667-3738">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="cd667-3739">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3739">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="cd667-3740">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="cd667-3740">Service Fabric</span></span>
* <span data-ttu-id="cd667-3741">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="cd667-3741">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="cd667-3742">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="cd667-3742">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="cd667-3743">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="cd667-3743">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-3744">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-3744">SQL</span></span>

* <span data-ttu-id="cd667-3745">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3745">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="cd667-3746">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3746">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="cd667-3747">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3747">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-3748">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-3748">Storage</span></span>

* <span data-ttu-id="cd667-3749">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="cd667-3749">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="cd667-3750">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="cd667-3750">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="cd667-3751">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="cd667-3751">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="cd667-3752">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="cd667-3752">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="cd667-3753">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="cd667-3753">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="cd667-3754">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="cd667-3754">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-3755">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-3755">VM</span></span>

* <span data-ttu-id="cd667-3756">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="cd667-3756">Support configuring nsg</span></span>
* <span data-ttu-id="cd667-3757">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="cd667-3757">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="cd667-3758">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="cd667-3758">Support managed service identities</span></span>
* <span data-ttu-id="cd667-3759">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3759">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="cd667-3760">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="cd667-3760">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="cd667-3761">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-3761">May 10, 2017</span></span>

<span data-ttu-id="cd667-3762">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="cd667-3762">Version 2.0.6</span></span>

* <span data-ttu-id="cd667-3763">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="cd667-3763">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="cd667-3764">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="cd667-3764">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="cd667-3765">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="cd667-3765">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="cd667-3766">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="cd667-3766">Include Cognitive Services module</span></span>
* <span data-ttu-id="cd667-3767">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="cd667-3767">Include Service Fabric module</span></span>
* <span data-ttu-id="cd667-3768">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="cd667-3768">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="cd667-3769">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="cd667-3769">Add support for CDN commands</span></span>
* <span data-ttu-id="cd667-3770">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="cd667-3770">Remove Container module</span></span>
* <span data-ttu-id="cd667-3771">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3771">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="cd667-3772">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3772">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="cd667-3773">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-3773">Core</span></span>

* <span data-ttu-id="cd667-3774">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="cd667-3774">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="cd667-3775">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([#2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3775">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="cd667-3776">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3776">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="cd667-3777">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3777">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="cd667-3778">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3778">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="cd667-3779">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3779">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="cd667-3780">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3780">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="cd667-3781">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3781">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="cd667-3782">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3782">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="cd667-3783">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="cd667-3783">core: Improved performance</span></span>
* <span data-ttu-id="cd667-3784">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="cd667-3784">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="cd667-3785">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="cd667-3785">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-3786">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-3786">ACS</span></span>

* <span data-ttu-id="cd667-3787">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="cd667-3787">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="cd667-3788">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="cd667-3788">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="cd667-3789">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="cd667-3789">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="cd667-3790">Удален профиль Windows перед вызовом метода PUT для команды scale ([#2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3790">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-3791">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-3791">AppService</span></span>

* <span data-ttu-id="cd667-3792">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="cd667-3792">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="cd667-3793">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="cd667-3793">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="cd667-3794">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="cd667-3794">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="cd667-3795">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="cd667-3795">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="cd667-3796">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="cd667-3796">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="cd667-3797">Включена поддержка настройки строк подключения ([#2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3797">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="cd667-3798">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="cd667-3798">support slot swap with preview</span></span>
* <span data-ttu-id="cd667-3799">Устранены ошибки из команд службы приложений ([#2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3799">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="cd667-3800">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([#2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3800">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="cd667-3801">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="cd667-3801">CosmosDB</span></span>

* <span data-ttu-id="cd667-3802">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="cd667-3802">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="cd667-3803">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="cd667-3803">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="cd667-3804">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="cd667-3804">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="cd667-3805">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="cd667-3805">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="cd667-3806">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="cd667-3806">Data Lake Analytics</span></span>

* <span data-ttu-id="cd667-3807">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="cd667-3807">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="cd667-3808">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="cd667-3808">Add support for new catalog item type: package.</span></span> <span data-ttu-id="cd667-3809">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3809">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="cd667-3810">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="cd667-3810">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="cd667-3811">Таблица</span><span class="sxs-lookup"><span data-stu-id="cd667-3811">Table</span></span>
  * <span data-ttu-id="cd667-3812">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="cd667-3812">Table valued function</span></span>
  * <span data-ttu-id="cd667-3813">Представление</span><span class="sxs-lookup"><span data-stu-id="cd667-3813">View</span></span>
  * <span data-ttu-id="cd667-3814">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="cd667-3814">Table Statistics.</span></span> <span data-ttu-id="cd667-3815">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="cd667-3815">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="cd667-3816">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="cd667-3816">Data Lake Store</span></span>

* <span data-ttu-id="cd667-3817">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="cd667-3817">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="cd667-3818">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3818">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="cd667-3819">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="cd667-3819">missed help for access show.</span></span> <span data-ttu-id="cd667-3820">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="cd667-3820">adding it.</span></span> <span data-ttu-id="cd667-3821">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="cd667-3821">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="cd667-3822">Поиск</span><span class="sxs-lookup"><span data-stu-id="cd667-3822">Find</span></span>

* <span data-ttu-id="cd667-3823">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="cd667-3823">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="cd667-3824">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="cd667-3824">KeyVault</span></span>

* <span data-ttu-id="cd667-3825">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="cd667-3825">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="cd667-3826">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="cd667-3826">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="cd667-3827">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="cd667-3827">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="cd667-3828">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="cd667-3828">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="cd667-3829">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3829">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="cd667-3830">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="cd667-3830">Lab</span></span>

* <span data-ttu-id="cd667-3831">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="cd667-3831">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="cd667-3832">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="cd667-3832">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="cd667-3833">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="cd667-3833">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="cd667-3834">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="cd667-3834">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="cd667-3835">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="cd667-3835">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="cd667-3836">Монитор</span><span class="sxs-lookup"><span data-stu-id="cd667-3836">Monitor</span></span>

* <span data-ttu-id="cd667-3837">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3837">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="cd667-3838">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3838">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="cd667-3839">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-3839">Network</span></span>

* <span data-ttu-id="cd667-3840">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3840">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="cd667-3841">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3841">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="cd667-3842">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="cd667-3842">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="cd667-3843">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="cd667-3843">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="cd667-3844">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="cd667-3844">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="cd667-3845">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="cd667-3845">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="cd667-3846">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="cd667-3846">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="cd667-3847">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="cd667-3847">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="cd667-3848">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3848">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="cd667-3849">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="cd667-3849">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="cd667-3850">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3850">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="cd667-3851">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3851">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="cd667-3852">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="cd667-3852">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="cd667-3853">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="cd667-3853">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="cd667-3854">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="cd667-3854">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="cd667-3855">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="cd667-3855">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="cd667-3856">Профиль</span><span class="sxs-lookup"><span data-stu-id="cd667-3856">Profile</span></span>

* <span data-ttu-id="cd667-3857">Включена поддержка входа при отсутствии подписок ([#2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3857">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="cd667-3858">Включена поддержка сокращенных имен параметров в команде az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3858">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="cd667-3859">Redis</span><span class="sxs-lookup"><span data-stu-id="cd667-3859">Redis</span></span>

* <span data-ttu-id="cd667-3860">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="cd667-3860">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="cd667-3861">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="cd667-3861">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="cd667-3862">Ресурс</span><span class="sxs-lookup"><span data-stu-id="cd667-3862">Resource</span></span>

* <span data-ttu-id="cd667-3863">Добавлены команды определения managedapp и managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3863">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="cd667-3864">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3864">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="cd667-3865">Включена поддержка создания универсального ресурса ([#2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3865">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="cd667-3866">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="cd667-3866">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="cd667-3867">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="cd667-3867">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="cd667-3868">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="cd667-3868">Add docs for az lock update.</span></span> <span data-ttu-id="cd667-3869">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="cd667-3869">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="cd667-3870">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="cd667-3870">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="cd667-3871">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="cd667-3871">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="cd667-3872">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="cd667-3872">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="cd667-3873">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="cd667-3873">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="cd667-3874">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([#2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3874">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="cd667-3875">Роль</span><span class="sxs-lookup"><span data-stu-id="cd667-3875">Role</span></span>

* <span data-ttu-id="cd667-3876">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([#2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3876">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="cd667-3877">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3877">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="cd667-3878">Роль: устранены проблемы при обновлении определения роли ([#2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3878">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="cd667-3879">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="cd667-3879">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="cd667-3880">SQL</span><span class="sxs-lookup"><span data-stu-id="cd667-3880">SQL</span></span>

* <span data-ttu-id="cd667-3881">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="cd667-3881">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="cd667-3882">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3882">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="cd667-3883">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-3883">Storage</span></span>

* <span data-ttu-id="cd667-3884">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3884">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="cd667-3885">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="cd667-3885">Add support for incremental blob copy</span></span>
* <span data-ttu-id="cd667-3886">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="cd667-3886">Add support for large block blob upload</span></span>
* <span data-ttu-id="cd667-3887">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="cd667-3887">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-3888">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-3888">VM</span></span>

* <span data-ttu-id="cd667-3889">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="cd667-3889">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="cd667-3890">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="cd667-3890">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="cd667-3891">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="cd667-3891">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="cd667-3892">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="cd667-3892">az vm/vmss disk</span></span>
  3. <span data-ttu-id="cd667-3893">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="cd667-3893">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="cd667-3894">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="cd667-3894">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="cd667-3895">vm/vmss: добавлена поддержка создания из образа Marketplace, для которого требуются сведения о плане ([#1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3895">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="cd667-3896">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-3896">April 3, 2017</span></span>

<span data-ttu-id="cd667-3897">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="cd667-3897">Version 2.0.2</span></span>

<span data-ttu-id="cd667-3898">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="cd667-3898">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="cd667-3899">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="cd667-3899">Core</span></span>

* <span data-ttu-id="cd667-3900">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-3900">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="cd667-3901">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3901">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="cd667-3902">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3902">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="cd667-3903">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3903">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="cd667-3904">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3904">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="cd667-3905">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="cd667-3905">Add prompting for missing template parameters.</span></span> <span data-ttu-id="cd667-3906">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3906">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="cd667-3907">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd667-3907">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="cd667-3908">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="cd667-3908">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="cd667-3909">ACS</span><span class="sxs-lookup"><span data-stu-id="cd667-3909">ACS</span></span>

* <span data-ttu-id="cd667-3910">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3910">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="cd667-3911">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="cd667-3911">Add support for ssh key password prompting.</span></span> <span data-ttu-id="cd667-3912">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3912">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="cd667-3913">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="cd667-3913">Add support for windows clusters.</span></span> <span data-ttu-id="cd667-3914">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3914">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="cd667-3915">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="cd667-3915">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="cd667-3916">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3916">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="cd667-3917">AppService</span><span class="sxs-lookup"><span data-stu-id="cd667-3917">AppService</span></span>

* <span data-ttu-id="cd667-3918">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3918">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="cd667-3919">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3919">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="cd667-3920">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3920">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="cd667-3921">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3921">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="cd667-3922">Data Lake</span><span class="sxs-lookup"><span data-stu-id="cd667-3922">DataLake</span></span>

* <span data-ttu-id="cd667-3923">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="cd667-3923">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="cd667-3924">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="cd667-3924">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="cd667-3925">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="cd667-3925">DocuemntDB</span></span>

* <span data-ttu-id="cd667-3926">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3926">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="cd667-3927">ВМ</span><span class="sxs-lookup"><span data-stu-id="cd667-3927">VM</span></span>

* <span data-ttu-id="cd667-3928">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3928">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="cd667-3929">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3929">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="cd667-3930">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3930">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="cd667-3931">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3931">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="cd667-3932">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3932">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="cd667-3933">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3933">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="cd667-3934">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="cd667-3934">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="cd667-3935">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="cd667-3935">February 27, 2017</span></span>

<span data-ttu-id="cd667-3936">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="cd667-3936">Version 2.0.0</span></span>

<span data-ttu-id="cd667-3937">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="cd667-3937">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="cd667-3938">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="cd667-3938">Container Service (acs)</span></span>
- <span data-ttu-id="cd667-3939">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="cd667-3939">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="cd667-3940">Сеть</span><span class="sxs-lookup"><span data-stu-id="cd667-3940">Networking</span></span>
- <span data-ttu-id="cd667-3941">Память</span><span class="sxs-lookup"><span data-stu-id="cd667-3941">Storage</span></span>

<span data-ttu-id="cd667-3942">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3942">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="cd667-3943">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="cd667-3943">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="cd667-3944">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="cd667-3944">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="cd667-3945">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="cd667-3945">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="cd667-3946">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="cd667-3946">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="cd667-3947">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="cd667-3947">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="cd667-3948">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="cd667-3948">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="cd667-3949">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="cd667-3949">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="cd667-3950">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="cd667-3950">Provide feedback from the command line with the `az feedback` command</span></span>

# <a name="beta-release-notes"></a>[<span data-ttu-id="cd667-3951">Заметки о выпуске бета-версии</span><span class="sxs-lookup"><span data-stu-id="cd667-3951">Beta release notes</span></span>](#tab/azure-cli-beta)

<span data-ttu-id="cd667-3952">Бета-версия Azure CLI позволяет перейти с метода аутентификации платформы AAD (версия 1.0) на [платформу удостоверений Майкрософт (версия 2.0)](/azure/active-directory/develop/v2-overview).</span><span class="sxs-lookup"><span data-stu-id="cd667-3952">The Azure CLI beta release is a migration from the authentican method of AAD platform (v1.0) to [Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview).</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="cd667-3953">23 июня 2020 года</span><span class="sxs-lookup"><span data-stu-id="cd667-3953">June 23, 2020</span></span>

### <a name="things-to-know-about-the-new-azure-cli-beta-release"></a><span data-ttu-id="cd667-3954">Сведения о новой бета-версии Azure CLI</span><span class="sxs-lookup"><span data-stu-id="cd667-3954">Things to know about the new Azure CLI beta release</span></span>

-   <span data-ttu-id="cd667-3955">Бета-версия Azure CLI поддерживает все команды интерфейса командной строки, которые включены в текущую выпущенную версию.</span><span class="sxs-lookup"><span data-stu-id="cd667-3955">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span>
-   <span data-ttu-id="cd667-3956">После установки бета-версии требуется выполнить повторный вход.</span><span class="sxs-lookup"><span data-stu-id="cd667-3956">Relogin is required after install the beta version.</span></span>
-   <span data-ttu-id="cd667-3957">Бета-версия поддерживает только платформу Windows.</span><span class="sxs-lookup"><span data-stu-id="cd667-3957">The beta release only supports the Windows platform.</span></span>
-   <span data-ttu-id="cd667-3958">Azure Stack не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd667-3958">The Azure Stack is not supported.</span></span>
-   <span data-ttu-id="cd667-3959">Параметр `--use-cert-sn-issuer` не поддерживается, если для проверки подлинности используется ключ субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="cd667-3959">`--use-cert-sn-issuer` parameter is not supported when using service principal key to authenticate.</span></span>
-   <span data-ttu-id="cd667-3960">Пропуск проверки SSL с использованием `ADAL_PYTHON_SSL_NO_VERIFY` среды не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd667-3960">Skip SSL verification via environment `ADAL_PYTHON_SSL_NO_VERIFY` is not supported.</span></span>

<span data-ttu-id="cd667-3961">Если у вас возникли проблемы с использованием бета-версии, вы можете обратиться к группе разработчиков Azure CLI на [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span><span class="sxs-lookup"><span data-stu-id="cd667-3961">If you find any issues in the beta release, the Azure CLI engineering team welcomes your comments on [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span></span>

---
