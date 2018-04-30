---
title: Заметки о выпуске Azure CLI 2.0
description: Узнайте о последних обновлениях в Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 04/10/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: fd5d82e34089a9a884c25c9a5620526f9d30577a
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="33763-103">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="33763-103">Azure CLI 2.0 release notes</span></span>

## <a name="april-10-2018"></a><span data-ttu-id="33763-104">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="33763-104">April 10, 2018</span></span>

<span data-ttu-id="33763-105">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="33763-105">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="33763-106">ACR</span><span class="sxs-lookup"><span data-stu-id="33763-106">ACR</span></span>

* <span data-ttu-id="33763-107">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="33763-107">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="33763-108">ACS</span><span class="sxs-lookup"><span data-stu-id="33763-108">ACS</span></span>

* <span data-ttu-id="33763-109">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="33763-109">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="33763-110">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="33763-110">Appservice</span></span>

* [КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="33763-112">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="33763-112">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="33763-113">Batch AI</span><span class="sxs-lookup"><span data-stu-id="33763-113">BatchAI</span></span>

* <span data-ttu-id="33763-114">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="33763-114">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="33763-115">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="33763-115">Job level mounting</span></span>
 - <span data-ttu-id="33763-116">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="33763-116">Environment variables with secret values</span></span>
 - <span data-ttu-id="33763-117">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="33763-117">Performance counters settings</span></span>
 - <span data-ttu-id="33763-118">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="33763-118">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="33763-119">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="33763-119">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="33763-120">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="33763-120">Usage and limits reporting</span></span>
 - <span data-ttu-id="33763-121">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="33763-121">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="33763-122">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="33763-122">Support for custom images</span></span>
 - <span data-ttu-id="33763-123">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="33763-123">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="33763-124">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="33763-124">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="33763-125">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="33763-125">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="33763-126">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="33763-126">National clouds are supported</span></span>
* <span data-ttu-id="33763-127">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="33763-127">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="33763-128">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="33763-128">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="33763-129">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="33763-129">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="33763-130">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="33763-130">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="33763-131">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="33763-131">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="33763-132">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="33763-132">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="33763-133">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="33763-133">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="33763-134">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="33763-134">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="33763-135">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="33763-135">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="33763-136">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="33763-136">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="33763-137">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="33763-137">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="33763-138">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="33763-138">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="33763-139">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="33763-139">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="33763-140">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="33763-140">Billing</span></span>

* <span data-ttu-id="33763-141">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="33763-141">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="33763-142">Потребление</span><span class="sxs-lookup"><span data-stu-id="33763-142">Consumption</span></span>

* <span data-ttu-id="33763-143">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="33763-143">Added `marketplace` commands</span></span>
* <span data-ttu-id="33763-144">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="33763-144">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="33763-145">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="33763-145">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="33763-146">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="33763-146">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="33763-147">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="33763-147">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="33763-148">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="33763-148">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="33763-149">Контейнер</span><span class="sxs-lookup"><span data-stu-id="33763-149">Container</span></span>

* <span data-ttu-id="33763-150">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="33763-150">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="33763-151">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="33763-151">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="33763-152">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="33763-152">Extension</span></span>

* <span data-ttu-id="33763-153">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="33763-153">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="33763-154">Interactive</span><span class="sxs-lookup"><span data-stu-id="33763-154">Interactive</span></span>

* <span data-ttu-id="33763-155">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="33763-155">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="33763-156">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="33763-156">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="33763-157">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="33763-157">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="33763-158">Сеть</span><span class="sxs-lookup"><span data-stu-id="33763-158">Network</span></span>

* <span data-ttu-id="33763-159">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="33763-159">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="33763-160">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="33763-160">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="33763-161">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="33763-161">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="33763-162">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="33763-162">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="33763-163">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="33763-163">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="33763-164">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="33763-164">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="33763-165">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="33763-165">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="33763-166">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="33763-166">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="33763-167">Профиль</span><span class="sxs-lookup"><span data-stu-id="33763-167">Profile</span></span>

* <span data-ttu-id="33763-168">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="33763-168">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="33763-169">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="33763-169">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="33763-170">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="33763-170">RDBMS</span></span>

* <span data-ttu-id="33763-171">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="33763-171">Added `georestore` command</span></span>
* <span data-ttu-id="33763-172">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="33763-172">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="33763-173">Ресурс</span><span class="sxs-lookup"><span data-stu-id="33763-173">Resource</span></span>

* <span data-ttu-id="33763-174">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="33763-174">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="33763-175">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="33763-175">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="33763-176">SQL</span><span class="sxs-lookup"><span data-stu-id="33763-176">SQL</span></span>

* <span data-ttu-id="33763-177">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="33763-177">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="33763-178">Хранилище</span><span class="sxs-lookup"><span data-stu-id="33763-178">Storage</span></span>

* <span data-ttu-id="33763-179">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="33763-179">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="33763-180">ВМ</span><span class="sxs-lookup"><span data-stu-id="33763-180">VM</span></span>

* <span data-ttu-id="33763-181">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="33763-181">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="33763-182">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="33763-182">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="33763-184">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="33763-184">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="33763-185">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="33763-185">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="33763-186">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="33763-186">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="33763-187">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="33763-187">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="33763-188">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="33763-188">March 27, 2018</span></span>

<span data-ttu-id="33763-189">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="33763-189">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="33763-190">Core</span><span class="sxs-lookup"><span data-stu-id="33763-190">Core</span></span>

* <span data-ttu-id="33763-191">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="33763-191">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="33763-192">ACS</span><span class="sxs-lookup"><span data-stu-id="33763-192">ACS</span></span>

* <span data-ttu-id="33763-193">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="33763-193">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="33763-194">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="33763-194">Appservice</span></span>

* <span data-ttu-id="33763-195">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="33763-195">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="33763-196">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="33763-196">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="33763-197">Архивация</span><span class="sxs-lookup"><span data-stu-id="33763-197">Backup</span></span>

* <span data-ttu-id="33763-198">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="33763-198">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="33763-199">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="33763-199">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="33763-200">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="33763-200">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="33763-201">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="33763-201">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="33763-202">Контейнер</span><span class="sxs-lookup"><span data-stu-id="33763-202">Container</span></span>

* <span data-ttu-id="33763-203">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="33763-203">Added `container exec` command.</span></span> <span data-ttu-id="33763-204">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="33763-204">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="33763-205">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="33763-205">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="33763-206">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="33763-206">Extension</span></span>

* <span data-ttu-id="33763-207">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="33763-207">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="33763-208">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="33763-208">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="33763-209">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="33763-209">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="33763-210">Interactive</span><span class="sxs-lookup"><span data-stu-id="33763-210">Interactive</span></span>

* <span data-ttu-id="33763-211">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="33763-211">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="33763-212">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="33763-212">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="33763-213">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="33763-213">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="33763-214">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="33763-214">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="33763-215">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="33763-215">Lab</span></span>

* <span data-ttu-id="33763-216">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="33763-216">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="33763-217">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="33763-217">Monitor</span></span>

* <span data-ttu-id="33763-218">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="33763-218">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="33763-219">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="33763-219">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="33763-220">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="33763-220">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="33763-221">Сеть</span><span class="sxs-lookup"><span data-stu-id="33763-221">Network</span></span>

* <span data-ttu-id="33763-222">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="33763-222">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="33763-223">Профиль</span><span class="sxs-lookup"><span data-stu-id="33763-223">Profile</span></span>

* <span data-ttu-id="33763-224">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="33763-224">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="33763-225">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="33763-225">RDBMS</span></span>

* <span data-ttu-id="33763-226">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="33763-226">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="33763-227">Ресурс</span><span class="sxs-lookup"><span data-stu-id="33763-227">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="33763-229">Роль</span><span class="sxs-lookup"><span data-stu-id="33763-229">Role</span></span>

* <span data-ttu-id="33763-230">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="33763-230">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="33763-231">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="33763-231">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="33763-232">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="33763-232">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="33763-233">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="33763-233">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="33763-234">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="33763-234">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="33763-235">Хранилище</span><span class="sxs-lookup"><span data-stu-id="33763-235">Storage</span></span>

* <span data-ttu-id="33763-236">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="33763-236">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="33763-237">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049): проблемы, когда при отправке добавочного большого двоичного объекта игнорируются параметры условия.</span><span class="sxs-lookup"><span data-stu-id="33763-237">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="33763-238">ВМ</span><span class="sxs-lookup"><span data-stu-id="33763-238">VM</span></span>

