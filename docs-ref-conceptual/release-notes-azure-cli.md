---
title: Заметки о выпуске Azure CLI 2.0
description: Узнайте о последних обновлениях в Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 08/28/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 5d179a49ad64201270be7848a72535b871081125
ms.sourcegitcommit: c90bc90c9a2b3adf2836d7cfb84951cd3ab51317
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/06/2018
ms.locfileid: "43828751"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="a5b98-103">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="a5b98-103">Azure CLI 2.0 release notes</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="a5b98-104">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-104">August 28, 2018</span></span>

<span data-ttu-id="a5b98-105">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="a5b98-105">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="a5b98-106">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-106">Core</span></span>

* <span data-ttu-id="a5b98-107">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="a5b98-107">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="a5b98-108">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="a5b98-108">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="a5b98-109">ACR</span><span class="sxs-lookup"><span data-stu-id="a5b98-109">ACR</span></span>

* <span data-ttu-id="a5b98-110">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="a5b98-110">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="a5b98-111">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-111">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-112">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-112">ACS</span></span>

* <span data-ttu-id="a5b98-113">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-113">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="a5b98-114">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="a5b98-114">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-115">AppService</span><span class="sxs-lookup"><span data-stu-id="a5b98-115">AppService</span></span>

* <span data-ttu-id="a5b98-116">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="a5b98-116">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="a5b98-117">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="a5b98-117">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="a5b98-118">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="a5b98-118">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="a5b98-119">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="a5b98-119">Backup</span></span>

* <span data-ttu-id="a5b98-120">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="a5b98-120">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="a5b98-121">Служба Bot Service</span><span class="sxs-lookup"><span data-stu-id="a5b98-121">Bot Service</span></span>

* <span data-ttu-id="a5b98-122">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="a5b98-122">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a5b98-123">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a5b98-123">Cognitive Services</span></span>

* <span data-ttu-id="a5b98-124">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="a5b98-124">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="a5b98-125">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a5b98-125">IoT</span></span>

* <span data-ttu-id="a5b98-126">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="a5b98-126">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="a5b98-127">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a5b98-127">Monitor</span></span>

* <span data-ttu-id="a5b98-128">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="a5b98-128">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="a5b98-129">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="a5b98-129">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-130">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-130">Network</span></span>

* <span data-ttu-id="a5b98-131">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="a5b98-131">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="a5b98-132">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a5b98-132">Resource</span></span>

* <span data-ttu-id="a5b98-133">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="a5b98-133">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-134">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-134">Storage</span></span>

* <span data-ttu-id="a5b98-135">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="a5b98-135">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-136">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-136">VM</span></span>

* <span data-ttu-id="a5b98-137">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="a5b98-137">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="a5b98-138">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-138">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="a5b98-139">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-139">Auguest 14, 2018</span></span>

<span data-ttu-id="a5b98-140">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="a5b98-140">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="a5b98-141">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-141">Core</span></span>

* <span data-ttu-id="a5b98-142">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-142">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="a5b98-143">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="a5b98-143">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="a5b98-144">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="a5b98-144">Telemetry</span></span>

* <span data-ttu-id="a5b98-145">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="a5b98-145">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="a5b98-146">ACR</span><span class="sxs-lookup"><span data-stu-id="a5b98-146">ACR</span></span>

* <span data-ttu-id="a5b98-147">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-147">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="a5b98-148">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-148">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-149">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-149">ACS</span></span>

* <span data-ttu-id="a5b98-150">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="a5b98-150">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="a5b98-151">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="a5b98-151">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="a5b98-152">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="a5b98-152">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="a5b98-153">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="a5b98-153">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="a5b98-154">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="a5b98-154">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="a5b98-155">AppService</span><span class="sxs-lookup"><span data-stu-id="a5b98-155">AppService</span></span>

* <span data-ttu-id="a5b98-156">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-156">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="a5b98-157">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="a5b98-157">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="a5b98-158">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a5b98-158">BatchAI</span></span>

* <span data-ttu-id="a5b98-159">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="a5b98-159">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="a5b98-160">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a5b98-160">Container</span></span>

* <span data-ttu-id="a5b98-161">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="a5b98-161">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="a5b98-162">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a5b98-162">IoT</span></span>

* <span data-ttu-id="a5b98-163">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="a5b98-163">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="a5b98-164">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-164">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="a5b98-165">IoT Central</span><span class="sxs-lookup"><span data-stu-id="a5b98-165">Iot Central</span></span>

* <span data-ttu-id="a5b98-166">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="a5b98-166">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="a5b98-167">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a5b98-167">KeyVault</span></span>


* <span data-ttu-id="a5b98-168">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="a5b98-168">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="a5b98-169">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="a5b98-169">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="a5b98-170">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="a5b98-170">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="a5b98-171">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="a5b98-171">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="a5b98-172">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="a5b98-172">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="a5b98-173">Передача</span><span class="sxs-lookup"><span data-stu-id="a5b98-173">Relay</span></span>

* <span data-ttu-id="a5b98-174">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a5b98-174">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="a5b98-175">SQL</span><span class="sxs-lookup"><span data-stu-id="a5b98-175">Sql</span></span>

* <span data-ttu-id="a5b98-176">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-176">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-177">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-177">Storage</span></span>

* <span data-ttu-id="a5b98-178">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="a5b98-178">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="a5b98-179">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="a5b98-179">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="a5b98-180">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="a5b98-180">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="a5b98-181">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="a5b98-181">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="a5b98-182">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="a5b98-182">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-183">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-183">VM</span></span>

* <span data-ttu-id="a5b98-184">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="a5b98-184">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="a5b98-185">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-185">July 31, 2018</span></span>

<span data-ttu-id="a5b98-186">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="a5b98-186">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="a5b98-187">ACR</span><span class="sxs-lookup"><span data-stu-id="a5b98-187">ACR</span></span>

* <span data-ttu-id="a5b98-188">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-188">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="a5b98-189">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-189">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-190">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-190">ACS</span></span>

* <span data-ttu-id="a5b98-191">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="a5b98-191">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="a5b98-192">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a5b98-192">Batch</span></span>

* <span data-ttu-id="a5b98-193">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="a5b98-193">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="a5b98-194">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a5b98-194">Container</span></span>

* <span data-ttu-id="a5b98-195">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="a5b98-195">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-196">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-196">Network</span></span>

* <span data-ttu-id="a5b98-197">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="a5b98-197">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="a5b98-198">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a5b98-198">Resource</span></span>

* <span data-ttu-id="a5b98-199">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="a5b98-199">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="a5b98-200">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="a5b98-200">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="a5b98-201">Роль</span><span class="sxs-lookup"><span data-stu-id="a5b98-201">Role</span></span>

* <span data-ttu-id="a5b98-202">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="a5b98-202">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="a5b98-203">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="a5b98-203">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="a5b98-204">поиска</span><span class="sxs-lookup"><span data-stu-id="a5b98-204">Search</span></span>

* <span data-ttu-id="a5b98-205">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="a5b98-205">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="a5b98-206">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="a5b98-206">Service Bus</span></span>

* <span data-ttu-id="a5b98-207">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="a5b98-207">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="a5b98-208">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="a5b98-208">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="a5b98-209">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="a5b98-209">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="a5b98-210">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-210">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-211">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-211">Storage</span></span>

* <span data-ttu-id="a5b98-212">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="a5b98-212">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="a5b98-213">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="a5b98-213">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-214">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-214">VM</span></span>

* <span data-ttu-id="a5b98-215">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="a5b98-215">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="a5b98-216">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-216">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="a5b98-217">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="a5b98-217">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="a5b98-218">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]. Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="a5b98-218">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="a5b98-219">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-219">July 18, 2018</span></span>

<span data-ttu-id="a5b98-220">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="a5b98-220">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="a5b98-221">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-221">Core</span></span>

* <span data-ttu-id="a5b98-222">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="a5b98-222">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="a5b98-223">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="a5b98-223">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="a5b98-224">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]. Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="a5b98-224">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="a5b98-225">ACR</span><span class="sxs-lookup"><span data-stu-id="a5b98-225">ACR</span></span>

* <span data-ttu-id="a5b98-226">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]. Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="a5b98-226">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="a5b98-227">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-227">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="a5b98-228">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="a5b98-228">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="a5b98-229">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="a5b98-229">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-230">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-230">ACS</span></span>

* <span data-ttu-id="a5b98-231">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="a5b98-231">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-232">AppService</span><span class="sxs-lookup"><span data-stu-id="a5b98-232">AppService</span></span>

* <span data-ttu-id="a5b98-233">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="a5b98-233">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="a5b98-234">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a5b98-234">Batch</span></span>

* <span data-ttu-id="a5b98-235">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="a5b98-235">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="a5b98-236">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="a5b98-236">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a5b98-237">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="a5b98-237">Batch AI</span></span>

* <span data-ttu-id="a5b98-238">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-238">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="a5b98-239">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a5b98-239">Container</span></span>

* <span data-ttu-id="a5b98-240">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="a5b98-240">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="a5b98-241">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="a5b98-241">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-242">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-242">Network</span></span>

* <span data-ttu-id="a5b98-243">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-243">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="a5b98-244">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-244">Added `network nic wait`</span></span>
* <span data-ttu-id="a5b98-245">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="a5b98-245">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="a5b98-246">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="a5b98-246">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="a5b98-247">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a5b98-247">Resource</span></span>

* <span data-ttu-id="a5b98-248">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-248">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="a5b98-249">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-249">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="a5b98-250">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-250">Added `deployment wait` command</span></span>
* <span data-ttu-id="a5b98-251">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="a5b98-251">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="a5b98-252">SQL</span><span class="sxs-lookup"><span data-stu-id="a5b98-252">SQL</span></span>

* <span data-ttu-id="a5b98-253">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-253">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="a5b98-254">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-254">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="a5b98-255">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-255">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-256">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-256">Storage</span></span>

* <span data-ttu-id="a5b98-257">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-257">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-258">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-258">VM</span></span>

* <span data-ttu-id="a5b98-259">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]. По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a5b98-259">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="a5b98-260">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-260">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="a5b98-261">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-261">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="a5b98-262">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-262">July 3, 2018</span></span>

<span data-ttu-id="a5b98-263">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="a5b98-263">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="a5b98-264">AKS</span><span class="sxs-lookup"><span data-stu-id="a5b98-264">AKS</span></span>

* <span data-ttu-id="a5b98-265">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="a5b98-265">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="a5b98-266">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-266">July 3, 2018</span></span>

<span data-ttu-id="a5b98-267">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="a5b98-267">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="a5b98-268">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-268">Core</span></span>

* <span data-ttu-id="a5b98-269">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="a5b98-269">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="a5b98-270">ACR</span><span class="sxs-lookup"><span data-stu-id="a5b98-270">ACR</span></span>

* <span data-ttu-id="a5b98-271">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="a5b98-271">Added polling build status</span></span>
* <span data-ttu-id="a5b98-272">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="a5b98-272">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="a5b98-273">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-273">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-274">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-274">ACS</span></span>

* <span data-ttu-id="a5b98-275">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a5b98-275">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="a5b98-276">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a5b98-276">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="a5b98-277">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-277">Updated options for `aks browse` command.</span></span> <span data-ttu-id="a5b98-278">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-278">Added `--listen-port` support</span></span>
* <span data-ttu-id="a5b98-279">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-279">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="a5b98-280">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="a5b98-280">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="a5b98-281">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-281">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-282">AppService</span><span class="sxs-lookup"><span data-stu-id="a5b98-282">AppService</span></span>