* <span data-ttu-id="33763-239">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="33763-239">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="33763-240">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="33763-240">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="33763-241">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="33763-241">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="33763-242">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="33763-242">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="33763-243">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="33763-243">March 13, 2018</span></span>

<span data-ttu-id="33763-244">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="33763-244">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="33763-245">ACR</span><span class="sxs-lookup"><span data-stu-id="33763-245">ACR</span></span>

* <span data-ttu-id="33763-246">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="33763-246">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="33763-247">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="33763-247">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="33763-248">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="33763-248">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="33763-249">ACS</span><span class="sxs-lookup"><span data-stu-id="33763-249">ACS</span></span>

* <span data-ttu-id="33763-250">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="33763-250">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="33763-251">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="33763-251">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="33763-252">Помощник</span><span class="sxs-lookup"><span data-stu-id="33763-252">Advisor</span></span>

* <span data-ttu-id="33763-253">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="33763-253">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="33763-254">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="33763-254">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="33763-255">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="33763-255">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="33763-256">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="33763-256">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="33763-257">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="33763-257">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="33763-258">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="33763-258">Appservice</span></span>

* <span data-ttu-id="33763-259">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="33763-259">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="33763-260">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="33763-260">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="33763-261">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="33763-261">Eventhubs</span></span>

* <span data-ttu-id="33763-262">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="33763-262">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="33763-263">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="33763-263">Extension</span></span>

* <span data-ttu-id="33763-264">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="33763-264">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="33763-265">Interactive</span><span class="sxs-lookup"><span data-stu-id="33763-265">Interactive</span></span>

* <span data-ttu-id="33763-266">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625): теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="33763-266">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="33763-267">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016): при использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="33763-267">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="33763-268">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688): если при загрузке таблицы команд возникало исключение, опережающий ввод не выполнялся.</span><span class="sxs-lookup"><span data-stu-id="33763-268">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="33763-269">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="33763-269">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="33763-270">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="33763-270">Monitor</span></span>

* <span data-ttu-id="33763-271">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="33763-271">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="33763-272">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="33763-272">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="33763-273">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="33763-273">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="33763-274">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="33763-274">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="33763-275">Сеть</span><span class="sxs-lookup"><span data-stu-id="33763-275">Network</span></span>

* <span data-ttu-id="33763-276">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="33763-276">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="33763-277">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="33763-277">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="33763-278">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="33763-278">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="33763-279">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="33763-279">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="33763-280">Профиль</span><span class="sxs-lookup"><span data-stu-id="33763-280">Profile</span></span>

* <span data-ttu-id="33763-281">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="33763-281">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="33763-282">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="33763-282">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="33763-283">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="33763-283">RDBMS</span></span>

* <span data-ttu-id="33763-284">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="33763-284">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="33763-285">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="33763-285">Service Bus</span></span>

* <span data-ttu-id="33763-286">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="33763-286">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="33763-287">Хранилище</span><span class="sxs-lookup"><span data-stu-id="33763-287">Storage</span></span>

* <span data-ttu-id="33763-288">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="33763-288">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="33763-289">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286): при пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="33763-289">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="33763-290">ВМ</span><span class="sxs-lookup"><span data-stu-id="33763-290">VM</span></span>

* <span data-ttu-id="33763-291">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="33763-291">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="33763-292">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="33763-292">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="33763-293">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="33763-293">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="33763-294">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="33763-294">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="33763-295">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="33763-295">February 27, 2018</span></span>

<span data-ttu-id="33763-296">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="33763-296">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="33763-297">Core</span><span class="sxs-lookup"><span data-stu-id="33763-297">Core</span></span>

* <span data-ttu-id="33763-298">Исправлена ошибка с установкой Homebrew [№ 5184](https://github.com/Azure/azure-cli/issues/5184).</span><span class="sxs-lookup"><span data-stu-id="33763-298">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="33763-299">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="33763-299">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="33763-300">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="33763-300">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="33763-301">ACS</span><span class="sxs-lookup"><span data-stu-id="33763-301">ACS</span></span>

* <span data-ttu-id="33763-302">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="33763-302">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="33763-303">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="33763-303">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="33763-304">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="33763-304">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="33763-305">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="33763-305">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="33763-306">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="33763-306">Appservice</span></span>

* <span data-ttu-id="33763-307">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="33763-307">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="33763-308">Исправлена ошибка с сообщением `Free` о недопустимом SKU [№ 5538](https://github.com/Azure/azure-cli/issues/5538)</span><span class="sxs-lookup"><span data-stu-id="33763-308">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="33763-309">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="33763-309">Cognitive Services</span></span>

* <span data-ttu-id="33763-310">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="33763-310">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="33763-311">Потребление</span><span class="sxs-lookup"><span data-stu-id="33763-311">Consumption</span></span>

* <span data-ttu-id="33763-312">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="33763-312">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="33763-313">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="33763-313">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="33763-314">Контейнер</span><span class="sxs-lookup"><span data-stu-id="33763-314">Container</span></span>

* <span data-ttu-id="33763-315">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="33763-315">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="33763-316">Сеть</span><span class="sxs-lookup"><span data-stu-id="33763-316">Network</span></span>

* <span data-ttu-id="33763-317">Исправлена ошибка с отсутствующим клиентом в `network vnet-gateway vpn-client generate` [№ 5559](https://github.com/Azure/azure-cli/issues/5559).</span><span class="sxs-lookup"><span data-stu-id="33763-317">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="33763-318">Ресурс</span><span class="sxs-lookup"><span data-stu-id="33763-318">Resource</span></span>

* <span data-ttu-id="33763-319">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="33763-319">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="33763-320">Роль</span><span class="sxs-lookup"><span data-stu-id="33763-320">Role</span></span>

* <span data-ttu-id="33763-321">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="33763-321">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="33763-322">SQL</span><span class="sxs-lookup"><span data-stu-id="33763-322">SQL</span></span>

* <span data-ttu-id="33763-323">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="33763-323">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="33763-324">Хранилище</span><span class="sxs-lookup"><span data-stu-id="33763-324">Storage</span></span>

* <span data-ttu-id="33763-325">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="33763-325">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="33763-326">ВМ</span><span class="sxs-lookup"><span data-stu-id="33763-326">VM</span></span>

* <span data-ttu-id="33763-327">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="33763-327">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="33763-328">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="33763-328">February 13, 2018</span></span>

<span data-ttu-id="33763-329">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="33763-329">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="33763-330">Core</span><span class="sxs-lookup"><span data-stu-id="33763-330">Core</span></span>

* <span data-ttu-id="33763-331">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="33763-331">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="33763-332">ACS</span><span class="sxs-lookup"><span data-stu-id="33763-332">ACS</span></span>

* <span data-ttu-id="33763-333">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="33763-333">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="33763-334">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="33763-334">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="33763-335">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="33763-335">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="33763-336">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="33763-336">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="33763-337">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="33763-337">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="33763-338">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="33763-338">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="33763-339">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="33763-339">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="33763-340">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="33763-340">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="33763-341">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="33763-341">Appservice</span></span>

* <span data-ttu-id="33763-342">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="33763-342">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="33763-343">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="33763-343">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="33763-344">CDN</span><span class="sxs-lookup"><span data-stu-id="33763-344">CDN</span></span>

* <span data-ttu-id="33763-345">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="33763-345">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="33763-346">Контейнер</span><span class="sxs-lookup"><span data-stu-id="33763-346">Container</span></span>

* <span data-ttu-id="33763-347">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="33763-347">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="33763-348">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="33763-348">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="33763-349">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="33763-349">CosmosDB</span></span>

* <span data-ttu-id="33763-350">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="33763-350">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="33763-351">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="33763-351">Extension</span></span>

* <span data-ttu-id="33763-352">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="33763-352">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="33763-353">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="33763-353">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="33763-354">Отзыв</span><span class="sxs-lookup"><span data-stu-id="33763-354">Feedback</span></span>

* <span data-ttu-id="33763-355">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="33763-355">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="33763-356">Interactive</span><span class="sxs-lookup"><span data-stu-id="33763-356">Interactive</span></span>

* <span data-ttu-id="33763-357">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="33763-357">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="33763-358">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="33763-358">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="33763-359">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="33763-359">IoT</span></span>

* <span data-ttu-id="33763-360">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="33763-360">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="33763-361">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="33763-361">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="33763-362">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="33763-362">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="33763-363">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="33763-363">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="33763-364">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="33763-364">Monitor</span></span>

* <span data-ttu-id="33763-365">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="33763-365">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="33763-366">Сеть</span><span class="sxs-lookup"><span data-stu-id="33763-366">Network</span></span>

* <span data-ttu-id="33763-367">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="33763-367">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="33763-368">Профиль</span><span class="sxs-lookup"><span data-stu-id="33763-368">Profile</span></span>

* <span data-ttu-id="33763-369">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="33763-369">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="33763-370">Ресурс</span><span class="sxs-lookup"><span data-stu-id="33763-370">Resource</span></span>

* <span data-ttu-id="33763-371">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="33763-371">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="33763-372">Роль</span><span class="sxs-lookup"><span data-stu-id="33763-372">Role</span></span>

* <span data-ttu-id="33763-373">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="33763-373">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="33763-374">SQL</span><span class="sxs-lookup"><span data-stu-id="33763-374">SQL</span></span>

* <span data-ttu-id="33763-375">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="33763-375">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="33763-376">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="33763-376">Added `sql db rename`</span></span>
* <span data-ttu-id="33763-377">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="33763-377">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="33763-378">Хранилище</span><span class="sxs-lookup"><span data-stu-id="33763-378">Storage</span></span>

* <span data-ttu-id="33763-379">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="33763-379">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="33763-380">ВМ</span><span class="sxs-lookup"><span data-stu-id="33763-380">VM</span></span>

* <span data-ttu-id="33763-381">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="33763-381">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="33763-382">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="33763-382">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="33763-383">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="33763-383">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="33763-384">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="33763-384">January 31, 2018</span></span>

<span data-ttu-id="33763-385">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="33763-385">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="33763-386">Core</span><span class="sxs-lookup"><span data-stu-id="33763-386">Core</span></span>

* <span data-ttu-id="33763-387">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="33763-387">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="33763-388">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="33763-388">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="33763-389">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="33763-389">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="33763-390">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="33763-390">Use `--verbose` to see</span></span>
* <span data-ttu-id="33763-391">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="33763-391">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="33763-392">ACS</span><span class="sxs-lookup"><span data-stu-id="33763-392">ACS</span></span>

* <span data-ttu-id="33763-393">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="33763-393">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="33763-394">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="33763-394">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="33763-395">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="33763-395">Appservice</span></span>

* <span data-ttu-id="33763-396">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="33763-396">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="33763-397">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="33763-397">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="33763-398">CDN</span><span class="sxs-lookup"><span data-stu-id="33763-398">CDN</span></span>

* <span data-ttu-id="33763-399">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="33763-399">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="33763-400">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="33763-400">CosmosDB</span></span>

* <span data-ttu-id="33763-401">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="33763-401">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="33763-402">Interactive</span><span class="sxs-lookup"><span data-stu-id="33763-402">Interactive</span></span>

* <span data-ttu-id="33763-403">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="33763-403">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="33763-404">Сеть</span><span class="sxs-lookup"><span data-stu-id="33763-404">Network</span></span>

* <span data-ttu-id="33763-405">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="33763-405">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="33763-406">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="33763-406">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="33763-407">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="33763-407">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="33763-408">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="33763-408">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="33763-409">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="33763-409">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="33763-410">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="33763-410">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="33763-411">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="33763-411">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="33763-412">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="33763-412">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="33763-413">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="33763-413">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="33763-414">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="33763-414">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="33763-415">Профиль</span><span class="sxs-lookup"><span data-stu-id="33763-415">Profile</span></span>

* <span data-ttu-id="33763-416">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="33763-416">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="33763-417">Ресурс</span><span class="sxs-lookup"><span data-stu-id="33763-417">Resource</span></span>

* <span data-ttu-id="33763-418">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="33763-418">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="33763-419">Хранилище</span><span class="sxs-lookup"><span data-stu-id="33763-419">Storage</span></span>

* <span data-ttu-id="33763-420">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="33763-420">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="33763-421">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="33763-421">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="33763-422">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="33763-422">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="33763-423">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="33763-423">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="33763-424">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="33763-424">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="33763-425">ВМ</span><span class="sxs-lookup"><span data-stu-id="33763-425">VM</span></span>

* <span data-ttu-id="33763-426">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="33763-426">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="33763-427">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="33763-427">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="33763-428">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="33763-428">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="33763-429">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="33763-429">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="33763-430">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="33763-430">January 17, 2018</span></span>

<span data-ttu-id="33763-431">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="33763-431">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="33763-432">ACR</span><span class="sxs-lookup"><span data-stu-id="33763-432">ACR</span></span>

* <span data-ttu-id="33763-433">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="33763-433">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="33763-434">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="33763-434">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="33763-435">ACS</span><span class="sxs-lookup"><span data-stu-id="33763-435">ACS</span></span>

* <span data-ttu-id="33763-436">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="33763-436">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="33763-437">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="33763-437">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="33763-438">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="33763-438">Appservice</span></span>

* <span data-ttu-id="33763-439">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="33763-439">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="33763-440">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="33763-440">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="33763-441">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="33763-441">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="33763-442">Архивация</span><span class="sxs-lookup"><span data-stu-id="33763-442">Backup</span></span>

* <span data-ttu-id="33763-443">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="33763-443">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="33763-444">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="33763-444">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="33763-445">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="33763-445">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="33763-446">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="33763-446">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="33763-447">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="33763-447">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="33763-448">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="33763-448">Batch</span></span>

* <span data-ttu-id="33763-449">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="33763-449">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="33763-450">Облако</span><span class="sxs-lookup"><span data-stu-id="33763-450">Cloud</span></span>

* <span data-ttu-id="33763-451">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="33763-451">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="33763-452">Потребление</span><span class="sxs-lookup"><span data-stu-id="33763-452">Consumption</span></span>

* <span data-ttu-id="33763-453">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="33763-453">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="33763-454">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="33763-454">Event Grid</span></span>

* <span data-ttu-id="33763-455">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="33763-455">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="33763-456">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="33763-456">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="33763-457">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="33763-457">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="33763-458">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="33763-458">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="33763-459">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="33763-459">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="33763-460">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="33763-460">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="33763-461">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="33763-461">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="33763-462">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="33763-462">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="33763-463">Interactive</span><span class="sxs-lookup"><span data-stu-id="33763-463">Interactive</span></span>

* <span data-ttu-id="33763-464">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="33763-464">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="33763-465">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="33763-465">Fixed errors on startup</span></span>
* <span data-ttu-id="33763-466">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="33763-466">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="33763-467">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="33763-467">IoT</span></span>

* <span data-ttu-id="33763-468">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="33763-468">Added support for device provisioning service</span></span>
* <span data-ttu-id="33763-469">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="33763-469">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="33763-470">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="33763-470">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="33763-471">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="33763-471">Monitor</span></span>

* <span data-ttu-id="33763-472">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="33763-472">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="33763-473">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="33763-473">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="33763-474">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="33763-474">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="33763-475">Сеть</span><span class="sxs-lookup"><span data-stu-id="33763-475">Network</span></span>

* <span data-ttu-id="33763-476">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="33763-476">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="33763-477">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="33763-477">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="33763-478">Профиль</span><span class="sxs-lookup"><span data-stu-id="33763-478">Profile</span></span>

* <span data-ttu-id="33763-479">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="33763-479">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="33763-480">Роль</span><span class="sxs-lookup"><span data-stu-id="33763-480">Role</span></span>

* <span data-ttu-id="33763-481">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="33763-481">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="33763-482">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="33763-482">Service Fabric</span></span>

* <span data-ttu-id="33763-483">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="33763-483">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="33763-484">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="33763-484">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="33763-485">ВМ</span><span class="sxs-lookup"><span data-stu-id="33763-485">VM</span></span>

* <span data-ttu-id="33763-486">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="33763-486">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="33763-487">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="33763-487">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="33763-488">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="33763-488">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="33763-489">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="33763-489">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="33763-490">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="33763-490">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="33763-491">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="33763-491">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="33763-492">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="33763-492">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="33763-493">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="33763-493">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="33763-494">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="33763-494">December 19, 2017</span></span>

<span data-ttu-id="33763-495">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="33763-495">Version 2.0.23</span></span>

* <span data-ttu-id="33763-496">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="33763-496">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="33763-497">Контейнер</span><span class="sxs-lookup"><span data-stu-id="33763-497">Container</span></span>

* <span data-ttu-id="33763-498">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="33763-498">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="33763-499">Сеть</span><span class="sxs-lookup"><span data-stu-id="33763-499">Network</span></span>

* <span data-ttu-id="33763-500">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="33763-500">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="33763-501">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="33763-501">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="33763-502">Хранилище</span><span class="sxs-lookup"><span data-stu-id="33763-502">Storage</span></span>

* <span data-ttu-id="33763-503">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="33763-503">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="33763-504">ВМ</span><span class="sxs-lookup"><span data-stu-id="33763-504">VM</span></span>

* <span data-ttu-id="33763-505">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="33763-505">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="33763-506">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="33763-506">December 5, 2017</span></span>

<span data-ttu-id="33763-507">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="33763-507">Version 2.0.22</span></span>

* <span data-ttu-id="33763-508">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="33763-508">Removed `az component` commands.</span></span> <span data-ttu-id="33763-509">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="33763-509">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="33763-510">Core</span><span class="sxs-lookup"><span data-stu-id="33763-510">Core</span></span>
* <span data-ttu-id="33763-511">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="33763-511">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="33763-512">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="33763-512">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="33763-513">ACS</span><span class="sxs-lookup"><span data-stu-id="33763-513">ACS</span></span>

* <span data-ttu-id="33763-514">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="33763-514">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="33763-515">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="33763-515">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="33763-516">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="33763-516">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="33763-517">Помощник</span><span class="sxs-lookup"><span data-stu-id="33763-517">Advisor</span></span>

* <span data-ttu-id="33763-518">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="33763-518">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="33763-519">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="33763-519">Appservice</span></span>

* <span data-ttu-id="33763-520">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="33763-520">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="33763-521">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="33763-521">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="33763-522">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="33763-522">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="33763-523">Потребление</span><span class="sxs-lookup"><span data-stu-id="33763-523">Consumption</span></span>

* <span data-ttu-id="33763-524">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="33763-524">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="33763-525">Контейнер</span><span class="sxs-lookup"><span data-stu-id="33763-525">Container</span></span>

* <span data-ttu-id="33763-526">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="33763-526">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="33763-527">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="33763-527">Monitor</span></span>

* <span data-ttu-id="33763-528">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="33763-528">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="33763-529">Ресурс</span><span class="sxs-lookup"><span data-stu-id="33763-529">Resource</span></span>

* <span data-ttu-id="33763-530">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="33763-530">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="33763-531">Роль</span><span class="sxs-lookup"><span data-stu-id="33763-531">Role</span></span>

* <span data-ttu-id="33763-532">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="33763-532">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="33763-533">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="33763-533">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="33763-534">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="33763-534">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="33763-535">SQL</span><span class="sxs-lookup"><span data-stu-id="33763-535">SQL</span></span>

* <span data-ttu-id="33763-536">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="33763-536">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="33763-537">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="33763-537">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="33763-538">ВМ</span><span class="sxs-lookup"><span data-stu-id="33763-538">VM</span></span>

* <span data-ttu-id="33763-539">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="33763-539">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="33763-540">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="33763-540">November 14, 2017</span></span>

<span data-ttu-id="33763-541">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="33763-541">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="33763-542">ACR</span><span class="sxs-lookup"><span data-stu-id="33763-542">ACR</span></span>

* <span data-ttu-id="33763-543">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="33763-543">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="33763-544">ACS</span><span class="sxs-lookup"><span data-stu-id="33763-544">ACS</span></span>

* <span data-ttu-id="33763-545">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="33763-545">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="33763-546">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="33763-546">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="33763-547">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="33763-547">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="33763-548">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="33763-548">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="33763-549">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="33763-549">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="33763-550">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="33763-550">Appservice</span></span>

* <span data-ttu-id="33763-551">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="33763-551">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="33763-552">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="33763-552">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="33763-553">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="33763-553">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="33763-554">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="33763-554">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="33763-555">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="33763-555">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="33763-556">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="33763-556">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="33763-557">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="33763-557">Batch</span></span>

* <span data-ttu-id="33763-558">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="33763-558">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="33763-559">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="33763-559">Batchai</span></span>

* <span data-ttu-id="33763-560">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="33763-560">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="33763-561">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="33763-561">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="33763-562">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="33763-562">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="33763-563">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="33763-563">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="33763-564">Облако</span><span class="sxs-lookup"><span data-stu-id="33763-564">Cloud</span></span>

* <span data-ttu-id="33763-565">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="33763-565">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="33763-566">Контейнер</span><span class="sxs-lookup"><span data-stu-id="33763-566">Container</span></span>

* <span data-ttu-id="33763-567">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="33763-567">Added support to open multiple ports</span></span>
* <span data-ttu-id="33763-568">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="33763-568">Added container group restart policy</span></span>
* <span data-ttu-id="33763-569">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="33763-569">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="33763-570">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="33763-570">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="33763-571">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="33763-571">Data Lake Analytics</span></span>

* <span data-ttu-id="33763-572">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="33763-572">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="33763-573">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="33763-573">Data Lake Store</span></span>

* <span data-ttu-id="33763-574">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="33763-574">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="33763-575">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="33763-575">Extension</span></span>

* <span data-ttu-id="33763-576">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="33763-576">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="33763-577">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="33763-577">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="33763-578">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="33763-578">IoT</span></span>

* <span data-ttu-id="33763-579">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="33763-579">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="33763-580">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="33763-580">Monitor</span></span>

* <span data-ttu-id="33763-581">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="33763-581">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="33763-582">Сеть</span><span class="sxs-lookup"><span data-stu-id="33763-582">Network</span></span>

* <span data-ttu-id="33763-583">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="33763-583">Added support for CAA DNS records</span></span>
* <span data-ttu-id="33763-584">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="33763-584">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="33763-585">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="33763-585">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="33763-586">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="33763-586">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="33763-587">Резервирование</span><span class="sxs-lookup"><span data-stu-id="33763-587">Reservations</span></span>

* <span data-ttu-id="33763-588">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="33763-588">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="33763-589">Ресурс</span><span class="sxs-lookup"><span data-stu-id="33763-589">Resource</span></span>

* <span data-ttu-id="33763-590">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="33763-590">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="33763-591">SQL</span><span class="sxs-lookup"><span data-stu-id="33763-591">SQL</span></span>

* <span data-ttu-id="33763-592">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="33763-592">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="33763-593">Хранилище</span><span class="sxs-lookup"><span data-stu-id="33763-593">Storage</span></span>

* <span data-ttu-id="33763-594">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="33763-594">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="33763-595">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="33763-595">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="33763-596">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="33763-596">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="33763-597">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="33763-597">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="33763-598">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="33763-598">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="33763-599">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="33763-599">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="33763-600">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="33763-600">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="33763-601">ВМ</span><span class="sxs-lookup"><span data-stu-id="33763-601">VM</span></span>

* <span data-ttu-id="33763-602">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="33763-602">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="33763-603">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="33763-603">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="33763-604">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="33763-604">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="33763-605">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="33763-605">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="33763-606">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="33763-606">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="33763-607">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="33763-607">October 24, 2017</span></span>

<span data-ttu-id="33763-608">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="33763-608">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="33763-609">Core</span><span class="sxs-lookup"><span data-stu-id="33763-609">Core</span></span>

* <span data-ttu-id="33763-610">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="33763-610">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="33763-611">ACR</span><span class="sxs-lookup"><span data-stu-id="33763-611">ACR</span></span>

* <span data-ttu-id="33763-612">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="33763-612">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="33763-613">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="33763-613">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="33763-614">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="33763-614">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="33763-615">ACS</span><span class="sxs-lookup"><span data-stu-id="33763-615">ACS</span></span>

* <span data-ttu-id="33763-616">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="33763-616">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="33763-617">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="33763-617">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="33763-618">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="33763-618">Appservice</span></span>

* <span data-ttu-id="33763-619">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="33763-619">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="33763-620">Компонент</span><span class="sxs-lookup"><span data-stu-id="33763-620">Component</span></span>

* <span data-ttu-id="33763-621">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="33763-621">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="33763-622">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="33763-622">Monitor</span></span>

* <span data-ttu-id="33763-623">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="33763-623">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="33763-624">Ресурс</span><span class="sxs-lookup"><span data-stu-id="33763-624">Resource</span></span>

* <span data-ttu-id="33763-625">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="33763-625">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="33763-626">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="33763-626">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="33763-627">ВМ</span><span class="sxs-lookup"><span data-stu-id="33763-627">VM</span></span>

* <span data-ttu-id="33763-628">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="33763-628">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="33763-629">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="33763-629">October 9, 2017</span></span>

<span data-ttu-id="33763-630">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="33763-630">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="33763-631">Core</span><span class="sxs-lookup"><span data-stu-id="33763-631">Core</span></span>

* <span data-ttu-id="33763-632">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="33763-632">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="33763-633">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="33763-633">Appservice</span></span>

* <span data-ttu-id="33763-634">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="33763-634">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="33763-635">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="33763-635">Batch</span></span>

* <span data-ttu-id="33763-636">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="33763-636">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="33763-637">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="33763-637">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="33763-638">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="33763-638">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="33763-639">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="33763-639">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="33763-640">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="33763-640">Batchai</span></span>

* <span data-ttu-id="33763-641">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="33763-641">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="33763-642">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="33763-642">Keyvault</span></span>

* <span data-ttu-id="33763-643">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="33763-643">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="33763-644">(#4448)</span><span class="sxs-lookup"><span data-stu-id="33763-644">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="33763-645">Сеть</span><span class="sxs-lookup"><span data-stu-id="33763-645">Network</span></span>

* <span data-ttu-id="33763-646">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="33763-646">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="33763-647">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="33763-647">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="33763-648">Ресурс</span><span class="sxs-lookup"><span data-stu-id="33763-648">Resource</span></span>

* <span data-ttu-id="33763-649">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="33763-649">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="33763-650">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="33763-650">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="33763-651">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="33763-651">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="33763-652">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="33763-652">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="33763-653">SQL</span><span class="sxs-lookup"><span data-stu-id="33763-653">Sql</span></span>

* <span data-ttu-id="33763-654">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="33763-654">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="33763-655">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="33763-655">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="33763-656">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="33763-656">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="33763-657">Хранилище</span><span class="sxs-lookup"><span data-stu-id="33763-657">Storage</span></span>

* <span data-ttu-id="33763-658">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="33763-658">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="33763-659">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="33763-659">Vm</span></span>

* <span data-ttu-id="33763-660">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="33763-660">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="33763-661">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="33763-661">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="33763-662">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="33763-662">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="33763-663">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="33763-663">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="33763-664">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="33763-664">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="33763-665">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="33763-665">September 22, 2017</span></span>

<span data-ttu-id="33763-666">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="33763-666">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="33763-667">Ресурс</span><span class="sxs-lookup"><span data-stu-id="33763-667">Resource</span></span>

* <span data-ttu-id="33763-668">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="33763-668">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="33763-669">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="33763-669">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="33763-670">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="33763-670">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="33763-671">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="33763-671">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="33763-672">Сеть</span><span class="sxs-lookup"><span data-stu-id="33763-672">Network</span></span>

* <span data-ttu-id="33763-673">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="33763-673">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="33763-674">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="33763-674">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="33763-675">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="33763-675">Added `asg` application security group commands</span></span>
* <span data-ttu-id="33763-676">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="33763-676">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="33763-677">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="33763-677">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="33763-678">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="33763-678">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="33763-679">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="33763-679">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="33763-680">Хранилище</span><span class="sxs-lookup"><span data-stu-id="33763-680">Storage</span></span>

* <span data-ttu-id="33763-681">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="33763-681">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="33763-682">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="33763-682">Eventgrid</span></span>

* <span data-ttu-id="33763-683">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="33763-683">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="33763-684">SQL</span><span class="sxs-lookup"><span data-stu-id="33763-684">SQL</span></span>

* <span data-ttu-id="33763-685">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="33763-685">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="33763-686">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="33763-686">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="33763-687">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="33763-687">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="33763-688">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="33763-688">Keyvault</span></span>

* <span data-ttu-id="33763-689">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="33763-689">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="33763-690">ВМ</span><span class="sxs-lookup"><span data-stu-id="33763-690">VM</span></span>

* <span data-ttu-id="33763-691">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="33763-691">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="33763-692">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="33763-692">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="33763-693">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="33763-693">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="33763-694">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="33763-694">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="33763-695">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="33763-695">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="33763-696">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="33763-696">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="33763-697">ACS</span><span class="sxs-lookup"><span data-stu-id="33763-697">ACS</span></span>

* <span data-ttu-id="33763-698">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="33763-698">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="33763-699">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="33763-699">Appservice</span></span>

* <span data-ttu-id="33763-700">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="33763-700">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="33763-701">Архивация</span><span class="sxs-lookup"><span data-stu-id="33763-701">Backup</span></span>

* <span data-ttu-id="33763-702">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="33763-702">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="33763-703">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="33763-703">September 11, 2017</span></span>

<span data-ttu-id="33763-704">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="33763-704">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="33763-705">Core</span><span class="sxs-lookup"><span data-stu-id="33763-705">Core</span></span>

* <span data-ttu-id="33763-706">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="33763-706">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="33763-707">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="33763-707">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="33763-708">ACS</span><span class="sxs-lookup"><span data-stu-id="33763-708">Acs</span></span>

* <span data-ttu-id="33763-709">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="33763-709">Added `acs list-locations` command</span></span>
* <span data-ttu-id="33763-710">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="33763-710">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="33763-711">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="33763-711">Appservice</span></span>

* <span data-ttu-id="33763-712">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="33763-712">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="33763-713">CDN</span><span class="sxs-lookup"><span data-stu-id="33763-713">CDN</span></span>

* <span data-ttu-id="33763-714">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="33763-714">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="33763-715">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="33763-715">Extension</span></span>

* <span data-ttu-id="33763-716">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="33763-716">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="33763-717">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="33763-717">Keyvault</span></span>

* <span data-ttu-id="33763-718">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="33763-718">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="33763-719">Сеть</span><span class="sxs-lookup"><span data-stu-id="33763-719">Network</span></span>

* <span data-ttu-id="33763-720">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="33763-720">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="33763-721">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="33763-721">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="33763-722">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="33763-722">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="33763-723">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="33763-723">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="33763-724">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="33763-724">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="33763-725">Ресурс</span><span class="sxs-lookup"><span data-stu-id="33763-725">Resource</span></span>

* <span data-ttu-id="33763-726">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="33763-726">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="33763-727">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="33763-727">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="33763-728">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="33763-728">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="33763-729">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="33763-729">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="33763-730">SQL</span><span class="sxs-lookup"><span data-stu-id="33763-730">SQL</span></span>

* <span data-ttu-id="33763-731">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="33763-731">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="33763-732">ВМ</span><span class="sxs-lookup"><span data-stu-id="33763-732">VM</span></span>

* <span data-ttu-id="33763-733">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="33763-733">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="33763-734">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="33763-734">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="33763-735">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="33763-735">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="33763-736">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="33763-736">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="33763-737">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="33763-737">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="33763-738">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="33763-738">August 31, 2017</span></span>

<span data-ttu-id="33763-739">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="33763-739">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="33763-740">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="33763-740">Keyvault</span></span>

* <span data-ttu-id="33763-741">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="33763-741">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="33763-742">Sf</span><span class="sxs-lookup"><span data-stu-id="33763-742">Sf</span></span>

* <span data-ttu-id="33763-743">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="33763-743">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="33763-744">Хранилище</span><span class="sxs-lookup"><span data-stu-id="33763-744">Storage</span></span>

* <span data-ttu-id="33763-745">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="33763-745">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="33763-746">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="33763-746">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="33763-747">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="33763-747">August 28, 2017</span></span>

<span data-ttu-id="33763-748">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="33763-748">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="33763-749">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="33763-749">CLI</span></span>

* <span data-ttu-id="33763-750">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="33763-750">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="33763-751">ACS</span><span class="sxs-lookup"><span data-stu-id="33763-751">ACS</span></span>

* <span data-ttu-id="33763-752">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="33763-752">Corrected preview regions</span></span>
* <span data-ttu-id="33763-753">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="33763-753">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="33763-754">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="33763-754">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="33763-755">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="33763-755">Appservice</span></span>

* <span data-ttu-id="33763-756">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="33763-756">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="33763-757">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="33763-757">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="33763-758">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="33763-758">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="33763-759">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="33763-759">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="33763-760">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="33763-760">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="33763-761">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="33763-761">IoT</span></span>

* <span data-ttu-id="33763-762">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="33763-762">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="33763-763">Сеть</span><span class="sxs-lookup"><span data-stu-id="33763-763">Network</span></span>

* <span data-ttu-id="33763-764">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="33763-764">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="33763-765">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="33763-765">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="33763-766">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="33763-766">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="33763-767">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="33763-767">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="33763-768">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="33763-768">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="33763-769">Профиль</span><span class="sxs-lookup"><span data-stu-id="33763-769">Profile</span></span>

* <span data-ttu-id="33763-770">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="33763-770">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="33763-771">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="33763-771">Service Fabric</span></span>

* <span data-ttu-id="33763-772">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="33763-772">Preview release</span></span>
* <span data-ttu-id="33763-773">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="33763-773">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="33763-774">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="33763-774">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="33763-775">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="33763-775">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="33763-776">Хранилище</span><span class="sxs-lookup"><span data-stu-id="33763-776">Storage</span></span>

* <span data-ttu-id="33763-777">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="33763-777">Enabled setting blob tier</span></span>
* <span data-ttu-id="33763-778">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="33763-778">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="33763-779">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="33763-779">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="33763-780">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="33763-780">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="33763-781">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="33763-781">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="33763-782">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="33763-782">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="33763-783">ВМ</span><span class="sxs-lookup"><span data-stu-id="33763-783">VM</span></span>

* <span data-ttu-id="33763-784">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="33763-784">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="33763-785">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="33763-785">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="33763-786">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="33763-786">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="33763-787">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="33763-787">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="33763-788">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="33763-788">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="33763-789">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="33763-789">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="33763-790">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="33763-790">August 15, 2017</span></span>

<span data-ttu-id="33763-791">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="33763-791">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="33763-792">ACS</span><span class="sxs-lookup"><span data-stu-id="33763-792">ACS</span></span>

* <span data-ttu-id="33763-793">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="33763-793">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="33763-794">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="33763-794">Appservice</span></span>

* <span data-ttu-id="33763-795">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="33763-795">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="33763-796">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="33763-796">Event Grid</span></span>

* <span data-ttu-id="33763-797">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="33763-797">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="33763-798">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="33763-798">August 11, 2017</span></span>

<span data-ttu-id="33763-799">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="33763-799">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="33763-800">ACS</span><span class="sxs-lookup"><span data-stu-id="33763-800">ACS</span></span>

* <span data-ttu-id="33763-801">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="33763-801">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="33763-802">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="33763-802">Batch</span></span>

* <span data-ttu-id="33763-803">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="33763-803">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="33763-804">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="33763-804">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="33763-805">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="33763-805">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="33763-806">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="33763-806">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="33763-807">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="33763-807">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="33763-808">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="33763-808">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="33763-809">Компонент</span><span class="sxs-lookup"><span data-stu-id="33763-809">Component</span></span>

* <span data-ttu-id="33763-810">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="33763-810">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="33763-811">Контейнер</span><span class="sxs-lookup"><span data-stu-id="33763-811">Container</span></span>

* <span data-ttu-id="33763-812">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="33763-812">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="33763-813">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="33763-813">Data Lake Store</span></span>

* <span data-ttu-id="33763-814">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="33763-814">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="33763-815">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="33763-815">Event Grid</span></span>

* <span data-ttu-id="33763-816">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="33763-816">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="33763-817">Сеть</span><span class="sxs-lookup"><span data-stu-id="33763-817">Network</span></span>

* <span data-ttu-id="33763-818">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="33763-818">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="33763-819">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="33763-819">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="33763-820">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="33763-820">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="33763-821">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="33763-821">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="33763-822">Профиль</span><span class="sxs-lookup"><span data-stu-id="33763-822">Profile</span></span>

* <span data-ttu-id="33763-823">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="33763-823">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="33763-824">Хранилище</span><span class="sxs-lookup"><span data-stu-id="33763-824">Storage</span></span>

* <span data-ttu-id="33763-825">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="33763-825">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="33763-826">ВМ</span><span class="sxs-lookup"><span data-stu-id="33763-826">VM</span></span>

* <span data-ttu-id="33763-827">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="33763-827">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="33763-828">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="33763-828">Exposed `list-skus` command</span></span>
* <span data-ttu-id="33763-829">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="33763-829">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="33763-830">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="33763-830">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="33763-831">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="33763-831">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="33763-832">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="33763-832">July 28, 2017</span></span>

<span data-ttu-id="33763-833">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="33763-833">Version 2.0.12</span></span>

* <span data-ttu-id="33763-834">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="33763-834">Added container commands</span></span>
* <span data-ttu-id="33763-835">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="33763-835">Added billing and consumption modules</span></span>

```
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

### <a name="core"></a><span data-ttu-id="33763-836">Core</span><span class="sxs-lookup"><span data-stu-id="33763-836">Core</span></span>

* <span data-ttu-id="33763-837">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="33763-837">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="33763-838">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="33763-838">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="33763-839">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="33763-839">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="33763-840">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="33763-840">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="33763-841">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="33763-841">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="33763-842">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="33763-842">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="33763-843">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="33763-843">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="33763-844">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="33763-844">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="33763-845">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="33763-845">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="33763-846">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="33763-846">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="33763-847">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="33763-847">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="33763-848">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="33763-848">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="33763-849">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="33763-849">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="33763-850">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="33763-850">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="33763-851">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="33763-851">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="33763-852">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="33763-852">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="33763-853">ACR</span><span class="sxs-lookup"><span data-stu-id="33763-853">ACR</span></span>

* <span data-ttu-id="33763-854">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="33763-854">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="33763-855">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="33763-855">Support SKU update for managed registries</span></span>
* <span data-ttu-id="33763-856">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="33763-856">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="33763-857">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="33763-857">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="33763-858">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="33763-858">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="33763-859">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="33763-859">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="33763-860">ACS</span><span class="sxs-lookup"><span data-stu-id="33763-860">ACS</span></span>

* <span data-ttu-id="33763-861">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="33763-861">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="33763-862">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="33763-862">Appservice</span></span>

* <span data-ttu-id="33763-863">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="33763-863">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="33763-864">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="33763-864">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="33763-865">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="33763-865">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="33763-866">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="33763-866">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="33763-867">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="33763-867">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="33763-868">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="33763-868">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="33763-869">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="33763-869">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="33763-870">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="33763-870">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="33763-871">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="33763-871">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="33763-872">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="33763-872">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="33763-873">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="33763-873">Batch</span></span>

* <span data-ttu-id="33763-874">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="33763-874">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="33763-875">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="33763-875">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="33763-876">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="33763-876">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="33763-877">CDN</span><span class="sxs-lookup"><span data-stu-id="33763-877">CDN</span></span>

* <span data-ttu-id="33763-878">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="33763-878">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="33763-879">Облако</span><span class="sxs-lookup"><span data-stu-id="33763-879">Cloud</span></span>

* <span data-ttu-id="33763-880">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="33763-880">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="33763-881">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="33763-881">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="33763-882">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="33763-882">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="33763-883">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="33763-883">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="33763-884">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="33763-884">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="33763-885">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="33763-885">CosmosDB</span></span>

* <span data-ttu-id="33763-886">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="33763-886">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="33763-887">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="33763-887">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="33763-888">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="33763-888">Data Lake Analytics</span></span>

* <span data-ttu-id="33763-889">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="33763-889">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="33763-890">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="33763-890">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="33763-891">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="33763-891">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="33763-892">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="33763-892">Data Lake Store</span></span>

* <span data-ttu-id="33763-893">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="33763-893">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="33763-894">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="33763-894">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="33763-895">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="33763-895">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="33763-896">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="33763-896">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="33763-897">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="33763-897">Interactive</span></span>

* <span data-ttu-id="33763-898">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="33763-898">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="33763-899">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="33763-899">Increased test coverage</span></span>
* <span data-ttu-id="33763-900">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="33763-900">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="33763-901">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="33763-901">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="33763-902">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="33763-902">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="33763-903">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="33763-903">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="33763-904">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="33763-904">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="33763-905">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="33763-905">Added `--progress` flag</span></span>
* <span data-ttu-id="33763-906">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="33763-906">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="33763-907">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="33763-907">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="33763-908">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="33763-908">IoT</span></span>

* <span data-ttu-id="33763-909">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="33763-909">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="33763-910">(3934).</span><span class="sxs-lookup"><span data-stu-id="33763-910">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="33763-911">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="33763-911">Key vault</span></span>

* <span data-ttu-id="33763-912">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="33763-912">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="33763-913">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="33763-913">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="33763-914">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="33763-914">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="33763-915">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="33763-915">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="33763-916">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="33763-916">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="33763-917">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="33763-917">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="33763-918">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="33763-918">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="33763-919">(3307).</span><span class="sxs-lookup"><span data-stu-id="33763-919">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="33763-920">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="33763-920">Lab</span></span>

* <span data-ttu-id="33763-921">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="33763-921">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="33763-922">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="33763-922">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="33763-923">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="33763-923">Monitor</span></span>

* <span data-ttu-id="33763-924">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="33763-924">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="33763-925">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="33763-925">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="33763-926">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="33763-926">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="33763-927">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="33763-927">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="33763-928">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="33763-928">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="33763-929">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="33763-929">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="33763-930">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="33763-930">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="33763-931">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="33763-931">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="33763-932">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="33763-932">`location` no longer required</span></span>
  * <span data-ttu-id="33763-933">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="33763-933">Add name and ID support for target</span></span>
  * <span data-ttu-id="33763-934">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="33763-934">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="33763-935">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="33763-935">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="33763-936">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="33763-936">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="33763-937">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="33763-937">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="33763-938">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="33763-938">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="33763-939">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="33763-939">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="33763-940">Сеть</span><span class="sxs-lookup"><span data-stu-id="33763-940">Network</span></span>

* <span data-ttu-id="33763-941">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="33763-941">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="33763-942">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="33763-942">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="33763-943">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="33763-943">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="33763-944">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="33763-944">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="33763-945">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="33763-945">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="33763-946">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="33763-946">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="33763-947">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="33763-947">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="33763-948">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="33763-948">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="33763-949">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="33763-949">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="33763-950">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="33763-950">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="33763-951">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="33763-951">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="33763-952">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="33763-952">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="33763-953">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="33763-953">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="33763-954">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="33763-954">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="33763-955">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="33763-955">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="33763-956">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="33763-956">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="33763-957">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="33763-957">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="33763-958">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="33763-958">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="33763-959">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="33763-959">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="33763-960">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="33763-960">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="33763-961">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="33763-961">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="33763-962">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="33763-962">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="33763-963">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="33763-963">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="33763-964">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="33763-964">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="33763-965">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="33763-965">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="33763-966">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="33763-966">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="33763-967">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="33763-967">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="33763-968">Профиль</span><span class="sxs-lookup"><span data-stu-id="33763-968">Profile</span></span>

* <span data-ttu-id="33763-969">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="33763-969">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="33763-970">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="33763-970">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="33763-971">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="33763-971">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="33763-972">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="33763-972">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="33763-973">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="33763-973">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="33763-974">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="33763-974">RDBMS</span></span>

* <span data-ttu-id="33763-975">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="33763-975">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="33763-976">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="33763-976">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="33763-977">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="33763-977">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="33763-978">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="33763-978">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="33763-979">Ресурс</span><span class="sxs-lookup"><span data-stu-id="33763-979">Resource</span></span>

* <span data-ttu-id="33763-980">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="33763-980">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="33763-981">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="33763-981">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="33763-982">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="33763-982">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="33763-983">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="33763-983">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="33763-984">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="33763-984">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="33763-985">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="33763-985">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="33763-986">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="33763-986">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="33763-987">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="33763-987">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="33763-988">Роль</span><span class="sxs-lookup"><span data-stu-id="33763-988">Role</span></span>

* <span data-ttu-id="33763-989">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="33763-989">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="33763-990">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="33763-990">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="33763-991">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="33763-991">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="33763-992">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="33763-992">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="33763-993">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="33763-993">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="33763-994">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="33763-994">Service Fabric</span></span>
* <span data-ttu-id="33763-995">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="33763-995">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="33763-996">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="33763-996">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="33763-997">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="33763-997">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="33763-998">SQL</span><span class="sxs-lookup"><span data-stu-id="33763-998">SQL</span></span>

* <span data-ttu-id="33763-999">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="33763-999">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="33763-1000">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="33763-1000">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="33763-1001">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="33763-1001">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="33763-1002">Хранилище</span><span class="sxs-lookup"><span data-stu-id="33763-1002">Storage</span></span>

* <span data-ttu-id="33763-1003">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="33763-1003">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="33763-1004">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="33763-1004">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="33763-1005">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="33763-1005">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="33763-1006">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="33763-1006">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="33763-1007">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="33763-1007">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="33763-1008">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="33763-1008">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="33763-1009">ВМ</span><span class="sxs-lookup"><span data-stu-id="33763-1009">VM</span></span>

* <span data-ttu-id="33763-1010">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="33763-1010">Support configuring nsg</span></span>
* <span data-ttu-id="33763-1011">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="33763-1011">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="33763-1012">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="33763-1012">Support managed service identities</span></span>
* <span data-ttu-id="33763-1013">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="33763-1013">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="33763-1014">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="33763-1014">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="33763-1015">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="33763-1015">May 10, 2017</span></span>

<span data-ttu-id="33763-1016">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="33763-1016">Version 2.0.6</span></span>

* <span data-ttu-id="33763-1017">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="33763-1017">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="33763-1018">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="33763-1018">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="33763-1019">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="33763-1019">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="33763-1020">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="33763-1020">Include Cognitive Services module</span></span>
* <span data-ttu-id="33763-1021">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="33763-1021">Include Service Fabric module</span></span>
* <span data-ttu-id="33763-1022">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="33763-1022">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="33763-1023">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="33763-1023">Add support for CDN commands</span></span>
* <span data-ttu-id="33763-1024">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="33763-1024">Remove Container module</span></span>
* <span data-ttu-id="33763-1025">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="33763-1025">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="33763-1026">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="33763-1026">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="33763-1027">Core</span><span class="sxs-lookup"><span data-stu-id="33763-1027">Core</span></span>

* <span data-ttu-id="33763-1028">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="33763-1028">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="33763-1029">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="33763-1029">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="33763-1030">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="33763-1030">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="33763-1031">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="33763-1031">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="33763-1032">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="33763-1032">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="33763-1033">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="33763-1033">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="33763-1034">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="33763-1034">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="33763-1035">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="33763-1035">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="33763-1036">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="33763-1036">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="33763-1037">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="33763-1037">core: Improved performance</span></span>
* <span data-ttu-id="33763-1038">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="33763-1038">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="33763-1039">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="33763-1039">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="33763-1040">ACS</span><span class="sxs-lookup"><span data-stu-id="33763-1040">ACS</span></span>

* <span data-ttu-id="33763-1041">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="33763-1041">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="33763-1042">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="33763-1042">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="33763-1043">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="33763-1043">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="33763-1044">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="33763-1044">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="33763-1045">AppService</span><span class="sxs-lookup"><span data-stu-id="33763-1045">AppService</span></span>

* <span data-ttu-id="33763-1046">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="33763-1046">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="33763-1047">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="33763-1047">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="33763-1048">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="33763-1048">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="33763-1049">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="33763-1049">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="33763-1050">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="33763-1050">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="33763-1051">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="33763-1051">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="33763-1052">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="33763-1052">support slot swap with preview</span></span>
* <span data-ttu-id="33763-1053">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="33763-1053">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="33763-1054">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="33763-1054">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="33763-1055">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="33763-1055">CosmosDB</span></span>

* <span data-ttu-id="33763-1056">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="33763-1056">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="33763-1057">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="33763-1057">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="33763-1058">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="33763-1058">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="33763-1059">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="33763-1059">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="33763-1060">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="33763-1060">Data Lake Analytics</span></span>

* <span data-ttu-id="33763-1061">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="33763-1061">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="33763-1062">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="33763-1062">Add support for new catalog item type: package.</span></span> <span data-ttu-id="33763-1063">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="33763-1063">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="33763-1064">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="33763-1064">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="33763-1065">Таблица</span><span class="sxs-lookup"><span data-stu-id="33763-1065">Table</span></span>
  * <span data-ttu-id="33763-1066">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="33763-1066">Table valued function</span></span>
  * <span data-ttu-id="33763-1067">Просмотр</span><span class="sxs-lookup"><span data-stu-id="33763-1067">View</span></span>
  * <span data-ttu-id="33763-1068">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="33763-1068">Table Statistics.</span></span> <span data-ttu-id="33763-1069">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="33763-1069">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="33763-1070">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="33763-1070">Data Lake Store</span></span>

* <span data-ttu-id="33763-1071">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="33763-1071">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="33763-1072">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="33763-1072">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="33763-1073">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="33763-1073">missed help for access show.</span></span> <span data-ttu-id="33763-1074">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="33763-1074">adding it.</span></span> <span data-ttu-id="33763-1075">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="33763-1075">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="33763-1076">Поиск</span><span class="sxs-lookup"><span data-stu-id="33763-1076">Find</span></span>

* <span data-ttu-id="33763-1077">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="33763-1077">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="33763-1078">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="33763-1078">KeyVault</span></span>

* <span data-ttu-id="33763-1079">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="33763-1079">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="33763-1080">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="33763-1080">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="33763-1081">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="33763-1081">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="33763-1082">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="33763-1082">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="33763-1083">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="33763-1083">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="33763-1084">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="33763-1084">Lab</span></span>

* <span data-ttu-id="33763-1085">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="33763-1085">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="33763-1086">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="33763-1086">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="33763-1087">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="33763-1087">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="33763-1088">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="33763-1088">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="33763-1089">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="33763-1089">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="33763-1090">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="33763-1090">Monitor</span></span>

* <span data-ttu-id="33763-1091">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="33763-1091">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="33763-1092">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="33763-1092">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="33763-1093">Сеть</span><span class="sxs-lookup"><span data-stu-id="33763-1093">Network</span></span>

* <span data-ttu-id="33763-1094">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="33763-1094">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="33763-1095">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="33763-1095">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="33763-1096">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="33763-1096">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="33763-1097">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="33763-1097">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="33763-1098">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="33763-1098">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="33763-1099">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="33763-1099">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="33763-1100">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="33763-1100">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="33763-1101">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="33763-1101">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="33763-1102">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="33763-1102">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="33763-1103">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="33763-1103">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="33763-1104">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="33763-1104">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="33763-1105">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="33763-1105">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="33763-1106">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="33763-1106">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="33763-1107">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="33763-1107">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="33763-1108">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="33763-1108">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="33763-1109">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="33763-1109">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="33763-1110">Профиль</span><span class="sxs-lookup"><span data-stu-id="33763-1110">Profile</span></span>

* <span data-ttu-id="33763-1111">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="33763-1111">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="33763-1112">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="33763-1112">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="33763-1113">Redis</span><span class="sxs-lookup"><span data-stu-id="33763-1113">Redis</span></span>

* <span data-ttu-id="33763-1114">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="33763-1114">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="33763-1115">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="33763-1115">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="33763-1116">Ресурс</span><span class="sxs-lookup"><span data-stu-id="33763-1116">Resource</span></span>

* <span data-ttu-id="33763-1117">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="33763-1117">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="33763-1118">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="33763-1118">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="33763-1119">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="33763-1119">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="33763-1120">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="33763-1120">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="33763-1121">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="33763-1121">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="33763-1122">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="33763-1122">Add docs for az lock update.</span></span> <span data-ttu-id="33763-1123">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="33763-1123">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="33763-1124">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="33763-1124">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="33763-1125">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="33763-1125">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="33763-1126">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="33763-1126">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="33763-1127">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="33763-1127">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="33763-1128">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="33763-1128">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="33763-1129">Роль</span><span class="sxs-lookup"><span data-stu-id="33763-1129">Role</span></span>

* <span data-ttu-id="33763-1130">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="33763-1130">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="33763-1131">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="33763-1131">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="33763-1132">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="33763-1132">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="33763-1133">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="33763-1133">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="33763-1134">SQL</span><span class="sxs-lookup"><span data-stu-id="33763-1134">SQL</span></span>

* <span data-ttu-id="33763-1135">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="33763-1135">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="33763-1136">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="33763-1136">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="33763-1137">Хранилище</span><span class="sxs-lookup"><span data-stu-id="33763-1137">Storage</span></span>

* <span data-ttu-id="33763-1138">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="33763-1138">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="33763-1139">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="33763-1139">Add support for incremental blob copy</span></span>
* <span data-ttu-id="33763-1140">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="33763-1140">Add support for large block blob upload</span></span>
* <span data-ttu-id="33763-1141">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="33763-1141">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="33763-1142">ВМ</span><span class="sxs-lookup"><span data-stu-id="33763-1142">VM</span></span>

* <span data-ttu-id="33763-1143">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="33763-1143">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="33763-1144">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="33763-1144">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="33763-1145">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="33763-1145">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="33763-1146">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="33763-1146">az vm/vmss disk</span></span>
  3. <span data-ttu-id="33763-1147">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="33763-1147">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="33763-1148">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="33763-1148">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="33763-1149">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="33763-1149">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="33763-1150">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="33763-1150">April 3, 2017</span></span>

<span data-ttu-id="33763-1151">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="33763-1151">Version 2.0.2</span></span>

<span data-ttu-id="33763-1152">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="33763-1152">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="33763-1153">Core</span><span class="sxs-lookup"><span data-stu-id="33763-1153">Core</span></span>

* <span data-ttu-id="33763-1154">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="33763-1154">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="33763-1155">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="33763-1155">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="33763-1156">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="33763-1156">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="33763-1157">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="33763-1157">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="33763-1158">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="33763-1158">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="33763-1159">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="33763-1159">Add prompting for missing template parameters.</span></span> <span data-ttu-id="33763-1160">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="33763-1160">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="33763-1161">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="33763-1161">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="33763-1162">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="33763-1162">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="33763-1163">ACS</span><span class="sxs-lookup"><span data-stu-id="33763-1163">ACS</span></span>

* <span data-ttu-id="33763-1164">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="33763-1164">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="33763-1165">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="33763-1165">Add support for ssh key password prompting.</span></span> <span data-ttu-id="33763-1166">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="33763-1166">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="33763-1167">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="33763-1167">Add support for windows clusters.</span></span> <span data-ttu-id="33763-1168">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="33763-1168">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="33763-1169">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="33763-1169">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="33763-1170">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="33763-1170">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="33763-1171">AppService</span><span class="sxs-lookup"><span data-stu-id="33763-1171">AppService</span></span>

* <span data-ttu-id="33763-1172">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="33763-1172">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="33763-1173">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="33763-1173">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="33763-1174">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="33763-1174">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="33763-1175">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="33763-1175">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="33763-1176">Data Lake</span><span class="sxs-lookup"><span data-stu-id="33763-1176">DataLake</span></span>

* <span data-ttu-id="33763-1177">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="33763-1177">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="33763-1178">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="33763-1178">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="33763-1179">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="33763-1179">DocuemntDB</span></span>

* <span data-ttu-id="33763-1180">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="33763-1180">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="33763-1181">ВМ</span><span class="sxs-lookup"><span data-stu-id="33763-1181">VM</span></span>

* <span data-ttu-id="33763-1182">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="33763-1182">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="33763-1183">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="33763-1183">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="33763-1184">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="33763-1184">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="33763-1185">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="33763-1185">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="33763-1186">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="33763-1186">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="33763-1187">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="33763-1187">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="33763-1188">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="33763-1188">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="33763-1189">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="33763-1189">February 27, 2017</span></span>

<span data-ttu-id="33763-1190">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="33763-1190">Version 2.0.0</span></span>

<span data-ttu-id="33763-1191">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="33763-1191">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="33763-1192">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="33763-1192">Container Service (acs)</span></span>
- <span data-ttu-id="33763-1193">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="33763-1193">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="33763-1194">Сеть</span><span class="sxs-lookup"><span data-stu-id="33763-1194">Networking</span></span>
- <span data-ttu-id="33763-1195">Хранилище</span><span class="sxs-lookup"><span data-stu-id="33763-1195">Storage</span></span>

<span data-ttu-id="33763-1196">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="33763-1196">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="33763-1197">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="33763-1197">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="33763-1198">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="33763-1198">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="33763-1199">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="33763-1199">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="33763-1200">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="33763-1200">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="33763-1201">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="33763-1201">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="33763-1202">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="33763-1202">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="33763-1203">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="33763-1203">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="33763-1204">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="33763-1204">Provide feedback from the command line with the `az feedback` command</span></span>