* <span data-ttu-id="a5b98-283">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-283">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="a5b98-284">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="a5b98-284">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="a5b98-285">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="a5b98-285">Backup</span></span>

* <span data-ttu-id="a5b98-286">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="a5b98-286">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="a5b98-287">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a5b98-287">BatchAI</span></span>

* <span data-ttu-id="a5b98-288">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-288">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="a5b98-289">Облако</span><span class="sxs-lookup"><span data-stu-id="a5b98-289">Cloud</span></span>

* <span data-ttu-id="a5b98-290">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-290">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="a5b98-291">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a5b98-291">Container</span></span>

* <span data-ttu-id="a5b98-292">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="a5b98-292">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="a5b98-293">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-293">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="a5b98-294">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="a5b98-294">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="a5b98-295">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a5b98-295">Extension</span></span>

* <span data-ttu-id="a5b98-296">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="a5b98-296">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-297">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-297">Network</span></span>

* <span data-ttu-id="a5b98-298">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-298">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="a5b98-299">Rdbms</span><span class="sxs-lookup"><span data-stu-id="a5b98-299">Rdbms</span></span>

* <span data-ttu-id="a5b98-300">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-300">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="a5b98-301">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a5b98-301">Resource</span></span>

* <span data-ttu-id="a5b98-302">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-302">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-303">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-303">VM</span></span>

* <span data-ttu-id="a5b98-304">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="a5b98-304">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="a5b98-305">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-305">June 25, 2018</span></span>

<span data-ttu-id="a5b98-306">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="a5b98-306">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="a5b98-307">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="a5b98-307">CLI</span></span>

* <span data-ttu-id="a5b98-308">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="a5b98-308">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="a5b98-309">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-309">June 19, 2018</span></span>

<span data-ttu-id="a5b98-310">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="a5b98-310">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="a5b98-311">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-311">Core</span></span>

* <span data-ttu-id="a5b98-312">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="a5b98-312">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="a5b98-313">ACR</span><span class="sxs-lookup"><span data-stu-id="a5b98-313">ACR</span></span>

* <span data-ttu-id="a5b98-314">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-314">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="a5b98-315">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="a5b98-315">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-316">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-316">ACS</span></span>

* <span data-ttu-id="a5b98-317">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-317">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="a5b98-318">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-318">Added `--update` support</span></span>
* <span data-ttu-id="a5b98-319">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-319">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="a5b98-320">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-320">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="a5b98-321">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-321">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="a5b98-322">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-322">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="a5b98-323">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-323">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="a5b98-324">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-324">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-325">AppService</span><span class="sxs-lookup"><span data-stu-id="a5b98-325">AppService</span></span>

* <span data-ttu-id="a5b98-326">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="a5b98-326">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="a5b98-327">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-327">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="a5b98-328">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a5b98-328">Batch</span></span>

* <span data-ttu-id="a5b98-329">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-329">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a5b98-330">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="a5b98-330">Batch AI</span></span>

* <span data-ttu-id="a5b98-331">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="a5b98-331">Added support for workspaces.</span></span> <span data-ttu-id="a5b98-332">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-332">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="a5b98-333">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-333">Added support for experiments.</span></span> <span data-ttu-id="a5b98-334">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="a5b98-334">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="a5b98-335">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="a5b98-335">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="a5b98-336">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-336">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="a5b98-337">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-337">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="a5b98-338">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-338">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="a5b98-339">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="a5b98-339">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="a5b98-340">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-340">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="a5b98-341">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-341">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="a5b98-342">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-342">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="a5b98-343">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-343">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="a5b98-344">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-344">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="a5b98-345">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-345">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="a5b98-346">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="a5b98-346">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="a5b98-347">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-347">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="a5b98-348">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="a5b98-348">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="a5b98-349">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="a5b98-349">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="a5b98-350">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="a5b98-350">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="a5b98-351">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="a5b98-351">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="a5b98-352">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="a5b98-352">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="a5b98-353">Карты</span><span class="sxs-lookup"><span data-stu-id="a5b98-353">Maps</span></span>

* <span data-ttu-id="a5b98-354">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-354">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-355">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-355">Network</span></span>

* <span data-ttu-id="a5b98-356">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="a5b98-356">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="a5b98-357">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="a5b98-357">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="a5b98-358">#6502</span><span class="sxs-lookup"><span data-stu-id="a5b98-358">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="a5b98-359">Резервирование</span><span class="sxs-lookup"><span data-stu-id="a5b98-359">Reservations</span></span>

* <span data-ttu-id="a5b98-360">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-360">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="a5b98-361">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-361">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="a5b98-362">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-362">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="a5b98-363">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-363">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="a5b98-364">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-364">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="a5b98-365">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-365">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="a5b98-366">Роль</span><span class="sxs-lookup"><span data-stu-id="a5b98-366">Role</span></span>

* <span data-ttu-id="a5b98-367">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="a5b98-367">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="a5b98-368">SQL</span><span class="sxs-lookup"><span data-stu-id="a5b98-368">SQL</span></span>

* <span data-ttu-id="a5b98-369">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="a5b98-369">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-370">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-370">Storage</span></span>

* <span data-ttu-id="a5b98-371">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="a5b98-371">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-372">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-372">VM</span></span>

* <span data-ttu-id="a5b98-373">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-373">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="a5b98-374">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-374">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="a5b98-375">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="a5b98-375">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="a5b98-376">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-376">June 13, 2018</span></span>

<span data-ttu-id="a5b98-377">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="a5b98-377">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="a5b98-378">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-378">Core</span></span>

* <span data-ttu-id="a5b98-379">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="a5b98-379">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="a5b98-380">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-380">June 13, 2018</span></span>

<span data-ttu-id="a5b98-381">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="a5b98-381">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="a5b98-382">AKS</span><span class="sxs-lookup"><span data-stu-id="a5b98-382">AKS</span></span>

* <span data-ttu-id="a5b98-383">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="a5b98-383">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="a5b98-384">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="a5b98-384">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="a5b98-385">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="a5b98-385">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="a5b98-386">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="a5b98-386">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="a5b98-387">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a5b98-387">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-388">AppService</span><span class="sxs-lookup"><span data-stu-id="a5b98-388">AppService</span></span>

* <span data-ttu-id="a5b98-389">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="a5b98-389">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="a5b98-390">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-390">June 5, 2018</span></span>

<span data-ttu-id="a5b98-391">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="a5b98-391">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="a5b98-392">Interactive</span><span class="sxs-lookup"><span data-stu-id="a5b98-392">Interactive</span></span>

* <span data-ttu-id="a5b98-393">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="a5b98-393">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="a5b98-394">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-394">June 5, 2018</span></span>

<span data-ttu-id="a5b98-395">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="a5b98-395">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="a5b98-396">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-396">Core</span></span>

* <span data-ttu-id="a5b98-397">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="a5b98-397">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="a5b98-398">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="a5b98-398">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="a5b98-399">ACR</span><span class="sxs-lookup"><span data-stu-id="a5b98-399">ACR</span></span>

* <span data-ttu-id="a5b98-400">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="a5b98-400">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="a5b98-401">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-401">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="a5b98-402">AKS</span><span class="sxs-lookup"><span data-stu-id="a5b98-402">AKS</span></span>

* <span data-ttu-id="a5b98-403">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="a5b98-403">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="a5b98-404">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a5b98-404">Batch</span></span>

* <span data-ttu-id="a5b98-405">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="a5b98-405">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="a5b98-406">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a5b98-406">IOT</span></span>

* <span data-ttu-id="a5b98-407">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="a5b98-407">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-408">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-408">Network</span></span>

* <span data-ttu-id="a5b98-409">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-409">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="a5b98-410">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="a5b98-410">Policy Insights</span></span>

* <span data-ttu-id="a5b98-411">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a5b98-411">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="a5b98-412">ARM</span><span class="sxs-lookup"><span data-stu-id="a5b98-412">ARM</span></span>

* <span data-ttu-id="a5b98-413">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-413">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="a5b98-414">SQL</span><span class="sxs-lookup"><span data-stu-id="a5b98-414">SQL</span></span>

* <span data-ttu-id="a5b98-415">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="a5b98-415">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="a5b98-416">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="a5b98-416">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="a5b98-417">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-417">Storage</span></span>

* <span data-ttu-id="a5b98-418">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-418">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-419">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-419">VM</span></span>

* <span data-ttu-id="a5b98-420">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-420">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="a5b98-421">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-421">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="a5b98-422">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-422">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="a5b98-423">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-423">May 22, 2018</span></span>

<span data-ttu-id="a5b98-424">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="a5b98-424">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="a5b98-425">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-425">Core</span></span>

* <span data-ttu-id="a5b98-426">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-426">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-427">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-427">ACS</span></span>

* <span data-ttu-id="a5b98-428">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-428">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="a5b98-429">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="a5b98-429">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-430">AppService</span><span class="sxs-lookup"><span data-stu-id="a5b98-430">AppService</span></span>

* <span data-ttu-id="a5b98-431">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="a5b98-431">Improved generic update commands</span></span>
* <span data-ttu-id="a5b98-432">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-432">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="a5b98-433">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a5b98-433">Container</span></span>

* <span data-ttu-id="a5b98-434">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="a5b98-434">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="a5b98-435">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a5b98-435">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="a5b98-436">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a5b98-436">Extension</span></span>

* <span data-ttu-id="a5b98-437">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="a5b98-437">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="a5b98-438">Interactive</span><span class="sxs-lookup"><span data-stu-id="a5b98-438">Interactive</span></span>

* <span data-ttu-id="a5b98-439">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="a5b98-439">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="a5b98-440">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="a5b98-440">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="a5b98-441">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a5b98-441">KeyVault</span></span>

* <span data-ttu-id="a5b98-442">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="a5b98-442">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-443">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-443">Network</span></span>

* <span data-ttu-id="a5b98-444">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="a5b98-444">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="a5b98-445">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="a5b98-445">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="a5b98-446">SQL</span><span class="sxs-lookup"><span data-stu-id="a5b98-446">SQL</span></span>

* <span data-ttu-id="a5b98-447">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="a5b98-447">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="a5b98-448">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-448">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="a5b98-449">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-449">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="a5b98-450">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="a5b98-450">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="a5b98-451">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="a5b98-451">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="a5b98-452">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-452">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="a5b98-453">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-453">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="a5b98-454">`edition`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-454">`edition`.</span></span> <span data-ttu-id="a5b98-455">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-455">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="a5b98-456">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-456">`elasticPoolName`.</span></span> <span data-ttu-id="a5b98-457">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-457">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="a5b98-458">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="a5b98-458">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="a5b98-459">`edition`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-459">`edition`.</span></span> <span data-ttu-id="a5b98-460">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-460">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="a5b98-461">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-461">`dtu`.</span></span> <span data-ttu-id="a5b98-462">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-462">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="a5b98-463">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-463">`databaseDtuMin`.</span></span> <span data-ttu-id="a5b98-464">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-464">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="a5b98-465">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-465">`databaseDtuMax`.</span></span> <span data-ttu-id="a5b98-466">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-466">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="a5b98-467">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-467">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="a5b98-468">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-468">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-469">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-469">Storage</span></span>

* <span data-ttu-id="a5b98-470">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-470">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="a5b98-471">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-471">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-472">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-472">VM</span></span>

* <span data-ttu-id="a5b98-473">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-473">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="a5b98-474">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-474">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="a5b98-475">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-475">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="a5b98-476">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="a5b98-476">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="a5b98-477">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-477">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="a5b98-478">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-478">May 7, 2018</span></span>

<span data-ttu-id="a5b98-479">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="a5b98-479">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="a5b98-480">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-480">Core</span></span>

* <span data-ttu-id="a5b98-481">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="a5b98-481">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="a5b98-482">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-482">Added limited support for positional arguments</span></span>
* <span data-ttu-id="a5b98-483">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-483">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="a5b98-484">#5591</span><span class="sxs-lookup"><span data-stu-id="a5b98-484">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="a5b98-485">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-485">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="a5b98-486">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="a5b98-486">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="a5b98-487">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="a5b98-487">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="a5b98-488">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-488">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="a5b98-489">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="a5b98-489">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="a5b98-490">ACR</span><span class="sxs-lookup"><span data-stu-id="a5b98-490">ACR</span></span>

* <span data-ttu-id="a5b98-491">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="a5b98-491">Added ACR Build commands</span></span>
* <span data-ttu-id="a5b98-492">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="a5b98-492">Improved resource not found error messages</span></span>
* <span data-ttu-id="a5b98-493">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="a5b98-493">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="a5b98-494">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="a5b98-494">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="a5b98-495">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="a5b98-495">Improved repository commands error messages</span></span>
* <span data-ttu-id="a5b98-496">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="a5b98-496">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-497">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-497">ACS</span></span>

* <span data-ttu-id="a5b98-498">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="a5b98-498">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="a5b98-499">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="a5b98-499">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="a5b98-500">AMS</span><span class="sxs-lookup"><span data-stu-id="a5b98-500">AMS</span></span>

* <span data-ttu-id="a5b98-501">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="a5b98-501">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-502">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a5b98-502">Appservice</span></span>

* <span data-ttu-id="a5b98-503">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="a5b98-503">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="a5b98-504">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-504">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="a5b98-505">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="a5b98-505">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="a5b98-506">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a5b98-506">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a5b98-507">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="a5b98-507">Batch AI</span></span>

* <span data-ttu-id="a5b98-508">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="a5b98-508">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a5b98-509">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a5b98-509">Cognitive Services</span></span>

* <span data-ttu-id="a5b98-510">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="a5b98-510">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="a5b98-511">Потребление</span><span class="sxs-lookup"><span data-stu-id="a5b98-511">Consumption</span></span>

* <span data-ttu-id="a5b98-512">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="a5b98-512">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="a5b98-513">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a5b98-513">Container</span></span>

* <span data-ttu-id="a5b98-514">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="a5b98-514">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="a5b98-515">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="a5b98-515">Cosmos DB</span></span>

* <span data-ttu-id="a5b98-516">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a5b98-516">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="a5b98-517">DMS</span><span class="sxs-lookup"><span data-stu-id="a5b98-517">DMS</span></span>

* <span data-ttu-id="a5b98-518">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="a5b98-518">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="a5b98-519">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a5b98-519">Extension</span></span>

* <span data-ttu-id="a5b98-520">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="a5b98-520">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="a5b98-521">Interactive</span><span class="sxs-lookup"><span data-stu-id="a5b98-521">Interactive</span></span>

* <span data-ttu-id="a5b98-522">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="a5b98-522">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="a5b98-523">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="a5b98-523">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="a5b98-524">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="a5b98-524">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="a5b98-525">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="a5b98-525">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="a5b98-526">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="a5b98-526">Lab</span></span>

* <span data-ttu-id="a5b98-527">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="a5b98-527">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-528">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-528">Network</span></span>

* <span data-ttu-id="a5b98-529">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="a5b98-529">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="a5b98-530">Профиль</span><span class="sxs-lookup"><span data-stu-id="a5b98-530">Profile</span></span>

* <span data-ttu-id="a5b98-531">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-531">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="a5b98-532">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="a5b98-532">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="a5b98-533">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-533">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="a5b98-534">Redis</span><span class="sxs-lookup"><span data-stu-id="a5b98-534">Redis</span></span>

* <span data-ttu-id="a5b98-535">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-535">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="a5b98-536">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="a5b98-536">Deprecated `redis list-all`.</span></span> <span data-ttu-id="a5b98-537">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-537">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="a5b98-538">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-538">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="a5b98-539">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="a5b98-539">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="a5b98-540">Роль</span><span class="sxs-lookup"><span data-stu-id="a5b98-540">Role</span></span>

* <span data-ttu-id="a5b98-541">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="a5b98-541">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-542">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-542">Storage</span></span>

* <span data-ttu-id="a5b98-543">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="a5b98-543">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="a5b98-544">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="a5b98-544">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="a5b98-545">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="a5b98-545">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="a5b98-546">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="a5b98-546">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="a5b98-547">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="a5b98-547">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-548">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-548">VM</span></span>

* <span data-ttu-id="a5b98-549">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="a5b98-549">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="a5b98-550">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="a5b98-550">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="a5b98-551">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]. Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="a5b98-551">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="a5b98-552">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-552">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="a5b98-553">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="a5b98-553">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="a5b98-554">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="a5b98-554">Added write accelerator support</span></span>
* <span data-ttu-id="a5b98-555">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-555">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="a5b98-556">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="a5b98-556">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="a5b98-557">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="a5b98-557">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="a5b98-558">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-558">April 10, 2018</span></span>

<span data-ttu-id="a5b98-559">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="a5b98-559">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="a5b98-560">ACR</span><span class="sxs-lookup"><span data-stu-id="a5b98-560">ACR</span></span>

* <span data-ttu-id="a5b98-561">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="a5b98-561">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-562">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-562">ACS</span></span>

* <span data-ttu-id="a5b98-563">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="a5b98-563">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-564">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a5b98-564">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="a5b98-566">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="a5b98-566">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="a5b98-567">Batch AI</span><span class="sxs-lookup"><span data-stu-id="a5b98-567">BatchAI</span></span>

* <span data-ttu-id="a5b98-568">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="a5b98-568">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="a5b98-569">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="a5b98-569">Job level mounting</span></span>
 - <span data-ttu-id="a5b98-570">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-570">Environment variables with secret values</span></span>
 - <span data-ttu-id="a5b98-571">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="a5b98-571">Performance counters settings</span></span>
 - <span data-ttu-id="a5b98-572">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="a5b98-572">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="a5b98-573">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-573">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="a5b98-574">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="a5b98-574">Usage and limits reporting</span></span>
 - <span data-ttu-id="a5b98-575">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-575">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="a5b98-576">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-576">Support for custom images</span></span>
 - <span data-ttu-id="a5b98-577">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="a5b98-577">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="a5b98-578">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="a5b98-578">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="a5b98-579">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-579">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="a5b98-580">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="a5b98-580">National clouds are supported</span></span>
* <span data-ttu-id="a5b98-581">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="a5b98-581">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="a5b98-582">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="a5b98-582">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="a5b98-583">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="a5b98-583">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="a5b98-584">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="a5b98-584">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="a5b98-585">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="a5b98-585">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="a5b98-586">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="a5b98-586">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="a5b98-587">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-587">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="a5b98-588">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="a5b98-588">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="a5b98-589">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="a5b98-589">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="a5b98-590">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-590">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="a5b98-591">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="a5b98-591">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="a5b98-592">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-592">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="a5b98-593">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-593">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="a5b98-594">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="a5b98-594">Billing</span></span>

* <span data-ttu-id="a5b98-595">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="a5b98-595">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="a5b98-596">Потребление</span><span class="sxs-lookup"><span data-stu-id="a5b98-596">Consumption</span></span>

* <span data-ttu-id="a5b98-597">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-597">Added `marketplace` commands</span></span>
* <span data-ttu-id="a5b98-598">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-598">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="a5b98-599">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-599">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="a5b98-600">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-600">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="a5b98-601">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-601">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="a5b98-602">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-602">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="a5b98-603">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a5b98-603">Container</span></span>

* <span data-ttu-id="a5b98-604">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-604">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="a5b98-605">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="a5b98-605">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="a5b98-606">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a5b98-606">Extension</span></span>

* <span data-ttu-id="a5b98-607">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="a5b98-607">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="a5b98-608">Interactive</span><span class="sxs-lookup"><span data-stu-id="a5b98-608">Interactive</span></span>

* <span data-ttu-id="a5b98-609">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="a5b98-609">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="a5b98-610">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="a5b98-610">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="a5b98-611">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-611">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-612">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-612">Network</span></span>

* <span data-ttu-id="a5b98-613">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-613">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="a5b98-614">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-614">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="a5b98-615">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="a5b98-615">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="a5b98-616">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="a5b98-616">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="a5b98-617">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="a5b98-617">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="a5b98-618">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-618">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="a5b98-619">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-619">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="a5b98-620">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="a5b98-620">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="a5b98-621">Профиль</span><span class="sxs-lookup"><span data-stu-id="a5b98-621">Profile</span></span>

* <span data-ttu-id="a5b98-622">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-622">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="a5b98-623">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-623">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="a5b98-624">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="a5b98-624">RDBMS</span></span>

* <span data-ttu-id="a5b98-625">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-625">Added `georestore` command</span></span>
* <span data-ttu-id="a5b98-626">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-626">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="a5b98-627">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a5b98-627">Resource</span></span>

* <span data-ttu-id="a5b98-628">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-628">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="a5b98-629">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-629">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="a5b98-630">SQL</span><span class="sxs-lookup"><span data-stu-id="a5b98-630">SQL</span></span>

* <span data-ttu-id="a5b98-631">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-631">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-632">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-632">Storage</span></span>

* <span data-ttu-id="a5b98-633">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="a5b98-633">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-634">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-634">VM</span></span>

* <span data-ttu-id="a5b98-635">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="a5b98-635">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="a5b98-636">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="a5b98-636">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="a5b98-638">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-638">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="a5b98-639">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-639">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="a5b98-640">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="a5b98-640">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="a5b98-641">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="a5b98-641">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="a5b98-642">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-642">March 27, 2018</span></span>

<span data-ttu-id="a5b98-643">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="a5b98-643">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="a5b98-644">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-644">Core</span></span>

* <span data-ttu-id="a5b98-645">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="a5b98-645">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-646">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-646">ACS</span></span>

* <span data-ttu-id="a5b98-647">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="a5b98-647">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-648">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a5b98-648">Appservice</span></span>

* <span data-ttu-id="a5b98-649">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-649">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="a5b98-650">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-650">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="a5b98-651">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="a5b98-651">Backup</span></span>

* <span data-ttu-id="a5b98-652">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-652">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="a5b98-653">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="a5b98-653">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="a5b98-654">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="a5b98-654">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="a5b98-655">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-655">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="a5b98-656">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a5b98-656">Container</span></span>

* <span data-ttu-id="a5b98-657">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-657">Added `container exec` command.</span></span> <span data-ttu-id="a5b98-658">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a5b98-658">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="a5b98-659">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a5b98-659">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="a5b98-660">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a5b98-660">Extension</span></span>

* <span data-ttu-id="a5b98-661">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="a5b98-661">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="a5b98-662">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-662">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="a5b98-663">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a5b98-663">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="a5b98-664">Interactive</span><span class="sxs-lookup"><span data-stu-id="a5b98-664">Interactive</span></span>

* <span data-ttu-id="a5b98-665">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="a5b98-665">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="a5b98-666">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-666">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="a5b98-667">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="a5b98-667">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="a5b98-668">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="a5b98-668">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="a5b98-669">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="a5b98-669">Lab</span></span>

* <span data-ttu-id="a5b98-670">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-670">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="a5b98-671">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a5b98-671">Monitor</span></span>

* <span data-ttu-id="a5b98-672">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="a5b98-672">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="a5b98-673">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="a5b98-673">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="a5b98-674">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="a5b98-674">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-675">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-675">Network</span></span>

* <span data-ttu-id="a5b98-676">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="a5b98-676">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="a5b98-677">Профиль</span><span class="sxs-lookup"><span data-stu-id="a5b98-677">Profile</span></span>

* <span data-ttu-id="a5b98-678">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-678">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="a5b98-679">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="a5b98-679">RDBMS</span></span>

* <span data-ttu-id="a5b98-680">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="a5b98-680">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="a5b98-681">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a5b98-681">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="a5b98-683">Роль</span><span class="sxs-lookup"><span data-stu-id="a5b98-683">Role</span></span>

* <span data-ttu-id="a5b98-684">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-684">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="a5b98-685">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="a5b98-685">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="a5b98-686">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="a5b98-686">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="a5b98-687">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-687">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="a5b98-688">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-688">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-689">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-689">Storage</span></span>

* <span data-ttu-id="a5b98-690">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="a5b98-690">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="a5b98-691">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049): проблемы, когда при отправке добавочного большого двоичного объекта игнорируются параметры условия.</span><span class="sxs-lookup"><span data-stu-id="a5b98-691">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-692">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-692">VM</span></span>

* <span data-ttu-id="a5b98-693">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="a5b98-693">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="a5b98-694">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-694">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="a5b98-695">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="a5b98-695">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="a5b98-696">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="a5b98-696">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="a5b98-697">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-697">March 13, 2018</span></span>

<span data-ttu-id="a5b98-698">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="a5b98-698">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="a5b98-699">ACR</span><span class="sxs-lookup"><span data-stu-id="a5b98-699">ACR</span></span>

* <span data-ttu-id="a5b98-700">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-700">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="a5b98-701">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="a5b98-701">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="a5b98-702">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="a5b98-702">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-703">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-703">ACS</span></span>

* <span data-ttu-id="a5b98-704">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="a5b98-704">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="a5b98-705">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="a5b98-705">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="a5b98-706">Помощник</span><span class="sxs-lookup"><span data-stu-id="a5b98-706">Advisor</span></span>

* <span data-ttu-id="a5b98-707">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-707">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="a5b98-708">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-708">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="a5b98-709">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-709">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="a5b98-710">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-710">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="a5b98-711">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-711">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-712">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a5b98-712">Appservice</span></span>

* <span data-ttu-id="a5b98-713">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="a5b98-713">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="a5b98-714">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-714">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="a5b98-715">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="a5b98-715">Eventhubs</span></span>

* <span data-ttu-id="a5b98-716">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a5b98-716">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="a5b98-717">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a5b98-717">Extension</span></span>

* <span data-ttu-id="a5b98-718">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="a5b98-718">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="a5b98-719">Interactive</span><span class="sxs-lookup"><span data-stu-id="a5b98-719">Interactive</span></span>

* <span data-ttu-id="a5b98-720">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625): теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="a5b98-720">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="a5b98-721">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016): при использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="a5b98-721">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="a5b98-722">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688): если при загрузке таблицы команд возникало исключение, опережающий ввод не выполнялся.</span><span class="sxs-lookup"><span data-stu-id="a5b98-722">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="a5b98-723">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="a5b98-723">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="a5b98-724">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a5b98-724">Monitor</span></span>

* <span data-ttu-id="a5b98-725">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="a5b98-725">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="a5b98-726">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-726">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="a5b98-727">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-727">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="a5b98-728">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-728">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-729">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-729">Network</span></span>

* <span data-ttu-id="a5b98-730">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-730">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="a5b98-731">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="a5b98-731">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="a5b98-732">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-732">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="a5b98-733">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-733">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="a5b98-734">Профиль</span><span class="sxs-lookup"><span data-stu-id="a5b98-734">Profile</span></span>

* <span data-ttu-id="a5b98-735">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="a5b98-735">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="a5b98-736">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-736">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="a5b98-737">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="a5b98-737">RDBMS</span></span>

* <span data-ttu-id="a5b98-738">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="a5b98-738">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="a5b98-739">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="a5b98-739">Service Bus</span></span>

* <span data-ttu-id="a5b98-740">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a5b98-740">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-741">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-741">Storage</span></span>

* <span data-ttu-id="a5b98-742">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="a5b98-742">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="a5b98-743">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286): при пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="a5b98-743">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-744">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-744">VM</span></span>

* <span data-ttu-id="a5b98-745">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="a5b98-745">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="a5b98-746">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="a5b98-746">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="a5b98-747">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-747">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="a5b98-748">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="a5b98-748">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="a5b98-749">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="a5b98-749">February 27, 2018</span></span>

<span data-ttu-id="a5b98-750">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="a5b98-750">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="a5b98-751">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-751">Core</span></span>

* <span data-ttu-id="a5b98-752">Исправлена ошибка с установкой Homebrew [№ 5184](https://github.com/Azure/azure-cli/issues/5184).</span><span class="sxs-lookup"><span data-stu-id="a5b98-752">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="a5b98-753">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="a5b98-753">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="a5b98-754">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-754">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-755">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-755">ACS</span></span>

* <span data-ttu-id="a5b98-756">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a5b98-756">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="a5b98-757">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="a5b98-757">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="a5b98-758">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-758">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="a5b98-759">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-759">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-760">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a5b98-760">Appservice</span></span>

* <span data-ttu-id="a5b98-761">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="a5b98-761">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="a5b98-762">Исправлена ошибка с сообщением `Free` о недопустимом SKU [№ 5538](https://github.com/Azure/azure-cli/issues/5538)</span><span class="sxs-lookup"><span data-stu-id="a5b98-762">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a5b98-763">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="a5b98-763">Cognitive Services</span></span>

* <span data-ttu-id="a5b98-764">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="a5b98-764">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="a5b98-765">Потребление</span><span class="sxs-lookup"><span data-stu-id="a5b98-765">Consumption</span></span>

* <span data-ttu-id="a5b98-766">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="a5b98-766">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="a5b98-767">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="a5b98-767">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="a5b98-768">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a5b98-768">Container</span></span>

* <span data-ttu-id="a5b98-769">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="a5b98-769">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-770">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-770">Network</span></span>

* <span data-ttu-id="a5b98-771">Исправлена ошибка с отсутствующим клиентом в `network vnet-gateway vpn-client generate` [№ 5559](https://github.com/Azure/azure-cli/issues/5559).</span><span class="sxs-lookup"><span data-stu-id="a5b98-771">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="a5b98-772">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a5b98-772">Resource</span></span>

* <span data-ttu-id="a5b98-773">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="a5b98-773">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="a5b98-774">Роль</span><span class="sxs-lookup"><span data-stu-id="a5b98-774">Role</span></span>

* <span data-ttu-id="a5b98-775">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="a5b98-775">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="a5b98-776">SQL</span><span class="sxs-lookup"><span data-stu-id="a5b98-776">SQL</span></span>

* <span data-ttu-id="a5b98-777">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-777">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-778">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-778">Storage</span></span>

* <span data-ttu-id="a5b98-779">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-779">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-780">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-780">VM</span></span>

* <span data-ttu-id="a5b98-781">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="a5b98-781">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="a5b98-782">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-782">February 13, 2018</span></span>

<span data-ttu-id="a5b98-783">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="a5b98-783">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="a5b98-784">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-784">Core</span></span>

* <span data-ttu-id="a5b98-785">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="a5b98-785">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-786">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-786">ACS</span></span>

* <span data-ttu-id="a5b98-787">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="a5b98-787">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="a5b98-788">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-788">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="a5b98-789">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="a5b98-789">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="a5b98-790">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="a5b98-790">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="a5b98-791">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="a5b98-791">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="a5b98-792">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-792">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="a5b98-793">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="a5b98-793">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="a5b98-794">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-794">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-795">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a5b98-795">Appservice</span></span>

* <span data-ttu-id="a5b98-796">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="a5b98-796">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="a5b98-797">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-797">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="a5b98-798">CDN</span><span class="sxs-lookup"><span data-stu-id="a5b98-798">CDN</span></span>

* <span data-ttu-id="a5b98-799">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-799">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="a5b98-800">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a5b98-800">Container</span></span>

* <span data-ttu-id="a5b98-801">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="a5b98-801">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="a5b98-802">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a5b98-802">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a5b98-803">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a5b98-803">CosmosDB</span></span>

* <span data-ttu-id="a5b98-804">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="a5b98-804">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="a5b98-805">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a5b98-805">Extension</span></span>

* <span data-ttu-id="a5b98-806">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-806">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="a5b98-807">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-807">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="a5b98-808">Отзыв</span><span class="sxs-lookup"><span data-stu-id="a5b98-808">Feedback</span></span>

* <span data-ttu-id="a5b98-809">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="a5b98-809">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="a5b98-810">Interactive</span><span class="sxs-lookup"><span data-stu-id="a5b98-810">Interactive</span></span>

* <span data-ttu-id="a5b98-811">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="a5b98-811">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="a5b98-812">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="a5b98-812">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="a5b98-813">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a5b98-813">IoT</span></span>

* <span data-ttu-id="a5b98-814">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="a5b98-814">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="a5b98-815">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="a5b98-815">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="a5b98-816">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-816">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="a5b98-817">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="a5b98-817">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="a5b98-818">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a5b98-818">Monitor</span></span>

* <span data-ttu-id="a5b98-819">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-819">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-820">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-820">Network</span></span>

* <span data-ttu-id="a5b98-821">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="a5b98-821">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="a5b98-822">Профиль</span><span class="sxs-lookup"><span data-stu-id="a5b98-822">Profile</span></span>

* <span data-ttu-id="a5b98-823">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5b98-823">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="a5b98-824">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a5b98-824">Resource</span></span>

* <span data-ttu-id="a5b98-825">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-825">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="a5b98-826">Роль</span><span class="sxs-lookup"><span data-stu-id="a5b98-826">Role</span></span>

* <span data-ttu-id="a5b98-827">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="a5b98-827">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="a5b98-828">SQL</span><span class="sxs-lookup"><span data-stu-id="a5b98-828">SQL</span></span>

* <span data-ttu-id="a5b98-829">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-829">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="a5b98-830">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-830">Added `sql db rename`</span></span>
* <span data-ttu-id="a5b98-831">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="a5b98-831">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-832">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-832">Storage</span></span>

* <span data-ttu-id="a5b98-833">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="a5b98-833">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-834">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-834">VM</span></span>

* <span data-ttu-id="a5b98-835">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="a5b98-835">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="a5b98-836">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="a5b98-836">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="a5b98-837">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="a5b98-837">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="a5b98-838">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-838">January 31, 2018</span></span>

<span data-ttu-id="a5b98-839">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="a5b98-839">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="a5b98-840">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-840">Core</span></span>

* <span data-ttu-id="a5b98-841">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="a5b98-841">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="a5b98-842">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="a5b98-842">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="a5b98-843">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="a5b98-843">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="a5b98-844">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="a5b98-844">Use `--verbose` to see</span></span>
* <span data-ttu-id="a5b98-845">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="a5b98-845">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-846">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-846">ACS</span></span>

* <span data-ttu-id="a5b98-847">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-847">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="a5b98-848">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-848">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-849">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a5b98-849">Appservice</span></span>

* <span data-ttu-id="a5b98-850">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="a5b98-850">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="a5b98-851">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="a5b98-851">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="a5b98-852">CDN</span><span class="sxs-lookup"><span data-stu-id="a5b98-852">CDN</span></span>

* <span data-ttu-id="a5b98-853">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-853">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a5b98-854">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a5b98-854">CosmosDB</span></span>

* <span data-ttu-id="a5b98-855">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="a5b98-855">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="a5b98-856">Interactive</span><span class="sxs-lookup"><span data-stu-id="a5b98-856">Interactive</span></span>

* <span data-ttu-id="a5b98-857">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="a5b98-857">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-858">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-858">Network</span></span>

* <span data-ttu-id="a5b98-859">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-859">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="a5b98-860">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a5b98-860">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="a5b98-861">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-861">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="a5b98-862">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-862">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="a5b98-863">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-863">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="a5b98-864">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="a5b98-864">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="a5b98-865">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="a5b98-865">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="a5b98-866">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="a5b98-866">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="a5b98-867">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-867">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="a5b98-868">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-868">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="a5b98-869">Профиль</span><span class="sxs-lookup"><span data-stu-id="a5b98-869">Profile</span></span>

* <span data-ttu-id="a5b98-870">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="a5b98-870">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="a5b98-871">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a5b98-871">Resource</span></span>

* <span data-ttu-id="a5b98-872">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="a5b98-872">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-873">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-873">Storage</span></span>

* <span data-ttu-id="a5b98-874">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="a5b98-874">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="a5b98-875">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="a5b98-875">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="a5b98-876">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-876">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="a5b98-877">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-877">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="a5b98-878">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="a5b98-878">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-879">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-879">VM</span></span>

* <span data-ttu-id="a5b98-880">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="a5b98-880">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="a5b98-881">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-881">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="a5b98-882">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="a5b98-882">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="a5b98-883">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-883">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="a5b98-884">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-884">January 17, 2018</span></span>

<span data-ttu-id="a5b98-885">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="a5b98-885">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="a5b98-886">ACR</span><span class="sxs-lookup"><span data-stu-id="a5b98-886">ACR</span></span>

* <span data-ttu-id="a5b98-887">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="a5b98-887">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="a5b98-888">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="a5b98-888">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-889">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-889">ACS</span></span>

* <span data-ttu-id="a5b98-890">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-890">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="a5b98-891">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="a5b98-891">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-892">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a5b98-892">Appservice</span></span>

* <span data-ttu-id="a5b98-893">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="a5b98-893">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="a5b98-894">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-894">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="a5b98-895">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-895">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="a5b98-896">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="a5b98-896">Backup</span></span>

* <span data-ttu-id="a5b98-897">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="a5b98-897">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="a5b98-898">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="a5b98-898">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="a5b98-899">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="a5b98-899">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="a5b98-900">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="a5b98-900">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="a5b98-901">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="a5b98-901">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="a5b98-902">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a5b98-902">Batch</span></span>

* <span data-ttu-id="a5b98-903">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="a5b98-903">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="a5b98-904">Облако</span><span class="sxs-lookup"><span data-stu-id="a5b98-904">Cloud</span></span>

* <span data-ttu-id="a5b98-905">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="a5b98-905">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="a5b98-906">Потребление</span><span class="sxs-lookup"><span data-stu-id="a5b98-906">Consumption</span></span>

* <span data-ttu-id="a5b98-907">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-907">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="a5b98-908">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="a5b98-908">Event Grid</span></span>

* <span data-ttu-id="a5b98-909">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-909">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="a5b98-910">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-910">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="a5b98-911">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-911">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="a5b98-912">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-912">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="a5b98-913">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-913">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="a5b98-914">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-914">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="a5b98-915">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-915">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="a5b98-916">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-916">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="a5b98-917">Interactive</span><span class="sxs-lookup"><span data-stu-id="a5b98-917">Interactive</span></span>

* <span data-ttu-id="a5b98-918">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="a5b98-918">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="a5b98-919">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="a5b98-919">Fixed errors on startup</span></span>
* <span data-ttu-id="a5b98-920">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5b98-920">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="a5b98-921">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a5b98-921">IoT</span></span>

* <span data-ttu-id="a5b98-922">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="a5b98-922">Added support for device provisioning service</span></span>
* <span data-ttu-id="a5b98-923">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="a5b98-923">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="a5b98-924">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="a5b98-924">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="a5b98-925">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a5b98-925">Monitor</span></span>

* <span data-ttu-id="a5b98-926">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="a5b98-926">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="a5b98-927">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-927">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="a5b98-928">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="a5b98-928">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-929">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-929">Network</span></span>

* <span data-ttu-id="a5b98-930">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="a5b98-930">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="a5b98-931">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="a5b98-931">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="a5b98-932">Профиль</span><span class="sxs-lookup"><span data-stu-id="a5b98-932">Profile</span></span>

* <span data-ttu-id="a5b98-933">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a5b98-933">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="a5b98-934">Роль</span><span class="sxs-lookup"><span data-stu-id="a5b98-934">Role</span></span>

* <span data-ttu-id="a5b98-935">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-935">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a5b98-936">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a5b98-936">Service Fabric</span></span>

* <span data-ttu-id="a5b98-937">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="a5b98-937">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="a5b98-938">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="a5b98-938">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-939">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-939">VM</span></span>

* <span data-ttu-id="a5b98-940">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-940">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="a5b98-941">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="a5b98-941">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="a5b98-942">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-942">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="a5b98-943">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="a5b98-943">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="a5b98-944">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="a5b98-944">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="a5b98-945">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-945">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="a5b98-946">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-946">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="a5b98-947">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-947">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="a5b98-948">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-948">December 19, 2017</span></span>

<span data-ttu-id="a5b98-949">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="a5b98-949">Version 2.0.23</span></span>

* <span data-ttu-id="a5b98-950">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a5b98-950">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="a5b98-951">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a5b98-951">Container</span></span>

* <span data-ttu-id="a5b98-952">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a5b98-952">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-953">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-953">Network</span></span>

* <span data-ttu-id="a5b98-954">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a5b98-954">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="a5b98-955">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a5b98-955">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-956">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-956">Storage</span></span>

* <span data-ttu-id="a5b98-957">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="a5b98-957">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-958">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-958">VM</span></span>

* <span data-ttu-id="a5b98-959">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="a5b98-959">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="a5b98-960">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-960">December 5, 2017</span></span>

<span data-ttu-id="a5b98-961">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="a5b98-961">Version 2.0.22</span></span>

* <span data-ttu-id="a5b98-962">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-962">Removed `az component` commands.</span></span> <span data-ttu-id="a5b98-963">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-963">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="a5b98-964">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-964">Core</span></span>
* <span data-ttu-id="a5b98-965">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="a5b98-965">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="a5b98-966">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="a5b98-966">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-967">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-967">ACS</span></span>

* <span data-ttu-id="a5b98-968">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-968">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="a5b98-969">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-969">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="a5b98-970">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="a5b98-970">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="a5b98-971">Помощник</span><span class="sxs-lookup"><span data-stu-id="a5b98-971">Advisor</span></span>

* <span data-ttu-id="a5b98-972">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a5b98-972">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-973">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a5b98-973">Appservice</span></span>

* <span data-ttu-id="a5b98-974">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-974">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="a5b98-975">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="a5b98-975">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="a5b98-976">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-976">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="a5b98-977">Потребление</span><span class="sxs-lookup"><span data-stu-id="a5b98-977">Consumption</span></span>

* <span data-ttu-id="a5b98-978">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="a5b98-978">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="a5b98-979">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a5b98-979">Container</span></span>

* <span data-ttu-id="a5b98-980">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="a5b98-980">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="a5b98-981">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a5b98-981">Monitor</span></span>

* <span data-ttu-id="a5b98-982">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="a5b98-982">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="a5b98-983">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a5b98-983">Resource</span></span>

* <span data-ttu-id="a5b98-984">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="a5b98-984">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="a5b98-985">Роль</span><span class="sxs-lookup"><span data-stu-id="a5b98-985">Role</span></span>

* <span data-ttu-id="a5b98-986">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-986">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="a5b98-987">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="a5b98-987">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="a5b98-988">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-988">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="a5b98-989">SQL</span><span class="sxs-lookup"><span data-stu-id="a5b98-989">SQL</span></span>

* <span data-ttu-id="a5b98-990">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-990">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="a5b98-991">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-991">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-992">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-992">VM</span></span>

* <span data-ttu-id="a5b98-993">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-993">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="a5b98-994">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-994">November 14, 2017</span></span>

<span data-ttu-id="a5b98-995">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="a5b98-995">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="a5b98-996">ACR</span><span class="sxs-lookup"><span data-stu-id="a5b98-996">ACR</span></span>

* <span data-ttu-id="a5b98-997">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="a5b98-997">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="a5b98-998">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-998">ACS</span></span>

* <span data-ttu-id="a5b98-999">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="a5b98-999">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="a5b98-1000">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1000">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="a5b98-1001">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1001">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="a5b98-1002">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1002">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="a5b98-1003">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1003">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-1004">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a5b98-1004">Appservice</span></span>

* <span data-ttu-id="a5b98-1005">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1005">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="a5b98-1006">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1006">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="a5b98-1007">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1007">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="a5b98-1008">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1008">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="a5b98-1009">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="a5b98-1009">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="a5b98-1010">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1010">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="a5b98-1011">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a5b98-1011">Batch</span></span>

* <span data-ttu-id="a5b98-1012">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1012">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="a5b98-1013">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="a5b98-1013">Batchai</span></span>

* <span data-ttu-id="a5b98-1014">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1014">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="a5b98-1015">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1015">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="a5b98-1016">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1016">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="a5b98-1017">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1017">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="a5b98-1018">Облако</span><span class="sxs-lookup"><span data-stu-id="a5b98-1018">Cloud</span></span>

* <span data-ttu-id="a5b98-1019">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1019">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="a5b98-1020">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a5b98-1020">Container</span></span>

* <span data-ttu-id="a5b98-1021">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1021">Added support to open multiple ports</span></span>
* <span data-ttu-id="a5b98-1022">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1022">Added container group restart policy</span></span>
* <span data-ttu-id="a5b98-1023">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1023">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="a5b98-1024">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1024">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a5b98-1025">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a5b98-1025">Data Lake Analytics</span></span>

* <span data-ttu-id="a5b98-1026">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1026">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a5b98-1027">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a5b98-1027">Data Lake Store</span></span>

* <span data-ttu-id="a5b98-1028">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1028">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="a5b98-1029">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a5b98-1029">Extension</span></span>

* <span data-ttu-id="a5b98-1030">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1030">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="a5b98-1031">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1031">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="a5b98-1032">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a5b98-1032">IoT</span></span>

* <span data-ttu-id="a5b98-1033">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1033">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="a5b98-1034">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a5b98-1034">Monitor</span></span>

* <span data-ttu-id="a5b98-1035">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1035">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-1036">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-1036">Network</span></span>

* <span data-ttu-id="a5b98-1037">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1037">Added support for CAA DNS records</span></span>
* <span data-ttu-id="a5b98-1038">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1038">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="a5b98-1039">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1039">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="a5b98-1040">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1040">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="a5b98-1041">Резервирование</span><span class="sxs-lookup"><span data-stu-id="a5b98-1041">Reservations</span></span>

* <span data-ttu-id="a5b98-1042">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="a5b98-1042">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="a5b98-1043">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a5b98-1043">Resource</span></span>

* <span data-ttu-id="a5b98-1044">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1044">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="a5b98-1045">SQL</span><span class="sxs-lookup"><span data-stu-id="a5b98-1045">SQL</span></span>

* <span data-ttu-id="a5b98-1046">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1046">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-1047">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1047">Storage</span></span>

* <span data-ttu-id="a5b98-1048">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1048">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="a5b98-1049">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1049">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="a5b98-1050">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1050">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="a5b98-1051">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1051">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="a5b98-1052">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1052">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="a5b98-1053">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1053">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="a5b98-1054">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1054">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-1055">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-1055">VM</span></span>

* <span data-ttu-id="a5b98-1056">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1056">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="a5b98-1057">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1057">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="a5b98-1058">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1058">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="a5b98-1059">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1059">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="a5b98-1060">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1060">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="a5b98-1061">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1061">October 24, 2017</span></span>

<span data-ttu-id="a5b98-1062">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="a5b98-1062">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="a5b98-1063">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-1063">Core</span></span>

* <span data-ttu-id="a5b98-1064">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1064">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="a5b98-1065">ACR</span><span class="sxs-lookup"><span data-stu-id="a5b98-1065">ACR</span></span>

* <span data-ttu-id="a5b98-1066">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1066">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="a5b98-1067">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="a5b98-1067">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="a5b98-1068">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="a5b98-1068">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-1069">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-1069">ACS</span></span>

* <span data-ttu-id="a5b98-1070">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1070">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="a5b98-1071">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1071">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-1072">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a5b98-1072">Appservice</span></span>

* <span data-ttu-id="a5b98-1073">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1073">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="a5b98-1074">Компонент</span><span class="sxs-lookup"><span data-stu-id="a5b98-1074">Component</span></span>

* <span data-ttu-id="a5b98-1075">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="a5b98-1075">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="a5b98-1076">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a5b98-1076">Monitor</span></span>

* <span data-ttu-id="a5b98-1077">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1077">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="a5b98-1078">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a5b98-1078">Resource</span></span>

* <span data-ttu-id="a5b98-1079">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1079">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="a5b98-1080">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="a5b98-1080">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-1081">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-1081">VM</span></span>

* <span data-ttu-id="a5b98-1082">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1082">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="a5b98-1083">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1083">October 9, 2017</span></span>

<span data-ttu-id="a5b98-1084">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="a5b98-1084">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="a5b98-1085">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-1085">Core</span></span>

* <span data-ttu-id="a5b98-1086">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1086">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-1087">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a5b98-1087">Appservice</span></span>

* <span data-ttu-id="a5b98-1088">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1088">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="a5b98-1089">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a5b98-1089">Batch</span></span>

* <span data-ttu-id="a5b98-1090">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="a5b98-1090">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="a5b98-1091">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1091">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="a5b98-1092">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1092">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="a5b98-1093">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1093">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="a5b98-1094">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="a5b98-1094">Batchai</span></span>

* <span data-ttu-id="a5b98-1095">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="a5b98-1095">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="a5b98-1096">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a5b98-1096">Keyvault</span></span>

* <span data-ttu-id="a5b98-1097">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1097">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="a5b98-1098">(#4448)</span><span class="sxs-lookup"><span data-stu-id="a5b98-1098">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="a5b98-1099">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-1099">Network</span></span>

* <span data-ttu-id="a5b98-1100">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1100">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="a5b98-1101">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1101">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="a5b98-1102">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a5b98-1102">Resource</span></span>

* <span data-ttu-id="a5b98-1103">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1103">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="a5b98-1104">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1104">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="a5b98-1105">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1105">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="a5b98-1106">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1106">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="a5b98-1107">SQL</span><span class="sxs-lookup"><span data-stu-id="a5b98-1107">Sql</span></span>

* <span data-ttu-id="a5b98-1108">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1108">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="a5b98-1109">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1109">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="a5b98-1110">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1110">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-1111">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1111">Storage</span></span>

* <span data-ttu-id="a5b98-1112">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1112">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-1113">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="a5b98-1113">Vm</span></span>

* <span data-ttu-id="a5b98-1114">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1114">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="a5b98-1115">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1115">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="a5b98-1116">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1116">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="a5b98-1117">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1117">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="a5b98-1118">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1118">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="a5b98-1119">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1119">September 22, 2017</span></span>

<span data-ttu-id="a5b98-1120">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="a5b98-1120">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="a5b98-1121">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a5b98-1121">Resource</span></span>

* <span data-ttu-id="a5b98-1122">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="a5b98-1122">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="a5b98-1123">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="a5b98-1123">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="a5b98-1124">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1124">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="a5b98-1125">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1125">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-1126">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-1126">Network</span></span>

* <span data-ttu-id="a5b98-1127">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1127">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="a5b98-1128">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1128">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="a5b98-1129">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1129">Added `asg` application security group commands</span></span>
* <span data-ttu-id="a5b98-1130">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1130">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="a5b98-1131">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1131">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="a5b98-1132">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1132">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="a5b98-1133">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1133">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-1134">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1134">Storage</span></span>

* <span data-ttu-id="a5b98-1135">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="a5b98-1135">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="a5b98-1136">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="a5b98-1136">Eventgrid</span></span>

* <span data-ttu-id="a5b98-1137">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="a5b98-1137">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="a5b98-1138">SQL</span><span class="sxs-lookup"><span data-stu-id="a5b98-1138">SQL</span></span>

* <span data-ttu-id="a5b98-1139">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1139">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="a5b98-1140">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="a5b98-1140">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="a5b98-1141">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1141">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="a5b98-1142">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a5b98-1142">Keyvault</span></span>

* <span data-ttu-id="a5b98-1143">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="a5b98-1143">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-1144">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-1144">VM</span></span>

* <span data-ttu-id="a5b98-1145">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1145">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="a5b98-1146">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="a5b98-1146">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="a5b98-1147">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1147">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="a5b98-1148">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1148">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="a5b98-1149">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1149">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="a5b98-1150">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1150">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-1151">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-1151">ACS</span></span>

* <span data-ttu-id="a5b98-1152">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="a5b98-1152">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-1153">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a5b98-1153">Appservice</span></span>

* <span data-ttu-id="a5b98-1154">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="a5b98-1154">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="a5b98-1155">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="a5b98-1155">Backup</span></span>

* <span data-ttu-id="a5b98-1156">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1156">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="a5b98-1157">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1157">September 11, 2017</span></span>

<span data-ttu-id="a5b98-1158">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="a5b98-1158">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="a5b98-1159">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-1159">Core</span></span>

* <span data-ttu-id="a5b98-1160">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1160">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="a5b98-1161">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1161">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-1162">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-1162">Acs</span></span>

* <span data-ttu-id="a5b98-1163">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1163">Added `acs list-locations` command</span></span>
* <span data-ttu-id="a5b98-1164">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1164">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-1165">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a5b98-1165">Appservice</span></span>

* <span data-ttu-id="a5b98-1166">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1166">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="a5b98-1167">CDN</span><span class="sxs-lookup"><span data-stu-id="a5b98-1167">CDN</span></span>

* <span data-ttu-id="a5b98-1168">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1168">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="a5b98-1169">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="a5b98-1169">Extension</span></span>

* <span data-ttu-id="a5b98-1170">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a5b98-1170">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="a5b98-1171">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a5b98-1171">Keyvault</span></span>

* <span data-ttu-id="a5b98-1172">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1172">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-1173">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-1173">Network</span></span>

* <span data-ttu-id="a5b98-1174">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1174">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="a5b98-1175">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1175">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="a5b98-1176">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1176">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="a5b98-1177">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1177">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="a5b98-1178">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1178">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="a5b98-1179">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a5b98-1179">Resource</span></span>

* <span data-ttu-id="a5b98-1180">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1180">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="a5b98-1181">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1181">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="a5b98-1182">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1182">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="a5b98-1183">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1183">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="a5b98-1184">SQL</span><span class="sxs-lookup"><span data-stu-id="a5b98-1184">SQL</span></span>

* <span data-ttu-id="a5b98-1185">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1185">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-1186">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-1186">VM</span></span>

* <span data-ttu-id="a5b98-1187">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1187">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="a5b98-1188">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1188">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="a5b98-1189">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1189">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="a5b98-1190">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1190">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="a5b98-1191">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1191">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="a5b98-1192">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1192">August 31, 2017</span></span>

<span data-ttu-id="a5b98-1193">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="a5b98-1193">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="a5b98-1194">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a5b98-1194">Keyvault</span></span>

* <span data-ttu-id="a5b98-1195">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1195">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="a5b98-1196">Sf</span><span class="sxs-lookup"><span data-stu-id="a5b98-1196">Sf</span></span>

* <span data-ttu-id="a5b98-1197">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1197">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-1198">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1198">Storage</span></span>

* <span data-ttu-id="a5b98-1199">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1199">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="a5b98-1200">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1200">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="a5b98-1201">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1201">August 28, 2017</span></span>

<span data-ttu-id="a5b98-1202">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="a5b98-1202">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="a5b98-1203">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="a5b98-1203">CLI</span></span>

* <span data-ttu-id="a5b98-1204">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1204">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-1205">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-1205">ACS</span></span>

* <span data-ttu-id="a5b98-1206">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1206">Corrected preview regions</span></span>
* <span data-ttu-id="a5b98-1207">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1207">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="a5b98-1208">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1208">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-1209">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a5b98-1209">Appservice</span></span>

* <span data-ttu-id="a5b98-1210">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1210">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="a5b98-1211">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1211">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="a5b98-1212">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1212">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="a5b98-1213">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1213">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="a5b98-1214">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1214">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="a5b98-1215">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a5b98-1215">IoT</span></span>

* <span data-ttu-id="a5b98-1216">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1216">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-1217">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-1217">Network</span></span>

* <span data-ttu-id="a5b98-1218">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1218">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="a5b98-1219">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1219">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="a5b98-1220">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1220">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="a5b98-1221">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1221">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="a5b98-1222">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1222">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="a5b98-1223">Профиль</span><span class="sxs-lookup"><span data-stu-id="a5b98-1223">Profile</span></span>

* <span data-ttu-id="a5b98-1224">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1224">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a5b98-1225">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a5b98-1225">Service Fabric</span></span>

* <span data-ttu-id="a5b98-1226">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1226">Preview release</span></span>
* <span data-ttu-id="a5b98-1227">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1227">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="a5b98-1228">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1228">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="a5b98-1229">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1229">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-1230">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1230">Storage</span></span>

* <span data-ttu-id="a5b98-1231">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1231">Enabled setting blob tier</span></span>
* <span data-ttu-id="a5b98-1232">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1232">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="a5b98-1233">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1233">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="a5b98-1234">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1234">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="a5b98-1235">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1235">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="a5b98-1236">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1236">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-1237">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-1237">VM</span></span>

* <span data-ttu-id="a5b98-1238">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1238">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="a5b98-1239">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1239">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="a5b98-1240">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1240">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="a5b98-1241">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1241">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="a5b98-1242">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1242">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="a5b98-1243">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1243">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="a5b98-1244">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1244">August 15, 2017</span></span>

<span data-ttu-id="a5b98-1245">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="a5b98-1245">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-1246">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-1246">ACS</span></span>

* <span data-ttu-id="a5b98-1247">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1247">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-1248">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a5b98-1248">Appservice</span></span>

* <span data-ttu-id="a5b98-1249">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1249">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="a5b98-1250">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="a5b98-1250">Event Grid</span></span>

* <span data-ttu-id="a5b98-1251">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1251">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="a5b98-1252">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1252">August 11, 2017</span></span>

<span data-ttu-id="a5b98-1253">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="a5b98-1253">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-1254">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-1254">ACS</span></span>

* <span data-ttu-id="a5b98-1255">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1255">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="a5b98-1256">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a5b98-1256">Batch</span></span>

* <span data-ttu-id="a5b98-1257">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1257">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="a5b98-1258">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1258">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="a5b98-1259">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1259">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="a5b98-1260">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1260">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="a5b98-1261">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1261">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="a5b98-1262">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1262">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="a5b98-1263">Компонент</span><span class="sxs-lookup"><span data-stu-id="a5b98-1263">Component</span></span>

* <span data-ttu-id="a5b98-1264">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1264">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="a5b98-1265">Контейнер</span><span class="sxs-lookup"><span data-stu-id="a5b98-1265">Container</span></span>

* <span data-ttu-id="a5b98-1266">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1266">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="a5b98-1267">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a5b98-1267">Data Lake Store</span></span>

* <span data-ttu-id="a5b98-1268">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1268">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="a5b98-1269">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="a5b98-1269">Event Grid</span></span>

* <span data-ttu-id="a5b98-1270">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="a5b98-1270">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-1271">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-1271">Network</span></span>

* <span data-ttu-id="a5b98-1272">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1272">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="a5b98-1273">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1273">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="a5b98-1274">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1274">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="a5b98-1275">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1275">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="a5b98-1276">Профиль</span><span class="sxs-lookup"><span data-stu-id="a5b98-1276">Profile</span></span>

* <span data-ttu-id="a5b98-1277">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1277">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-1278">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1278">Storage</span></span>

* <span data-ttu-id="a5b98-1279">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1279">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-1280">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-1280">VM</span></span>

* <span data-ttu-id="a5b98-1281">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1281">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="a5b98-1282">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1282">Exposed `list-skus` command</span></span>
* <span data-ttu-id="a5b98-1283">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1283">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="a5b98-1284">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1284">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="a5b98-1285">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1285">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="a5b98-1286">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1286">July 28, 2017</span></span>

<span data-ttu-id="a5b98-1287">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="a5b98-1287">Version 2.0.12</span></span>

* <span data-ttu-id="a5b98-1288">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1288">Added container commands</span></span>
* <span data-ttu-id="a5b98-1289">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1289">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="a5b98-1290">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-1290">Core</span></span>

* <span data-ttu-id="a5b98-1291">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1291">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="a5b98-1292">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1292">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="a5b98-1293">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1293">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="a5b98-1294">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1294">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="a5b98-1295">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1295">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="a5b98-1296">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1296">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="a5b98-1297">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1297">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="a5b98-1298">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1298">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="a5b98-1299">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1299">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="a5b98-1300">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1300">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="a5b98-1301">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1301">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="a5b98-1302">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1302">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="a5b98-1303">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1303">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="a5b98-1304">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1304">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="a5b98-1305">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1305">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="a5b98-1306">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1306">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="a5b98-1307">ACR</span><span class="sxs-lookup"><span data-stu-id="a5b98-1307">ACR</span></span>

* <span data-ttu-id="a5b98-1308">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1308">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="a5b98-1309">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1309">Support SKU update for managed registries</span></span>
* <span data-ttu-id="a5b98-1310">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1310">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="a5b98-1311">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1311">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="a5b98-1312">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1312">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="a5b98-1313">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1313">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-1314">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-1314">ACS</span></span>

* <span data-ttu-id="a5b98-1315">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1315">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-1316">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="a5b98-1316">Appservice</span></span>

* <span data-ttu-id="a5b98-1317">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1317">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="a5b98-1318">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1318">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="a5b98-1319">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1319">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="a5b98-1320">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1320">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="a5b98-1321">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1321">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="a5b98-1322">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1322">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="a5b98-1323">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1323">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="a5b98-1324">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1324">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="a5b98-1325">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1325">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="a5b98-1326">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1326">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="a5b98-1327">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="a5b98-1327">Batch</span></span>

* <span data-ttu-id="a5b98-1328">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1328">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="a5b98-1329">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1329">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="a5b98-1330">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1330">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="a5b98-1331">CDN</span><span class="sxs-lookup"><span data-stu-id="a5b98-1331">CDN</span></span>

* <span data-ttu-id="a5b98-1332">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1332">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="a5b98-1333">Облако</span><span class="sxs-lookup"><span data-stu-id="a5b98-1333">Cloud</span></span>

* <span data-ttu-id="a5b98-1334">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1334">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="a5b98-1335">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1335">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="a5b98-1336">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1336">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="a5b98-1337">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1337">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="a5b98-1338">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1338">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a5b98-1339">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a5b98-1339">CosmosDB</span></span>

* <span data-ttu-id="a5b98-1340">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1340">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="a5b98-1341">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1341">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a5b98-1342">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a5b98-1342">Data Lake Analytics</span></span>

* <span data-ttu-id="a5b98-1343">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1343">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="a5b98-1344">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1344">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="a5b98-1345">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1345">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a5b98-1346">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a5b98-1346">Data Lake Store</span></span>

* <span data-ttu-id="a5b98-1347">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1347">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="a5b98-1348">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1348">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="a5b98-1349">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1349">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="a5b98-1350">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1350">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="a5b98-1351">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="a5b98-1351">Interactive</span></span>

* <span data-ttu-id="a5b98-1352">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1352">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="a5b98-1353">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1353">Increased test coverage</span></span>
* <span data-ttu-id="a5b98-1354">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1354">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="a5b98-1355">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1355">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="a5b98-1356">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1356">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="a5b98-1357">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1357">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="a5b98-1358">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1358">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="a5b98-1359">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1359">Added `--progress` flag</span></span>
* <span data-ttu-id="a5b98-1360">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1360">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="a5b98-1361">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1361">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="a5b98-1362">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="a5b98-1362">IoT</span></span>

* <span data-ttu-id="a5b98-1363">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="a5b98-1363">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="a5b98-1364">(3934).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1364">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="a5b98-1365">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a5b98-1365">Key vault</span></span>

* <span data-ttu-id="a5b98-1366">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="a5b98-1366">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="a5b98-1367">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1367">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="a5b98-1368">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="a5b98-1368">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="a5b98-1369">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="a5b98-1369">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="a5b98-1370">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1370">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="a5b98-1371">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1371">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="a5b98-1372">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="a5b98-1372">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="a5b98-1373">(3307).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1373">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="a5b98-1374">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="a5b98-1374">Lab</span></span>

* <span data-ttu-id="a5b98-1375">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1375">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="a5b98-1376">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1376">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="a5b98-1377">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a5b98-1377">Monitor</span></span>

* <span data-ttu-id="a5b98-1378">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1378">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="a5b98-1379">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1379">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="a5b98-1380">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1380">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="a5b98-1381">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1381">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="a5b98-1382">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1382">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="a5b98-1383">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="a5b98-1383">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="a5b98-1384">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="a5b98-1384">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="a5b98-1385">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="a5b98-1385">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="a5b98-1386">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="a5b98-1386">`location` no longer required</span></span>
  * <span data-ttu-id="a5b98-1387">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="a5b98-1387">Add name and ID support for target</span></span>
  * <span data-ttu-id="a5b98-1388">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="a5b98-1388">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="a5b98-1389">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="a5b98-1389">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="a5b98-1390">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="a5b98-1390">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="a5b98-1391">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1391">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="a5b98-1392">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1392">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="a5b98-1393">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1393">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-1394">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-1394">Network</span></span>

* <span data-ttu-id="a5b98-1395">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1395">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="a5b98-1396">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1396">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="a5b98-1397">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1397">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="a5b98-1398">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1398">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="a5b98-1399">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1399">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="a5b98-1400">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1400">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="a5b98-1401">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1401">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="a5b98-1402">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1402">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="a5b98-1403">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1403">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="a5b98-1404">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1404">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="a5b98-1405">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1405">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="a5b98-1406">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1406">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="a5b98-1407">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1407">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="a5b98-1408">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1408">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="a5b98-1409">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1409">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="a5b98-1410">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1410">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="a5b98-1411">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1411">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="a5b98-1412">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1412">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="a5b98-1413">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1413">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="a5b98-1414">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1414">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="a5b98-1415">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1415">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="a5b98-1416">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1416">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="a5b98-1417">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1417">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="a5b98-1418">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1418">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="a5b98-1419">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1419">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="a5b98-1420">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1420">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="a5b98-1421">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1421">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="a5b98-1422">Профиль</span><span class="sxs-lookup"><span data-stu-id="a5b98-1422">Profile</span></span>

* <span data-ttu-id="a5b98-1423">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1423">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="a5b98-1424">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1424">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="a5b98-1425">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1425">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="a5b98-1426">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1426">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="a5b98-1427">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1427">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="a5b98-1428">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="a5b98-1428">RDBMS</span></span>

* <span data-ttu-id="a5b98-1429">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1429">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="a5b98-1430">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1430">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="a5b98-1431">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1431">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="a5b98-1432">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1432">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="a5b98-1433">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a5b98-1433">Resource</span></span>

* <span data-ttu-id="a5b98-1434">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1434">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="a5b98-1435">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1435">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="a5b98-1436">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1436">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="a5b98-1437">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1437">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="a5b98-1438">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1438">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="a5b98-1439">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1439">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="a5b98-1440">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1440">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="a5b98-1441">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1441">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="a5b98-1442">Роль</span><span class="sxs-lookup"><span data-stu-id="a5b98-1442">Role</span></span>

* <span data-ttu-id="a5b98-1443">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1443">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="a5b98-1444">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1444">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="a5b98-1445">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1445">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="a5b98-1446">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1446">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="a5b98-1447">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1447">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a5b98-1448">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a5b98-1448">Service Fabric</span></span>
* <span data-ttu-id="a5b98-1449">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1449">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="a5b98-1450">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1450">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="a5b98-1451">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1451">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="a5b98-1452">SQL</span><span class="sxs-lookup"><span data-stu-id="a5b98-1452">SQL</span></span>

* <span data-ttu-id="a5b98-1453">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1453">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="a5b98-1454">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1454">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="a5b98-1455">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1455">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-1456">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1456">Storage</span></span>

* <span data-ttu-id="a5b98-1457">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1457">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="a5b98-1458">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1458">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="a5b98-1459">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1459">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="a5b98-1460">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="a5b98-1460">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="a5b98-1461">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1461">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="a5b98-1462">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1462">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-1463">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-1463">VM</span></span>

* <span data-ttu-id="a5b98-1464">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1464">Support configuring nsg</span></span>
* <span data-ttu-id="a5b98-1465">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1465">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="a5b98-1466">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1466">Support managed service identities</span></span>
* <span data-ttu-id="a5b98-1467">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1467">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="a5b98-1468">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1468">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="a5b98-1469">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1469">May 10, 2017</span></span>

<span data-ttu-id="a5b98-1470">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="a5b98-1470">Version 2.0.6</span></span>

* <span data-ttu-id="a5b98-1471">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1471">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="a5b98-1472">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1472">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="a5b98-1473">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1473">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="a5b98-1474">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1474">Include Cognitive Services module</span></span>
* <span data-ttu-id="a5b98-1475">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1475">Include Service Fabric module</span></span>
* <span data-ttu-id="a5b98-1476">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1476">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="a5b98-1477">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1477">Add support for CDN commands</span></span>
* <span data-ttu-id="a5b98-1478">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1478">Remove Container module</span></span>
* <span data-ttu-id="a5b98-1479">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1479">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="a5b98-1480">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1480">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="a5b98-1481">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-1481">Core</span></span>

* <span data-ttu-id="a5b98-1482">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1482">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="a5b98-1483">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1483">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="a5b98-1484">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1484">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="a5b98-1485">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1485">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="a5b98-1486">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1486">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="a5b98-1487">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1487">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="a5b98-1488">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1488">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="a5b98-1489">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1489">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="a5b98-1490">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1490">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="a5b98-1491">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1491">core: Improved performance</span></span>
* <span data-ttu-id="a5b98-1492">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1492">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="a5b98-1493">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1493">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-1494">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-1494">ACS</span></span>

* <span data-ttu-id="a5b98-1495">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1495">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="a5b98-1496">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1496">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="a5b98-1497">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1497">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="a5b98-1498">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1498">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-1499">AppService</span><span class="sxs-lookup"><span data-stu-id="a5b98-1499">AppService</span></span>

* <span data-ttu-id="a5b98-1500">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1500">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="a5b98-1501">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1501">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="a5b98-1502">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1502">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="a5b98-1503">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1503">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="a5b98-1504">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1504">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="a5b98-1505">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1505">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="a5b98-1506">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1506">support slot swap with preview</span></span>
* <span data-ttu-id="a5b98-1507">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1507">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="a5b98-1508">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1508">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a5b98-1509">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a5b98-1509">CosmosDB</span></span>

* <span data-ttu-id="a5b98-1510">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1510">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="a5b98-1511">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1511">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="a5b98-1512">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1512">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="a5b98-1513">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1513">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a5b98-1514">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a5b98-1514">Data Lake Analytics</span></span>

* <span data-ttu-id="a5b98-1515">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1515">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="a5b98-1516">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1516">Add support for new catalog item type: package.</span></span> <span data-ttu-id="a5b98-1517">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1517">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="a5b98-1518">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="a5b98-1518">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="a5b98-1519">Таблица</span><span class="sxs-lookup"><span data-stu-id="a5b98-1519">Table</span></span>
  * <span data-ttu-id="a5b98-1520">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="a5b98-1520">Table valued function</span></span>
  * <span data-ttu-id="a5b98-1521">Просмотр</span><span class="sxs-lookup"><span data-stu-id="a5b98-1521">View</span></span>
  * <span data-ttu-id="a5b98-1522">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1522">Table Statistics.</span></span> <span data-ttu-id="a5b98-1523">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1523">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a5b98-1524">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a5b98-1524">Data Lake Store</span></span>

* <span data-ttu-id="a5b98-1525">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1525">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="a5b98-1526">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1526">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="a5b98-1527">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1527">missed help for access show.</span></span> <span data-ttu-id="a5b98-1528">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1528">adding it.</span></span> <span data-ttu-id="a5b98-1529">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="a5b98-1529">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="a5b98-1530">Поиск</span><span class="sxs-lookup"><span data-stu-id="a5b98-1530">Find</span></span>

* <span data-ttu-id="a5b98-1531">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1531">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="a5b98-1532">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="a5b98-1532">KeyVault</span></span>

* <span data-ttu-id="a5b98-1533">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1533">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="a5b98-1534">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1534">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="a5b98-1535">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1535">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="a5b98-1536">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1536">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="a5b98-1537">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1537">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="a5b98-1538">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="a5b98-1538">Lab</span></span>

* <span data-ttu-id="a5b98-1539">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1539">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="a5b98-1540">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1540">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="a5b98-1541">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1541">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="a5b98-1542">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1542">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="a5b98-1543">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1543">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="a5b98-1544">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="a5b98-1544">Monitor</span></span>

* <span data-ttu-id="a5b98-1545">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1545">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="a5b98-1546">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1546">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="a5b98-1547">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-1547">Network</span></span>

* <span data-ttu-id="a5b98-1548">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1548">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="a5b98-1549">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1549">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="a5b98-1550">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1550">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="a5b98-1551">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1551">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="a5b98-1552">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1552">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="a5b98-1553">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1553">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="a5b98-1554">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1554">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="a5b98-1555">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1555">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="a5b98-1556">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1556">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="a5b98-1557">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="a5b98-1557">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="a5b98-1558">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1558">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="a5b98-1559">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1559">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="a5b98-1560">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1560">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="a5b98-1561">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1561">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="a5b98-1562">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1562">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="a5b98-1563">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1563">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="a5b98-1564">Профиль</span><span class="sxs-lookup"><span data-stu-id="a5b98-1564">Profile</span></span>

* <span data-ttu-id="a5b98-1565">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1565">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="a5b98-1566">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1566">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="a5b98-1567">Redis</span><span class="sxs-lookup"><span data-stu-id="a5b98-1567">Redis</span></span>

* <span data-ttu-id="a5b98-1568">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1568">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="a5b98-1569">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1569">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="a5b98-1570">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a5b98-1570">Resource</span></span>

* <span data-ttu-id="a5b98-1571">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1571">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="a5b98-1572">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1572">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="a5b98-1573">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1573">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="a5b98-1574">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1574">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="a5b98-1575">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="a5b98-1575">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="a5b98-1576">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1576">Add docs for az lock update.</span></span> <span data-ttu-id="a5b98-1577">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="a5b98-1577">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="a5b98-1578">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1578">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="a5b98-1579">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="a5b98-1579">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="a5b98-1580">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1580">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="a5b98-1581">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="a5b98-1581">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="a5b98-1582">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1582">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="a5b98-1583">Роль</span><span class="sxs-lookup"><span data-stu-id="a5b98-1583">Role</span></span>

* <span data-ttu-id="a5b98-1584">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1584">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="a5b98-1585">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1585">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="a5b98-1586">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1586">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="a5b98-1587">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1587">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="a5b98-1588">SQL</span><span class="sxs-lookup"><span data-stu-id="a5b98-1588">SQL</span></span>

* <span data-ttu-id="a5b98-1589">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1589">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="a5b98-1590">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1590">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="a5b98-1591">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1591">Storage</span></span>

* <span data-ttu-id="a5b98-1592">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1592">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="a5b98-1593">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1593">Add support for incremental blob copy</span></span>
* <span data-ttu-id="a5b98-1594">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1594">Add support for large block blob upload</span></span>
* <span data-ttu-id="a5b98-1595">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1595">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-1596">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-1596">VM</span></span>

* <span data-ttu-id="a5b98-1597">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1597">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="a5b98-1598">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="a5b98-1598">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="a5b98-1599">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="a5b98-1599">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="a5b98-1600">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="a5b98-1600">az vm/vmss disk</span></span>
  3. <span data-ttu-id="a5b98-1601">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1601">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="a5b98-1602">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1602">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="a5b98-1603">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1603">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="a5b98-1604">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1604">April 3, 2017</span></span>

<span data-ttu-id="a5b98-1605">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="a5b98-1605">Version 2.0.2</span></span>

<span data-ttu-id="a5b98-1606">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1606">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="a5b98-1607">Core</span><span class="sxs-lookup"><span data-stu-id="a5b98-1607">Core</span></span>

* <span data-ttu-id="a5b98-1608">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1608">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="a5b98-1609">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1609">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="a5b98-1610">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1610">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="a5b98-1611">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1611">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a5b98-1612">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1612">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="a5b98-1613">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="a5b98-1613">Add prompting for missing template parameters.</span></span> <span data-ttu-id="a5b98-1614">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1614">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="a5b98-1615">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1615">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="a5b98-1616">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1616">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="a5b98-1617">ACS</span><span class="sxs-lookup"><span data-stu-id="a5b98-1617">ACS</span></span>

* <span data-ttu-id="a5b98-1618">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1618">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="a5b98-1619">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="a5b98-1619">Add support for ssh key password prompting.</span></span> <span data-ttu-id="a5b98-1620">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1620">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="a5b98-1621">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="a5b98-1621">Add support for windows clusters.</span></span> <span data-ttu-id="a5b98-1622">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1622">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="a5b98-1623">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="a5b98-1623">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="a5b98-1624">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1624">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="a5b98-1625">AppService</span><span class="sxs-lookup"><span data-stu-id="a5b98-1625">AppService</span></span>

* <span data-ttu-id="a5b98-1626">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1626">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="a5b98-1627">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1627">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="a5b98-1628">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1628">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="a5b98-1629">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1629">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="a5b98-1630">Data Lake</span><span class="sxs-lookup"><span data-stu-id="a5b98-1630">DataLake</span></span>

* <span data-ttu-id="a5b98-1631">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1631">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="a5b98-1632">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1632">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="a5b98-1633">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="a5b98-1633">DocuemntDB</span></span>

* <span data-ttu-id="a5b98-1634">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1634">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="a5b98-1635">ВМ</span><span class="sxs-lookup"><span data-stu-id="a5b98-1635">VM</span></span>

* <span data-ttu-id="a5b98-1636">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1636">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="a5b98-1637">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1637">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="a5b98-1638">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1638">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="a5b98-1639">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1639">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a5b98-1640">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1640">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="a5b98-1641">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1641">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="a5b98-1642">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1642">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="a5b98-1643">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1643">February 27, 2017</span></span>

<span data-ttu-id="a5b98-1644">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="a5b98-1644">Version 2.0.0</span></span>

<span data-ttu-id="a5b98-1645">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="a5b98-1645">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="a5b98-1646">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="a5b98-1646">Container Service (acs)</span></span>
- <span data-ttu-id="a5b98-1647">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="a5b98-1647">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="a5b98-1648">Сеть</span><span class="sxs-lookup"><span data-stu-id="a5b98-1648">Networking</span></span>
- <span data-ttu-id="a5b98-1649">служба хранилища.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1649">Storage</span></span>

<span data-ttu-id="a5b98-1650">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1650">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="a5b98-1651">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1651">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="a5b98-1652">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1652">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="a5b98-1653">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1653">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="a5b98-1654">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="a5b98-1654">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="a5b98-1655">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="a5b98-1655">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="a5b98-1656">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="a5b98-1656">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="a5b98-1657">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="a5b98-1657">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="a5b98-1658">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="a5b98-1658">Provide feedback from the command line with the `az feedback` command</span></span>

