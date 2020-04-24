---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 04/21/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 10dfdc316ba00f8a7019f0724aab231e344c1c6d
ms.sourcegitcommit: 89ec9fa7ebd2170b55201cd51fb386fd9351d7ca
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2020
ms.locfileid: "81728599"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="70a96-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="70a96-103">Azure CLI release notes</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="70a96-104">21 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-104">April 21, 2020</span></span>

<span data-ttu-id="70a96-105">Версия 2.4.0</span><span class="sxs-lookup"><span data-stu-id="70a96-105">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-106">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-106">ACR</span></span>

* <span data-ttu-id="70a96-107">`az acr run --cmd`: отключает переопределение рабочего каталога.</span><span class="sxs-lookup"><span data-stu-id="70a96-107">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="70a96-108">Включена поддержка выделенной конечной точки данных.</span><span class="sxs-lookup"><span data-stu-id="70a96-108">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="70a96-109">AKS</span><span class="sxs-lookup"><span data-stu-id="70a96-109">AKS</span></span>

* <span data-ttu-id="70a96-110">`az aks list -o table` теперь показывает privateFqdn как FQDN для частных кластеров.</span><span class="sxs-lookup"><span data-stu-id="70a96-110">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="70a96-111">Добавлен параметр --uptime-sla.</span><span class="sxs-lookup"><span data-stu-id="70a96-111">Add --uptime-sla</span></span>
* <span data-ttu-id="70a96-112">Обновлен пакет containerservice.</span><span class="sxs-lookup"><span data-stu-id="70a96-112">Update containerservice package</span></span>
* <span data-ttu-id="70a96-113">Включена поддержка общедоступных IP-адресов узлов.</span><span class="sxs-lookup"><span data-stu-id="70a96-113">Add node public IP support</span></span>
* <span data-ttu-id="70a96-114">Исправлена опечатка в команде справки.</span><span class="sxs-lookup"><span data-stu-id="70a96-114">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="70a96-115">AppConfig</span><span class="sxs-lookup"><span data-stu-id="70a96-115">AppConfig</span></span>

* <span data-ttu-id="70a96-116">Разрешена ссылка на хранилище ключей для команд kv list и export.</span><span class="sxs-lookup"><span data-stu-id="70a96-116">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="70a96-117">Исправлена ошибка при отображении значений ключей.</span><span class="sxs-lookup"><span data-stu-id="70a96-117">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-118">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-118">AppService</span></span>

* <span data-ttu-id="70a96-119">`az functionapp create`: изменен способ настройки linuxFxVersion для приложений-функций dotnet в Linux.</span><span class="sxs-lookup"><span data-stu-id="70a96-119">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="70a96-120">Это должно исправить ошибку, препятствующую созданию приложений dotnet для использования в Linux.</span><span class="sxs-lookup"><span data-stu-id="70a96-120">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="70a96-121">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az webapp create` Исправлена ошибка для сохранения существующих параметров AppSettings с помощью az webapp create.</span><span class="sxs-lookup"><span data-stu-id="70a96-121">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="70a96-122">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az webapp up` Исправлена ошибка для создания группы ресурсов для команды az webapp up при использовании флага -g.</span><span class="sxs-lookup"><span data-stu-id="70a96-122">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="70a96-123">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az webapp config` Исправлена ошибка для отображения значений для выходных данных не в формате JSON с помощью команды az webapp config connection-string list.</span><span class="sxs-lookup"><span data-stu-id="70a96-123">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="70a96-124">ARM</span><span class="sxs-lookup"><span data-stu-id="70a96-124">ARM</span></span>

* <span data-ttu-id="70a96-125">`az deployment create/validate`: Добавлен параметр `--no-prompt` для пропуска запроса отсутствующих параметров для шаблона ARM.</span><span class="sxs-lookup"><span data-stu-id="70a96-125">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="70a96-126">`az deployment group/mg/sub/tenant validate`: включена поддержка комментариев в файле параметров развертывания.</span><span class="sxs-lookup"><span data-stu-id="70a96-126">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="70a96-127">`az deployment`: удалено `is_preview` для параметра `--handle-extended-json-format`.</span><span class="sxs-lookup"><span data-stu-id="70a96-127">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="70a96-128">`az deployment group/mg/sub/tenant cancel`: включена поддержка отмены развертывания для шаблона ARM.</span><span class="sxs-lookup"><span data-stu-id="70a96-128">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="70a96-129">`az deployment group/mg/sub/tenant validate`: улучшено отображение сообщения об ошибке при сбое проверки развертывания.</span><span class="sxs-lookup"><span data-stu-id="70a96-129">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="70a96-130">`az deployment-scripts`: добавлена новая команда для DeploymentScripts.</span><span class="sxs-lookup"><span data-stu-id="70a96-130">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="70a96-131">`az resource tag`: добавлен параметр `--is-incremental` для инкрементного добавления тегов к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="70a96-131">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="70a96-132">ARO</span><span class="sxs-lookup"><span data-stu-id="70a96-132">ARO</span></span>

* <span data-ttu-id="70a96-133">`az aro`:  добавлен модуль команды aro Azure RedHat OpenShift версии 4.</span><span class="sxs-lookup"><span data-stu-id="70a96-133">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="70a96-134">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-134">Batch</span></span>

* <span data-ttu-id="70a96-135">Обновлен API пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="70a96-135">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="70a96-136">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="70a96-136">Compute</span></span>

* <span data-ttu-id="70a96-137">`az sig image-version create`: добавлен тип учетной записи хранения Premium_LRS.</span><span class="sxs-lookup"><span data-stu-id="70a96-137">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="70a96-138">`az vmss update`: устранена проблема с обновлением уведомления о завершении.</span><span class="sxs-lookup"><span data-stu-id="70a96-138">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="70a96-139">`az vm/vmss create`: включена поддержка версии специализированного образа.</span><span class="sxs-lookup"><span data-stu-id="70a96-139">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="70a96-140">API SIG версии 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="70a96-140">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="70a96-141">`az sig image-version create`: добавлен параметр --target-region-encryption.</span><span class="sxs-lookup"><span data-stu-id="70a96-141">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="70a96-142">Исправлена ошибка, из-за которой тесты завершались сбоем при последовательном выполнении из-за дублирования имени хранилища ключей в глобальном кэше в памяти.</span><span class="sxs-lookup"><span data-stu-id="70a96-142">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="70a96-143">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70a96-143">CosmosDB</span></span>

* <span data-ttu-id="70a96-144">Включена поддержка `az cosmosdb private-link-resource/private-endpoint-connection`.</span><span class="sxs-lookup"><span data-stu-id="70a96-144">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="70a96-145">IoT Central</span><span class="sxs-lookup"><span data-stu-id="70a96-145">IoT Central</span></span>

* <span data-ttu-id="70a96-146">Прекращена поддержка `az iotcentral`.</span><span class="sxs-lookup"><span data-stu-id="70a96-146">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="70a96-147">Добавлен модуль команды `az iot central`.</span><span class="sxs-lookup"><span data-stu-id="70a96-147">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-148">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-148">Monitor</span></span>

* <span data-ttu-id="70a96-149">Включена поддержка сценария приватного канала для монитора.</span><span class="sxs-lookup"><span data-stu-id="70a96-149">Support private link scenario for monitor</span></span>
* <span data-ttu-id="70a96-150">Исправлен неправильный способ имитации в test_monitor_general_operations.py.</span><span class="sxs-lookup"><span data-stu-id="70a96-150">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="70a96-151">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-151">Network</span></span>

* <span data-ttu-id="70a96-152">Прекращена поддержка SKU для команды public ip update.</span><span class="sxs-lookup"><span data-stu-id="70a96-152">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="70a96-153">`az network private-endpoint`: включена поддержка закрытой группы зон DNS.</span><span class="sxs-lookup"><span data-stu-id="70a96-153">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="70a96-154">Включена функция локального контекста для параметра vnet/subnet.</span><span class="sxs-lookup"><span data-stu-id="70a96-154">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="70a96-155">Исправлен неправильный пример использования в test_nw_flow_log_delete.</span><span class="sxs-lookup"><span data-stu-id="70a96-155">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="70a96-156">Упаковка</span><span class="sxs-lookup"><span data-stu-id="70a96-156">Packaging</span></span>

* <span data-ttu-id="70a96-157">Прекращена поддержка пакета Ubuntu/Disco.</span><span class="sxs-lookup"><span data-stu-id="70a96-157">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="70a96-158">RBAC</span><span class="sxs-lookup"><span data-stu-id="70a96-158">RBAC</span></span>

* <span data-ttu-id="70a96-159">`az ad app create/update`: включена поддержка параметра --optional-claims.</span><span class="sxs-lookup"><span data-stu-id="70a96-159">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="70a96-160">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="70a96-160">RDBMS</span></span>

* <span data-ttu-id="70a96-161">Добавлены команды администратора Azure Active Directory для PostgreSQL и MySQL.</span><span class="sxs-lookup"><span data-stu-id="70a96-161">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="70a96-162">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="70a96-162">Service Fabric</span></span>

* <span data-ttu-id="70a96-163">Исправление 12891: `az sf application update --application-parameters` удаляет старые параметры, отсутствующие в запросе.</span><span class="sxs-lookup"><span data-stu-id="70a96-163">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="70a96-164">Исправление 12470: включена поддержка az sf create cluster, исправлены ошибки в устойчивости и надежности обновления, поиск VMSS выполняется корректно в коде при указании имени типа узла.</span><span class="sxs-lookup"><span data-stu-id="70a96-164">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-165">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-165">SQL</span></span>

* <span data-ttu-id="70a96-166">Добавлены `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`.</span><span class="sxs-lookup"><span data-stu-id="70a96-166">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="70a96-167">`az sql midb`: обновление и отображение политик долгосрочного хранения, отображение и удаление долгосрочных резервных копий, восстановление долгосрочных резервных копий.</span><span class="sxs-lookup"><span data-stu-id="70a96-167">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-168">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-168">Storage</span></span>

* <span data-ttu-id="70a96-169">Обновлена версия azure-mgmt-storage до 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="70a96-169">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="70a96-170">`az storage logging off`: включено отключение ведения журналов для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="70a96-170">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="70a96-171">`az storage account update`: включена автоматическая смена ключа для CMK.</span><span class="sxs-lookup"><span data-stu-id="70a96-171">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="70a96-172">`az storage account encryption-scope create/update/list/show`: включена настройка области шифрования.</span><span class="sxs-lookup"><span data-stu-id="70a96-172">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="70a96-173">`az storage container create`: добавлены параметры --default-encryption-scope и --deny-encryption-scope-override для настройки области шифрования на уровне контейнера.</span><span class="sxs-lookup"><span data-stu-id="70a96-173">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="70a96-174">Опрос</span><span class="sxs-lookup"><span data-stu-id="70a96-174">Survey</span></span>

* <span data-ttu-id="70a96-175">Добавлен параметр для отключения ссылки опроса.</span><span class="sxs-lookup"><span data-stu-id="70a96-175">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="70a96-176">01 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-176">April 01, 2020</span></span>

<span data-ttu-id="70a96-177">Версия 2.3.1</span><span class="sxs-lookup"><span data-stu-id="70a96-177">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-178">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-178">ACR</span></span>

* <span data-ttu-id="70a96-179">Исправлена неправильная версия azure-mgmt-containerregistry для Linux.</span><span class="sxs-lookup"><span data-stu-id="70a96-179">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="70a96-180">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-180">Profile</span></span>

* <span data-ttu-id="70a96-181">az login: Исправлена ошибка входа в облачных профилях, отличающихся от `latest`.</span><span class="sxs-lookup"><span data-stu-id="70a96-181">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="70a96-182">31 марта 2020 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-182">March 31, 2020</span></span>

<span data-ttu-id="70a96-183">Версия 2.3.0</span><span class="sxs-lookup"><span data-stu-id="70a96-183">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-184">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-184">ACR</span></span>

* <span data-ttu-id="70a96-185">az acr task update: исключение пустого указателя.</span><span class="sxs-lookup"><span data-stu-id="70a96-185">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="70a96-186">`az acr import`: Отредактировано справочное сообщение и сообщение об ошибке для уточнения того, как использовать параметры --source и --registry.</span><span class="sxs-lookup"><span data-stu-id="70a96-186">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="70a96-187">Добавлено средство проверки для аргумента registry_name.</span><span class="sxs-lookup"><span data-stu-id="70a96-187">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="70a96-188">`az acr login`: удален флаг предпросмотра для --expose-token.</span><span class="sxs-lookup"><span data-stu-id="70a96-188">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="70a96-189">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр ветви az acr task create/update.</span><span class="sxs-lookup"><span data-stu-id="70a96-189">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="70a96-190">Клиент az acr task update теперь может независимо обновлять контекст, токен GitHub и триггеры.</span><span class="sxs-lookup"><span data-stu-id="70a96-190">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="70a96-191">az acr agentpool: новая функция.</span><span class="sxs-lookup"><span data-stu-id="70a96-191">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="70a96-192">AKS</span><span class="sxs-lookup"><span data-stu-id="70a96-192">AKS</span></span>

* <span data-ttu-id="70a96-193">Исправлена ошибка с apiServerAccessProfile при обновлении --api-server-authorized-ip-ranges.</span><span class="sxs-lookup"><span data-stu-id="70a96-193">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="70a96-194">Обновление AKS: при обновлении исходящие IP-адреса переопределяются с помощью входных значений.</span><span class="sxs-lookup"><span data-stu-id="70a96-194">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="70a96-195">Не создаются имена субъектов-служб для кластеров MSI и реализована поддержка присоединение ACR к кластерам MSI.</span><span class="sxs-lookup"><span data-stu-id="70a96-195">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="70a96-196">AMS</span><span class="sxs-lookup"><span data-stu-id="70a96-196">AMS</span></span>

* <span data-ttu-id="70a96-197">Исправление 12469: не удается добавить content-key-policy для FairPlay из-за проблем с параметром ask.</span><span class="sxs-lookup"><span data-stu-id="70a96-197">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="70a96-198">AppConfig</span><span class="sxs-lookup"><span data-stu-id="70a96-198">AppConfig</span></span>

* <span data-ttu-id="70a96-199">Добавлен параметр --skip-keyvault для экспорта kv.</span><span class="sxs-lookup"><span data-stu-id="70a96-199">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-200">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-200">AppService</span></span>

* <span data-ttu-id="70a96-201">Исправление 12509: удален тег, добавлявшийся по умолчанию при создании приложения с помощью az webapp up.</span><span class="sxs-lookup"><span data-stu-id="70a96-201">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="70a96-202">az functionapp create: обновлено меню справки для --runtime-version и добавлено предупреждение, когда пользователь указывает параметр --runtime-version для DotNet.</span><span class="sxs-lookup"><span data-stu-id="70a96-202">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="70a96-203">az functionapp create: изменен способ установки JavaVersion для приложений-функций Windows.</span><span class="sxs-lookup"><span data-stu-id="70a96-203">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="70a96-204">ARM</span><span class="sxs-lookup"><span data-stu-id="70a96-204">ARM</span></span>

* <span data-ttu-id="70a96-205">az deployment create/validate: по умолчанию используется параметр --handle-extended-json-format.</span><span class="sxs-lookup"><span data-stu-id="70a96-205">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="70a96-206">az lock create: в справочную документацию добавлены примеры создания подресурсов.</span><span class="sxs-lookup"><span data-stu-id="70a96-206">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="70a96-207">Список az deployment {group/mg/sub/tenant}: реализована поддержка фильтрации ProvisioningState.</span><span class="sxs-lookup"><span data-stu-id="70a96-207">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="70a96-208">az deployment: исправлена ошибка синтаксического анализа комментария в последнем аргументе.</span><span class="sxs-lookup"><span data-stu-id="70a96-208">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="70a96-209">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="70a96-209">Backup</span></span>

* <span data-ttu-id="70a96-210">Добавлена возможность восстановления нескольких файлов.</span><span class="sxs-lookup"><span data-stu-id="70a96-210">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="70a96-211">Добавлена возможность резервного копирования только дисков с ОС.</span><span class="sxs-lookup"><span data-stu-id="70a96-211">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="70a96-212">Добавлен параметр restore-as-unmanaged-disk, позволяющий задать неуправляемое восстановление.</span><span class="sxs-lookup"><span data-stu-id="70a96-212">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="70a96-213">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="70a96-213">Compute</span></span>

* <span data-ttu-id="70a96-214">az vm create: для --nsg-rule добавлен вариант NONE.</span><span class="sxs-lookup"><span data-stu-id="70a96-214">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="70a96-215">az vmss create/update: удален тег предпросмотра для автоматического восстановления VMSS.</span><span class="sxs-lookup"><span data-stu-id="70a96-215">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="70a96-216">az vm update: реализована поддержка --workspace.</span><span class="sxs-lookup"><span data-stu-id="70a96-216">az vm update: Support --workspace</span></span>
* <span data-ttu-id="70a96-217">Исправлена ошибка в коде инициализации VirtualMachineScaleSetExtension.</span><span class="sxs-lookup"><span data-stu-id="70a96-217">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="70a96-218">Версия VMAccessAgent обновлена до 2.4.</span><span class="sxs-lookup"><span data-stu-id="70a96-218">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="70a96-219">az vmss set-orchestration-service-state: реализована поддержка состояния службы оркестрации наборов VMSS.</span><span class="sxs-lookup"><span data-stu-id="70a96-219">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="70a96-220">Версия API диска обновлена до 2019-11-01.</span><span class="sxs-lookup"><span data-stu-id="70a96-220">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="70a96-221">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun.</span><span class="sxs-lookup"><span data-stu-id="70a96-221">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="70a96-222">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70a96-222">Cosmos DB</span></span>

* <span data-ttu-id="70a96-223">Добавлен отсутствовавший параметр --type для перенаправления в связи с устареванием.</span><span class="sxs-lookup"><span data-stu-id="70a96-223">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="70a96-224">Docker</span><span class="sxs-lookup"><span data-stu-id="70a96-224">Docker</span></span>

* <span data-ttu-id="70a96-225">Обновление до Alpine 3.11 и Python 3.6.10.</span><span class="sxs-lookup"><span data-stu-id="70a96-225">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="70a96-226">Расширение</span><span class="sxs-lookup"><span data-stu-id="70a96-226">Extension</span></span>

* <span data-ttu-id="70a96-227">Добавлена возможность загрузки расширений в системный путь через пакеты.</span><span class="sxs-lookup"><span data-stu-id="70a96-227">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="70a96-228">HDInsight</span><span class="sxs-lookup"><span data-stu-id="70a96-228">HDInsight</span></span>

* <span data-ttu-id="70a96-229">(az hdinsight create:) Добавлена возможность указания клиентами минимальной поддерживаемой версии TLS с помощью параметра `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="70a96-229">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="70a96-230">Допустимые значения: 1.0,1.1,1.2.</span><span class="sxs-lookup"><span data-stu-id="70a96-230">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="70a96-231">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-231">IoT</span></span>

* <span data-ttu-id="70a96-232">Добавлен параметр codeowner.</span><span class="sxs-lookup"><span data-stu-id="70a96-232">Add codeowner</span></span>
* <span data-ttu-id="70a96-233">az iot hub create: номер SKU по умолчанию изменен с F1 на S1.</span><span class="sxs-lookup"><span data-stu-id="70a96-233">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="70a96-234">iot hub: реализована поддержка IotHub в профиле 2019-03-01-hybrid.</span><span class="sxs-lookup"><span data-stu-id="70a96-234">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="70a96-235">IoT Central</span><span class="sxs-lookup"><span data-stu-id="70a96-235">IoTCentral</span></span>

* <span data-ttu-id="70a96-236">Обновлены сведения об ошибках, шаблон приложения по умолчанию и сообщение с подсказкой.</span><span class="sxs-lookup"><span data-stu-id="70a96-236">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="70a96-237">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70a96-237">KeyVault</span></span>

* <span data-ttu-id="70a96-238">Реализована поддержка резервного копирования и восстановления сертификатов.</span><span class="sxs-lookup"><span data-stu-id="70a96-238">Support certificate backup/restore</span></span>
* <span data-ttu-id="70a96-239">keyvault create/update: добавлена поддержка параметра --retention-days.</span><span class="sxs-lookup"><span data-stu-id="70a96-239">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="70a96-240">При перечислении больше не показываются управляемые ключи и секреты.</span><span class="sxs-lookup"><span data-stu-id="70a96-240">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="70a96-241">az keyvault create: реализована поддержка `--network-acls`, `--network-acls-ips` и `--network-acls-vnets` для указания сетевых правил при создании хранилища.</span><span class="sxs-lookup"><span data-stu-id="70a96-241">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="70a96-242">Блокировка</span><span class="sxs-lookup"><span data-stu-id="70a96-242">Lock</span></span>

* <span data-ttu-id="70a96-243">Исправлена ошибка с командой az lock delete, не работавшей с Microsoft.DocumentDB.</span><span class="sxs-lookup"><span data-stu-id="70a96-243">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-244">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-244">Monitor</span></span>

* <span data-ttu-id="70a96-245">az monitor clone: добавлена возможность клонирования правил метрики из одного ресурса в другой.</span><span class="sxs-lookup"><span data-stu-id="70a96-245">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="70a96-246">Исправлена ошибка IcM179210086: не удается создать настраиваемое оповещение для метрики Application Insights.</span><span class="sxs-lookup"><span data-stu-id="70a96-246">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="70a96-247">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="70a96-247">NetAppFiles</span></span>

* <span data-ttu-id="70a96-248">az volume create: для томов защиты данных добавлены операции репликации (approve, suspend, resume, status, remove).</span><span class="sxs-lookup"><span data-stu-id="70a96-248">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="70a96-249">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-249">Network</span></span>

* <span data-ttu-id="70a96-250">az network application-gateway waf-policy managed-rule rule-set add: добавлена поддержка Microsoft_BotManagerRuleSet.</span><span class="sxs-lookup"><span data-stu-id="70a96-250">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="70a96-251">Журнал потоков наблюдателя за сетями: исправлены неправильные сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="70a96-251">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="70a96-252">Добавлена поддержка имен узлов в прослушивателе шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="70a96-252">support host names in application gateway listener</span></span>
* <span data-ttu-id="70a96-253">az network nat gateway: добавлена возможность создания пустого ресурса без общедоступного IP-адреса или общедоступного IP-префикса.</span><span class="sxs-lookup"><span data-stu-id="70a96-253">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="70a96-254">Добавлена возможность создания VPN-шлюза.</span><span class="sxs-lookup"><span data-stu-id="70a96-254">Support vpn gateway generation</span></span>
* <span data-ttu-id="70a96-255">Реализована поддержка `--if-none-match` для `az network dns record-set {} add-record`.</span><span class="sxs-lookup"><span data-stu-id="70a96-255">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="70a96-256">Упаковка</span><span class="sxs-lookup"><span data-stu-id="70a96-256">Packaging</span></span>

* <span data-ttu-id="70a96-257">Прекращена поддержка Python 3.5.</span><span class="sxs-lookup"><span data-stu-id="70a96-257">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="70a96-258">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-258">Profile</span></span>

* <span data-ttu-id="70a96-259">az login: добавлен показ предупреждений об ошибках MFA.</span><span class="sxs-lookup"><span data-stu-id="70a96-259">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="70a96-260">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="70a96-260">RDBMS</span></span>

* <span data-ttu-id="70a96-261">Добавлены команды управления ключами шифрования данных сервера для PostgreSQL и MySQL.</span><span class="sxs-lookup"><span data-stu-id="70a96-261">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="70a96-262">10 марта 2020 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-262">March 10, 2020</span></span>

<span data-ttu-id="70a96-263">Версия 2.2.0</span><span class="sxs-lookup"><span data-stu-id="70a96-263">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-264">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-264">ACR</span></span>

* <span data-ttu-id="70a96-265">Исправлена команда `az acr login`, которая неправильно вызывала ошибку.</span><span class="sxs-lookup"><span data-stu-id="70a96-265">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="70a96-266">Добавлена новая команда `az acr helm install-cli`.</span><span class="sxs-lookup"><span data-stu-id="70a96-266">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="70a96-267">Добавлена частная ссылка и включена поддержка CMK.</span><span class="sxs-lookup"><span data-stu-id="70a96-267">Add private link and CMK support</span></span>
* <span data-ttu-id="70a96-268">Добавлена команда private-link-resource list.</span><span class="sxs-lookup"><span data-stu-id="70a96-268">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="70a96-269">AKS</span><span class="sxs-lookup"><span data-stu-id="70a96-269">AKS</span></span>

* <span data-ttu-id="70a96-270">Исправлена функция поиска AKS в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="70a96-270">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="70a96-271">az aks: устранены ошибки NoneType при мониторинге надстроек и пула агентов.</span><span class="sxs-lookup"><span data-stu-id="70a96-271">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="70a96-272">Добавлен параметр --nodepool-tags в пуле узлов при создании кластера Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="70a96-272">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="70a96-273">Добавлен параметр --tags при добавлении пула узлов в кластер или его обновлении.</span><span class="sxs-lookup"><span data-stu-id="70a96-273">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="70a96-274">aks create: добавлен параметр `--enable-private-cluster`.</span><span class="sxs-lookup"><span data-stu-id="70a96-274">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="70a96-275">Добавлен параметр --nodepool-labels в пуле узлов при создании кластера Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="70a96-275">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="70a96-276">Добавлен параметр --labels при добавлении нового пула узлов в кластер Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="70a96-276">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="70a96-277">Добавлен отсутствующий символ / в URL-адрес панели мониторинга.</span><span class="sxs-lookup"><span data-stu-id="70a96-277">add missing / in the dashboard url</span></span>
* <span data-ttu-id="70a96-278">Включена поддержка создания кластеров AKS для управляемых удостоверений</span><span class="sxs-lookup"><span data-stu-id="70a96-278">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="70a96-279">az aks: включена проверка состояния сетевого подключаемого модуля: Azure или Kubenet.</span><span class="sxs-lookup"><span data-stu-id="70a96-279">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="70a96-280">az aks: включена поддержка ключа сеанса AAD.</span><span class="sxs-lookup"><span data-stu-id="70a96-280">az aks: Add aad session key support</span></span>
* <span data-ttu-id="70a96-281">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az aks: включена поддержка изменений MSI для GF и BF для omsagent (мониторинг контейнеров) (1)</span><span class="sxs-lookup"><span data-stu-id="70a96-281">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="70a96-282">az aks use-dev-spaces: добавлен параметр типа конечной точки в команду use-dev-spaces для настройки конечной точки, созданной в контроллере Azure Dev Spaces.</span><span class="sxs-lookup"><span data-stu-id="70a96-282">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="70a96-283">AppConfig</span><span class="sxs-lookup"><span data-stu-id="70a96-283">AppConfig</span></span>

* <span data-ttu-id="70a96-284">Включена разблокировка с использованием kv set для добавления функции и ссылки на хранилище ключей.</span><span class="sxs-lookup"><span data-stu-id="70a96-284">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-285">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-285">AppService</span></span>

* <span data-ttu-id="70a96-286">az webapp create: устранена проблема с выполнением команды с параметром --runtime.</span><span class="sxs-lookup"><span data-stu-id="70a96-286">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="70a96-287">az functionapp deployment source config-zip: добавлено сообщение об ошибке, если группа ресурсов или имя функции недействительны или не существуют.</span><span class="sxs-lookup"><span data-stu-id="70a96-287">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="70a96-288">functionapp create: исправлено сообщение с предупреждением, которое появляется с `functionapp create` и в котором указан флаг `--functions_version`, но в имени флага ошибочно используется `_` вместо `-`.</span><span class="sxs-lookup"><span data-stu-id="70a96-288">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="70a96-289">az functionapp create: обновлен способ настройки linuxFxVersion и имени образа контейнера для приложений с функциями Linux.</span><span class="sxs-lookup"><span data-stu-id="70a96-289">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="70a96-290">az functionapp deployment source config-zip: устранена проблема, вызванная изменением параметров приложения во время развертывания ZIP, что приводит к ошибкам 5xx во время развертывания.</span><span class="sxs-lookup"><span data-stu-id="70a96-290">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="70a96-291">Исправление 5720946: не удается задать имя с помощью az webapp backup.</span><span class="sxs-lookup"><span data-stu-id="70a96-291">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="70a96-292">ARM</span><span class="sxs-lookup"><span data-stu-id="70a96-292">ARM</span></span>

* <span data-ttu-id="70a96-293">az resource: улучшены примеры для модуля ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70a96-293">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="70a96-294">az policy assignment list: Включена поддержка списков назначений политик в области группы управления.</span><span class="sxs-lookup"><span data-stu-id="70a96-294">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="70a96-295">Добавлены команды `az deployment group` и `az deployment operation group` для развертывания шаблонов в группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70a96-295">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="70a96-296">Это дубликат `az group deployment` и `az group deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="70a96-296">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="70a96-297">Добавлены команды `az deployment sub` и `az deployment operation sub` для развертывания шаблонов в области подписки.</span><span class="sxs-lookup"><span data-stu-id="70a96-297">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="70a96-298">Это дубликат `az deployment` и `az deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="70a96-298">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="70a96-299">Добавлены команды `az deployment mg` и `az deployment operation mg` для развертывания шаблонов в группах управления.</span><span class="sxs-lookup"><span data-stu-id="70a96-299">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="70a96-300">Добавлены команды `az deployment tenant` и `az deployment operation tenant` для развертывания шаблонов в области арендатора.</span><span class="sxs-lookup"><span data-stu-id="70a96-300">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="70a96-301">az policy assignment create: добавлено описание параметра `--location`.</span><span class="sxs-lookup"><span data-stu-id="70a96-301">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="70a96-302">az group deployment create: добавлен параметр `--aux-tenants` для включения поддержки перекрестных арендаторов.</span><span class="sxs-lookup"><span data-stu-id="70a96-302">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="70a96-303">CDN</span><span class="sxs-lookup"><span data-stu-id="70a96-303">CDN</span></span>

* <span data-ttu-id="70a96-304">Добавлены команды WAF CDN.</span><span class="sxs-lookup"><span data-stu-id="70a96-304">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="70a96-305">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="70a96-305">Compute</span></span>

* <span data-ttu-id="70a96-306">az sig image-version: добавлен параметр --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="70a96-306">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="70a96-307">az ppg show: добавлен параметр --colocation-status, чтобы включить выборку состояния совместного размещения всех ресурсов в группе размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="70a96-307">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="70a96-308">az vmss create/update: включена поддержка автоматического исправления.</span><span class="sxs-lookup"><span data-stu-id="70a96-308">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="70a96-309">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az image template: шаблон переименован в построитель.</span><span class="sxs-lookup"><span data-stu-id="70a96-309">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="70a96-310">az image builder create: добавлен параметр --image-template.</span><span class="sxs-lookup"><span data-stu-id="70a96-310">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="70a96-311">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70a96-311">Cosmos DB</span></span>

* <span data-ttu-id="70a96-312">Добавлены командлеты хранимой процедуры SQL, определяемых пользователем функций и триггеров.</span><span class="sxs-lookup"><span data-stu-id="70a96-312">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="70a96-313">az cosmosdb create: добавлен параметр --key-uri для добавления сведений о шифровании хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="70a96-313">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="70a96-314">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70a96-314">KeyVault</span></span>

* <span data-ttu-id="70a96-315">keyvault create: включена функция обратимого удаления по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-315">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-316">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-316">Monitor</span></span>

* <span data-ttu-id="70a96-317">az monitor metrics alert create: включена поддержка `~` в `--condition`.</span><span class="sxs-lookup"><span data-stu-id="70a96-317">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="70a96-318">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-318">Network</span></span>

* <span data-ttu-id="70a96-319">az network application-gateway rewrite-rule create: включена поддержка конфигурации URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="70a96-319">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="70a96-320">az network dns zone import: для параметра --zone-name в будущем можно будет не учитывать регистр.</span><span class="sxs-lookup"><span data-stu-id="70a96-320">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="70a96-321">az network private-endpoint/private-link-service: удалена метка предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="70a96-321">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="70a96-322">az network bastion: включена поддержка бастиона.</span><span class="sxs-lookup"><span data-stu-id="70a96-322">az network bastion: support bastion</span></span>
* <span data-ttu-id="70a96-323">az network vnet list-available-ips: включена поддержка списка доступных IP-адресов в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="70a96-323">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="70a96-324">az network watcher flow-log create/list/delete/update: добавлены новые команды для управления журналами потоков Наблюдателя и предоставлен параметр --location для явного определения Наблюдателя.</span><span class="sxs-lookup"><span data-stu-id="70a96-324">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="70a96-325">az network watcher flow-log configure: поддержка прекращена.</span><span class="sxs-lookup"><span data-stu-id="70a96-325">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="70a96-326">az network watcher flow-log show: включена поддержка параметров --location и --name для получения результатов в формате ARM; поддержка предыдущего форматированного вывода прекращена.</span><span class="sxs-lookup"><span data-stu-id="70a96-326">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="70a96-327">Политика</span><span class="sxs-lookup"><span data-stu-id="70a96-327">Policy</span></span>

* <span data-ttu-id="70a96-328">az policy assignment create: исправлена ошибка, из-за которой автоматически генерируемое имя назначения политики превышало предельное значение.</span><span class="sxs-lookup"><span data-stu-id="70a96-328">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="70a96-329">RBAC</span><span class="sxs-lookup"><span data-stu-id="70a96-329">RBAC</span></span>

* <span data-ttu-id="70a96-330">az ad group show: исправлено значение --group, обрабатываемое как проблема с регулярными выражениями.</span><span class="sxs-lookup"><span data-stu-id="70a96-330">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="70a96-331">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="70a96-331">RDBMS</span></span>

* <span data-ttu-id="70a96-332">Обновлена версия пакета SDK azure-mgmt-rdbms до 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="70a96-332">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="70a96-333">az postgres private-endpoint-connection: включено управление подключениями частных конечных точек Postgres.</span><span class="sxs-lookup"><span data-stu-id="70a96-333">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="70a96-334">az postgres private-link-resource: включено управление ресурсами частных ссылок Postgres.</span><span class="sxs-lookup"><span data-stu-id="70a96-334">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="70a96-335">az mysql private-endpoint-connection: включено управление подключениями частных конечных точек MySQL.</span><span class="sxs-lookup"><span data-stu-id="70a96-335">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="70a96-336">az mysql private-link-resource: включено управление ресурсами частных ссылок MySQL.</span><span class="sxs-lookup"><span data-stu-id="70a96-336">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="70a96-337">az mariadb private-endpoint-connection: включено управление подключениями частных конечных точек MariaDB.</span><span class="sxs-lookup"><span data-stu-id="70a96-337">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="70a96-338">az mariadb private-link-resource: включено управление ресурсами частных ссылок MariaDB.</span><span class="sxs-lookup"><span data-stu-id="70a96-338">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="70a96-339">Обновление тестов частной конечной точки RDBMS</span><span class="sxs-lookup"><span data-stu-id="70a96-339">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-340">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-340">SQL</span></span>

* <span data-ttu-id="70a96-341">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention.</span><span class="sxs-lookup"><span data-stu-id="70a96-341">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="70a96-342">(sql server create:) добавлен необязательный флаг включения и отключения доступа к общедоступным сетям в команду создания SQL Server.</span><span class="sxs-lookup"><span data-stu-id="70a96-342">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="70a96-343">(sql server update:) внесены некоторые изменения для клиентов.</span><span class="sxs-lookup"><span data-stu-id="70a96-343">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="70a96-344">Добавлено свойство minimal_tls_version для MI и SQL DB.</span><span class="sxs-lookup"><span data-stu-id="70a96-344">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-345">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-345">Storage</span></span>

* <span data-ttu-id="70a96-346">az storage blob delete-batch: исправлено неправильное поведение флага `--dryrun`.</span><span class="sxs-lookup"><span data-stu-id="70a96-346">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="70a96-347">az storage account network-rule add (исправление): добавлено требование того, чтобы операция была идемпотентной.</span><span class="sxs-lookup"><span data-stu-id="70a96-347">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="70a96-348">az storage account create/update: включена поддержка предпочтения маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="70a96-348">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="70a96-349">Обновлена версия azure-mgmt-storage до 8.0.0.</span><span class="sxs-lookup"><span data-stu-id="70a96-349">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="70a96-350">az storage container immutability create: добавлен параметр --allow-protected-append-write.</span><span class="sxs-lookup"><span data-stu-id="70a96-350">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="70a96-351">az storage account private-link-resource list: включена поддержка вывода списка ресурсов частной ссылки для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="70a96-351">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="70a96-352">az storage account private-endpoint-connection approve/reject/show/delete: включена поддержка управления подключениями к частным конечным точкам.</span><span class="sxs-lookup"><span data-stu-id="70a96-352">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="70a96-353">az storage account blob-service-properties update: добавлены параметры --enable-restore-policy и --restore-days.</span><span class="sxs-lookup"><span data-stu-id="70a96-353">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="70a96-354">az storage blob restore: включена поддержка восстановления диапазонов BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="70a96-354">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="70a96-355">18 февраля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-355">February 18, 2020</span></span>

<span data-ttu-id="70a96-356">Версия 2.1.0</span><span class="sxs-lookup"><span data-stu-id="70a96-356">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-357">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-357">ACR</span></span>

* <span data-ttu-id="70a96-358">Добавлен новый аргумент `--expose-token` для `az acr login`.</span><span class="sxs-lookup"><span data-stu-id="70a96-358">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="70a96-359">Исправлены неправильные выходные данные `az acr task identity show -n Name -r Registry -o table`.</span><span class="sxs-lookup"><span data-stu-id="70a96-359">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="70a96-360">az acr login: отображение CLIError при наличии ошибок, возвращаемых командой docker.</span><span class="sxs-lookup"><span data-stu-id="70a96-360">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-361">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-361">ACS</span></span>

* <span data-ttu-id="70a96-362">aks create/update: добавление проверки `--vnet-subnet-id`.</span><span class="sxs-lookup"><span data-stu-id="70a96-362">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="70a96-363">Aladdin</span><span class="sxs-lookup"><span data-stu-id="70a96-363">Aladdin</span></span>

* <span data-ttu-id="70a96-364">Выполнение синтаксического анализа созданных примеров в _help.py для команд.</span><span class="sxs-lookup"><span data-stu-id="70a96-364">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="70a96-365">AMS</span><span class="sxs-lookup"><span data-stu-id="70a96-365">AMS</span></span>

* <span data-ttu-id="70a96-366">az ams теперь предоставляется в общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="70a96-366">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="70a96-367">AppConfig</span><span class="sxs-lookup"><span data-stu-id="70a96-367">AppConfig</span></span>

* <span data-ttu-id="70a96-368">Исправлено справочное сообщение, чтобы исключить неподдерживаемый фильтр ключей или меток.</span><span class="sxs-lookup"><span data-stu-id="70a96-368">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="70a96-369">Удален тег preview для большинства команд, кроме управляемого удостоверения и флагов функций.</span><span class="sxs-lookup"><span data-stu-id="70a96-369">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="70a96-370">Добавлен управляемый ключ клиента при обновлении магазинов.</span><span class="sxs-lookup"><span data-stu-id="70a96-370">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-371">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-371">AppService</span></span>

* <span data-ttu-id="70a96-372">az webapp list-runtimes: исправлена ошибка для list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="70a96-372">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="70a96-373">Добавлена команда az webapp|functionapp config ssl create.</span><span class="sxs-lookup"><span data-stu-id="70a96-373">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="70a96-374">Включена поддержка приложений-функций версии 3 и Node 12.</span><span class="sxs-lookup"><span data-stu-id="70a96-374">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="70a96-375">ARM</span><span class="sxs-lookup"><span data-stu-id="70a96-375">ARM</span></span>

* <span data-ttu-id="70a96-376">az policy assignment create: исправлено сообщение об ошибке, если параметр `--policy` является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="70a96-376">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="70a96-377">az group deployment create: Устранена ошибка stat: path too long for Windows при использовании большого файла parameters.json.</span><span class="sxs-lookup"><span data-stu-id="70a96-377">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="70a96-378">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="70a96-378">Backup</span></span>

* <span data-ttu-id="70a96-379">Исправлен поток восстановления на уровне элемента в OLR.</span><span class="sxs-lookup"><span data-stu-id="70a96-379">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="70a96-380">Включена поддержка восстановления в виде файлов для баз данных SQL и SAP.</span><span class="sxs-lookup"><span data-stu-id="70a96-380">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="70a96-381">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="70a96-381">Compute</span></span>

* <span data-ttu-id="70a96-382">vm/vmss/availability-set update: add --ppg: разрешено обновление ProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="70a96-382">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="70a96-383">vmss create: add --data-disk-iops and --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="70a96-383">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="70a96-384">az vm host: удален тег preview для `vm host` и `vm host group`.</span><span class="sxs-lookup"><span data-stu-id="70a96-384">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="70a96-385">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправление 10728. `az vm create`: автоматическое создание подсети, если указанные виртуальная сеть и подсеть не существуют.</span><span class="sxs-lookup"><span data-stu-id="70a96-385">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="70a96-386">Повышена надежность списка образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="70a96-386">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="70a96-387">Eventhub</span><span class="sxs-lookup"><span data-stu-id="70a96-387">Eventhub</span></span>

* <span data-ttu-id="70a96-388">Включена поддержка Azure Stack для профиля 2019-03-01-hybrid.</span><span class="sxs-lookup"><span data-stu-id="70a96-388">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="70a96-389">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70a96-389">KeyVault</span></span>

* <span data-ttu-id="70a96-390">az keyvault key create: добавлено новое значение `import` для параметра `--ops`.</span><span class="sxs-lookup"><span data-stu-id="70a96-390">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="70a96-391">az keyvault key list-versions: включена поддержка параметров `--id` для определения ключей.</span><span class="sxs-lookup"><span data-stu-id="70a96-391">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="70a96-392">Включена поддержка подключений к частным конечным точкам.</span><span class="sxs-lookup"><span data-stu-id="70a96-392">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="70a96-393">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-393">Network</span></span>

* <span data-ttu-id="70a96-394">Выполнена активация azure-mgmt-network 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="70a96-394">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="70a96-395">az network private-link-service update/create: включена поддержка --enable-proxy-protocol.</span><span class="sxs-lookup"><span data-stu-id="70a96-395">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="70a96-396">Добавлена функция монитора подключения версии 2.</span><span class="sxs-lookup"><span data-stu-id="70a96-396">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="70a96-397">Упаковка</span><span class="sxs-lookup"><span data-stu-id="70a96-397">Packaging</span></span>

* <span data-ttu-id="70a96-398">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка Python 2.7.</span><span class="sxs-lookup"><span data-stu-id="70a96-398">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="70a96-399">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-399">Profile</span></span>

* <span data-ttu-id="70a96-400">Предварительный просмотр: В учетные записи подписок добавлены новые атрибуты `homeTenantId` и `managedByTenants`.</span><span class="sxs-lookup"><span data-stu-id="70a96-400">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="70a96-401">Чтобы изменения вступили в силу, повторно выполните команду `az login`.</span><span class="sxs-lookup"><span data-stu-id="70a96-401">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="70a96-402">az login: отображение предупреждения, если подписка связана с несколькими клиентами, но по умолчанию используется с первым из них</span><span class="sxs-lookup"><span data-stu-id="70a96-402">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="70a96-403">(чтобы выбрать определенный клиент при доступе к этой подписке, включите `--tenant` в `az login`).</span><span class="sxs-lookup"><span data-stu-id="70a96-403">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="70a96-404">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-404">Role</span></span>

* <span data-ttu-id="70a96-405">az role assignment create: исправлена ошибка с кодом HTTP 400, возникающая при присвоении роли субъекту-службе по отображаемому имени.</span><span class="sxs-lookup"><span data-stu-id="70a96-405">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-406">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-406">SQL</span></span>

* <span data-ttu-id="70a96-407">Обновлен командлет `az sql mi update` Управляемого экземпляра SQL (добавлены два новых параметра: tier и family).</span><span class="sxs-lookup"><span data-stu-id="70a96-407">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-408">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-408">Storage</span></span>

* <span data-ttu-id="70a96-409">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az storage account create`: Тип учетной записи хранения по умолчанию изменен на StorageV2.</span><span class="sxs-lookup"><span data-stu-id="70a96-409">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="70a96-410">4 февраля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-410">February 04, 2020</span></span>

<span data-ttu-id="70a96-411">Версия 2.0.81</span><span class="sxs-lookup"><span data-stu-id="70a96-411">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-412">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-412">ACS</span></span>

* <span data-ttu-id="70a96-413">Добавлена возможность задания выделенных исходящих портов и времени ожидания подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="70a96-413">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="70a96-414">Выполнено обновление до API версии 2019-11-01.</span><span class="sxs-lookup"><span data-stu-id="70a96-414">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-415">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-415">ACR</span></span>

* <span data-ttu-id="70a96-416">[Критическое изменение] `az acr delete` будет выводить запрос.</span><span class="sxs-lookup"><span data-stu-id="70a96-416">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="70a96-417">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда az acr task delete будет выводить запрос.</span><span class="sxs-lookup"><span data-stu-id="70a96-417">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="70a96-418">Добавлена новая группа команд az acr taskrun show/list/delete для управления выполнением задач.</span><span class="sxs-lookup"><span data-stu-id="70a96-418">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="70a96-419">AKS</span><span class="sxs-lookup"><span data-stu-id="70a96-419">AKS</span></span>

* <span data-ttu-id="70a96-420">Каждый кластер получает отдельный субъект-службу для улучшения изоляции.</span><span class="sxs-lookup"><span data-stu-id="70a96-420">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="70a96-421">AppConfig</span><span class="sxs-lookup"><span data-stu-id="70a96-421">AppConfig</span></span>

* <span data-ttu-id="70a96-422">Поддержка импорта ссылок на хранилище ключей из службы приложений и их экспорта в нее.</span><span class="sxs-lookup"><span data-stu-id="70a96-422">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="70a96-423">Поддержка импорта и экспорта всех меток между файлами appconfig.</span><span class="sxs-lookup"><span data-stu-id="70a96-423">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="70a96-424">Проверка имен ключей и функций перед настройкой и импортом.</span><span class="sxs-lookup"><span data-stu-id="70a96-424">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="70a96-425">Предоставление изменений номера SKU в хранилище конфигураций.</span><span class="sxs-lookup"><span data-stu-id="70a96-425">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="70a96-426">Новая группа команд для управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="70a96-426">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-427">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-427">AppService</span></span>

* <span data-ttu-id="70a96-428">Azure Stack: команды поверхности в профиле 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="70a96-428">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="70a96-429">functionapp: добавлена возможность создавать приложения-функции Java в Linux.</span><span class="sxs-lookup"><span data-stu-id="70a96-429">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="70a96-430">ARM</span><span class="sxs-lookup"><span data-stu-id="70a96-430">ARM</span></span>

* <span data-ttu-id="70a96-431">Исправление ошибки 10246: аварийное завершение `az resource tag` в случае, если переданный параметр `--ids` являлся идентификатором группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70a96-431">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="70a96-432">Исправление ошибки 11658: команда `az group export` не поддерживала параметры `--query` и `--output`.</span><span class="sxs-lookup"><span data-stu-id="70a96-432">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="70a96-433">Исправление ошибки 10279: код выхода `az group deployment validate` был равен 0, если проверка не пройдена.</span><span class="sxs-lookup"><span data-stu-id="70a96-433">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="70a96-434">Исправление ошибки 9916: улучшено сообщение об ошибке из-за конфликта между тегом и другими условиями фильтра для команды `az resource list`.</span><span class="sxs-lookup"><span data-stu-id="70a96-434">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="70a96-435">Добавлен новый параметр `--managed-by` для добавления данных managedBy для команды `az group create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-435">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="70a96-436">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="70a96-436">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="70a96-437">Добавлена подгруппа `monitor` для управления мониторингом Log Analytics в кластере Azure Red Hat OpensShift.</span><span class="sxs-lookup"><span data-stu-id="70a96-437">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="70a96-438">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="70a96-438">BotService</span></span>

* <span data-ttu-id="70a96-439">Исправление ошибки 11697: команда `az bot create` не являлась идемпотентной.</span><span class="sxs-lookup"><span data-stu-id="70a96-439">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="70a96-440">Проверки исправления имен изменены для выполнения только в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="70a96-440">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="70a96-441">CDN</span><span class="sxs-lookup"><span data-stu-id="70a96-441">CDN</span></span>

* <span data-ttu-id="70a96-442">Добавлена поддержка функции rulesEngine.</span><span class="sxs-lookup"><span data-stu-id="70a96-442">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="70a96-443">Добавлена новая группа команд cdn endpoint rule для управления правилами.</span><span class="sxs-lookup"><span data-stu-id="70a96-443">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="70a96-444">Пакет azure-mgmt-cdn обновлен до версии 4.0.0 для использования API версии 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="70a96-444">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="70a96-445">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="70a96-445">Deployment Manager</span></span>

* <span data-ttu-id="70a96-446">Добавлена операция вывода списка всех ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70a96-446">Add list operation for all resources.</span></span>
* <span data-ttu-id="70a96-447">Улучшен ресурс шага для нового типа шага.</span><span class="sxs-lookup"><span data-stu-id="70a96-447">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="70a96-448">Пакет azure-mgmt-deploymentmanager обновлен для использования версии 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="70a96-448">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="70a96-449">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-449">IoT</span></span>

* <span data-ttu-id="70a96-450">Команды IoT hub Job объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="70a96-450">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="70a96-451">IoT Central</span><span class="sxs-lookup"><span data-stu-id="70a96-451">IoT Central</span></span>

* <span data-ttu-id="70a96-452">Добавлена поддержка создания и обновления приложений с новыми SKU: ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="70a96-452">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="70a96-453">Key Vault</span><span class="sxs-lookup"><span data-stu-id="70a96-453">Key Vault</span></span>

* <span data-ttu-id="70a96-454">Добавлена новая команда `az keyvault key download` для скачивания ключей.</span><span class="sxs-lookup"><span data-stu-id="70a96-454">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="70a96-455">Разное</span><span class="sxs-lookup"><span data-stu-id="70a96-455">Misc</span></span>

* <span data-ttu-id="70a96-456">Исправление ошибки 6371: поддержка завершения имен файлов и переменных среды в Bash.</span><span class="sxs-lookup"><span data-stu-id="70a96-456">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="70a96-457">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-457">Network</span></span>

* <span data-ttu-id="70a96-458">Исправление ошибки 2092: для команды az network dns record-set add/remove добавлено предупреждение, отображаемое, если набор записей не найден.</span><span class="sxs-lookup"><span data-stu-id="70a96-458">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="70a96-459">В будущем для подтверждения этого автоматического создания будет добавлен дополнительный аргумент.</span><span class="sxs-lookup"><span data-stu-id="70a96-459">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="70a96-460">Политика</span><span class="sxs-lookup"><span data-stu-id="70a96-460">Policy</span></span>

* <span data-ttu-id="70a96-461">Добавлена новая команда `az policy metadata` для получения ресурсов метаданных расширенной политики.</span><span class="sxs-lookup"><span data-stu-id="70a96-461">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="70a96-462">`az policy remediation create`: С помощью параметра `--resource-discovery-mode` можно указать, следует ли повторно оценить соответствие перед исправлением.</span><span class="sxs-lookup"><span data-stu-id="70a96-462">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="70a96-463">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-463">Profile</span></span>

* <span data-ttu-id="70a96-464">`az account get-access-token`: Добавлен параметр `--tenant` для получения маркера для арендатора напрямую, без необходимости указывать подписку.</span><span class="sxs-lookup"><span data-stu-id="70a96-464">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="70a96-465">RBAC</span><span class="sxs-lookup"><span data-stu-id="70a96-465">RBAC</span></span>

* <span data-ttu-id="70a96-466">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправление ошибки 11883: `az role assignment create`: пустая область приведет к ошибке.</span><span class="sxs-lookup"><span data-stu-id="70a96-466">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="70a96-467">Безопасность</span><span class="sxs-lookup"><span data-stu-id="70a96-467">Security</span></span>

* <span data-ttu-id="70a96-468">Добавлены новые команды `az atp show` и `az atp update` для просмотра и настройки дополнительных параметров защиты от угроз для учетных записей хранения.</span><span class="sxs-lookup"><span data-stu-id="70a96-468">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-469">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-469">SQL</span></span>

* <span data-ttu-id="70a96-470">`sql dw create`: параметры `--zone-redundant` и `--read-replica-count` объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="70a96-470">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="70a96-471">Эти параметры не применяются к хранилищу данных.</span><span class="sxs-lookup"><span data-stu-id="70a96-471">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="70a96-472">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql db create`: Значения WideWorldImportersStd и WideWorldImportersFull больше не являются задокументированным допустимыми значениями для команды az sql db create --sample-name.</span><span class="sxs-lookup"><span data-stu-id="70a96-472">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="70a96-473">Эти примеры базы данных всегда будут приводить к сбою создания.</span><span class="sxs-lookup"><span data-stu-id="70a96-473">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="70a96-474">Добавлены новые команды `sql db classification show/list/update/delete` и `sql db classification recommendation list/enable/disable` для управления классификациями конфиденциальности баз данных SQL.</span><span class="sxs-lookup"><span data-stu-id="70a96-474">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="70a96-475">`az sql db audit-policy`: устранены пустые действия аудита и группы.</span><span class="sxs-lookup"><span data-stu-id="70a96-475">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-476">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-476">Storage</span></span>

* <span data-ttu-id="70a96-477">Добавлена новая группа команд `az storage share-rm` для использования поставщика ресурсов Microsoft.Storage в операциях управления файловыми ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="70a96-477">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="70a96-478">Исправление ошибки 11415: ошибка разрешения для `az storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-478">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="70a96-479">Добавлены интеграция AzCopy 10.3.3 и поддержка Win32.</span><span class="sxs-lookup"><span data-stu-id="70a96-479">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="70a96-480">`az storage copy`: добавлены параметры `--include-path`, `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="70a96-480">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="70a96-481">`az storage remove`: параметры `--inlcude` и `--exclude` заменены параметрами `--include-path`, `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="70a96-481">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="70a96-482">`az storage sync`: добавлены параметры `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="70a96-482">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="70a96-483">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="70a96-483">ServiceFabric</span></span>

* <span data-ttu-id="70a96-484">Добавлены новые команды для управления приложениями и службами.</span><span class="sxs-lookup"><span data-stu-id="70a96-484">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="70a96-485">13 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-485">January 13, 2020</span></span>

<span data-ttu-id="70a96-486">Версия 2.0.80</span><span class="sxs-lookup"><span data-stu-id="70a96-486">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="70a96-487">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="70a96-487">Compute</span></span>

* <span data-ttu-id="70a96-488">Обновление диска: добавлены параметры --disk-encryption-set и --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="70a96-488">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="70a96-489">Создание и обновление моментального снимка: добавлены параметры --disk-encryption-set и --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="70a96-489">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-490">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-490">Storage</span></span>

* <span data-ttu-id="70a96-491">Обновление azure-mgmt-storage до версии 7.1.0</span><span class="sxs-lookup"><span data-stu-id="70a96-491">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="70a96-492">`az storage account create`: добавлены параметры `--encryption-key-type-for-table` и `--encryption-key-type-for-queue` для включения поддержки службы шифрования таблиц и очередей.</span><span class="sxs-lookup"><span data-stu-id="70a96-492">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="70a96-493">7 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-493">January 07, 2020</span></span>

<span data-ttu-id="70a96-494">Версия 2.0.79</span><span class="sxs-lookup"><span data-stu-id="70a96-494">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-495">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-495">ACR</span></span>

* <span data-ttu-id="70a96-496">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --os для команд acr build, acr task create/update, acr run и acr pack.</span><span class="sxs-lookup"><span data-stu-id="70a96-496">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="70a96-497">Вместо этого используется параметр --platform.</span><span class="sxs-lookup"><span data-stu-id="70a96-497">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="70a96-498">AppConfig</span><span class="sxs-lookup"><span data-stu-id="70a96-498">AppConfig</span></span>

* <span data-ttu-id="70a96-499">Добавлена поддержка импорта и экспорта флагов функций.</span><span class="sxs-lookup"><span data-stu-id="70a96-499">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="70a96-500">Добавлена новая команда az appconfig kv set-keyvault для создания ссылки на хранилище ключей.</span><span class="sxs-lookup"><span data-stu-id="70a96-500">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="70a96-501">Добавлена поддержка различных соглашений об именовании при экспорте флагов функций в файл.</span><span class="sxs-lookup"><span data-stu-id="70a96-501">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-502">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-502">AppService</span></span>

* <span data-ttu-id="70a96-503">Устранена проблема № 7154: обновлена документация по команде <> — теперь в ней используются обратные, а не одинарные кавычки.</span><span class="sxs-lookup"><span data-stu-id="70a96-503">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="70a96-504">Устранена проблема № 11287 (webapp up): по умолчанию для приложения, созданного с использованием этого флага, должен быть включен SSL.</span><span class="sxs-lookup"><span data-stu-id="70a96-504">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="70a96-505">Устранена проблема № 11592: добавлен флаг az webapp up для статических сайтов HTML.</span><span class="sxs-lookup"><span data-stu-id="70a96-505">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="70a96-506">ARM</span><span class="sxs-lookup"><span data-stu-id="70a96-506">ARM</span></span>

* <span data-ttu-id="70a96-507">Исправлена ошибка с командой `az resource tag`: невозможно было обновить теги хранилища Служб восстановления.</span><span class="sxs-lookup"><span data-stu-id="70a96-507">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="70a96-508">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="70a96-508">Backup</span></span>

* <span data-ttu-id="70a96-509">Добавлена новая команда backup protection undelete для включения функции обратимого удаления рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="70a96-509">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="70a96-510">Добавлен новый параметр --soft-delete-feature-state для команды set backup-properties.</span><span class="sxs-lookup"><span data-stu-id="70a96-510">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="70a96-511">Добавлена поддержка исключения диска для рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="70a96-511">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="70a96-512">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="70a96-512">Compute</span></span>

* <span data-ttu-id="70a96-513">Исправлен сбой `vm create` в профиле Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="70a96-513">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="70a96-514">Добавлена поддержка определений списков и метрик запросов для виртуальной машины (vm monitor metrics tail/list-definitions).</span><span class="sxs-lookup"><span data-stu-id="70a96-514">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="70a96-515">Добавлено новое действия повторного применения команды az vm</span><span class="sxs-lookup"><span data-stu-id="70a96-515">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="70a96-516">HDInsight</span><span class="sxs-lookup"><span data-stu-id="70a96-516">HDInsight</span></span>

* <span data-ttu-id="70a96-517">Включена поддержка создания кластера Kafka с помощью прокси-сервера Kafka RESTful.</span><span class="sxs-lookup"><span data-stu-id="70a96-517">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="70a96-518">Обновление azure-mgmt-hdinsight до версии 1.3.0</span><span class="sxs-lookup"><span data-stu-id="70a96-518">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="70a96-519">Прочее</span><span class="sxs-lookup"><span data-stu-id="70a96-519">Misc.</span></span>

* <span data-ttu-id="70a96-520">Добавлена команда `az version show` предварительного просмотра для отображения версий модулей и расширений Azure CLI в формате JSON по умолчанию или в формате, настроенном с помощью параметра --output</span><span class="sxs-lookup"><span data-stu-id="70a96-520">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="70a96-521">Центры событий</span><span class="sxs-lookup"><span data-stu-id="70a96-521">Event Hubs</span></span>

* <span data-ttu-id="70a96-522">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az eventhubs eventhub update и az eventhubs eventhub create.</span><span class="sxs-lookup"><span data-stu-id="70a96-522">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="70a96-523">Данный параметр недопустим для сущностей концентратора событий.</span><span class="sxs-lookup"><span data-stu-id="70a96-523">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="70a96-524">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="70a96-524">Service Bus</span></span>

* <span data-ttu-id="70a96-525">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az servicebus topic create, az servicebus topic update, az servicebus queue create и az servicebus queue update.</span><span class="sxs-lookup"><span data-stu-id="70a96-525">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="70a96-526">Этот параметр является недопустимым для разделов и очередей служебной шины.</span><span class="sxs-lookup"><span data-stu-id="70a96-526">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="70a96-527">RBAC</span><span class="sxs-lookup"><span data-stu-id="70a96-527">RBAC</span></span>

* <span data-ttu-id="70a96-528">Устранена проблема № 11712: команда `az ad app/sp show` не возвращала код выхода 3, если приложение или субъект-служба не существует.</span><span class="sxs-lookup"><span data-stu-id="70a96-528">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-529">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-529">Storage</span></span>

* <span data-ttu-id="70a96-530">`az storage account create`: удален флаг предварительного просмотра для параметра --enable-hierarchical-namespace.</span><span class="sxs-lookup"><span data-stu-id="70a96-530">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="70a96-531">Хранилище azure-mgmt-storage обновлено до версии 7.0.0 для использования API версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="70a96-531">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="70a96-532">Добавлены новые параметры (`--enable-delete-retention` и `--delete-retention-days`) для поддержки управления политикой хранения удаленных свойств службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="70a96-532">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="70a96-533">17 декабря 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-533">December 17, 2019</span></span>

<span data-ttu-id="70a96-534">2.0.78</span><span class="sxs-lookup"><span data-stu-id="70a96-534">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-535">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-535">ACR</span></span>

* <span data-ttu-id="70a96-536">Добавлена поддержка локального контекста во время выполнения задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="70a96-536">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-537">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-537">ACS</span></span>

* <span data-ttu-id="70a96-538">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде az openshift create параметр `--workspace-resource-id` переименован на `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="70a96-538">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="70a96-539">AMS</span><span class="sxs-lookup"><span data-stu-id="70a96-539">AMS</span></span>

* <span data-ttu-id="70a96-540">Команды show обновлены для возвращения ответа 3, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="70a96-540">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="70a96-541">AppConfig</span><span class="sxs-lookup"><span data-stu-id="70a96-541">AppConfig</span></span>

* <span data-ttu-id="70a96-542">Исправлена ошибка, возникающая при добавлении api-version в URL-адрес запроса.</span><span class="sxs-lookup"><span data-stu-id="70a96-542">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="70a96-543">Имеющееся решение не работает с разбивкой на страницы.</span><span class="sxs-lookup"><span data-stu-id="70a96-543">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="70a96-544">Добавлена поддержка отображения языков, кроме английского, так как наша внутренняя служба поддерживает Юникод для глобализации.</span><span class="sxs-lookup"><span data-stu-id="70a96-544">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-545">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-545">AppService</span></span>

* <span data-ttu-id="70a96-546">Устранена проблема № 11217 (webapp): теперь команда az webapp config ssl upload поддерживает параметр слота.</span><span class="sxs-lookup"><span data-stu-id="70a96-546">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="70a96-547">Устранена проблема № 10965. Ошибка: Имя не может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="70a96-547">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="70a96-548">Разрешено удаление по IP-адресу и подсети.</span><span class="sxs-lookup"><span data-stu-id="70a96-548">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="70a96-549">Добавлена поддержка импорта сертификатов из хранилища ключей: `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="70a96-549">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="70a96-550">ARM</span><span class="sxs-lookup"><span data-stu-id="70a96-550">ARM</span></span>

* <span data-ttu-id="70a96-551">Обновлен пакет ресурсов azure-mgmt-resource для использования версии 6.0.0</span><span class="sxs-lookup"><span data-stu-id="70a96-551">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="70a96-552">Добавлена межклиентская поддержка команды `az group deployment create` путем добавления нового параметра `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="70a96-552">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="70a96-553">Добавлен новый параметр `--metadata` для поддержки добавления метаданных определений наборов политик.</span><span class="sxs-lookup"><span data-stu-id="70a96-553">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="70a96-554">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="70a96-554">Backup</span></span>

* <span data-ttu-id="70a96-555">Добавлена поддержка резервного копирования для рабочей нагрузки SQL и SAP HANA.</span><span class="sxs-lookup"><span data-stu-id="70a96-555">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="70a96-556">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="70a96-556">BotService</span></span>

* <span data-ttu-id="70a96-557">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг --version из предварительной версии команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="70a96-557">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="70a96-558">Поддерживаются только боты пакетов SDK версии 4.</span><span class="sxs-lookup"><span data-stu-id="70a96-558">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="70a96-559">Добавлена проверка доступности имени для команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="70a96-559">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="70a96-560">Добавлена поддержка обновления URL-адреса значка для бота с помощью команды az bot update.</span><span class="sxs-lookup"><span data-stu-id="70a96-560">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="70a96-561">Добавлена поддержка обновления канала Direct Line с помощью команды az bot directline update.</span><span class="sxs-lookup"><span data-stu-id="70a96-561">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="70a96-562">Добавлена поддержка флага --enable-enhanced-auth в команде az bot directline create.</span><span class="sxs-lookup"><span data-stu-id="70a96-562">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="70a96-563">Следующие группы команд предоставляются в общедоступной, а не в предварительной версии: az bot authsetting.</span><span class="sxs-lookup"><span data-stu-id="70a96-563">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="70a96-564">Следующие команды в az bot предоставляются в общедоступной, а не в предварительной версии: create, prepare-deploy, show, delete и update.</span><span class="sxs-lookup"><span data-stu-id="70a96-564">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="70a96-565">Устранена проблема с командой az bot prepare-deploy, которая изменяла значение параметра --proj-file-path на нижний регистр (например, с Test.csproj на test.csproj).</span><span class="sxs-lookup"><span data-stu-id="70a96-565">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="70a96-566">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="70a96-566">Compute</span></span>

* <span data-ttu-id="70a96-567">vmss create/update: добавлен параметр --scale-on-policy, который определяет, какие виртуальные машины выбираются для удаления при масштабировании VMSS.</span><span class="sxs-lookup"><span data-stu-id="70a96-567">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="70a96-568">vm/vmss update: добавлен параметр --priority.</span><span class="sxs-lookup"><span data-stu-id="70a96-568">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="70a96-569">vm/vmss update: добавлен параметр --max-price.</span><span class="sxs-lookup"><span data-stu-id="70a96-569">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="70a96-570">Добавлена группа команд для шифрования дисков (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="70a96-570">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="70a96-571">disk create: добавлены параметры --encryption-type и --disk-encryption-set.</span><span class="sxs-lookup"><span data-stu-id="70a96-571">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="70a96-572">vm/vmss create. Добавлены параметры --os-disk-encryption-set и --data-disk-encryption-sets.</span><span class="sxs-lookup"><span data-stu-id="70a96-572">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="70a96-573">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-573">Core</span></span>

* <span data-ttu-id="70a96-574">Удалена поддержка Python версии 3.4.</span><span class="sxs-lookup"><span data-stu-id="70a96-574">Removed support for Python 3.4</span></span>
* <span data-ttu-id="70a96-575">Подключение к опросу HaTS в нескольких командах.</span><span class="sxs-lookup"><span data-stu-id="70a96-575">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="70a96-576">DLS</span><span class="sxs-lookup"><span data-stu-id="70a96-576">DLS</span></span>

* <span data-ttu-id="70a96-577">Обновлена версия пакета SDK для ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="70a96-577">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="70a96-578">Установка</span><span class="sxs-lookup"><span data-stu-id="70a96-578">Install</span></span>

* <span data-ttu-id="70a96-579">Добавлена поддержка установки скриптов Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="70a96-579">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="70a96-580">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-580">IOT</span></span>

* <span data-ttu-id="70a96-581">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --failover-region из команды manual-failover.</span><span class="sxs-lookup"><span data-stu-id="70a96-581">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="70a96-582">Теперь она будет выполнять отработку отказа в назначенный геопарный дополнительный регион.</span><span class="sxs-lookup"><span data-stu-id="70a96-582">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="70a96-583">Key Vault</span><span class="sxs-lookup"><span data-stu-id="70a96-583">Key Vault</span></span>

* <span data-ttu-id="70a96-584">Устранена проблема № 8095: (`az keyvault storage remove`): улучшено справочное сообщение.</span><span class="sxs-lookup"><span data-stu-id="70a96-584">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="70a96-585">Устранена проблема № 8921 (`az keyvault key/secret/certificate list/list-deleted/list-versions`): исправлена ошибка проверки в параметре `--maxresults`.</span><span class="sxs-lookup"><span data-stu-id="70a96-585">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="70a96-586">Устранена проблема № 10512 (`az keyvault set-policy`): улучшено сообщение об ошибке, возвращаемое, если не указан ни один из параметров `--object-id`, `--spn` или `--upn`.</span><span class="sxs-lookup"><span data-stu-id="70a96-586">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="70a96-587">Устранена проблема № 10846 (`az keyvault secret show-deleted`): при указании значения `--id` значение `--name/-n` не требовалось.</span><span class="sxs-lookup"><span data-stu-id="70a96-587">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="70a96-588">Устранена проблема № 11084: (`az keyvault secret download`): улучшено справочное сообщение параметра `--encoding`.</span><span class="sxs-lookup"><span data-stu-id="70a96-588">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="70a96-589">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-589">Network</span></span>

* <span data-ttu-id="70a96-590">az network application-gateway probe: добавлена поддержка параметра --port, позволяющего указать порт, который используется для проверки внутренних серверов при создании и обновлении.</span><span class="sxs-lookup"><span data-stu-id="70a96-590">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="70a96-591">az network application-gateway url-path-map create/update: исправлена ошибка с `--waf-policy`.</span><span class="sxs-lookup"><span data-stu-id="70a96-591">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="70a96-592">az network application-gateway: добавлена поддержка параметра `--rewrite-rule-set`.</span><span class="sxs-lookup"><span data-stu-id="70a96-592">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="70a96-593">az network list-service-aliases: добавлена поддержка перечисления псевдонимов служб, которые можно использовать для политик конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="70a96-593">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="70a96-594">az network dns zone import: добавлена поддержка символа .@ в имени записи.</span><span class="sxs-lookup"><span data-stu-id="70a96-594">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="70a96-595">Упаковка</span><span class="sxs-lookup"><span data-stu-id="70a96-595">Packaging</span></span>

* <span data-ttu-id="70a96-596">Снова добавлены сборки Edge для установки PIP.</span><span class="sxs-lookup"><span data-stu-id="70a96-596">Added back edge builds for pip install</span></span>
* <span data-ttu-id="70a96-597">Добавлен пакет Ubuntu eoan.</span><span class="sxs-lookup"><span data-stu-id="70a96-597">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="70a96-598">Политика</span><span class="sxs-lookup"><span data-stu-id="70a96-598">Policy</span></span>

* <span data-ttu-id="70a96-599">Добавлена поддержка API Политики версии 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="70a96-599">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="70a96-600">az policy set-definition: добавлена поддержка группирования в определениях наборов политик с помощью параметра `--definition-groups`.</span><span class="sxs-lookup"><span data-stu-id="70a96-600">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="70a96-601">Redis</span><span class="sxs-lookup"><span data-stu-id="70a96-601">Redis</span></span>

* <span data-ttu-id="70a96-602">В команду `az redis create` добавлена предварительная версия параметра `--replicas-per-master`.</span><span class="sxs-lookup"><span data-stu-id="70a96-602">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="70a96-603">Обновлена версия azure-mgmt-redis с 6.0.0 на 7.0.0 RC1.</span><span class="sxs-lookup"><span data-stu-id="70a96-603">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="70a96-604">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="70a96-604">ServiceFabric</span></span>

* <span data-ttu-id="70a96-605">Исправлена логика добавления типа узла, а также устранена проблема № 10963: при добавлении нового типа узла с уровнем устойчивости Gold возникала ошибка CLI.</span><span class="sxs-lookup"><span data-stu-id="70a96-605">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="70a96-606">Обновлена версия параметра ServiceFabricNodeVmExt до 1.1 в шаблоне создания.</span><span class="sxs-lookup"><span data-stu-id="70a96-606">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-607">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-607">SQL</span></span>

* <span data-ttu-id="70a96-608">В команды create и update базы данных SQL добавлены параметры --read-scale и --read-replicas для поддержки управления масштабированием операций чтения.</span><span class="sxs-lookup"><span data-stu-id="70a96-608">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-609">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-609">Storage</span></span>

* <span data-ttu-id="70a96-610">Выпущена общедоступная версия больших файловых ресурсов для команды создания и обновления учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="70a96-610">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="70a96-611">Выпущена общедоступная версия поддержки маркера SAS для делегирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="70a96-611">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="70a96-612">Добавлены новые команды (`az storage account blob-service-properties show` и `az storage account blob-service-properties update --enable-change-feed`) для управления свойствами службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="70a96-612">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="70a96-613">[ОЖИДАЕТСЯ КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] `az storage copy`: символ `*` больше не поддерживается в качестве подстановочного знака в URL-адресе. Тем не менее новые параметры--include-pattern и--exclude-pattern будут добавлены с поддержкой подстановочных знаков `*`.</span><span class="sxs-lookup"><span data-stu-id="70a96-613">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="70a96-614">Устранена проблема № 11043: добавлена поддержка удаления всего контейнера или общего ресурса в команде `az storage remove`.</span><span class="sxs-lookup"><span data-stu-id="70a96-614">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="70a96-615">26 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-615">November 26, 2019</span></span>

<span data-ttu-id="70a96-616">Версия 2.0.77</span><span class="sxs-lookup"><span data-stu-id="70a96-616">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-617">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-617">ACR</span></span>

* <span data-ttu-id="70a96-618">Параметр `--branch`, используемый при обновлении или создании задачи ACR, объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="70a96-618">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="70a96-619">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="70a96-619">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="70a96-620">Добавлен флаг `--workspace-resource-id` для создания кластера Azure Red Hat Openshift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="70a96-620">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="70a96-621">Добавлен флаг `monitor_profile` для создания кластера Azure Red Hat OpenShift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="70a96-621">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="70a96-622">AKS</span><span class="sxs-lookup"><span data-stu-id="70a96-622">AKS</span></span>

* <span data-ttu-id="70a96-623">Включена поддержка операции смены сертификата кластера с использованием команды az aks rotate-certs.</span><span class="sxs-lookup"><span data-stu-id="70a96-623">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="70a96-624">AppConfig</span><span class="sxs-lookup"><span data-stu-id="70a96-624">AppConfig</span></span>

* <span data-ttu-id="70a96-625">Включена поддержка использования символа ":" для разделителя `as az appconfig kv import`.</span><span class="sxs-lookup"><span data-stu-id="70a96-625">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="70a96-626">Исправлена проблема с перечислением значений ключей с несколькими метками, включая метку NULL.</span><span class="sxs-lookup"><span data-stu-id="70a96-626">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="70a96-627">Обновлен пакет SDK для плоскости управления, azure-mgmt-appconfiguration, до версии 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="70a96-627">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="70a96-628">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-628">AppService</span></span>

* <span data-ttu-id="70a96-629">Исправлена ошибка № 11100. Использование AttributeError для az webapp up при создании плана службы.</span><span class="sxs-lookup"><span data-stu-id="70a96-629">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="70a96-630">az webapp up. При принудительном создании или развертывании сайта для поддерживаемых языков значения по умолчанию не используются.</span><span class="sxs-lookup"><span data-stu-id="70a96-630">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="70a96-631">Включена поддержка Среды службы приложений: az appservice ase show | list | list-addresses | list-plans | create | update | delete.</span><span class="sxs-lookup"><span data-stu-id="70a96-631">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="70a96-632">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="70a96-632">Backup</span></span>

* <span data-ttu-id="70a96-633">Исправлена проблема в команде az backup policy list-associated-items.</span><span class="sxs-lookup"><span data-stu-id="70a96-633">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="70a96-634">Добавлен необязательный параметр BackupManagementType.</span><span class="sxs-lookup"><span data-stu-id="70a96-634">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="70a96-635">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="70a96-635">Compute</span></span>

* <span data-ttu-id="70a96-636">Обновлена версия API вычислений, дисков, моментальных снимков до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="70a96-636">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="70a96-637">vmss create. Улучшение для --orchestration-mode.</span><span class="sxs-lookup"><span data-stu-id="70a96-637">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="70a96-638">sig image-definition create. Добавлен параметр --os-state для указания того, являются ли виртуальные машины, созданные в этом образе, универсальными или специализированными.</span><span class="sxs-lookup"><span data-stu-id="70a96-638">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="70a96-639">sig image-definition create. Добавлен параметр --hyper-v-generation для указания создания гипервизора.</span><span class="sxs-lookup"><span data-stu-id="70a96-639">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="70a96-640">sig image-version create. Включена поддержка параметров --os-snapshot и --data-snapshots.</span><span class="sxs-lookup"><span data-stu-id="70a96-640">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="70a96-641">image create. Включена поддержка параметра --data-disk-caching для указания параметра кэширования для дисков данных.</span><span class="sxs-lookup"><span data-stu-id="70a96-641">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="70a96-642">Обновлена версия пакета SDK для вычислений Python до 10.0.0.</span><span class="sxs-lookup"><span data-stu-id="70a96-642">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="70a96-643">vm/vmss create. Добавлен фрагмент Spot в свойство перечисления Priority.</span><span class="sxs-lookup"><span data-stu-id="70a96-643">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="70a96-644">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименование параметра --max-billing в --max-price для виртуальных машин и Масштабируемых наборов виртуальных машин в соответствии с командлетами Swagger и PowerShell.</span><span class="sxs-lookup"><span data-stu-id="70a96-644">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="70a96-645">vm monitor log show. Включена поддержка запроса журналов в связанной рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="70a96-645">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="70a96-646">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-646">IOT</span></span>

* <span data-ttu-id="70a96-647">Исправление № 2531. Добавлены вспомогательные аргументы для обновления концентратора.</span><span class="sxs-lookup"><span data-stu-id="70a96-647">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="70a96-648">Исправление № 8323. Добавлены недостающие параметры для создания пользовательской конечной точки хранилища.</span><span class="sxs-lookup"><span data-stu-id="70a96-648">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="70a96-649">Исправлена ошибка регрессии. Отменены изменения, переопределяющие конечную точку хранилища по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-649">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="70a96-650">Key Vault</span><span class="sxs-lookup"><span data-stu-id="70a96-650">Key Vault</span></span>

* <span data-ttu-id="70a96-651">Исправление № 11121. При использовании `az keyvault certificate list` для передачи `--include-pending` теперь не требуется значение `true` или `false`.</span><span class="sxs-lookup"><span data-stu-id="70a96-651">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="70a96-652">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="70a96-652">NetAppFiles</span></span>

* <span data-ttu-id="70a96-653">Обновлена версия azure-mgmt-netapp до 0.7.0, которая включает некоторые дополнительные свойства тома, связанные с предстоящими операциями репликации.</span><span class="sxs-lookup"><span data-stu-id="70a96-653">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="70a96-654">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-654">Network</span></span>

* <span data-ttu-id="70a96-655">application-gateway waf-config. Не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="70a96-655">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="70a96-656">application-gateway waf-policy. Добавлены управляемые правила подгрупп для контроля управляемых наборов правил и правил исключения.</span><span class="sxs-lookup"><span data-stu-id="70a96-656">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="70a96-657">application-gateway waf-policy. Добавлен параметр политики подгруппы для управления глобальной конфигурацией политики WAF.</span><span class="sxs-lookup"><span data-stu-id="70a96-657">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="70a96-658">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] application-gateway waf-policy. Переименовано правило подгруппы в пользовательское правило.</span><span class="sxs-lookup"><span data-stu-id="70a96-658">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="70a96-659">application-gateway http-listener. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="70a96-659">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="70a96-660">application-gateway url-path-map rule. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="70a96-660">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="70a96-661">Упаковка</span><span class="sxs-lookup"><span data-stu-id="70a96-661">Packaging</span></span>

* <span data-ttu-id="70a96-662">Удалена команда az wrapper в Python.</span><span class="sxs-lookup"><span data-stu-id="70a96-662">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="70a96-663">Включена поддержка Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="70a96-663">Added support for Python 3.8</span></span>
* <span data-ttu-id="70a96-664">Изменена версия на Python 3 для пакета RPM.</span><span class="sxs-lookup"><span data-stu-id="70a96-664">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="70a96-665">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-665">Profile</span></span>

* <span data-ttu-id="70a96-666">Исправлена ошибка при выполнении `az login -u {} -p {}` с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="70a96-666">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="70a96-667">Исправлена ошибка с `SSLError` при выполнении `az login` за прокси-сервером с самозаверяющим корневым сертификатом.</span><span class="sxs-lookup"><span data-stu-id="70a96-667">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="70a96-668">Исправлена ошибка № 10578. `az login` зависает при одновременном запуске нескольких экземпляров в Windows или WSL.</span><span class="sxs-lookup"><span data-stu-id="70a96-668">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="70a96-669">Исправлена ошибка № 11059. Сбой выполнения `az login --allow-no-subscriptions`, если в клиенте есть подписки.</span><span class="sxs-lookup"><span data-stu-id="70a96-669">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="70a96-670">Исправлена ошибка № 11238. После переименования подписки вход с помощью MSI приведет к тому, что одна и та же подписка появится дважды.</span><span class="sxs-lookup"><span data-stu-id="70a96-670">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="70a96-671">RBAC</span><span class="sxs-lookup"><span data-stu-id="70a96-671">RBAC</span></span>

* <span data-ttu-id="70a96-672">Исправлена ошибка № 10996. Исправлена ошибка с `--force-change-password-next-login` в `az ad user update`, если `--password` не указывается.</span><span class="sxs-lookup"><span data-stu-id="70a96-672">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="70a96-673">Redis</span><span class="sxs-lookup"><span data-stu-id="70a96-673">Redis</span></span>

* <span data-ttu-id="70a96-674">Исправлена ошибка № 2902. Предотвращена настройка конфигураций памяти при обновлении кэша с номером SKU "Базовый".</span><span class="sxs-lookup"><span data-stu-id="70a96-674">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="70a96-675">Резервирование</span><span class="sxs-lookup"><span data-stu-id="70a96-675">Reservations</span></span>

* <span data-ttu-id="70a96-676">Обновлена версия пакета SDK до 0.6.0</span><span class="sxs-lookup"><span data-stu-id="70a96-676">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="70a96-677">Добавлены сведения о плане выставления счетов после вызова Get-Catalogs.</span><span class="sxs-lookup"><span data-stu-id="70a96-677">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="70a96-678">Добавлена новая команда `az reservations reservation-order calculate` для вычисления стоимости резервирования.</span><span class="sxs-lookup"><span data-stu-id="70a96-678">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="70a96-679">Добавлена новая команда `az reservations reservation-order purchase` для приобретения нового резервирования.</span><span class="sxs-lookup"><span data-stu-id="70a96-679">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="70a96-680">Rest</span><span class="sxs-lookup"><span data-stu-id="70a96-680">Rest</span></span>
* <span data-ttu-id="70a96-681">Изменена версия `az rest` на общедоступную.</span><span class="sxs-lookup"><span data-stu-id="70a96-681">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-682">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-682">SQL</span></span>

* <span data-ttu-id="70a96-683">Обновлена версия azure-mgmt-sql до 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="70a96-683">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-684">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-684">Storage</span></span>

* <span data-ttu-id="70a96-685">storage account create. Добавлен параметр --enable-hierarchical-namespace для включения поддержки семантики файловой системы в службе больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="70a96-685">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="70a96-686">Удалено несвязанное исключение из сообщения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="70a96-686">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="70a96-687">Исправлены проблемы, из-за которых появлялось неверное сообщение об отсутствии нужных разрешений на выполнение требуемой операции</span><span class="sxs-lookup"><span data-stu-id="70a96-687">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="70a96-688">при блокировке правилами сети (AuthenticationFailed).</span><span class="sxs-lookup"><span data-stu-id="70a96-688">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="70a96-689">4 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-689">November 4, 2019</span></span>

<span data-ttu-id="70a96-690">Версия 2.0.76</span><span class="sxs-lookup"><span data-stu-id="70a96-690">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-691">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-691">ACR</span></span>

* <span data-ttu-id="70a96-692">В команду `az acr pack build` добавлен параметр предварительной версии `--pack-image-tag`.</span><span class="sxs-lookup"><span data-stu-id="70a96-692">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="70a96-693">Добавлена поддержка включения аудита при создании реестра.</span><span class="sxs-lookup"><span data-stu-id="70a96-693">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="70a96-694">Включена поддержка функции RBAC, распространяющаяся на репозиторий.</span><span class="sxs-lookup"><span data-stu-id="70a96-694">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="70a96-695">AKS</span><span class="sxs-lookup"><span data-stu-id="70a96-695">AKS</span></span>

* <span data-ttu-id="70a96-696">В команду `az aks create` добавлены `--enable-cluster-autoscaler`, `--min-count` и `--max-count`, что позволяет автоматически масштабировать кластер для пула узлов.</span><span class="sxs-lookup"><span data-stu-id="70a96-696">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="70a96-697">Добавлены указанные выше флаги, а также `--update-cluster-autoscaler` и `--disable-cluster-autoscaler` в команду `az aks update`, что позволяет обновлять средство автоматического масштабирования кластера.</span><span class="sxs-lookup"><span data-stu-id="70a96-697">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="70a96-698">AppConfig</span><span class="sxs-lookup"><span data-stu-id="70a96-698">AppConfig</span></span>

* <span data-ttu-id="70a96-699">Добавлена группа команд функции appconfig для управления флагами функций, хранимыми в Конфигурации приложений.</span><span class="sxs-lookup"><span data-stu-id="70a96-699">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="70a96-700">Исправлена незначительная ошибка команды экспорта в файл appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="70a96-700">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="70a96-701">Прерывание чтения содержимого конечного файла во время экспорта.</span><span class="sxs-lookup"><span data-stu-id="70a96-701">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-702">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-702">AppService</span></span>

* <span data-ttu-id="70a96-703">`az appservice plan create`: Добавлена поддержка определения persitescaling при создании плана appservice.</span><span class="sxs-lookup"><span data-stu-id="70a96-703">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="70a96-704">Исправлена проблема, из-за которой операция webapp config ssl bind удаляла существующие теги из ресурса.</span><span class="sxs-lookup"><span data-stu-id="70a96-704">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="70a96-705">Добавлен флаг `--build-remote` для `az functionapp deployment source config-zip` для включения поддержки действия удаленной сборки во время развертывания приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="70a96-705">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="70a96-706">Изменена версия узла по умолчанию для приложений-функций на ~10 для Windows</span><span class="sxs-lookup"><span data-stu-id="70a96-706">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="70a96-707">В `az functionapp create` добавлено свойство `--runtime-version`.</span><span class="sxs-lookup"><span data-stu-id="70a96-707">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="70a96-708">ARM</span><span class="sxs-lookup"><span data-stu-id="70a96-708">ARM</span></span>

* <span data-ttu-id="70a96-709">`az deployment/group deployment validate`: В `--handle-extended-json-format` добавлен параметр для включения поддержки многострочности и комментариев в шаблоне JSON при развертывании.</span><span class="sxs-lookup"><span data-stu-id="70a96-709">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="70a96-710">Версия azure-mgmt-resource обновлена до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="70a96-710">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="70a96-711">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="70a96-711">Backup</span></span>

* <span data-ttu-id="70a96-712">Добавлена поддержка резервного копирования AzureFiles.</span><span class="sxs-lookup"><span data-stu-id="70a96-712">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="70a96-713">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="70a96-713">Compute</span></span>

* <span data-ttu-id="70a96-714">`az vm create`: Добавлено предупреждение при одновременном определении ускоренной сети и существующей сетевой карты.</span><span class="sxs-lookup"><span data-stu-id="70a96-714">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="70a96-715">`az vm create`: Добавлен параметр `--vmss` для определения существующего масштабируемого набора виртуальных машин, которому должна быть назначена виртуальная машина.</span><span class="sxs-lookup"><span data-stu-id="70a96-715">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="70a96-716">`az vm/vmss create`: Добавлена локальная копия файла псевдонима изображения, к которой можно получить доступ в ограниченной сетевой среде.</span><span class="sxs-lookup"><span data-stu-id="70a96-716">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="70a96-717">`az vmss create`: Добавлен параметр `--orchestration-mode` для определения того, как виртуальные машины управляются масштабируемым набором.</span><span class="sxs-lookup"><span data-stu-id="70a96-717">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="70a96-718">`az vm/vmss update`: Добавлен параметр `--ultra-ssd-enabled`, чтобы разрешить обновление параметра Ultra SSD.</span><span class="sxs-lookup"><span data-stu-id="70a96-718">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="70a96-719">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az vm extension set`: Исправлена ошибка, из-за которой пользователям не удавалось определять расширение на виртуальной машине с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="70a96-719">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="70a96-720">Добавлены новые команды `az vm image terms accept/cancel/show` для управления условиями использования образов Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="70a96-720">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="70a96-721">Расширение VMAccessForLinux обновлено до версии 1.5.</span><span class="sxs-lookup"><span data-stu-id="70a96-721">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="70a96-722">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70a96-722">CosmosDB</span></span>

* <span data-ttu-id="70a96-723">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql container create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="70a96-723">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="70a96-724">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az gremlin graph create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="70a96-724">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="70a96-725">`az sql container create`: Добавлены команды `--unique-key-policy` и `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="70a96-725">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="70a96-726">`az sql container create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-726">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="70a96-727">`gremlin graph create`: Добавлена команда `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="70a96-727">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="70a96-728">`gremlin graph create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-728">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="70a96-729">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="70a96-729">Fixed typo in help message</span></span>
* <span data-ttu-id="70a96-730">База данных: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="70a96-730">database: Added deprecation information</span></span>
* <span data-ttu-id="70a96-731">Коллекция: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="70a96-731">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="70a96-732">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-732">IoT</span></span>

* <span data-ttu-id="70a96-733">Добавлен новый тип источника маршрутизации: DigitalTwinChangeEvents.</span><span class="sxs-lookup"><span data-stu-id="70a96-733">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="70a96-734">Добавлены отсутствующие компоненты в `az iot hub create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-734">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="70a96-735">Key Vault</span><span class="sxs-lookup"><span data-stu-id="70a96-735">Key Vault</span></span>

* <span data-ttu-id="70a96-736">Исправлена непредвиденная ошибка с отсутствием файла сертификата.</span><span class="sxs-lookup"><span data-stu-id="70a96-736">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="70a96-737">Исправлена ошибка с неработающей командой `az keyvault recover/purge`.</span><span class="sxs-lookup"><span data-stu-id="70a96-737">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="70a96-738">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="70a96-738">NetAppFiles</span></span>

* <span data-ttu-id="70a96-739">Пакет azure-mgmt-netapp обновлен до версии 0.6.0 для включения поддержки API версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="70a96-739">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="70a96-740">Эта новая версия API включает:</span><span class="sxs-lookup"><span data-stu-id="70a96-740">This new API version includes:</span></span>

    - <span data-ttu-id="70a96-741">При создании тома с использованием `--protocol-types` допускается NFSv4.1 вместо NFSv4.</span><span class="sxs-lookup"><span data-stu-id="70a96-741">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="70a96-742">Свойство политики экспорта томов теперь называется nfsv41, а не nfsv4.</span><span class="sxs-lookup"><span data-stu-id="70a96-742">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="70a96-743">Параметр `--creation-token` для тома переименован в `--file-path`.</span><span class="sxs-lookup"><span data-stu-id="70a96-743">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="70a96-744">Дата создания моментального снимка теперь имеет значение Created.</span><span class="sxs-lookup"><span data-stu-id="70a96-744">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="70a96-745">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-745">Network</span></span>

* <span data-ttu-id="70a96-746">`az network private-dns link vnet create/update`: Добавлена поддержка связывания виртуальных сетей между клиентами.</span><span class="sxs-lookup"><span data-stu-id="70a96-746">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="70a96-747">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az network vnet subnet list`: Параметры `--resource-group` и `--vnet-name` теперь являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="70a96-747">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="70a96-748">`az network public-ip prefix create`: Включена поддержка определения версии IP-адреса (IPv4, IPv6) при создании.</span><span class="sxs-lookup"><span data-stu-id="70a96-748">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="70a96-749">Версия azure-mgmt-network обновлена до 7.0.0 и версия api-version до 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="70a96-749">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="70a96-750">`az network vrouter`: Включена поддержка нового виртуального маршрутизатора службы и пиринга виртуальных маршрутизаторов.</span><span class="sxs-lookup"><span data-stu-id="70a96-750">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="70a96-751">`az network express-route gateway connection`: Добавлена поддержка параметра `--internet-security`.</span><span class="sxs-lookup"><span data-stu-id="70a96-751">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="70a96-752">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-752">Profile</span></span>

* <span data-ttu-id="70a96-753">Исправлена ошибка с неработающей командой `az account get-access-token --resource-type ms-graph`.</span><span class="sxs-lookup"><span data-stu-id="70a96-753">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="70a96-754">Удалено предупреждение из `az login`.</span><span class="sxs-lookup"><span data-stu-id="70a96-754">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="70a96-755">RBAC</span><span class="sxs-lookup"><span data-stu-id="70a96-755">RBAC</span></span>

* <span data-ttu-id="70a96-756">Исправление `az ad app update --id {} --display-name {}` не работает.</span><span class="sxs-lookup"><span data-stu-id="70a96-756">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="70a96-757">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="70a96-757">ServiceFabric</span></span>

* <span data-ttu-id="70a96-758">`az sf cluster create`: Исправлена проблема путем изменения VMSS для вычислений с использованием файла template.json для Service Fabric Linux и Windows со стандартных дисков на управляемые.</span><span class="sxs-lookup"><span data-stu-id="70a96-758">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-759">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-759">SQL</span></span>

* <span data-ttu-id="70a96-760">Добавлены параметры `--compute-model`, `--auto-pause-delay` и `--min-capacity` для включения поддержки операций CRUD для нового предложения Базы данных SQL: Модель бессерверных вычислений.</span><span class="sxs-lookup"><span data-stu-id="70a96-760">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-761">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-761">Storage</span></span>

* <span data-ttu-id="70a96-762">`az storage account create/update`: Добавлен параметр --enable-files-adds и группа аргументов свойств Azure Active Directory для включения поддержки аутентификации доменных служб Azure Active Directory для Файлов Azure.</span><span class="sxs-lookup"><span data-stu-id="70a96-762">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="70a96-763">Расширена команда `az storage account keys list/renew` для включения поддержки перечисления или повторного создания ключей Kerberos для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="70a96-763">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="70a96-764">15 октября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-764">October 15, 2019</span></span>

<span data-ttu-id="70a96-765">Версия 2.0.75</span><span class="sxs-lookup"><span data-stu-id="70a96-765">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="70a96-766">AKS</span><span class="sxs-lookup"><span data-stu-id="70a96-766">AKS</span></span>

* <span data-ttu-id="70a96-767">Для параметра `--load-balancer-sku` изменено значение по умолчанию на `standard`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="70a96-767">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="70a96-768">Для параметра `--vm-set-type` изменено значение по умолчанию на `virtualmachinescalesets`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="70a96-768">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="70a96-769">AMS</span><span class="sxs-lookup"><span data-stu-id="70a96-769">AMS</span></span>

* <span data-ttu-id="70a96-770">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя `job start` изменено на `job create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-770">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="70a96-771">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В параметре `--ask` команды `content-key-policy create` вместо кодировки UTF8 теперь используется шестнадцатеричная строка из 32 символов.</span><span class="sxs-lookup"><span data-stu-id="70a96-771">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-772">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-772">AppService</span></span>

* <span data-ttu-id="70a96-773">Добавлены команды `webapp config access-restriction show|set|add|remove`.</span><span class="sxs-lookup"><span data-stu-id="70a96-773">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="70a96-774">Улучшена обработка ошибок в `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="70a96-774">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="70a96-775">Для `appservice plan update` добавлена поддержка номера SKU `Isolated`.</span><span class="sxs-lookup"><span data-stu-id="70a96-775">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="70a96-776">ARM</span><span class="sxs-lookup"><span data-stu-id="70a96-776">ARM</span></span>

* <span data-ttu-id="70a96-777">В `deployment create` добавлен параметр `--handle-extended-json-format` для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="70a96-777">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="70a96-778">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="70a96-778">Compute</span></span>

* <span data-ttu-id="70a96-779">Добавлен параметр `--enable-agent` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-779">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="70a96-780">Внесены изменения в `vm create`, позволяющие автоматически использовать номер SKU "Стандартный" для общедоступных IP-адресов при использовании зон.</span><span class="sxs-lookup"><span data-stu-id="70a96-780">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="70a96-781">Внесены изменения в `vm create`, позволяющие автоматически создавать допустимое имя для виртуальной машины, если оно не задано.</span><span class="sxs-lookup"><span data-stu-id="70a96-781">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="70a96-782">В `vmss create` добавлен параметр `--computer-name-prefix` для поддержки пользовательского префикса имени для виртуальных машин в VMSS.</span><span class="sxs-lookup"><span data-stu-id="70a96-782">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="70a96-783">В `vm create` добавлен параметр `--workspace` для автоматического включения рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="70a96-783">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="70a96-784">API коллекций обновлен до версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="70a96-784">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="70a96-785">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-785">Core</span></span>

* <span data-ttu-id="70a96-786">Добавлена проверка синтаксиса для параметра `--set` в универсальной команде обновления.</span><span class="sxs-lookup"><span data-stu-id="70a96-786">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="70a96-787">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-787">IoT</span></span>

* <span data-ttu-id="70a96-788">Исправлена проблема, при которой `iot hub show` неправильно выдавал ошибку "Ресурс не найден".</span><span class="sxs-lookup"><span data-stu-id="70a96-788">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-789">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-789">Monitor</span></span>

* <span data-ttu-id="70a96-790">В `monitor log-analytics workspace` добавлена поддержка CRUD.</span><span class="sxs-lookup"><span data-stu-id="70a96-790">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="70a96-791">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-791">Network</span></span>

* <span data-ttu-id="70a96-792">В `network private-dns link vnet [create|update]` добавлена поддержка виртуального канала для клиентов.</span><span class="sxs-lookup"><span data-stu-id="70a96-792">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="70a96-793">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для `network vnet subnet list` теперь требуются параметры `--resource-group` и `--vnet-name`.</span><span class="sxs-lookup"><span data-stu-id="70a96-793">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-794">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-794">SQL</span></span>

* <span data-ttu-id="70a96-795">В `sql mi ad-admin` добавлены команды, которые поддерживают назначение администратора AAD в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="70a96-795">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-796">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-796">Storage</span></span>

* <span data-ttu-id="70a96-797">В `storage copy` добавлен параметр `--preserve-s2s-access-tier`, позволяющий сохранить уровень доступа во время копирования между службами.</span><span class="sxs-lookup"><span data-stu-id="70a96-797">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="70a96-798">В `storage account [create|update]` добавлен параметр `--enable-large-file-share` для поддержки общих папок большого размера в учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="70a96-798">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="70a96-799">24 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-799">September 24, 2019</span></span>

<span data-ttu-id="70a96-800">Версия 2.0.74</span><span class="sxs-lookup"><span data-stu-id="70a96-800">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-801">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-801">ACR</span></span>

* <span data-ttu-id="70a96-802">В `acr config retention update` добавлен обязательный параметр `--type`.</span><span class="sxs-lookup"><span data-stu-id="70a96-802">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="70a96-803">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованный параметр `--name -n` изменен на `--registry -r ` для группы команд `acr config`.</span><span class="sxs-lookup"><span data-stu-id="70a96-803">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="70a96-804">AKS</span><span class="sxs-lookup"><span data-stu-id="70a96-804">AKS</span></span>

* <span data-ttu-id="70a96-805">В команду `aks create` добавлен параметр `--load-balancer-sku`, позволяющий создать кластер AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="70a96-805">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="70a96-806">В команды `aks [create|update]` добавлены параметры `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` и `--load-balancer-outbound-ip-prefixes`, позволяющие обновлять профиль подсистемы балансировки нагрузки у кластера AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="70a96-806">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="70a96-807">В команду `aks create` добавлен параметр `--vm-set-type`, позволяющий указывать типы виртуальных машин в кластере AKS.</span><span class="sxs-lookup"><span data-stu-id="70a96-807">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="70a96-808">ARM</span><span class="sxs-lookup"><span data-stu-id="70a96-808">ARM</span></span>

* <span data-ttu-id="70a96-809">В команду `group deployment create` добавлен параметр `--handle-extended-json-format`, для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="70a96-809">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="70a96-810">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="70a96-810">Compute</span></span>

* <span data-ttu-id="70a96-811">В команды `vmss [create|update]` добавлен параметр `--terminate-notification-time`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="70a96-811">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="70a96-812">В команду `vmss update` добавлен параметр `--enable-terminate-notification`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="70a96-812">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="70a96-813">В команды `[vm|vmss] create` добавлены параметры `--priority,`, `--eviction-policy,` и `--max-billing`.</span><span class="sxs-lookup"><span data-stu-id="70a96-813">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="70a96-814">Изменена команда `disk create`, которая теперь позволяет указать точный размер отправки на диск.</span><span class="sxs-lookup"><span data-stu-id="70a96-814">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="70a96-815">В `snapshot create` добавлена поддержка добавочных моментальных снимков для управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="70a96-815">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="70a96-816">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70a96-816">Cosmos DB</span></span>

* <span data-ttu-id="70a96-817">В команду `cosmosdb keys list` добавлен параметр `--type <key-type>` для отображения ключей, ключей только для чтения или строк подключения.</span><span class="sxs-lookup"><span data-stu-id="70a96-817">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="70a96-818">Добавлена команда `cosmosdb keys regenerate`.</span><span class="sxs-lookup"><span data-stu-id="70a96-818">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="70a96-819">[УСТАРЕЛО] Команды `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` и `cosmosdb list-read-only-keys` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="70a96-819">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="70a96-820">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="70a96-820">EventGrid</span></span>

* <span data-ttu-id="70a96-821">Исправлен текст справки по конечной точке — дана ссылка на правильный параметр.</span><span class="sxs-lookup"><span data-stu-id="70a96-821">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="70a96-822">Key Vault</span><span class="sxs-lookup"><span data-stu-id="70a96-822">Key Vault</span></span>

* <span data-ttu-id="70a96-823">Исправлена проблема, из-за которой вход с помощью клиента (`login -t`) мог приводить к сбою `keyvault create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-823">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-824">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-824">Monitor</span></span>

* <span data-ttu-id="70a96-825">Исправлена проблема с тем, что символ `:` являлся недопустимым в аргументе `--condition` для `monitor metrics alert create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-825">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="70a96-826">Политика</span><span class="sxs-lookup"><span data-stu-id="70a96-826">Policy</span></span>

* <span data-ttu-id="70a96-827">Добавлена поддержка API Политики версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="70a96-827">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="70a96-828">В команду `policy assignment create` добавлен параметр `--enforcement-mode`.</span><span class="sxs-lookup"><span data-stu-id="70a96-828">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-829">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-829">Storage</span></span>

* <span data-ttu-id="70a96-830">В команду `az storage copy` добавлен параметр `--blob-type`.</span><span class="sxs-lookup"><span data-stu-id="70a96-830">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="70a96-831">10 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-831">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-832">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-832">ACR</span></span>

* <span data-ttu-id="70a96-833">Добавлена группа команд `acr config retention` для настройки политики хранения.</span><span class="sxs-lookup"><span data-stu-id="70a96-833">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="70a96-834">AKS</span><span class="sxs-lookup"><span data-stu-id="70a96-834">AKS</span></span>

* <span data-ttu-id="70a96-835">Добавлена возможность интеграции ACR с помощью следующих команд:</span><span class="sxs-lookup"><span data-stu-id="70a96-835">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="70a96-836">В `aks [create|update]` добавлен параметр `--attach-acr` для подключения ACR к кластеру AKS.</span><span class="sxs-lookup"><span data-stu-id="70a96-836">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="70a96-837">В `aks update` добавлен параметр `--detach-acr` для отключения ACR от кластера AKS.</span><span class="sxs-lookup"><span data-stu-id="70a96-837">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="70a96-838">ARM</span><span class="sxs-lookup"><span data-stu-id="70a96-838">ARM</span></span>

* <span data-ttu-id="70a96-839">Добавлена возможность использования API версии 2019-05-10.</span><span class="sxs-lookup"><span data-stu-id="70a96-839">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="70a96-840">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-840">Batch</span></span>

* <span data-ttu-id="70a96-841">Добавлены новые параметры конфигурации JSON в `--json-file` для `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="70a96-841">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="70a96-842">Добавлен параметр `MountConfigurations` для подключений файловой системы (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="70a96-842">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="70a96-843">Добавлено необязательное свойство `publicIPs` в `NetworkConfiguration` для общедоступных IP-адресов в пулах (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="70a96-843">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="70a96-844">В `--image` добавлена поддержка коллекций общих образов.</span><span class="sxs-lookup"><span data-stu-id="70a96-844">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="70a96-845">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `--start-task-wait-for-success` в `batch pool create` изменено на `true`.</span><span class="sxs-lookup"><span data-stu-id="70a96-845">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="70a96-846">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `Scope` в `AutoUserSpecification` задано как Pool (ранее `Task` на узлах Windows и `Pool` на узлах Linux).</span><span class="sxs-lookup"><span data-stu-id="70a96-846">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="70a96-847">Этот аргумент можно задать только в конфигурации JSON с помощью `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="70a96-847">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="70a96-848">HDInsight</span><span class="sxs-lookup"><span data-stu-id="70a96-848">HDInsight</span></span>

* <span data-ttu-id="70a96-849">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="70a96-849">GA release</span></span>
* <span data-ttu-id="70a96-850">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--workernode-count/-c` в `az hdinsight resize` теперь является обязательным.</span><span class="sxs-lookup"><span data-stu-id="70a96-850">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="70a96-851">Key Vault</span><span class="sxs-lookup"><span data-stu-id="70a96-851">Key Vault</span></span>

* <span data-ttu-id="70a96-852">Исправлена проблема, когда подсети не удавалось удалить из сетевых правил.</span><span class="sxs-lookup"><span data-stu-id="70a96-852">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="70a96-853">Исправлена проблема, когда дублированные подсети и IP-адреса могли быть добавлены к сетевым правилам.</span><span class="sxs-lookup"><span data-stu-id="70a96-853">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="70a96-854">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-854">Network</span></span>

* <span data-ttu-id="70a96-855">Добавлен параметр `--interval` в `network watcher flow-log` для выбора значения интервала анализа трафика.</span><span class="sxs-lookup"><span data-stu-id="70a96-855">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="70a96-856">Добавлена команда `network application-gateway identity` для управления удостоверением шлюза.</span><span class="sxs-lookup"><span data-stu-id="70a96-856">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="70a96-857">Добавлена возможность указать идентификатор Key Vault в команде `network application-gateway ssl-cert`.</span><span class="sxs-lookup"><span data-stu-id="70a96-857">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="70a96-858">Добавлена команда `network express-route peering peer-connection [show|list]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-858">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="70a96-859">Политика</span><span class="sxs-lookup"><span data-stu-id="70a96-859">Policy</span></span>

* <span data-ttu-id="70a96-860">Добавлена возможность использования API версии 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="70a96-860">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="70a96-861">27 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-861">August 27, 2019</span></span>

<span data-ttu-id="70a96-862">Версия 2.0.72</span><span class="sxs-lookup"><span data-stu-id="70a96-862">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-863">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-863">ACR</span></span>

* <span data-ttu-id="70a96-864">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка SKU `classic`.</span><span class="sxs-lookup"><span data-stu-id="70a96-864">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="70a96-865">Управление API</span><span class="sxs-lookup"><span data-stu-id="70a96-865">API Management</span></span>

* <span data-ttu-id="70a96-866">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена группа команд `apim`.</span><span class="sxs-lookup"><span data-stu-id="70a96-866">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-867">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-867">AppService</span></span>

* <span data-ttu-id="70a96-868">Исправлена проблема с командой `webapp webjob continuous start` при указании слота.</span><span class="sxs-lookup"><span data-stu-id="70a96-868">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="70a96-869">Изменена команда `webapp up` для обнаружения и удаления папки `env` из файла, используемого для развертывания.</span><span class="sxs-lookup"><span data-stu-id="70a96-869">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="70a96-870">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70a96-870">Keyvault</span></span>

* <span data-ttu-id="70a96-871">Исправлена ошибка в команде `keyvault secret set`, которая игнорировала аргумент `--expires`.</span><span class="sxs-lookup"><span data-stu-id="70a96-871">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="70a96-872">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-872">Network</span></span>

* <span data-ttu-id="70a96-873">Добавлена поддержка IPv6-адресов для аргументов `--private-ip-address-version`.</span><span class="sxs-lookup"><span data-stu-id="70a96-873">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="70a96-874">Добавлены новые команды `network private-endpoint [create|update|list-types]` для управления закрытыми конечными точками.</span><span class="sxs-lookup"><span data-stu-id="70a96-874">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="70a96-875">Добавлена группа команд для `network private-link-service`.</span><span class="sxs-lookup"><span data-stu-id="70a96-875">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="70a96-876">Добавлены аргументы `--private-endpoint-network-policies` и `--private-link-service-network-policies` для команды `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="70a96-876">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="70a96-877">RBAC</span><span class="sxs-lookup"><span data-stu-id="70a96-877">RBAC</span></span>

* <span data-ttu-id="70a96-878">Исправлена проблема с `ad app update --homepage`, когда домашнюю страницу нельзя было обновить.</span><span class="sxs-lookup"><span data-stu-id="70a96-878">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="70a96-879">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="70a96-879">ServiceFabric</span></span>

* <span data-ttu-id="70a96-880">Добавлена поддержка имен Key Vault в смешанном регистре.</span><span class="sxs-lookup"><span data-stu-id="70a96-880">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="70a96-881">Исправлена проблема с использованием сертификатов в Key Vault.</span><span class="sxs-lookup"><span data-stu-id="70a96-881">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="70a96-882">Исправлена проблема с использованием файлов сертификатов PFX.</span><span class="sxs-lookup"><span data-stu-id="70a96-882">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="70a96-883">Исправлена проблема с `sf cluster certificate add`, когда группа ресурсов Key Vault не была указана.</span><span class="sxs-lookup"><span data-stu-id="70a96-883">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="70a96-884">Исправлена проблема с неработающей командой `sf cluster set`.</span><span class="sxs-lookup"><span data-stu-id="70a96-884">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="70a96-885">SignalR</span><span class="sxs-lookup"><span data-stu-id="70a96-885">SignalR</span></span>

* <span data-ttu-id="70a96-886">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="70a96-886">Added new commands:</span></span>
  * <span data-ttu-id="70a96-887">`signalr cors`: Управление CORS SignalR</span><span class="sxs-lookup"><span data-stu-id="70a96-887">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="70a96-888">`signalr restart`: Перезапуск службы SignalR</span><span class="sxs-lookup"><span data-stu-id="70a96-888">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="70a96-889">`signalr update`: Обновление службы SignalR</span><span class="sxs-lookup"><span data-stu-id="70a96-889">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="70a96-890">Добавлен аргумент `--service-mode` для команды `signalr create`</span><span class="sxs-lookup"><span data-stu-id="70a96-890">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-891">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-891">Storage</span></span>

* <span data-ttu-id="70a96-892">Добавлена команда `storage account revoke-delegation-keys`.</span><span class="sxs-lookup"><span data-stu-id="70a96-892">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="70a96-893">13 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-893">August 13, 2019</span></span>

<span data-ttu-id="70a96-894">Версия 2.0.71</span><span class="sxs-lookup"><span data-stu-id="70a96-894">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-895">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-895">AppService</span></span>

* <span data-ttu-id="70a96-896">Исправлена проблема, из-за которой выполнение команд `webapp webjob continuous` для слотов завершалось сбоем.</span><span class="sxs-lookup"><span data-stu-id="70a96-896">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="70a96-897">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="70a96-897">BotService</span></span>

* <span data-ttu-id="70a96-898">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка создания ботов на основе пакета SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="70a96-898">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="70a96-899">Cognitive Services:</span><span class="sxs-lookup"><span data-stu-id="70a96-899">CognitiveServices</span></span>

* <span data-ttu-id="70a96-900">Добавлены команды `cognitiveservices account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="70a96-900">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="70a96-901">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70a96-901">Cosmos DB</span></span>

* <span data-ttu-id="70a96-902">Удалено предупреждение при обновлении нескольких расположений для записи.</span><span class="sxs-lookup"><span data-stu-id="70a96-902">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="70a96-903">Добавлены команды CRUD для ресурсов CosmosDB SQL, MongoDB, Cassandra, Gremlin и ресурсов таблиц, а также пропускной способности ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70a96-903">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="70a96-904">HDInsight</span><span class="sxs-lookup"><span data-stu-id="70a96-904">HDInsight</span></span>

<span data-ttu-id="70a96-905">Этот выпуск содержит большое число критических изменений.</span><span class="sxs-lookup"><span data-stu-id="70a96-905">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="70a96-906">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="70a96-906">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="70a96-907">Переименование `--storage-default-container` в `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="70a96-907">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="70a96-908">Переименование `--storage-default-filesystem` в `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="70a96-908">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="70a96-909">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--name` для `application create`, чтобы представлять имя приложения вместо имени кластера.</span><span class="sxs-lookup"><span data-stu-id="70a96-909">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="70a96-910">Добавлен аргумент `--cluster-name` для `application create`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="70a96-910">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="70a96-911">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="70a96-911">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="70a96-912">Переименование `--application-type` в `--type`</span><span class="sxs-lookup"><span data-stu-id="70a96-912">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="70a96-913">Переименование `--marketplace-identifier` в `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="70a96-913">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="70a96-914">Переименование `--https-endpoint-access-mode` в `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="70a96-914">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="70a96-915">Переименован аргумент `--https-endpoint-destination-port` на `--destination-port`.</span><span class="sxs-lookup"><span data-stu-id="70a96-915">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="70a96-916">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="70a96-916">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="70a96-917">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Переименован аргумент `--target-instance-count` на `--workernode-count` для `hdinsight resize`.</span><span class="sxs-lookup"><span data-stu-id="70a96-917">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="70a96-918">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены все команды в группе `hdinsight script-action`, чтобы использовать параметр `--name` в качестве имени действия скрипта.</span><span class="sxs-lookup"><span data-stu-id="70a96-918">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="70a96-919">Добавлен аргумент `--cluster-name` для всех команд `hdinsight script-action`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="70a96-919">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="70a96-920">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименован аргумент `--script-execution-id` на `--execution-id`для всех команд `hdinsight script-action`.</span><span class="sxs-lookup"><span data-stu-id="70a96-920">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="70a96-921">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `hdinsight script-action show` переименована в `hdinsight script-action show-execution-details`.</span><span class="sxs-lookup"><span data-stu-id="70a96-921">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="70a96-922">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Изменены параметры для `hdinsight script-action execute --roles`, чтобы они разделялись пробелами, а не запятыми.</span><span class="sxs-lookup"><span data-stu-id="70a96-922">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="70a96-923">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--persisted` для `hdinsight script-action list`.</span><span class="sxs-lookup"><span data-stu-id="70a96-923">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="70a96-924">Изменен параметр `hdinsight create --cluster-configurations`, чтобы принимать путь к локальному файлу JSON или строке JSON.</span><span class="sxs-lookup"><span data-stu-id="70a96-924">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="70a96-925">Добавлена команда `hdinsight script-action list-execution-history`.</span><span class="sxs-lookup"><span data-stu-id="70a96-925">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="70a96-926">Изменен параметр `hdinsight monitor enable --workspace`, чтобы принимать идентификатор или имя рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="70a96-926">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="70a96-927">Добавлен аргумент `hdinsight monitor enable --primary-key`, который требуется, если в качестве параметра указан идентификатор рабочей области.</span><span class="sxs-lookup"><span data-stu-id="70a96-927">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="70a96-928">Добавлены дополнительные примеры и обновленные описания для справочных сообщений.</span><span class="sxs-lookup"><span data-stu-id="70a96-928">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="70a96-929">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="70a96-929">Interactive</span></span>

* <span data-ttu-id="70a96-930">Исправлена ошибка загрузки.</span><span class="sxs-lookup"><span data-stu-id="70a96-930">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="70a96-931">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="70a96-931">Kubernetes</span></span>

* <span data-ttu-id="70a96-932">Теперь используется `https`, если порт контейнера панели мониторинга использует `https`.</span><span class="sxs-lookup"><span data-stu-id="70a96-932">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="70a96-933">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-933">Network</span></span>

* <span data-ttu-id="70a96-934">Добавлен аргумент `--yes` для `network dns record-set cname delete`.</span><span class="sxs-lookup"><span data-stu-id="70a96-934">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="70a96-935">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-935">Profile</span></span>

* <span data-ttu-id="70a96-936">Добавлен аргумент `--resource-type` для `account get-access-token`, чтобы получать маркеры доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="70a96-936">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="70a96-937">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="70a96-937">ServiceFabric</span></span>

* <span data-ttu-id="70a96-938">Добавлены все поддерживаемые версии ОС для команды sf cluster create.</span><span class="sxs-lookup"><span data-stu-id="70a96-938">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="70a96-939">Исправлена ошибка проверки основного сертификата.</span><span class="sxs-lookup"><span data-stu-id="70a96-939">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-940">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-940">Storage</span></span>

* <span data-ttu-id="70a96-941">Добавлена команда `storage copy`.</span><span class="sxs-lookup"><span data-stu-id="70a96-941">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="70a96-942">30 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-942">July 30, 2019</span></span>

<span data-ttu-id="70a96-943">Версия 2.0.70</span><span class="sxs-lookup"><span data-stu-id="70a96-943">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-944">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-944">ACR</span></span>

* <span data-ttu-id="70a96-945">Исправлена проблема № 9952 (регрессия в команде `acr pack build`).</span><span class="sxs-lookup"><span data-stu-id="70a96-945">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="70a96-946">Удалено имя образа построителя по умолчанию в `acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="70a96-946">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-947">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-947">Appservice</span></span>

* <span data-ttu-id="70a96-948">Команда `webapp config ssl` изменена для отображения сообщения, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="70a96-948">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="70a96-949">Исправлена проблема, когда команда `functionapp create` не принимала тип учетной записи хранения `Standard_RAGRS`.</span><span class="sxs-lookup"><span data-stu-id="70a96-949">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="70a96-950">Исправлена проблема, когда команда `webapp up` завершала работу со сбоем в случае выполнения со старой версией Python.</span><span class="sxs-lookup"><span data-stu-id="70a96-950">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="70a96-951">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-951">Network</span></span>

* <span data-ttu-id="70a96-952">Удален недопустимый параметр `--ids` из `network nic ip-config add` (исправление проблемы № 9861).</span><span class="sxs-lookup"><span data-stu-id="70a96-952">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="70a96-953">Исправлена проблема № 9604.</span><span class="sxs-lookup"><span data-stu-id="70a96-953">Fixes #9604.</span></span> <span data-ttu-id="70a96-954">Добавлен параметр `--root-certs` в `network application-gateway http-settings [create|update]` для поддержки связанных с пользователем доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="70a96-954">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="70a96-955">Исправлен аргумент `--subscription` для `network dns record-set ns create` (проблема № 9965).</span><span class="sxs-lookup"><span data-stu-id="70a96-955">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="70a96-956">RBAC</span><span class="sxs-lookup"><span data-stu-id="70a96-956">RBAC</span></span>

* <span data-ttu-id="70a96-957">Добавлена команда `user update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-957">Added `user update` command</span></span>
* <span data-ttu-id="70a96-958">[УСТАРЕЛО]`--upn-or-object-id` не рекомендуется использовать в связанных с пользователями командах.</span><span class="sxs-lookup"><span data-stu-id="70a96-958">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="70a96-959">Вместо этого применяйте аргумент `--id`.</span><span class="sxs-lookup"><span data-stu-id="70a96-959">Use replacement argument `--id`</span></span>
* <span data-ttu-id="70a96-960">Добавлен аргумент `--id` в связанные с пользователями команды.</span><span class="sxs-lookup"><span data-stu-id="70a96-960">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-961">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-961">SQL</span></span>

* <span data-ttu-id="70a96-962">Добавлены команды управления для ключей и предохранителя TDE управляемого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="70a96-962">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-963">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-963">Storage</span></span>

* <span data-ttu-id="70a96-964">Добавлена команда `storage remove`.</span><span class="sxs-lookup"><span data-stu-id="70a96-964">Added `storage remove` command</span></span>
* <span data-ttu-id="70a96-965">Исправлена проблема с `storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-965">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-966">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-966">VM</span></span>

* <span data-ttu-id="70a96-967">Изменена команда `list-skus` для использования новой версии API для вывода сведений о зонах.</span><span class="sxs-lookup"><span data-stu-id="70a96-967">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="70a96-968">Изменено значение по умолчанию параметра `--single-placement-group` на `false` для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-968">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="70a96-969">Добавлена возможность выбирать номера SKU хранилища ZRS для `[snapshot|disk] create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-969">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="70a96-970">Добавлена новая группа команд `vm host` для поддержки выделенных узлов.</span><span class="sxs-lookup"><span data-stu-id="70a96-970">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="70a96-971">Добавлены параметры `--host` и `--host-group` в команде `vm create` для указания выделенного узла виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="70a96-971">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="70a96-972">16 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-972">July 16, 2019</span></span>

<span data-ttu-id="70a96-973">Версия 2.0.69</span><span class="sxs-lookup"><span data-stu-id="70a96-973">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-974">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-974">Appservice</span></span>

* <span data-ttu-id="70a96-975">Изменены команды `webapp identity`. Теперь они возвращают правильное сообщение об ошибке, если параметр ResourceGroupName или имя приложения недопустимы.</span><span class="sxs-lookup"><span data-stu-id="70a96-975">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="70a96-976">Исправлена команда `webapp list`. Теперь она возвращает правильное значение для параметра numberOfSites, если не указан параметр ResourceGroup.</span><span class="sxs-lookup"><span data-stu-id="70a96-976">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="70a96-977">Исправлены побочные эффекты для команд `appservice plan create` и `webapp create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-977">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="70a96-978">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-978">Core</span></span>

* <span data-ttu-id="70a96-979">Исправлена ошибка, при которой отображался параметр `--subscription`, хотя он был неприменим.</span><span class="sxs-lookup"><span data-stu-id="70a96-979">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="70a96-980">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-980">Batch</span></span>

* <span data-ttu-id="70a96-981">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `batch pool node-agent-skus list` заменена на `batch pool supported-images list`.</span><span class="sxs-lookup"><span data-stu-id="70a96-981">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="70a96-982">Добавлена поддержка правил безопасности, которые блокируют сетевой доступ к пулу на основе исходного порта трафика при использовании параметра `--json-file` команды `batch pool create network`.</span><span class="sxs-lookup"><span data-stu-id="70a96-982">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="70a96-983">Добавлена поддержка выполнения задачи в рабочей папке контейнера или рабочей папке задачи пакета при использовании параметра `--json-file` команды `batch task create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-983">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="70a96-984">Исправлена ошибка в параметре `--application-package-references` команды `batch pool create`, которая позволяла работать только со значениями по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-984">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="70a96-985">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="70a96-985">Eventhubs</span></span>

* <span data-ttu-id="70a96-986">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="70a96-986">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="70a96-987">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="70a96-987">RDBMS</span></span>

* <span data-ttu-id="70a96-988">Добавлен необязательный параметр для указания номера SKU реплики в команде создания реплики.</span><span class="sxs-lookup"><span data-stu-id="70a96-988">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="70a96-989">Исправлена ошибка теста CI при создании реплики MySQL.</span><span class="sxs-lookup"><span data-stu-id="70a96-989">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="70a96-990">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="70a96-990">Relay</span></span>

* <span data-ttu-id="70a96-991">Исправлена проблема с гибридным подключением при выключенной авторизации клиента ([8775](https://github.com/azure/azure-cli/issues/8775)).</span><span class="sxs-lookup"><span data-stu-id="70a96-991">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="70a96-992">Добавлен параметр `--requires-transport-security` для команды `relay wcfrelay create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-992">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="70a96-993">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="70a96-993">Servicebus</span></span>

* <span data-ttu-id="70a96-994">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="70a96-994">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-995">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-995">Storage</span></span>

* <span data-ttu-id="70a96-996">Добавлена возможность обновления учетной записи хранения для AADDS в службе "Файлы".</span><span class="sxs-lookup"><span data-stu-id="70a96-996">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="70a96-997">Устранена проблема, описанная здесь: `storage blob service-properties update --set`.</span><span class="sxs-lookup"><span data-stu-id="70a96-997">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="70a96-998">2 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-998">July 2, 2019</span></span>

<span data-ttu-id="70a96-999">Версия 2.0.68</span><span class="sxs-lookup"><span data-stu-id="70a96-999">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="70a96-1000">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-1000">Core</span></span>

* <span data-ttu-id="70a96-1001">Командные модули теперь объединены в один распространяемый пакет Python.</span><span class="sxs-lookup"><span data-stu-id="70a96-1001">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="70a96-1002">В результате этого прекращается непосредственное использование множества пакетов `azure-cli-` в PyPI.</span><span class="sxs-lookup"><span data-stu-id="70a96-1002">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="70a96-1003">Это также должно уменьшить размер установки и повлияет только на пользователей, которые выполняли установку непосредственно через `pip`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1003">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-1004">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-1004">ACR</span></span>

* <span data-ttu-id="70a96-1005">В заданиях добавлена поддержка триггеров таймера.</span><span class="sxs-lookup"><span data-stu-id="70a96-1005">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-1006">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-1006">Appservice</span></span>

* <span data-ttu-id="70a96-1007">Внесены изменения в `functionapp create` для включения Application Insights по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-1007">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="70a96-1008">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена устаревшая команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1008">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="70a96-1009">Вместо нее используйте новую команду `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1009">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="70a96-1010">В `functionapp deployment config-zip` добавлена поддержка плана потребления приложения-функции Linux.</span><span class="sxs-lookup"><span data-stu-id="70a96-1010">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="70a96-1011">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70a96-1011">Cosmos DB</span></span>

* <span data-ttu-id="70a96-1012">Добавлена возможность отключения TTL.</span><span class="sxs-lookup"><span data-stu-id="70a96-1012">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="70a96-1013">DLS</span><span class="sxs-lookup"><span data-stu-id="70a96-1013">DLS</span></span>

* <span data-ttu-id="70a96-1014">Обновленная версия ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="70a96-1014">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="70a96-1015">Отзывы</span><span class="sxs-lookup"><span data-stu-id="70a96-1015">Feedback</span></span>

* <span data-ttu-id="70a96-1016">При сообщении о сбое при выполнении команды расширения `az feedback` теперь пытается открыть браузер по URL-адресу репозитория или проекта расширения из индекса.</span><span class="sxs-lookup"><span data-stu-id="70a96-1016">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="70a96-1017">HDInsight</span><span class="sxs-lookup"><span data-stu-id="70a96-1017">HDInsight</span></span>

* <span data-ttu-id="70a96-1018">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя группы команд `oms` изменилось на `monitor`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1018">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="70a96-1019">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--http-password/-p` стал обязательным.</span><span class="sxs-lookup"><span data-stu-id="70a96-1019">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="70a96-1020">Добавлены средства заполнения для `--cluster-admin-account` и средство заполнения для параметров `cluster-users-group-dns`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1020">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="70a96-1021">Параметр `cluster-users-group-dns` стал обязательным, если присутствует `—esp`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1021">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="70a96-1022">Добавлено время ожидания для всех существующих средств автоматического заполнения аргументов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1022">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="70a96-1023">Добавлено время ожидания для преобразования имени ресурса в идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="70a96-1023">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="70a96-1024">Внесены изменения в средства автоматического заполнения для выбора ресурсов из любой группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1024">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="70a96-1025">Это может быть группа ресурсов, отличная от той, которая указана с помощью `-g`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1025">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="70a96-1026">Добавлена поддержка параметров `--sub-domain-suffix` и `--disable_gateway_auth` в команде `hdinsight application create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1026">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="70a96-1027">Управляемые службы</span><span class="sxs-lookup"><span data-stu-id="70a96-1027">Managed Services</span></span>

* <span data-ttu-id="70a96-1028">Командный модуль управляемых служб выпущен в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="70a96-1028">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="70a96-1029">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-1029">Profile</span></span>
* <span data-ttu-id="70a96-1030">Аргумент `--subscription` подавляется для команды выхода.</span><span class="sxs-lookup"><span data-stu-id="70a96-1030">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="70a96-1031">RBAC</span><span class="sxs-lookup"><span data-stu-id="70a96-1031">RBAC</span></span>

* <span data-ttu-id="70a96-1032">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален аргумент `--password` для `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1032">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="70a96-1033">В команду `create` добавлен параметр `--assignee-principal-type` для устранения периодических сбоев из-за задержки репликации сервера AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="70a96-1033">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="70a96-1034">Исправлен сбой в `ad signed-in-user` при перечислении собственных объектов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1034">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="70a96-1035">Исправлена проблема, при которой `ad sp` не удавалось найти нужное приложение в субъекте-службе.</span><span class="sxs-lookup"><span data-stu-id="70a96-1035">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="70a96-1036">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="70a96-1036">RDBMS</span></span>

* <span data-ttu-id="70a96-1037">Добавлена поддержка репликации MariaDB.</span><span class="sxs-lookup"><span data-stu-id="70a96-1037">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-1038">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-1038">SQL</span></span>

* <span data-ttu-id="70a96-1039">Описаны допустимые значения для `sql db create --sample-name`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1039">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-1040">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-1040">Storage</span></span>

* <span data-ttu-id="70a96-1041">В `storage blob generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1041">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="70a96-1042">В `storage container generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1042">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="70a96-1043">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-1043">VM</span></span>

* <span data-ttu-id="70a96-1044">Исправлена ошибка, при которой команда `vmss create` возвращала сообщение об ошибке при выполнении с `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1044">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="70a96-1045">Прекращена проверка `vmss create --single-placement-group` на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="70a96-1045">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="70a96-1046">Команда не завершается сбоем, если для `--single-placement-group` задано значение `true`, а значение `--instance-count` больше 100 или указаны зоны доступности. Сама проверка теперь выполняется службой вычислений.</span><span class="sxs-lookup"><span data-stu-id="70a96-1046">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="70a96-1047">Исправлена ошибка, при которой команда `[vm|vmss] extension image list` завершалась сбоем при указании `--latest`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1047">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="70a96-1048">18 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1048">June 18, 2019</span></span>

<span data-ttu-id="70a96-1049">Версия 2.0.67</span><span class="sxs-lookup"><span data-stu-id="70a96-1049">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="70a96-1050">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-1050">Core</span></span>

<span data-ttu-id="70a96-1051">В этом выпуске добавлен новый тег [Предварительная версия], который яснее дает понять, что группа команд, команда или аргумент находятся в состоянии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="70a96-1051">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="70a96-1052">Ранее это указывалось в тексте справки или подразумевалось в номере версии командного модуля.</span><span class="sxs-lookup"><span data-stu-id="70a96-1052">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="70a96-1053">В будущем в интерфейсе командной строки номера версий отдельных пакетов не будут указываться.</span><span class="sxs-lookup"><span data-stu-id="70a96-1053">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="70a96-1054">Если команда доступна в предварительной версии, это также касается и всех ее аргументов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1054">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="70a96-1055">Если группа команд помечается как находящаяся в предварительной версии, значит все команды и аргументы также считаются доступными в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="70a96-1055">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="70a96-1056">В результате этого изменения несколько групп команд могут "внезапно" оказаться в состоянии предварительной версии в этом выпуске.</span><span class="sxs-lookup"><span data-stu-id="70a96-1056">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="70a96-1057">В действительности большинство пакетов, которые находились в состоянии предварительной версии, в этом выпуске будут считаться общедоступными.</span><span class="sxs-lookup"><span data-stu-id="70a96-1057">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-1058">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-1058">ACR</span></span>
* <span data-ttu-id="70a96-1059">Добавлена команда acr check-health.</span><span class="sxs-lookup"><span data-stu-id="70a96-1059">Added 'acr check-health' command</span></span>
* <span data-ttu-id="70a96-1060">Улучшена обработка ошибок с маркерами безопасности AAD и ошибок при получении внешних команд.</span><span class="sxs-lookup"><span data-stu-id="70a96-1060">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-1061">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-1061">ACS</span></span>
* <span data-ttu-id="70a96-1062">Устаревшие команды ACS теперь скрыты в тексте справки.</span><span class="sxs-lookup"><span data-stu-id="70a96-1062">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="70a96-1063">AMS</span><span class="sxs-lookup"><span data-stu-id="70a96-1063">AMS</span></span>
* <span data-ttu-id="70a96-1064">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в возврате строк времени ISO 8601 для archive-window-length и key-frame-interval-duration.</span><span class="sxs-lookup"><span data-stu-id="70a96-1064">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-1065">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-1065">AppService</span></span>
* <span data-ttu-id="70a96-1066">Добавлена маршрутизация на основе расположение для `webapp deleted list` и `webapp deleted restore`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1066">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="70a96-1067">Исправлена проблема, при которой целевой URL-адрес веб-приложения ("Вы можете запустить приложение в...") не был активным в Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="70a96-1067">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="70a96-1068">Устранена проблема, при которой создание приложений в некоторых SKU завершалось сбоем с ошибкой AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="70a96-1068">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="70a96-1069">Добавлена предварительная проверка в `[appservice|webapp] create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1069">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="70a96-1070">Исправлено `[webapp|functionapp] traffic-routing` для использования правильного actionHostName.</span><span class="sxs-lookup"><span data-stu-id="70a96-1070">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="70a96-1071">Добавлена поддержка слотов для команд `functionapp`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1071">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="70a96-1072">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-1072">Batch</span></span>
* <span data-ttu-id="70a96-1073">Исправлена регрессия проверки подлинности AAD, которую вызывал чрезмерный поток уведомлений об авторизации с помощью общего ключа.</span><span class="sxs-lookup"><span data-stu-id="70a96-1073">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="70a96-1074">Batch AI</span><span class="sxs-lookup"><span data-stu-id="70a96-1074">BatchAI</span></span>
* <span data-ttu-id="70a96-1075">Команды BatchAI теперь признаны устаревшими и скрыты.</span><span class="sxs-lookup"><span data-stu-id="70a96-1075">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="70a96-1076">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="70a96-1076">BotService</span></span>
* <span data-ttu-id="70a96-1077">Добавлены предупреждающие сообщения о прекращении поддержки и режиме обслуживания для команд, которые поддерживают пакет SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="70a96-1077">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="70a96-1078">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70a96-1078">CosmosDB</span></span>
* <span data-ttu-id="70a96-1079">[УСТАРЕЛО] использовать команду `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1079">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="70a96-1080">Добавлена команда `cosmosdb keys list`, заменяющая `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1080">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="70a96-1081">`cosmsodb create/update`: Добавлен новый формат для --location, который позволяет задавать свойство isZoneRedundant.</span><span class="sxs-lookup"><span data-stu-id="70a96-1081">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="70a96-1082">Нерекомендуемый старый формат.</span><span class="sxs-lookup"><span data-stu-id="70a96-1082">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="70a96-1083">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="70a96-1083">EventGrid</span></span>
* <span data-ttu-id="70a96-1084">Добавлены команды `eventgrid domain` для операций CRUD домена.</span><span class="sxs-lookup"><span data-stu-id="70a96-1084">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="70a96-1085">Добавлены команды `eventgrid domain topic` для операций CRUD разделов домена.</span><span class="sxs-lookup"><span data-stu-id="70a96-1085">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="70a96-1086">В `eventgrid [topic|event-subscription] list` добавлен аргумент `--odata-query` для фильтрации результатов с использованием синтаксиса OData.</span><span class="sxs-lookup"><span data-stu-id="70a96-1086">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="70a96-1087">`event-subscription create/update`: Добавлена ServiceBusQueue в качестве новых значений для параметра `--endpoint-type`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1087">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="70a96-1088">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в прекращении поддержки `--included-event-types All` с `eventgrid event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1088">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="70a96-1089">HDInsight</span><span class="sxs-lookup"><span data-stu-id="70a96-1089">HDInsight</span></span>
* <span data-ttu-id="70a96-1090">Добавлена поддержка параметра `--ssh-public-key` в команде `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1090">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="70a96-1091">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-1091">IoT</span></span>
* <span data-ttu-id="70a96-1092">Добавлена поддержка для повторного создания ключей политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="70a96-1092">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="70a96-1093">Добавлен пакет SDK и поддержка для службы подготовки репозитория DigitalTwin.</span><span class="sxs-lookup"><span data-stu-id="70a96-1093">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="70a96-1094">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-1094">Network</span></span>
* <span data-ttu-id="70a96-1095">Добавлена поддержка зон для Шлюза NAT.</span><span class="sxs-lookup"><span data-stu-id="70a96-1095">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="70a96-1096">Добавлена команда `network list-service-tags`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1096">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="70a96-1097">Исправлена проблема с `dns zone import`, при которой пользователям не удавалось импортировать записи А с подстановочным знаком.</span><span class="sxs-lookup"><span data-stu-id="70a96-1097">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="70a96-1098">Исправлена проблема с `watcher flow-log configure`, при которой не удавалось включить ведение журнала потоков в определенных регионах.</span><span class="sxs-lookup"><span data-stu-id="70a96-1098">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-1099">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-1099">Resource</span></span>
* <span data-ttu-id="70a96-1100">Добавлена команда `az rest` для вызовов REST.</span><span class="sxs-lookup"><span data-stu-id="70a96-1100">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="70a96-1101">Исправлена ошибка, возникавшая при использовании `policy assignment list` с группой ресурсов или уровнем подписки `--scope`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1101">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="70a96-1102">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="70a96-1102">ServiceBus</span></span>
* <span data-ttu-id="70a96-1103">Устранена проблема № [9319](https://github.com/azure/azure-cli/issues/9319) с `servicebus topic create --max-size`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1103">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-1104">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-1104">SQL</span></span>
* <span data-ttu-id="70a96-1105">Параметр `--location` стал необязательным для `sql [server|mi] create`. Если он не указан, используется расположение группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1105">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="70a96-1106">Исправлена ошибка "Объект NoneType не подлежит итерации" с `sql db list-editions --available`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1106">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="70a96-1107">SQLVm</span><span class="sxs-lookup"><span data-stu-id="70a96-1107">SQLVm</span></span>
* <span data-ttu-id="70a96-1108">Критическое изменение. Для `sql vm create` теперь требуется параметр `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1108">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="70a96-1109">Внесены изменения, позволяющие задавать SKU образа SQL при создании или обновлении виртуальной машины SQL.</span><span class="sxs-lookup"><span data-stu-id="70a96-1109">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-1110">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-1110">Storage</span></span>
* <span data-ttu-id="70a96-1111">Исправлена проблема с отсутствующим ключом учетной записи для `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1111">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="70a96-1112">Исправлена проблема с `storage blob sync` на платформе Linux.</span><span class="sxs-lookup"><span data-stu-id="70a96-1112">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-1113">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-1113">VM</span></span>
* <span data-ttu-id="70a96-1114">[Предварительная версия] Добавлены команды `vm image template` для создания образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="70a96-1114">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="70a96-1115">4 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1115">June 4, 2019</span></span>

<span data-ttu-id="70a96-1116">Версия 2.0.66</span><span class="sxs-lookup"><span data-stu-id="70a96-1116">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="70a96-1117">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-1117">Core</span></span>
* <span data-ttu-id="70a96-1118">Исправлена ошибка, из-за которой выполнение команды завершалось со сбоем, если параметр `--output yaml` использовался с параметром `--query`</span><span class="sxs-lookup"><span data-stu-id="70a96-1118">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-1119">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-1119">ACR</span></span>
* <span data-ttu-id="70a96-1120">Добавлена группа команд acr pack для создания заданий быстрой сборки с помощью пакетов сборок.</span><span class="sxs-lookup"><span data-stu-id="70a96-1120">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-1121">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-1121">ACS</span></span>
* <span data-ttu-id="70a96-1122">Разрешено включение и отключение надстройки панели мониторинга Kubernetes для AKS.</span><span class="sxs-lookup"><span data-stu-id="70a96-1122">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="70a96-1123">Если подписку нельзя использовать с Azure Red Hat OpenShift, будет отображаться соответствующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="70a96-1123">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="70a96-1124">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-1124">Batch</span></span>
* <span data-ttu-id="70a96-1125">Улучшена обработка ошибок, если не выполнен вход в учетную запись \[[№ 9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[№ 8978](https://github.com/Azure/azure-cli/issues/8978)\].</span><span class="sxs-lookup"><span data-stu-id="70a96-1125">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="70a96-1126">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-1126">IoT</span></span>
* <span data-ttu-id="70a96-1127">Добавлена поддержка для перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="70a96-1127">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="70a96-1128">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-1128">Network</span></span>
* <span data-ttu-id="70a96-1129">Добавлены команды `network application-gateway waf-policy` для поддержки настраиваемых правил WAF.</span><span class="sxs-lookup"><span data-stu-id="70a96-1129">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="70a96-1130">Добавлены аргументы `--waf-policy` и `--max-capacity` для команды `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="70a96-1130">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="70a96-1131">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-1131">Resource</span></span>
* <span data-ttu-id="70a96-1132">Улучшен вывод сообщения команды `deployment create` при отсутствии TTY.</span><span class="sxs-lookup"><span data-stu-id="70a96-1132">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="70a96-1133">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-1133">Role</span></span>
* <span data-ttu-id="70a96-1134">Обновлен текст справки.</span><span class="sxs-lookup"><span data-stu-id="70a96-1134">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="70a96-1135">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="70a96-1135">Compute</span></span>
* <span data-ttu-id="70a96-1136">Добавлена поддержка команды `vm create` для создания виртуальных машин из управляемого образа с номерами LUN дисков данных, которые не начинаются с 0 или для которых пропущены номера.</span><span class="sxs-lookup"><span data-stu-id="70a96-1136">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="70a96-1137">21 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1137">May 21, 2019</span></span>

<span data-ttu-id="70a96-1138">Версия 2.0.65</span><span class="sxs-lookup"><span data-stu-id="70a96-1138">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="70a96-1139">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-1139">Core</span></span>
* <span data-ttu-id="70a96-1140">Улучшена функция обратной связи при ошибках аутентификации.</span><span class="sxs-lookup"><span data-stu-id="70a96-1140">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="70a96-1141">Исправлена проблема, из-за которой интерфейс командной строки загружал расширения, которые не были совместимы с его базовой версией.</span><span class="sxs-lookup"><span data-stu-id="70a96-1141">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="70a96-1142">Исправлена проблема с запуском и неисправностью `clouds.config`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1142">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-1143">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-1143">ACR</span></span>
* <span data-ttu-id="70a96-1144">Добавлена поддержка управляемых удостоверений в Задачи.</span><span class="sxs-lookup"><span data-stu-id="70a96-1144">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-1145">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-1145">ACS</span></span>
* <span data-ttu-id="70a96-1146">Исправлена команда `openshift create`, используемая с пользовательским клиентом AAD.</span><span class="sxs-lookup"><span data-stu-id="70a96-1146">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-1147">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-1147">AppService</span></span>
* <span data-ttu-id="70a96-1148">[УСТАРЕЛО] Команда `functionapp devops-build` устарела и будет удалена в следующем выпуске.</span><span class="sxs-lookup"><span data-stu-id="70a96-1148">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="70a96-1149">Внесено изменение в `functionapp devops-pipeline` для получения журнала сборки из Azure DevOps в режиме подробного протоколирования.</span><span class="sxs-lookup"><span data-stu-id="70a96-1149">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="70a96-1150">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален неподдерживаемый флаг `--use_local_settings` из команды `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1150">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="70a96-1151">Внесено изменение в `webapp up` для возврата выходных данных JSON, если `--logs` не используется.</span><span class="sxs-lookup"><span data-stu-id="70a96-1151">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="70a96-1152">Добавлена поддержка записи ресурсов по умолчанию в локальную конфигурацию для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1152">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="70a96-1153">Добавлена поддержка `webapp up` для повторного развертывания приложения без использования аргумента `--location`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1153">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="70a96-1154">Устранена проблема, из-за которой нельзя было создать для Linux номер SKU с планом службы приложений "Бесплатный".</span><span class="sxs-lookup"><span data-stu-id="70a96-1154">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="70a96-1155">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="70a96-1155">BotService</span></span>
* <span data-ttu-id="70a96-1156">Внесено изменение для включения поддержки всех регистров в параметрах `--lang` для команд.</span><span class="sxs-lookup"><span data-stu-id="70a96-1156">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="70a96-1157">Обновлено описание модуля команды.</span><span class="sxs-lookup"><span data-stu-id="70a96-1157">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="70a96-1158">Потребление</span><span class="sxs-lookup"><span data-stu-id="70a96-1158">Consumption</span></span>
* <span data-ttu-id="70a96-1159">Добавлен отсутствующий обязательный параметр при выполнении `consumption usage list --billing-period-name`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1159">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="70a96-1160">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-1160">IoT</span></span>
* <span data-ttu-id="70a96-1161">Добавлена поддержка перечисления всех ключей.</span><span class="sxs-lookup"><span data-stu-id="70a96-1161">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="70a96-1162">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-1162">Network</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="70a96-1164">Добавлен аргумент `--nat-gateway` для `network vnet subnet [create|update]` для подключения к шлюзу NAT.</span><span class="sxs-lookup"><span data-stu-id="70a96-1164">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="70a96-1165">Исправлена проблема с `dns zone import`, из-за которой имена записей не сопоставлялись с типом записей.</span><span class="sxs-lookup"><span data-stu-id="70a96-1165">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="70a96-1166">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="70a96-1166">RDBMS</span></span>
* <span data-ttu-id="70a96-1167">Добавлена поддержка Postgres и MySQL для георепликации.</span><span class="sxs-lookup"><span data-stu-id="70a96-1167">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="70a96-1168">RBAC</span><span class="sxs-lookup"><span data-stu-id="70a96-1168">RBAC</span></span>
* <span data-ttu-id="70a96-1169">Добавлена поддержка области группы управления для `role assignment`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1169">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-1170">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-1170">Storage</span></span>
* <span data-ttu-id="70a96-1171">`storage blob sync`: добавьте команду синхронизации для хранилища BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1171">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="70a96-1172">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="70a96-1172">Compute</span></span>
* <span data-ttu-id="70a96-1173">Добавлен параметр `--computer-name` для `vm create` для установки имени виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="70a96-1173">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="70a96-1174">Переименован параметр `--ssh-key-value` в `--ssh-key-values` для `[vm|vmss] create` для приема нескольких значений пути или открытого ключа SSH.</span><span class="sxs-lookup"><span data-stu-id="70a96-1174">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="70a96-1175">__Примечание.__ Это **не** критическое изменение, благодаря которому `--ssh-key-value` будет правильно анализироваться, так как соответствует только `--ssh-key-values`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1175">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="70a96-1176">Внесено изменение в аргумент `ppg create` для `--type` — теперь он необязательный.</span><span class="sxs-lookup"><span data-stu-id="70a96-1176">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="70a96-1177">6 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1177">May 6, 2019</span></span>

<span data-ttu-id="70a96-1178">Версия 2.0.64</span><span class="sxs-lookup"><span data-stu-id="70a96-1178">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-1179">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-1179">ACS</span></span>
* <span data-ttu-id="70a96-1180">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--fqdn` из команд `openshift`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1180">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="70a96-1181">Внесено изменение для использования общедоступной версии API для Azure Red Hat Openshift.</span><span class="sxs-lookup"><span data-stu-id="70a96-1181">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="70a96-1182">Добавлен флаг `customer-admin-group-id` в `openshift create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1182">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="70a96-1183">[Общедоступная версия.] `(PREVIEW)` больше не используется для `aks create` в параметре `--network-policy`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1183">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-1184">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-1184">Appservice</span></span>
* <span data-ttu-id="70a96-1185">[УСТАРЕЛО] Команда `functionapp devops-build` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="70a96-1185">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="70a96-1186">Команда переименована в `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1186">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="70a96-1187">Исправлен процесс получения правильного имени пользователя для Cloud Shell, приводивший к ошибке выполнения `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1187">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="70a96-1188">Обновлена документация по `appservice plan --sku` в соответствии с поддерживаемыми планами службы приложений.</span><span class="sxs-lookup"><span data-stu-id="70a96-1188">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="70a96-1189">Добавлены необязательные аргументы для группы ресурсов и план для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1189">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="70a96-1190">Добавлена поддержка `webapp ssh` в соответствии с переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1190">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="70a96-1191">Добавлена поддержка `appserviceplan create` для ценовой категории "Бесплатный" в Linux.</span><span class="sxs-lookup"><span data-stu-id="70a96-1191">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="70a96-1192">Внесено изменение в `webapp up` для перевода в спящий режим на 30 с после установки параметра приложения `SCM_DO_BUILD_DURING_DEPLOYMENT=true` для обработки холодного запуска Kudu.</span><span class="sxs-lookup"><span data-stu-id="70a96-1192">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="70a96-1193">Добавлена поддержка среды выполнения `powershell` для `functionapp create` в Windows.</span><span class="sxs-lookup"><span data-stu-id="70a96-1193">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="70a96-1194">Добавлена команда `create-remote-connection`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1194">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="70a96-1195">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-1195">Batch</span></span>
* <span data-ttu-id="70a96-1196">Исправлена ошибка в проверяющем элементе управления для параметров `--application-package-references`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1196">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="70a96-1197">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="70a96-1197">Botservice</span></span>
* <span data-ttu-id="70a96-1198">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` для создания пустого бота веб-приложения по умолчанию (т. е. бот не развертывается в Службе приложений).</span><span class="sxs-lookup"><span data-stu-id="70a96-1198">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="70a96-1199">Добавлен флаг `--echo` в `bot create` для использования старого поведения с `-v v4`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1199">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="70a96-1200">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено значение по умолчанию `--version` на `v4`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1200">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="70a96-1201">__ПРИМЕЧАНИЕ.__ `bot prepare-publish` по-прежнему использует старое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-1201">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="70a96-1202">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `--lang` — значение `Csharp` больше не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-1202">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="70a96-1203">Если команда требует `--lang`, который не указан, команда завершит работу с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="70a96-1203">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="70a96-1204">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в аргументы `--appid` и `--password` для `bot create` — теперь они являются обязательными и их можно создать с помощью `ad app create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1204">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="70a96-1205">Добавлена проверка `--appid` и `--password`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1205">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="70a96-1206">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4`, чтобы не создавать или не использовать учетную запись хранения или Application Insights.</span><span class="sxs-lookup"><span data-stu-id="70a96-1206">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="70a96-1207">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v3`, чтобы требовать регион, где доступна служба Application Insights.</span><span class="sxs-lookup"><span data-stu-id="70a96-1207">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="70a96-1208">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot update`, чтобы влиять только на определенные свойства бота.</span><span class="sxs-lookup"><span data-stu-id="70a96-1208">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="70a96-1209">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в флаг `--lang` для принятия `Javascript` вместо `Node`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1209">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="70a96-1210">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`Node` больше не используется как допустимое значение `--lang`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1210">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="70a96-1211">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` — значение `SCM_DO_BUILD_DURING_DEPLOYMENT` больше не равно true.</span><span class="sxs-lookup"><span data-stu-id="70a96-1211">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="70a96-1212">Все развертывания через Kudu будут работать в соответствии с поведением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-1212">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="70a96-1213">Внесено изменение в `bot download` для ботов без файлов `.bot`, чтобы создавать файл конфигурации для определенного языка со значениями из параметров приложения для бота.</span><span class="sxs-lookup"><span data-stu-id="70a96-1213">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="70a96-1214">В команду `bot prepare-deploy` добавлена поддержка параметра `Typescript`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1214">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="70a96-1215">Добавлено предупреждающее сообщение в `bot prepare-deploy` для ботов `Javascript` и `Typescript`, когда `--code-dir` не содержит `package.json`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1215">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="70a96-1216">Внесено изменение в `bot prepare-deploy` для возврата `true` при успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="70a96-1216">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="70a96-1217">Включено ведение подробного журнала для `bot prepare-deploy`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1217">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="70a96-1218">Добавлены более доступные регионы Application Insights для `az bot create -v v3`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1218">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="70a96-1219">Configure</span><span class="sxs-lookup"><span data-stu-id="70a96-1219">Configure</span></span>
* <span data-ttu-id="70a96-1220">Добавлена поддержка конфигурации по умолчанию для аргумента на основе папки.</span><span class="sxs-lookup"><span data-stu-id="70a96-1220">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="70a96-1221">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="70a96-1221">Eventhubs</span></span>
* <span data-ttu-id="70a96-1222">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1222">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="70a96-1223">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1223">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="70a96-1224">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-1224">Network</span></span>
* <span data-ttu-id="70a96-1225">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--cache` на `--defer` для `vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1225">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="70a96-1226">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="70a96-1226">Policy Insights</span></span>
* <span data-ttu-id="70a96-1227">Добавлена поддержка `--expand PolicyEvaluationDetails` для результатов оценки политики запросов для ресурса.</span><span class="sxs-lookup"><span data-stu-id="70a96-1227">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="70a96-1228">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-1228">Role</span></span>
* <span data-ttu-id="70a96-1229">[УСТАРЕЛО] Внесено изменение в `create-for-rbac` для скрытия аргумента --password (поддержка прекращается в мае 2019 г.).</span><span class="sxs-lookup"><span data-stu-id="70a96-1229">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="70a96-1230">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="70a96-1230">Service Bus</span></span>
* <span data-ttu-id="70a96-1231">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1231">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="70a96-1232">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1232">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="70a96-1233">Внесено исправление в `topic [create|update]` — теперь `--max-size` поддерживает значения 10, 20, 40 и 80 ГБ для номера SKU ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="70a96-1233">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-1234">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-1234">SQL</span></span>
* <span data-ttu-id="70a96-1235">Добавлены команды `sql virtual-cluster [list|show|delete]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1235">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-1236">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-1236">VM</span></span>
* <span data-ttu-id="70a96-1237">Добавлены параметры `--protect-from-scale-in` и `--protect-from-scale-set-actions` для `vmss update`, чтобы включать обновления политики защиты для экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="70a96-1237">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="70a96-1238">Добавлены параметры `--instance-id` для `vmss update` для включения общего обновления экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="70a96-1238">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="70a96-1239">Добавлен параметр `--instance-id` для команды `vmss wait`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1239">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="70a96-1240">Добавлена новая группа команд `ppg` для управления группами размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="70a96-1240">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="70a96-1241">Добавлен параметр `--ppg` для `[vm|vmss] create` и `vm availability-set create` для управления PPG.</span><span class="sxs-lookup"><span data-stu-id="70a96-1241">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="70a96-1242">Добавлен параметр `--hyper-v-generation` для команды `image create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1242">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="70a96-1243">23 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1243">April 23, 2019</span></span>

<span data-ttu-id="70a96-1244">Версия 2.0.63</span><span class="sxs-lookup"><span data-stu-id="70a96-1244">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-1245">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-1245">ACS</span></span>
* <span data-ttu-id="70a96-1246">Внесено изменение в `aks get-credentials` для запроса на перезапись повторяющихся значений.</span><span class="sxs-lookup"><span data-stu-id="70a96-1246">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="70a96-1247">Удалено описание `(PREVIEW)` из команд Dev Spaces aks use-dev-spaces и aks remove-dev-spaces.</span><span class="sxs-lookup"><span data-stu-id="70a96-1247">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="70a96-1248">AMS</span><span class="sxs-lookup"><span data-stu-id="70a96-1248">AMS</span></span>
* <span data-ttu-id="70a96-1249">Исправлена ошибка с обновлением фильтров ресурсов и учетных записей.</span><span class="sxs-lookup"><span data-stu-id="70a96-1249">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-1250">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-1250">AppService</span></span>
* <span data-ttu-id="70a96-1251">Добавлена поддержка ASE и времени ожидания для `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1251">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="70a96-1252">Добавлена возможность настройки непрерывной интеграции и развертывания в конвейере Azure DevOps из репозитория Github для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="70a96-1252">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="70a96-1253">Добавлен аргумент `--github-pat` для `functionapp devops-build create` для получения личного маркера доступа Github.</span><span class="sxs-lookup"><span data-stu-id="70a96-1253">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="70a96-1254">Добавлен аргумент `--github-repository` для `functionapp devops-build create` для подключения репозитория Github, который содержит исходный код приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="70a96-1254">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="70a96-1255">Исправлена проблема со сбоем `az webapp up --logs` и обновлением .Net Core до версии 2.1 по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-1255">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="70a96-1256">Удалены ненужные параметры приложения-функции при создании приложения-функции с помощью плана потребления.</span><span class="sxs-lookup"><span data-stu-id="70a96-1256">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="70a96-1257">Внесены изменения в `webapp up`, чтобы строка ASP по умолчанию добавляла номера в конец для создания плана службы приложений на основе параметров SKU.</span><span class="sxs-lookup"><span data-stu-id="70a96-1257">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="70a96-1258">Добавлен параметр `-b` для `webapp up` для запуска приложения в браузере.</span><span class="sxs-lookup"><span data-stu-id="70a96-1258">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="70a96-1259">Внесены изменения в `webapp deployment source config zip` для обработки переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1259">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="70a96-1260">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="70a96-1260">Deployment Manager</span></span>
* <span data-ttu-id="70a96-1261">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Создание и администрирование артефактов, которые поддерживают развертывания</span><span class="sxs-lookup"><span data-stu-id="70a96-1261">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="70a96-1262">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="70a96-1262">Lab</span></span>
* <span data-ttu-id="70a96-1263">Исправлена ошибка, которая приводила к неожиданному завершению работы.</span><span class="sxs-lookup"><span data-stu-id="70a96-1263">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="70a96-1264">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-1264">Network</span></span>
* <span data-ttu-id="70a96-1265">Добавлено автоматическое делегирование сервера имен для `dns zone create` в родительском объекте во время создания дочерней зоны.</span><span class="sxs-lookup"><span data-stu-id="70a96-1265">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-1266">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-1266">Resource</span></span>
* <span data-ttu-id="70a96-1267">[УСТАРЕЛО] Не рекомендуются к использованию аргументы `--link-id`, `--target-id` и `--filter-string` для `resource link`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1267">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="70a96-1268">Используйте вместо них аргументы `--link`, `--target` и `--filter`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1268">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="70a96-1269">Исправлена проблема, из-за которой команды `resource link [create|update]` не работали.</span><span class="sxs-lookup"><span data-stu-id="70a96-1269">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="70a96-1270">Исправлена проблема, из-за которой удаление с помощью идентификатора ресурса приводило к сбою или ошибке.</span><span class="sxs-lookup"><span data-stu-id="70a96-1270">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-1271">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-1271">SQL</span></span>
* <span data-ttu-id="70a96-1272">Добавлена поддержка пользовательского часового пояса в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="70a96-1272">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="70a96-1273">Внесено изменение, чтобы разрешить использовать имя эластичного пула с `sql db update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1273">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="70a96-1274">В команду `sql server [create|update]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1274">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="70a96-1275">Добавлена команда `sql server wait`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1275">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-1276">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-1276">Storage</span></span>
* <span data-ttu-id="70a96-1277">Устранена проблема с двойной кодировкой маркеров SAS в `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1277">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-1278">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-1278">VM</span></span>
* <span data-ttu-id="70a96-1279">Добавлен флаг `--skip-shutdown` для `vm|vmss stop` для выключения виртуальных машин без завершения работы.</span><span class="sxs-lookup"><span data-stu-id="70a96-1279">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="70a96-1280">Добавлен аргумент `--storage-account-type` для `sig image-version create` настройки типа учетной записи профиля публикации.</span><span class="sxs-lookup"><span data-stu-id="70a96-1280">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="70a96-1281">Добавлен аргумент `--target-regions` для `sig image-version create` для указания типов учетных записей хранения, связанных с регионами.</span><span class="sxs-lookup"><span data-stu-id="70a96-1281">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="70a96-1282">9 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1282">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="70a96-1283">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-1283">Core</span></span>
* <span data-ttu-id="70a96-1284">Исправлена проблема, из-за которой для некоторых расширений отображалась версия `Unknown` и ее невозможно было обновить.</span><span class="sxs-lookup"><span data-stu-id="70a96-1284">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-1285">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-1285">ACR</span></span>
* <span data-ttu-id="70a96-1286">Добавлена поддержка запуска образа без контекста.</span><span class="sxs-lookup"><span data-stu-id="70a96-1286">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="70a96-1287">AMS</span><span class="sxs-lookup"><span data-stu-id="70a96-1287">AMS</span></span>
* [УСТАРЕЛО]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="70a96-1290">Добавлена поддержка новых параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1290">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="70a96-1291">Добавлен новый параметр `--filters` для `ams streaming-locator create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1291">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-1292">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-1292">AppService</span></span>
* <span data-ttu-id="70a96-1293">В команду `webapp up` добавлена поддержка параметра `--logs`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1293">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="70a96-1294">Исправлены ошибки в команде `functionapp devops-build create` при создании файла `azure-pipelines.yml`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1294">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="70a96-1295">Улучшена обработка и индикаторы ошибок с `unctionapp devops-build create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1295">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="70a96-1296">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--local-git` для команды `devops-build`. Обнаружение и обработка локального репозитория Git являются обязательными для создания конвейеров DevOps в Azure.</span><span class="sxs-lookup"><span data-stu-id="70a96-1296">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="70a96-1297">Добавлена поддержка создания плана функций Linux.</span><span class="sxs-lookup"><span data-stu-id="70a96-1297">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="70a96-1298">Добавлена возможность менять план для приложения-функции с помощью `functionapp update --plan`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1298">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="70a96-1299">Добавлена поддержка параметров горизонтального увеличения масштаба плана "Премиум" для Функций Azure.</span><span class="sxs-lookup"><span data-stu-id="70a96-1299">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="70a96-1300">CDN</span><span class="sxs-lookup"><span data-stu-id="70a96-1300">CDN</span></span>
* <span data-ttu-id="70a96-1301">Добавлена поддержка `Microsoft_Standard` и `Standard_ChinaCdn`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1301">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="70a96-1302">Отзывы</span><span class="sxs-lookup"><span data-stu-id="70a96-1302">Feedback</span></span>
* <span data-ttu-id="70a96-1303">Внесены изменения в `feedback` для отображения метаданных недавно выполненных команд.</span><span class="sxs-lookup"><span data-stu-id="70a96-1303">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="70a96-1304">Внесены изменения в `feedback`. Теперь при регистрации проблемы отображается запрос, в соответствии с которым пользователь должен открыть браузер и воспользоваться шаблоном проблемы.</span><span class="sxs-lookup"><span data-stu-id="70a96-1304">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="70a96-1305">Внесены изменения в `feedback`. Теперь текст проблемы выводится при запуске с параметром --verbose.</span><span class="sxs-lookup"><span data-stu-id="70a96-1305">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-1306">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-1306">Monitor</span></span>
* <span data-ttu-id="70a96-1307">Исправлена проблема, из-за которой у параметра count было недопустимое значение в `metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1307">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="70a96-1308">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-1308">Network</span></span>
* <span data-ttu-id="70a96-1309">Исправлен формат таблицы, которая не отображалась с помощью `vnet-gateway list-bgp-peer-status`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1309">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="70a96-1310">Добавлены команды `list-request-headers` и `list-response-headers` для `application-gateway rewrite-rule`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1310">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="70a96-1311">Добавлена команда `list-server-variables` для `application-gateway rewrite-rule condition`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1311">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="70a96-1312">Исправлена проблема, из-за которой обновление состояния соединения на порту ExpressRoute вызывало неизвестное исключение атрибута `express-route port update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1312">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="70a96-1313">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="70a96-1313">PrivateDNS</span></span>
* <span data-ttu-id="70a96-1314">Добавлена команда `network private-dns` для частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="70a96-1314">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-1315">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-1315">Resource</span></span>
* <span data-ttu-id="70a96-1316">Исправлена проблема с `deployment create` и `group deployment create`, из-за которой файл параметров с пустым набором параметров не работал.</span><span class="sxs-lookup"><span data-stu-id="70a96-1316">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="70a96-1317">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-1317">Role</span></span>
* <span data-ttu-id="70a96-1318">Внесены исправления в `create-for-rbac`. Теперь `--years` обрабатывается правильно.</span><span class="sxs-lookup"><span data-stu-id="70a96-1318">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="70a96-1319">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `role assignment delete`. Теперь появляется запрос при удалении всех назначений в рамках подписки без дополнительных условий.</span><span class="sxs-lookup"><span data-stu-id="70a96-1319">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-1320">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-1320">SQL</span></span>
* <span data-ttu-id="70a96-1321">Команда `sql mi [create|update]` обновлена с помощью свойств proxyOverride и publicDataEndpointEnabled.</span><span class="sxs-lookup"><span data-stu-id="70a96-1321">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-1322">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-1322">Storage</span></span>
* <span data-ttu-id="70a96-1323">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален результат выполнения `storage blob delete`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1323">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="70a96-1324">В команду `storage blob generate-sas` добавлен параметр `--full-uri` для создания полного URI большого двоичного объекта с помощью SAS.</span><span class="sxs-lookup"><span data-stu-id="70a96-1324">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="70a96-1325">В команду `storage file copy start` добавлен параметр `--file-snapshot` для копирования файла из моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="70a96-1325">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="70a96-1326">Внесены изменения в `storage blob copy cancel`. Теперь вместо исключения для NoPendingCopyOperation отображается только сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="70a96-1326">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="70a96-1327">26 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1327">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="70a96-1328">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-1328">Core</span></span>
* <span data-ttu-id="70a96-1329">Устранены проблемы с несовместимостью расширений для разработки.</span><span class="sxs-lookup"><span data-stu-id="70a96-1329">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="70a96-1330">Функция обработки ошибок теперь указывает клиентам на страницу проблем.</span><span class="sxs-lookup"><span data-stu-id="70a96-1330">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="70a96-1331">Cloud</span><span class="sxs-lookup"><span data-stu-id="70a96-1331">Cloud</span></span>
* <span data-ttu-id="70a96-1332">Исправлена ошибка с сообщением о не найденной подписке в `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1332">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-1333">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-1333">ACR</span></span>
* <span data-ttu-id="70a96-1334">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="70a96-1334">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="70a96-1335">Добавлено `--auth-mode` в команды `acr build`, `acr run`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1335">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="70a96-1336">Добавлена команда acr task credential для управления учетными данными для задачи.</span><span class="sxs-lookup"><span data-stu-id="70a96-1336">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="70a96-1337">Добавлено --no-wait в команду `acr build`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1337">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-1338">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-1338">AppService</span></span>
* <span data-ttu-id="70a96-1339">Исправлена ошибка с `webapp up`, из-за которой нельзя было правильно выполнить запуск из пустого каталога или скрипта неизвестного кода.</span><span class="sxs-lookup"><span data-stu-id="70a96-1339">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="70a96-1340">Исправлена ошибка, из-за которой не работали слоты для `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1340">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="70a96-1341">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="70a96-1341">BOT Service</span></span>
* <span data-ttu-id="70a96-1342">Добавлено `bot prepare-deploy` для подготовки к развертыванию ботов с помощью `webapp`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1342">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="70a96-1343">Изменено `bot create --kind registration` для отображения пароля, если пароль не указан.</span><span class="sxs-lookup"><span data-stu-id="70a96-1343">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="70a96-1344">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--endpoint` в `bot create --kind registration` на пустую строку (по умолчанию) вместо запрашиваемой.</span><span class="sxs-lookup"><span data-stu-id="70a96-1344">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="70a96-1345">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="70a96-1345">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="70a96-1346">CDN</span><span class="sxs-lookup"><span data-stu-id="70a96-1346">CDN</span></span>
* <span data-ttu-id="70a96-1347">Добавлена поддержка параметра `--no-wait` в команде `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1347">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="70a96-1348">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено поведение кэширования строки запроса `cdn endpoint create` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-1348">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="70a96-1349">IgnoreQueryString больше не используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-1349">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="70a96-1350">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="70a96-1350">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="70a96-1351">Сosmos DB</span><span class="sxs-lookup"><span data-stu-id="70a96-1351">Cosmosdb</span></span>
* <span data-ttu-id="70a96-1352">Добавлена поддержка `--enable-multiple-write-locations` для обновления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="70a96-1352">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="70a96-1353">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="70a96-1353">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="70a96-1354">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="70a96-1354">Interactive</span></span>
* <span data-ttu-id="70a96-1355">Исправлена несовместимость с интерактивным расширением, установленным с помощью azdev.</span><span class="sxs-lookup"><span data-stu-id="70a96-1355">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-1356">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-1356">Monitor</span></span>
* <span data-ttu-id="70a96-1357">Внесено изменение, разрешающее использовать значение измерения `*` для `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1357">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="70a96-1358">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-1358">Network</span></span>
* <span data-ttu-id="70a96-1359">Добавлена группа команд `rewrite-rule` для `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1359">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="70a96-1360">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-1360">Profile</span></span>
* <span data-ttu-id="70a96-1361">Включена поддержка учетной записи уровня клиентов для управляемого удостоверения службы для `login`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1361">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="70a96-1362">Postgres</span><span class="sxs-lookup"><span data-stu-id="70a96-1362">Postgres</span></span> 
* <span data-ttu-id="70a96-1363">Добавлены команды postgresql `replica` и команда `restart server`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1363">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="70a96-1364">Внесены изменения для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="70a96-1364">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-1365">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-1365">Resource</span></span>
* <span data-ttu-id="70a96-1366">Улучшены табличные выходные данные для `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1366">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="70a96-1367">Исправлена проблема с `deployment [create|validate]`, из-за которой secureObject типа не распознавался.</span><span class="sxs-lookup"><span data-stu-id="70a96-1367">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="70a96-1368">График</span><span class="sxs-lookup"><span data-stu-id="70a96-1368">Graph</span></span>
* <span data-ttu-id="70a96-1369">Добавлена поддержка параметра `--end-date` в команде `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1369">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="70a96-1370">Добавлена поддержка разрешений для `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1370">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="70a96-1371">Исправлена проблема с `ad app permission list`, из-за которой отсутствовали разрешения.</span><span class="sxs-lookup"><span data-stu-id="70a96-1371">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="70a96-1372">Изменено `ad sp delete` для пропуска удаления назначения роли, если текущая учетная запись не содержит подписок.</span><span class="sxs-lookup"><span data-stu-id="70a96-1372">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="70a96-1373">Изменено `ad app create` для использования `--identifier-uris` пустого списка (по умолчанию), если список не указан.</span><span class="sxs-lookup"><span data-stu-id="70a96-1373">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-1374">носителей.</span><span class="sxs-lookup"><span data-stu-id="70a96-1374">storage</span></span>
* <span data-ttu-id="70a96-1375">Добавлено `--snapshot` для `storage file download-batch` для скачивания из моментального снимка общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="70a96-1375">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="70a96-1376">Изменен индикатор выполнения `storage blob [download-batch|upload-batch]`, чтобы обобщить сведения и указать текущий большой двоичный объект.</span><span class="sxs-lookup"><span data-stu-id="70a96-1376">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="70a96-1377">Исправлена проблема с `storage account update` при обновлении параметров шифрования.</span><span class="sxs-lookup"><span data-stu-id="70a96-1377">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="70a96-1378">Исправлена проблема со сбоем `storage blob show` при использовании OAuth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="70a96-1378">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-1379">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-1379">VM</span></span>
* <span data-ttu-id="70a96-1380">Добавлена команда `image update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1380">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="70a96-1381">12 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1381">March 12, 2019</span></span>

<span data-ttu-id="70a96-1382">Версия 2.0.60</span><span class="sxs-lookup"><span data-stu-id="70a96-1382">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="70a96-1383">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-1383">Core</span></span>

* <span data-ttu-id="70a96-1384">Исправлена недопустимая ошибка в `cloud set` о том, что подписка не найдена.</span><span class="sxs-lookup"><span data-stu-id="70a96-1384">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-1385">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-1385">ACR</span></span>

* <span data-ttu-id="70a96-1386">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="70a96-1386">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-1387">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-1387">ACS</span></span>

* <span data-ttu-id="70a96-1388">Внесены изменения, в соответствии с которыми параметр `--listen-address` для `aks browse` игнорируется, если он не поддерживается kubectl.</span><span class="sxs-lookup"><span data-stu-id="70a96-1388">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="70a96-1389">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-1389">AppService</span></span>

* <span data-ttu-id="70a96-1390">Добавлено `[webapp|functionapp] deployment list-publishing-credentials` для получения URL-адреса публикации Kudu и связанных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="70a96-1390">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="70a96-1391">Удалена ошибочная инструкция печати для `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1391">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="70a96-1392">Исправлено `functionapp` для настройки правильного образа для среды выполнения в планах службы приложений Linux.</span><span class="sxs-lookup"><span data-stu-id="70a96-1392">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="70a96-1393">Удален тег предварительной версии для `webapp up` и добавлены усовершенствования в команду.</span><span class="sxs-lookup"><span data-stu-id="70a96-1393">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="70a96-1394">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="70a96-1394">Botservice</span></span>

* <span data-ttu-id="70a96-1395">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="70a96-1395">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="70a96-1396">Добавлено `Microsoft-BotFramework-AppId` и `Microsoft-BotFramework-AppPassword` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="70a96-1396">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="70a96-1397">Удалены одинарные кавычки из выходных данных команды `bot publish` в конце `bot create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1397">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="70a96-1398">Изменено `bot publish` для включения поддержки асинхронных операций.</span><span class="sxs-lookup"><span data-stu-id="70a96-1398">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="70a96-1399">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-1399">Container</span></span>

* <span data-ttu-id="70a96-1400">Добавлен аргумент `--no-wait` для команды `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="70a96-1400">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="70a96-1401">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="70a96-1401">EventHub</span></span>

* <span data-ttu-id="70a96-1402">Добавлен флаг `--skip-empty-archives` для `eventhub create|update` для включения поддержки пустых архивов при записи.</span><span class="sxs-lookup"><span data-stu-id="70a96-1402">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="70a96-1403">Поиск</span><span class="sxs-lookup"><span data-stu-id="70a96-1403">Find</span></span>

* <span data-ttu-id="70a96-1404">Основные обновления функций</span><span class="sxs-lookup"><span data-stu-id="70a96-1404">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="70a96-1405">HDInsight</span><span class="sxs-lookup"><span data-stu-id="70a96-1405">HDInsight</span></span>

* <span data-ttu-id="70a96-1406">Добавлен параметр `--storage-account-managed-identity` для `hdinsight create` для включения поддержки MSI ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="70a96-1406">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="70a96-1407">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-1407">Network</span></span>

* <span data-ttu-id="70a96-1408">Исправлена проблема с `vpn-connection update`, когда обновление VPN-подключения между шлюзами в разных подписках завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="70a96-1408">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="70a96-1409">Rdbms</span><span class="sxs-lookup"><span data-stu-id="70a96-1409">Rdbms</span></span>

* <span data-ttu-id="70a96-1410">Незначительные исправления для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="70a96-1410">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="70a96-1411">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-1411">Role</span></span>

* <span data-ttu-id="70a96-1412">Исправлено `role definition update` для использования идентификатора для правильного разрешения определения.</span><span class="sxs-lookup"><span data-stu-id="70a96-1412">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="70a96-1413">Изменено `ad app credential reset` для исключения предположения о том, что субъект-служба приложения всегда существует.</span><span class="sxs-lookup"><span data-stu-id="70a96-1413">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="70a96-1414">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="70a96-1414">Service Fabric</span></span>

* <span data-ttu-id="70a96-1415">Исправлена проблема с `sf cluster list` и невозможностью итерации.</span><span class="sxs-lookup"><span data-stu-id="70a96-1415">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="70a96-1416">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1416">February 26, 2019</span></span>

<span data-ttu-id="70a96-1417">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="70a96-1417">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="70a96-1418">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-1418">Core</span></span>

* <span data-ttu-id="70a96-1419">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="70a96-1419">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-1420">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-1420">ACR</span></span>

* <span data-ttu-id="70a96-1421">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1421">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="70a96-1422">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="70a96-1422">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-1423">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-1423">ACS</span></span>

* <span data-ttu-id="70a96-1424">Добавлен параметр `--listen-address` для команды `aks port-forward`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1424">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-1425">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-1425">AppService</span></span>

* <span data-ttu-id="70a96-1426">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1426">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="70a96-1427">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-1427">Batch</span></span>
* <span data-ttu-id="70a96-1428">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1428">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="70a96-1429">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1429">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="70a96-1430">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="70a96-1430">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="70a96-1431">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1431">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="70a96-1432">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="70a96-1432">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="70a96-1433">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="70a96-1433">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="70a96-1434">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70a96-1434">CosmosDB</span></span>

* <span data-ttu-id="70a96-1435">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="70a96-1435">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="70a96-1436">Kusto</span><span class="sxs-lookup"><span data-stu-id="70a96-1436">Kusto</span></span>

* <span data-ttu-id="70a96-1437">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="70a96-1437">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="70a96-1438">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-1438">Network</span></span>

* <span data-ttu-id="70a96-1439">Добавлен аргумент `--express-route-gateway-bypass` для команды `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="70a96-1439">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="70a96-1440">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1440">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="70a96-1441">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1441">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="70a96-1442">Добавлен аргумент `--legacy-mode` в команду `express-route peering [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1442">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="70a96-1443">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1443">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="70a96-1444">Добавлен аргумент `--gateway-default-site` для команды `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="70a96-1444">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="70a96-1445">Добавлены команды `ipsec-policy` для `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1445">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-1446">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-1446">Resource</span></span>

* <span data-ttu-id="70a96-1447">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="70a96-1447">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="70a96-1448">Добавлена поддержка файла параметров на основе URI для `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1448">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="70a96-1449">Добавлена поддержка определений и параметров на основе URI для `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1449">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="70a96-1450">Исправлена обработка параметров и правил для `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1450">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="70a96-1451">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="70a96-1451">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="70a96-1452">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-1452">Role</span></span>

* <span data-ttu-id="70a96-1453">Добавлена поддержка ролей приложений для `ad app [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1453">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-1454">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-1454">VM</span></span>

* <span data-ttu-id="70a96-1455">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="70a96-1455">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="70a96-1456">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1456">February 12, 2019</span></span>

<span data-ttu-id="70a96-1457">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="70a96-1457">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="70a96-1458">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-1458">Core</span></span>

* <span data-ttu-id="70a96-1459">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="70a96-1459">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="70a96-1460">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="70a96-1460">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-1461">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-1461">ACR</span></span>
* <span data-ttu-id="70a96-1462">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1462">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="70a96-1463">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1463">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-1464">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-1464">ACS</span></span>
* <span data-ttu-id="70a96-1465">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="70a96-1465">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="70a96-1466">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1466">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="70a96-1467">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="70a96-1467">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="70a96-1468">AMS</span><span class="sxs-lookup"><span data-stu-id="70a96-1468">AMS</span></span>
* <span data-ttu-id="70a96-1469">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1469">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="70a96-1470">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1470">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-1471">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-1471">Appservice</span></span>
* <span data-ttu-id="70a96-1472">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="70a96-1472">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="70a96-1473">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="70a96-1473">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="70a96-1474">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1474">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="70a96-1475">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="70a96-1475">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="70a96-1476">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="70a96-1476">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="70a96-1477">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="70a96-1477">Botservice</span></span>
* <span data-ttu-id="70a96-1478">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1478">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="70a96-1479">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1479">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="70a96-1480">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1480">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="70a96-1481">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="70a96-1481">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="70a96-1482">[УСТАРЕЛО] Аргумент `--proj-name` не рекомендуется к использованию. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1482">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="70a96-1483">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="70a96-1483">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="70a96-1484">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="70a96-1484">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="70a96-1485">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="70a96-1485">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="70a96-1486">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="70a96-1486">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="70a96-1487">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="70a96-1487">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="70a96-1488">Key Vault</span><span class="sxs-lookup"><span data-stu-id="70a96-1488">Key Vault</span></span>
* <span data-ttu-id="70a96-1489">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1489">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-1490">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-1490">Monitor</span></span>
* <span data-ttu-id="70a96-1491">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1491">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="70a96-1492">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-1492">Network</span></span>
* <span data-ttu-id="70a96-1493">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="70a96-1493">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="70a96-1494">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="70a96-1494">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="70a96-1495">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="70a96-1495">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="70a96-1496">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1496">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="70a96-1497">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="70a96-1497">Policy Insights</span></span>
* <span data-ttu-id="70a96-1498">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1498">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="70a96-1499">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="70a96-1499">RDBMS</span></span>
* <span data-ttu-id="70a96-1500">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="70a96-1500">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="70a96-1501">Redis</span><span class="sxs-lookup"><span data-stu-id="70a96-1501">Redis</span></span>
* <span data-ttu-id="70a96-1502">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="70a96-1502">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="70a96-1503">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="70a96-1503">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="70a96-1504">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="70a96-1504">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="70a96-1505">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="70a96-1505">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="70a96-1506">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1506">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="70a96-1507">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="70a96-1507">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="70a96-1508">[УСТАРЕЛО] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70a96-1508">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="70a96-1509">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-1509">Role</span></span>
* <span data-ttu-id="70a96-1510">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1510">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="70a96-1511">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-1511">SQL VM</span></span>
* <span data-ttu-id="70a96-1512">[УСТАРЕЛО] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="70a96-1512">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-1513">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-1513">VM</span></span>
* <span data-ttu-id="70a96-1514">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1514">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="70a96-1515">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1515">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="70a96-1516">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="70a96-1516">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="70a96-1517">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1517">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="70a96-1518">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1518">January 31, 2019</span></span>

<span data-ttu-id="70a96-1519">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="70a96-1519">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="70a96-1520">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-1520">Core</span></span>

* <span data-ttu-id="70a96-1521">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="70a96-1521">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="70a96-1522">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1522">January 28, 2019</span></span>

<span data-ttu-id="70a96-1523">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="70a96-1523">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-1524">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-1524">ACR</span></span>
* <span data-ttu-id="70a96-1525">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1525">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-1526">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-1526">ACS</span></span>
* <span data-ttu-id="70a96-1527">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1527">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="70a96-1528">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="70a96-1528">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="70a96-1529">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1529">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="70a96-1530">AMS</span><span class="sxs-lookup"><span data-stu-id="70a96-1530">AMS</span></span>
* <span data-ttu-id="70a96-1531">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1531">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="70a96-1532">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1532">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-1533">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-1533">Appservice</span></span>
* <span data-ttu-id="70a96-1534">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1534">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="70a96-1535">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="70a96-1535">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="70a96-1536">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="70a96-1536">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="70a96-1537">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-1537">Container</span></span>
* <span data-ttu-id="70a96-1538">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1538">Added `container start` command</span></span>
* <span data-ttu-id="70a96-1539">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70a96-1539">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="70a96-1540">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="70a96-1540">EventGrid</span></span>
* <span data-ttu-id="70a96-1541">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1541">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="70a96-1542">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1542">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="70a96-1543">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="70a96-1543">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="70a96-1544">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="70a96-1544">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="70a96-1545">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="70a96-1545">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="70a96-1546">HDInsight</span><span class="sxs-lookup"><span data-stu-id="70a96-1546">HDInsight</span></span>
* <span data-ttu-id="70a96-1547">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1547">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="70a96-1548">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1548">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="70a96-1549">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1549">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="70a96-1550">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="70a96-1550">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="70a96-1551">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1551">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="70a96-1552">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1552">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="70a96-1553">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-1553">IoT</span></span>
* <span data-ttu-id="70a96-1554">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="70a96-1554">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="70a96-1555">Kusto</span><span class="sxs-lookup"><span data-stu-id="70a96-1555">Kusto</span></span>
* <span data-ttu-id="70a96-1556">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="70a96-1556">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-1557">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-1557">Monitor</span></span>
* <span data-ttu-id="70a96-1558">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="70a96-1558">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="70a96-1559">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-1559">Profile</span></span>
* <span data-ttu-id="70a96-1560">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="70a96-1560">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="70a96-1561">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-1561">Network</span></span>
* <span data-ttu-id="70a96-1562">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1562">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="70a96-1563">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="70a96-1563">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-1564">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-1564">Resource</span></span>
* <span data-ttu-id="70a96-1565">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1565">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="70a96-1566">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1566">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="70a96-1567">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-1567">SQL Virtual Machine</span></span>
* <span data-ttu-id="70a96-1568">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="70a96-1568">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-1569">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-1569">Storage</span></span>
* <span data-ttu-id="70a96-1570">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="70a96-1570">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="70a96-1571">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="70a96-1571">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-1572">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-1572">VM</span></span>
* <span data-ttu-id="70a96-1573">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="70a96-1573">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="70a96-1574">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1574">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="70a96-1575">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1575">January 15, 2019</span></span>

<span data-ttu-id="70a96-1576">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="70a96-1576">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-1577">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-1577">ACR</span></span>
* <span data-ttu-id="70a96-1578">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="70a96-1578">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="70a96-1579">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="70a96-1579">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="70a96-1580">[УСТАРЕЛО] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="70a96-1580">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="70a96-1581">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-1581">ACS</span></span>
* <span data-ttu-id="70a96-1582">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="70a96-1582">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-1583">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-1583">Appservice</span></span>
* <span data-ttu-id="70a96-1584">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="70a96-1584">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="70a96-1585">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="70a96-1585">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="70a96-1586">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="70a96-1586">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="70a96-1587">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1587">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="70a96-1588">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="70a96-1588">Botservice</span></span>
* <span data-ttu-id="70a96-1589">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1589">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="70a96-1590">Configure</span><span class="sxs-lookup"><span data-stu-id="70a96-1590">Configure</span></span>
* <span data-ttu-id="70a96-1591">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1591">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="70a96-1592">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70a96-1592">CosmosDB</span></span>
* <span data-ttu-id="70a96-1593">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="70a96-1593">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="70a96-1594">HDInsight</span><span class="sxs-lookup"><span data-stu-id="70a96-1594">HDInsight</span></span>
* <span data-ttu-id="70a96-1595">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="70a96-1595">Added commands for managing applications</span></span>
* <span data-ttu-id="70a96-1596">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1596">Added commands for managing script actions</span></span>
* <span data-ttu-id="70a96-1597">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="70a96-1597">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="70a96-1598">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1598">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="70a96-1599">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-1599">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="70a96-1600">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-1600">Network</span></span>
* <span data-ttu-id="70a96-1601">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="70a96-1601">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="70a96-1602">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="70a96-1602">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="70a96-1603">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="70a96-1603">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="70a96-1604">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1604">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="70a96-1605">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-1605">Role</span></span>
* <span data-ttu-id="70a96-1606">[УСТАРЕЛО] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70a96-1606">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="70a96-1607">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="70a96-1607">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="70a96-1608">Безопасность</span><span class="sxs-lookup"><span data-stu-id="70a96-1608">Security</span></span>
* <span data-ttu-id="70a96-1609">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="70a96-1609">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-1610">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-1610">Storage</span></span>
* <span data-ttu-id="70a96-1611">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="70a96-1611">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="70a96-1612">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1612">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="70a96-1613">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1613">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="70a96-1614">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1614">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="70a96-1615">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1615">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-1616">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-1616">VM</span></span>
* <span data-ttu-id="70a96-1617">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="70a96-1617">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="70a96-1618">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1618">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="70a96-1619">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1619">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="70a96-1620">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="70a96-1620">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="70a96-1621">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-1621">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="70a96-1622">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="70a96-1622">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="70a96-1623">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1623">December 20, 2018</span></span>

<span data-ttu-id="70a96-1624">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="70a96-1624">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="70a96-1625">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-1625">Appservice</span></span>
* <span data-ttu-id="70a96-1626">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="70a96-1626">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="70a96-1627">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="70a96-1627">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="70a96-1628">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="70a96-1628">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="70a96-1629">IoT Central</span><span class="sxs-lookup"><span data-stu-id="70a96-1629">IoTCentral</span></span>
* <span data-ttu-id="70a96-1630">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="70a96-1630">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="70a96-1631">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-1631">Role</span></span>
* <span data-ttu-id="70a96-1632">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1632">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-1633">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-1633">SQL</span></span>
* <span data-ttu-id="70a96-1634">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="70a96-1634">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-1635">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-1635">VM</span></span>
* <span data-ttu-id="70a96-1636">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1636">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="70a96-1637">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1637">December 18, 2018</span></span>

<span data-ttu-id="70a96-1638">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="70a96-1638">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="70a96-1639">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-1639">ACR</span></span>
* <span data-ttu-id="70a96-1640">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70a96-1640">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="70a96-1641">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="70a96-1641">Condensed the table layout for task list</span></span>
* <span data-ttu-id="70a96-1642">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="70a96-1642">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-1643">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-1643">ACS</span></span>
* <span data-ttu-id="70a96-1644">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1644">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="70a96-1645">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="70a96-1645">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="70a96-1646">[УСТАРЕЛО] Команды `az acs` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="70a96-1646">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="70a96-1647">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1647">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="70a96-1648">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="70a96-1648">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="70a96-1649">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1649">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-1650">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-1650">Appservice</span></span>
* <span data-ttu-id="70a96-1651">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1651">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="70a96-1652">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="70a96-1652">Botservice</span></span>
* <span data-ttu-id="70a96-1653">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1653">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="70a96-1654">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="70a96-1654">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="70a96-1655">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="70a96-1655">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="70a96-1656">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="70a96-1656">Reduced Kudu network calls</span></span>
* <span data-ttu-id="70a96-1657">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="70a96-1657">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="70a96-1658">Потребление</span><span class="sxs-lookup"><span data-stu-id="70a96-1658">Consumption</span></span>
* <span data-ttu-id="70a96-1659">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="70a96-1659">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="70a96-1660">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70a96-1660">CosmosDB</span></span>
* <span data-ttu-id="70a96-1661">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="70a96-1661">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="70a96-1662">Maps</span><span class="sxs-lookup"><span data-stu-id="70a96-1662">Maps</span></span>
* <span data-ttu-id="70a96-1663">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="70a96-1663">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="70a96-1664">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-1664">Network</span></span>
* <span data-ttu-id="70a96-1665">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1665">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="70a96-1666">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="70a96-1666">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-1667">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-1667">Resource</span></span>
* <span data-ttu-id="70a96-1668">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1668">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="70a96-1669">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1669">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-1670">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-1670">Storage</span></span>
*  <span data-ttu-id="70a96-1671">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="70a96-1671">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-1672">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-1672">VM</span></span>
* <span data-ttu-id="70a96-1673">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="70a96-1673">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="70a96-1674">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1674">December 4, 2018</span></span>

<span data-ttu-id="70a96-1675">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="70a96-1675">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="70a96-1676">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-1676">Core</span></span>
* <span data-ttu-id="70a96-1677">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="70a96-1677">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="70a96-1678">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="70a96-1678">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-1679">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-1679">Appservice</span></span>
* <span data-ttu-id="70a96-1680">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="70a96-1680">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="70a96-1681">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="70a96-1681">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="70a96-1682">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-1682">Network</span></span>
* <span data-ttu-id="70a96-1683">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="70a96-1683">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="70a96-1684">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-1684">Role</span></span>
* <span data-ttu-id="70a96-1685">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="70a96-1685">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="70a96-1686">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-1686">VM</span></span>
* <span data-ttu-id="70a96-1687">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70a96-1687">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="70a96-1688">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="70a96-1688">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="70a96-1689">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="70a96-1689">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="70a96-1690">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="70a96-1690">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="70a96-1691">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1691">November 20, 2018</span></span>

<span data-ttu-id="70a96-1692">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="70a96-1692">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="70a96-1693">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-1693">Core</span></span>
* <span data-ttu-id="70a96-1694">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="70a96-1694">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-1695">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-1695">ACR</span></span>
* <span data-ttu-id="70a96-1696">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="70a96-1696">Added context token to task step</span></span>
* <span data-ttu-id="70a96-1697">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="70a96-1697">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="70a96-1698">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1698">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-1699">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-1699">Appservice</span></span>
* <span data-ttu-id="70a96-1700">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="70a96-1700">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="70a96-1701">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-1701">Updated the default `node_version`.</span></span> <span data-ttu-id="70a96-1702">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="70a96-1702">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="70a96-1703">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="70a96-1703">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="70a96-1704">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="70a96-1704">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="70a96-1705">IotCentral</span><span class="sxs-lookup"><span data-stu-id="70a96-1705">IotCentral</span></span>
* <span data-ttu-id="70a96-1706">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="70a96-1706">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="70a96-1707">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70a96-1707">KeyVault</span></span>
* <span data-ttu-id="70a96-1708">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="70a96-1708">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="70a96-1709">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-1709">Network</span></span>
* <span data-ttu-id="70a96-1710">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1710">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="70a96-1711">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1711">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="70a96-1712">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="70a96-1712">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="70a96-1713">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1713">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="70a96-1714">Rdbms</span><span class="sxs-lookup"><span data-stu-id="70a96-1714">Rdbms</span></span>
* <span data-ttu-id="70a96-1715">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="70a96-1715">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="70a96-1716">RBAC:</span><span class="sxs-lookup"><span data-stu-id="70a96-1716">Rbac</span></span>
* <span data-ttu-id="70a96-1717">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1717">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="70a96-1718">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="70a96-1718">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="70a96-1719">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-1719">Storage</span></span>
* <span data-ttu-id="70a96-1720">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="70a96-1720">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="70a96-1721">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1721">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="70a96-1722">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="70a96-1722">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="70a96-1723">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1723">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-1724">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-1724">VM</span></span>
* <span data-ttu-id="70a96-1725">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="70a96-1725">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="70a96-1726">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1726">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="70a96-1727">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1727">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="70a96-1728">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="70a96-1728">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="70a96-1729">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1729">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="70a96-1730">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1730">Added `snapshot wait` command</span></span>
* <span data-ttu-id="70a96-1731">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1731">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="70a96-1732">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1732">November 6, 2018</span></span>

<span data-ttu-id="70a96-1733">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="70a96-1733">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="70a96-1734">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-1734">Core</span></span>
* <span data-ttu-id="70a96-1735">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="70a96-1735">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-1736">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-1736">ACR</span></span>
* <span data-ttu-id="70a96-1737">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="70a96-1737">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="70a96-1738">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="70a96-1738">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-1739">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-1739">ACS</span></span>
* <span data-ttu-id="70a96-1740">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-1740">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="70a96-1741">Помощник</span><span class="sxs-lookup"><span data-stu-id="70a96-1741">Advisor</span></span>
* <span data-ttu-id="70a96-1742">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="70a96-1742">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="70a96-1743">AMS</span><span class="sxs-lookup"><span data-stu-id="70a96-1743">AMS</span></span>
* <span data-ttu-id="70a96-1744">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="70a96-1744">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="70a96-1745">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="70a96-1745">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="70a96-1746">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1746">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="70a96-1747">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="70a96-1747">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="70a96-1748">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1748">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="70a96-1749">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1749">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="70a96-1750">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1750">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="70a96-1751">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1751">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="70a96-1752">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1752">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="70a96-1753">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1753">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="70a96-1754">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1754">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="70a96-1755">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1755">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="70a96-1756">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="70a96-1756">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="70a96-1757">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="70a96-1757">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="70a96-1758">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1758">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="70a96-1759">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="70a96-1759">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="70a96-1760">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="70a96-1760">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-1761">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-1761">AppService</span></span>
* <span data-ttu-id="70a96-1762">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="70a96-1762">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="70a96-1763">Configure</span><span class="sxs-lookup"><span data-stu-id="70a96-1763">Configure</span></span>
* <span data-ttu-id="70a96-1764">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="70a96-1764">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="70a96-1765">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-1765">Container</span></span>
* <span data-ttu-id="70a96-1766">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="70a96-1766">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="70a96-1767">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="70a96-1767">EventHub</span></span>
* <span data-ttu-id="70a96-1768">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1768">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="70a96-1769">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="70a96-1769">Interactive</span></span>
* <span data-ttu-id="70a96-1770">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="70a96-1770">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-1771">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-1771">Monitor</span></span>
* <span data-ttu-id="70a96-1772">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1772">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="70a96-1773">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-1773">Network</span></span>
* <span data-ttu-id="70a96-1774">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1774">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="70a96-1775">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="70a96-1775">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="70a96-1776">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1776">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="70a96-1777">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-1777">Profile</span></span>
* <span data-ttu-id="70a96-1778">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1778">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="70a96-1779">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="70a96-1779">RDBMS</span></span>
* <span data-ttu-id="70a96-1780">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="70a96-1780">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-1781">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-1781">Resource</span></span>
* <span data-ttu-id="70a96-1782">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1782">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="70a96-1783">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-1783">Role</span></span>
* <span data-ttu-id="70a96-1784">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="70a96-1784">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="70a96-1785">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="70a96-1785">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="70a96-1786">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="70a96-1786">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-1787">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-1787">Storage</span></span>
* <span data-ttu-id="70a96-1788">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1788">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-1789">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-1789">VM</span></span>
* <span data-ttu-id="70a96-1790">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="70a96-1790">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="70a96-1791">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="70a96-1791">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="70a96-1792">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="70a96-1792">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="70a96-1793">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="70a96-1793">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="70a96-1794">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="70a96-1794">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="70a96-1795">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1795">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="70a96-1796">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1796">October 23, 2018</span></span>

<span data-ttu-id="70a96-1797">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="70a96-1797">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="70a96-1798">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-1798">Core</span></span>
* <span data-ttu-id="70a96-1799">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1799">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="70a96-1800">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1800">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-1801">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-1801">ACR</span></span>
* <span data-ttu-id="70a96-1802">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="70a96-1802">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="70a96-1803">CDN</span><span class="sxs-lookup"><span data-stu-id="70a96-1803">CDN</span></span>
* <span data-ttu-id="70a96-1804">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-1804">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="70a96-1805">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="70a96-1805">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="70a96-1806">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-1806">Container</span></span>
* <span data-ttu-id="70a96-1807">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="70a96-1807">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="70a96-1808">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="70a96-1808">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="70a96-1809">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1809">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="70a96-1810">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70a96-1810">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="70a96-1811">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="70a96-1811">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="70a96-1812">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="70a96-1812">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="70a96-1813">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1813">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="70a96-1814">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70a96-1814">CosmosDB</span></span>
* <span data-ttu-id="70a96-1815">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1815">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="70a96-1816">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="70a96-1816">Interactive</span></span>
* <span data-ttu-id="70a96-1817">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="70a96-1817">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="70a96-1818">IoT Central</span><span class="sxs-lookup"><span data-stu-id="70a96-1818">IoT Central</span></span>
* <span data-ttu-id="70a96-1819">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="70a96-1819">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="70a96-1820">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="70a96-1820">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-1821">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-1821">Monitor</span></span>
* <span data-ttu-id="70a96-1822">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="70a96-1822">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="70a96-1823">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="70a96-1823">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="70a96-1824">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="70a96-1824">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="70a96-1825">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="70a96-1825">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="70a96-1826">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1826">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="70a96-1827">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="70a96-1827">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="70a96-1828">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="70a96-1828">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="70a96-1829">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="70a96-1829">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="70a96-1830">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="70a96-1830">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="70a96-1831">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1831">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="70a96-1832">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-1832">Network</span></span>
* <span data-ttu-id="70a96-1833">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="70a96-1833">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="70a96-1834">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="70a96-1834">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="70a96-1835">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="70a96-1835">ServiceBus</span></span>
* <span data-ttu-id="70a96-1836">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="70a96-1836">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-1837">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-1837">SQL</span></span>
* <span data-ttu-id="70a96-1838">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="70a96-1838">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-1839">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-1839">Storage</span></span>
* <span data-ttu-id="70a96-1840">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="70a96-1840">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="70a96-1841">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="70a96-1841">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-1842">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-1842">VM</span></span>
* <span data-ttu-id="70a96-1843">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="70a96-1843">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="70a96-1844">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="70a96-1844">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="70a96-1845">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="70a96-1845">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="70a96-1846">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1846">October 16, 2018</span></span>

<span data-ttu-id="70a96-1847">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="70a96-1847">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-1848">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-1848">VM</span></span>
* <span data-ttu-id="70a96-1849">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="70a96-1849">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="70a96-1850">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1850">October 9, 2018</span></span>

<span data-ttu-id="70a96-1851">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="70a96-1851">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="70a96-1852">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-1852">Core</span></span>
* <span data-ttu-id="70a96-1853">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="70a96-1853">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-1854">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-1854">ACR</span></span>
* <span data-ttu-id="70a96-1855">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="70a96-1855">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-1856">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-1856">ACS</span></span>
* <span data-ttu-id="70a96-1857">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="70a96-1857">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="70a96-1858">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="70a96-1858">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="70a96-1859">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1859">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="70a96-1860">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="70a96-1860">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="70a96-1861">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-1861">Container</span></span>
* <span data-ttu-id="70a96-1862">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="70a96-1862">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="70a96-1863">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="70a96-1863">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="70a96-1864">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="70a96-1864">Event Hub</span></span>
* <span data-ttu-id="70a96-1865">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1865">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="70a96-1866">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="70a96-1866">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="70a96-1867">Модули</span><span class="sxs-lookup"><span data-stu-id="70a96-1867">Extensions</span></span>
* <span data-ttu-id="70a96-1868">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="70a96-1868">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="70a96-1869">HDInsight</span><span class="sxs-lookup"><span data-stu-id="70a96-1869">HDInsight</span></span>
* <span data-ttu-id="70a96-1870">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="70a96-1870">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="70a96-1871">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-1871">IoT</span></span>
* <span data-ttu-id="70a96-1872">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="70a96-1872">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="70a96-1873">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70a96-1873">KeyVault</span></span>
* <span data-ttu-id="70a96-1874">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="70a96-1874">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="70a96-1875">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-1875">Network</span></span>
* <span data-ttu-id="70a96-1876">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-1876">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="70a96-1877">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="70a96-1877">See #6052</span></span>
* <span data-ttu-id="70a96-1878">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1878">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="70a96-1879">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="70a96-1879">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="70a96-1880">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1880">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="70a96-1881">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1881">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="70a96-1882">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1882">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="70a96-1883">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1883">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="70a96-1884">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-1884">Role</span></span>
* <span data-ttu-id="70a96-1885">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1885">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="70a96-1886">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1886">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="70a96-1887">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="70a96-1887">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="70a96-1888">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="70a96-1888">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="70a96-1889">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="70a96-1889">Service Bus</span></span>
* <span data-ttu-id="70a96-1890">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="70a96-1890">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-1891">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-1891">VM</span></span>
* <span data-ttu-id="70a96-1892">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1892">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="70a96-1893">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="70a96-1893">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="70a96-1894">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1894">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="70a96-1895">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1895">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="70a96-1896">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="70a96-1896">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="70a96-1897">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="70a96-1897">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="70a96-1898">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1898">September 21, 2018</span></span>

<span data-ttu-id="70a96-1899">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="70a96-1899">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-1900">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-1900">ACR</span></span>
* <span data-ttu-id="70a96-1901">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="70a96-1901">Added ACR Task commands</span></span>
* <span data-ttu-id="70a96-1902">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="70a96-1902">Added quick run command</span></span>
* <span data-ttu-id="70a96-1903">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="70a96-1903">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="70a96-1904">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="70a96-1904">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="70a96-1905">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="70a96-1905">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="70a96-1906">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="70a96-1906">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-1907">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-1907">ACS</span></span>
* <span data-ttu-id="70a96-1908">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="70a96-1908">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="70a96-1909">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="70a96-1909">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-1910">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-1910">AppService</span></span>

* <span data-ttu-id="70a96-1911">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="70a96-1911">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="70a96-1912">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="70a96-1912">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="70a96-1913">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="70a96-1913">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="70a96-1914">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="70a96-1914">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="70a96-1915">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-1915">Batch</span></span>
* <span data-ttu-id="70a96-1916">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="70a96-1916">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="70a96-1917">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1917">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="70a96-1918">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1918">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="70a96-1919">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="70a96-1919">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="70a96-1920">Batch AI</span><span class="sxs-lookup"><span data-stu-id="70a96-1920">Batch AI</span></span> 
* <span data-ttu-id="70a96-1921">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1921">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="70a96-1922">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="70a96-1922">Cognitive Services</span></span>
* <span data-ttu-id="70a96-1923">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1923">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="70a96-1924">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1924">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="70a96-1925">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1925">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="70a96-1926">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1926">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="70a96-1927">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="70a96-1927">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="70a96-1928">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1928">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="70a96-1929">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-1929">Container</span></span>
* <span data-ttu-id="70a96-1930">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70a96-1930">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="70a96-1931">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="70a96-1931">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="70a96-1932">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="70a96-1932">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="70a96-1933">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70a96-1933">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="70a96-1934">Data Lake</span><span class="sxs-lookup"><span data-stu-id="70a96-1934">Datalake</span></span>
* <span data-ttu-id="70a96-1935">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="70a96-1935">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="70a96-1936">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="70a96-1936">Interactive Shell</span></span>
* <span data-ttu-id="70a96-1937">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="70a96-1937">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="70a96-1938">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1938">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="70a96-1939">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-1939">IoT</span></span>
* <span data-ttu-id="70a96-1940">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="70a96-1940">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="70a96-1941">Key Vault</span><span class="sxs-lookup"><span data-stu-id="70a96-1941">Key Vault</span></span>
* <span data-ttu-id="70a96-1942">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="70a96-1942">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="70a96-1943">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-1943">Network</span></span>
* <span data-ttu-id="70a96-1944">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1944">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="70a96-1945">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="70a96-1945">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="70a96-1946">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="70a96-1946">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="70a96-1947">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1947">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="70a96-1948">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1948">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="70a96-1949">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1949">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="70a96-1950">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="70a96-1950">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="70a96-1951">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1951">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="70a96-1952">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1952">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="70a96-1953">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1953">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="70a96-1954">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1954">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="70a96-1955">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1955">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="70a96-1956">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1956">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="70a96-1957">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="70a96-1957">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="70a96-1958">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1958">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="70a96-1959">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="70a96-1959">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="70a96-1960">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="70a96-1960">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="70a96-1961">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="70a96-1961">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="70a96-1962">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="70a96-1962">RDBMS</span></span>
* <span data-ttu-id="70a96-1963">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="70a96-1963">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="70a96-1964">резервирование.</span><span class="sxs-lookup"><span data-stu-id="70a96-1964">Reservation</span></span>
* <span data-ttu-id="70a96-1965">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70a96-1965">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="70a96-1966">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="70a96-1966">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="70a96-1967">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="70a96-1967">Manage App</span></span>
* <span data-ttu-id="70a96-1968">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="70a96-1968">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="70a96-1969">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="70a96-1969">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="70a96-1970">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-1970">Role</span></span>
* <span data-ttu-id="70a96-1971">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="70a96-1971">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="70a96-1972">SignalR</span><span class="sxs-lookup"><span data-stu-id="70a96-1972">SignalR</span></span>
* <span data-ttu-id="70a96-1973">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="70a96-1973">First release</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-1974">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-1974">Storage</span></span>
* <span data-ttu-id="70a96-1975">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="70a96-1975">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="70a96-1976">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="70a96-1976">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-1977">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-1977">VM</span></span>
* <span data-ttu-id="70a96-1978">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="70a96-1978">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="70a96-1979">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1979">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="70a96-1980">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-1980">August 28, 2018</span></span>

<span data-ttu-id="70a96-1981">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="70a96-1981">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="70a96-1982">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-1982">Core</span></span>

* <span data-ttu-id="70a96-1983">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="70a96-1983">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="70a96-1984">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="70a96-1984">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-1985">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-1985">ACR</span></span>

* <span data-ttu-id="70a96-1986">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="70a96-1986">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="70a96-1987">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1987">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-1988">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-1988">ACS</span></span>

* <span data-ttu-id="70a96-1989">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="70a96-1989">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="70a96-1990">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="70a96-1990">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-1991">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-1991">AppService</span></span>

* <span data-ttu-id="70a96-1992">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="70a96-1992">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="70a96-1993">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="70a96-1993">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="70a96-1994">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="70a96-1994">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="70a96-1995">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="70a96-1995">Backup</span></span>

* <span data-ttu-id="70a96-1996">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="70a96-1996">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="70a96-1997">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="70a96-1997">Bot Service</span></span>

* <span data-ttu-id="70a96-1998">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="70a96-1998">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="70a96-1999">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="70a96-1999">Cognitive Services</span></span>

* <span data-ttu-id="70a96-2000">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="70a96-2000">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="70a96-2001">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-2001">IoT</span></span>

* <span data-ttu-id="70a96-2002">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="70a96-2002">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-2003">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-2003">Monitor</span></span>

* <span data-ttu-id="70a96-2004">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="70a96-2004">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="70a96-2005">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="70a96-2005">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="70a96-2006">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-2006">Network</span></span>

* <span data-ttu-id="70a96-2007">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="70a96-2007">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-2008">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-2008">Resource</span></span>

* <span data-ttu-id="70a96-2009">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="70a96-2009">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-2010">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-2010">Storage</span></span>

* <span data-ttu-id="70a96-2011">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="70a96-2011">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2012">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2012">VM</span></span>

* <span data-ttu-id="70a96-2013">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="70a96-2013">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="70a96-2014">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2014">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="70a96-2015">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2015">Auguest 14, 2018</span></span>

<span data-ttu-id="70a96-2016">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="70a96-2016">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="70a96-2017">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-2017">Core</span></span>

* <span data-ttu-id="70a96-2018">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2018">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="70a96-2019">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="70a96-2019">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="70a96-2020">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="70a96-2020">Telemetry</span></span>

* <span data-ttu-id="70a96-2021">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="70a96-2021">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-2022">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-2022">ACR</span></span>

* <span data-ttu-id="70a96-2023">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2023">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="70a96-2024">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2024">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-2025">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-2025">ACS</span></span>

* <span data-ttu-id="70a96-2026">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="70a96-2026">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="70a96-2027">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="70a96-2027">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="70a96-2028">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="70a96-2028">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="70a96-2029">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="70a96-2029">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="70a96-2030">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="70a96-2030">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="70a96-2031">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-2031">AppService</span></span>

* <span data-ttu-id="70a96-2032">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2032">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="70a96-2033">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="70a96-2033">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="70a96-2034">Batch AI</span><span class="sxs-lookup"><span data-stu-id="70a96-2034">BatchAI</span></span>

* <span data-ttu-id="70a96-2035">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="70a96-2035">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="70a96-2036">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-2036">Container</span></span>

* <span data-ttu-id="70a96-2037">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="70a96-2037">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="70a96-2038">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-2038">IoT</span></span>

* <span data-ttu-id="70a96-2039">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="70a96-2039">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="70a96-2040">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2040">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="70a96-2041">IoT Central</span><span class="sxs-lookup"><span data-stu-id="70a96-2041">Iot Central</span></span>

* <span data-ttu-id="70a96-2042">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="70a96-2042">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="70a96-2043">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70a96-2043">KeyVault</span></span>


* <span data-ttu-id="70a96-2044">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="70a96-2044">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="70a96-2045">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="70a96-2045">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="70a96-2046">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="70a96-2046">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="70a96-2047">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="70a96-2047">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="70a96-2048">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="70a96-2048">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="70a96-2049">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="70a96-2049">Relay</span></span>

* <span data-ttu-id="70a96-2050">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="70a96-2050">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-2051">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-2051">Sql</span></span>

* <span data-ttu-id="70a96-2052">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2052">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-2053">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-2053">Storage</span></span>

* <span data-ttu-id="70a96-2054">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="70a96-2054">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="70a96-2055">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="70a96-2055">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="70a96-2056">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="70a96-2056">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="70a96-2057">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="70a96-2057">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="70a96-2058">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="70a96-2058">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2059">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2059">VM</span></span>

* <span data-ttu-id="70a96-2060">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="70a96-2060">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="70a96-2061">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2061">July 31, 2018</span></span>

<span data-ttu-id="70a96-2062">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="70a96-2062">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-2063">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-2063">ACR</span></span>

* <span data-ttu-id="70a96-2064">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2064">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="70a96-2065">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2065">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-2066">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-2066">ACS</span></span>

* <span data-ttu-id="70a96-2067">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="70a96-2067">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="70a96-2068">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-2068">Batch</span></span>

* <span data-ttu-id="70a96-2069">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="70a96-2069">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="70a96-2070">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-2070">Container</span></span>

* <span data-ttu-id="70a96-2071">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="70a96-2071">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="70a96-2072">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-2072">Network</span></span>

* <span data-ttu-id="70a96-2073">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="70a96-2073">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="70a96-2074">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-2074">Resource</span></span>

* <span data-ttu-id="70a96-2075">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="70a96-2075">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="70a96-2076">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="70a96-2076">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="70a96-2077">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-2077">Role</span></span>

* <span data-ttu-id="70a96-2078">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="70a96-2078">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="70a96-2079">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="70a96-2079">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="70a96-2080">Поиск</span><span class="sxs-lookup"><span data-stu-id="70a96-2080">Search</span></span>

* <span data-ttu-id="70a96-2081">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="70a96-2081">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="70a96-2082">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="70a96-2082">Service Bus</span></span>

* <span data-ttu-id="70a96-2083">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="70a96-2083">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="70a96-2084">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="70a96-2084">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="70a96-2085">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="70a96-2085">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="70a96-2086">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2086">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-2087">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-2087">Storage</span></span>

* <span data-ttu-id="70a96-2088">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="70a96-2088">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="70a96-2089">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="70a96-2089">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2090">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2090">VM</span></span>

* <span data-ttu-id="70a96-2091">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="70a96-2091">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="70a96-2092">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2092">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="70a96-2093">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="70a96-2093">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="70a96-2094">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="70a96-2094">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="70a96-2095">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2095">July 18, 2018</span></span>

<span data-ttu-id="70a96-2096">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="70a96-2096">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="70a96-2097">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-2097">Core</span></span>

* <span data-ttu-id="70a96-2098">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="70a96-2098">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="70a96-2099">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="70a96-2099">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="70a96-2100">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="70a96-2100">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-2101">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-2101">ACR</span></span>

* <span data-ttu-id="70a96-2102">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="70a96-2102">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="70a96-2103">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2103">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="70a96-2104">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="70a96-2104">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="70a96-2105">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="70a96-2105">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-2106">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-2106">ACS</span></span>

* <span data-ttu-id="70a96-2107">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="70a96-2107">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-2108">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-2108">AppService</span></span>

* <span data-ttu-id="70a96-2109">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="70a96-2109">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="70a96-2110">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-2110">Batch</span></span>

* <span data-ttu-id="70a96-2111">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="70a96-2111">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="70a96-2112">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="70a96-2112">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="70a96-2113">Batch AI</span><span class="sxs-lookup"><span data-stu-id="70a96-2113">Batch AI</span></span>

* <span data-ttu-id="70a96-2114">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2114">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="70a96-2115">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-2115">Container</span></span>

* <span data-ttu-id="70a96-2116">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="70a96-2116">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="70a96-2117">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="70a96-2117">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="70a96-2118">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-2118">Network</span></span>

* <span data-ttu-id="70a96-2119">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2119">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="70a96-2120">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2120">Added `network nic wait`</span></span>
* <span data-ttu-id="70a96-2121">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="70a96-2121">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="70a96-2122">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="70a96-2122">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="70a96-2123">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-2123">Resource</span></span>

* <span data-ttu-id="70a96-2124">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2124">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="70a96-2125">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2125">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="70a96-2126">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2126">Added `deployment wait` command</span></span>
* <span data-ttu-id="70a96-2127">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="70a96-2127">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-2128">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-2128">SQL</span></span>

* <span data-ttu-id="70a96-2129">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2129">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="70a96-2130">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2130">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="70a96-2131">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2131">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-2132">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-2132">Storage</span></span>

* <span data-ttu-id="70a96-2133">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2133">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2134">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2134">VM</span></span>

* <span data-ttu-id="70a96-2135">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-2135">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="70a96-2136">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2136">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="70a96-2137">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2137">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="70a96-2138">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2138">July 3, 2018</span></span>

<span data-ttu-id="70a96-2139">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="70a96-2139">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="70a96-2140">AKS</span><span class="sxs-lookup"><span data-stu-id="70a96-2140">AKS</span></span>

* <span data-ttu-id="70a96-2141">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="70a96-2141">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="70a96-2142">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2142">July 3, 2018</span></span>

<span data-ttu-id="70a96-2143">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="70a96-2143">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="70a96-2144">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-2144">Core</span></span>

* <span data-ttu-id="70a96-2145">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="70a96-2145">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-2146">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-2146">ACR</span></span>

* <span data-ttu-id="70a96-2147">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="70a96-2147">Added polling build status</span></span>
* <span data-ttu-id="70a96-2148">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="70a96-2148">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="70a96-2149">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2149">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-2150">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-2150">ACS</span></span>

* <span data-ttu-id="70a96-2151">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-2151">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="70a96-2152">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-2152">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="70a96-2153">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2153">Updated options for `aks browse` command.</span></span> <span data-ttu-id="70a96-2154">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2154">Added `--listen-port` support</span></span>
* <span data-ttu-id="70a96-2155">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2155">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="70a96-2156">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="70a96-2156">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="70a96-2157">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2157">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-2158">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-2158">AppService</span></span>

* <span data-ttu-id="70a96-2159">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2159">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="70a96-2160">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="70a96-2160">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="70a96-2161">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="70a96-2161">Backup</span></span>

* <span data-ttu-id="70a96-2162">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="70a96-2162">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="70a96-2163">Batch AI</span><span class="sxs-lookup"><span data-stu-id="70a96-2163">BatchAI</span></span>

* <span data-ttu-id="70a96-2164">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2164">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="70a96-2165">Cloud</span><span class="sxs-lookup"><span data-stu-id="70a96-2165">Cloud</span></span>

* <span data-ttu-id="70a96-2166">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2166">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="70a96-2167">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-2167">Container</span></span>

* <span data-ttu-id="70a96-2168">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="70a96-2168">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="70a96-2169">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2169">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="70a96-2170">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="70a96-2170">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="70a96-2171">Расширение</span><span class="sxs-lookup"><span data-stu-id="70a96-2171">Extension</span></span>

* <span data-ttu-id="70a96-2172">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="70a96-2172">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="70a96-2173">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-2173">Network</span></span>

* <span data-ttu-id="70a96-2174">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="70a96-2174">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="70a96-2175">Rdbms</span><span class="sxs-lookup"><span data-stu-id="70a96-2175">Rdbms</span></span>

* <span data-ttu-id="70a96-2176">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2176">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-2177">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-2177">Resource</span></span>

* <span data-ttu-id="70a96-2178">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2178">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2179">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2179">VM</span></span>

* <span data-ttu-id="70a96-2180">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="70a96-2180">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="70a96-2181">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2181">June 25, 2018</span></span>

<span data-ttu-id="70a96-2182">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="70a96-2182">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="70a96-2183">CLI</span><span class="sxs-lookup"><span data-stu-id="70a96-2183">CLI</span></span>

* <span data-ttu-id="70a96-2184">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="70a96-2184">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="70a96-2185">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2185">June 19, 2018</span></span>

<span data-ttu-id="70a96-2186">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="70a96-2186">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="70a96-2187">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-2187">Core</span></span>

* <span data-ttu-id="70a96-2188">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="70a96-2188">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-2189">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-2189">ACR</span></span>

* <span data-ttu-id="70a96-2190">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2190">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="70a96-2191">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="70a96-2191">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-2192">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-2192">ACS</span></span>

* <span data-ttu-id="70a96-2193">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2193">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="70a96-2194">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2194">Added `--update` support</span></span>
* <span data-ttu-id="70a96-2195">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2195">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="70a96-2196">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2196">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="70a96-2197">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2197">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="70a96-2198">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2198">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="70a96-2199">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2199">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="70a96-2200">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2200">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-2201">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-2201">AppService</span></span>

* <span data-ttu-id="70a96-2202">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="70a96-2202">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="70a96-2203">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2203">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="70a96-2204">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-2204">Batch</span></span>

* <span data-ttu-id="70a96-2205">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2205">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="70a96-2206">Batch AI</span><span class="sxs-lookup"><span data-stu-id="70a96-2206">Batch AI</span></span>

* <span data-ttu-id="70a96-2207">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="70a96-2207">Added support for workspaces.</span></span> <span data-ttu-id="70a96-2208">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2208">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="70a96-2209">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2209">Added support for experiments.</span></span> <span data-ttu-id="70a96-2210">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="70a96-2210">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="70a96-2211">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="70a96-2211">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="70a96-2212">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2212">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="70a96-2213">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2213">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="70a96-2214">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2214">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="70a96-2215">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="70a96-2215">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="70a96-2216">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2216">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="70a96-2217">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2217">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="70a96-2218">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2218">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="70a96-2219">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2219">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="70a96-2220">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2220">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="70a96-2221">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2221">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="70a96-2222">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="70a96-2222">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="70a96-2223">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2223">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="70a96-2224">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="70a96-2224">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="70a96-2225">[`--config`, `-c`] переименовано в [`--config-file`, `-f`].</span><span class="sxs-lookup"><span data-stu-id="70a96-2225">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="70a96-2226">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="70a96-2226">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="70a96-2227">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="70a96-2227">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="70a96-2228">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="70a96-2228">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="70a96-2229">Maps</span><span class="sxs-lookup"><span data-stu-id="70a96-2229">Maps</span></span>

* <span data-ttu-id="70a96-2230">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2230">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="70a96-2231">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-2231">Network</span></span>

* <span data-ttu-id="70a96-2232">Добавлена поддержка `https` в `network lb probe create` ([№ 6571](https://github.com/Azure/azure-cli/issues/6571)).</span><span class="sxs-lookup"><span data-stu-id="70a96-2232">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="70a96-2233">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="70a96-2233">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="70a96-2234">#6502</span><span class="sxs-lookup"><span data-stu-id="70a96-2234">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="70a96-2235">Резервирование</span><span class="sxs-lookup"><span data-stu-id="70a96-2235">Reservations</span></span>

* <span data-ttu-id="70a96-2236">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2236">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="70a96-2237">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2237">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="70a96-2238">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2238">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="70a96-2239">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2239">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="70a96-2240">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2240">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="70a96-2241">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2241">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="70a96-2242">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-2242">Role</span></span>

* <span data-ttu-id="70a96-2243">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="70a96-2243">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-2244">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-2244">SQL</span></span>

* <span data-ttu-id="70a96-2245">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="70a96-2245">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-2246">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-2246">Storage</span></span>

* <span data-ttu-id="70a96-2247">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="70a96-2247">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2248">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2248">VM</span></span>

* <span data-ttu-id="70a96-2249">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2249">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="70a96-2250">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2250">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="70a96-2251">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="70a96-2251">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="70a96-2252">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2252">June 13, 2018</span></span>

<span data-ttu-id="70a96-2253">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="70a96-2253">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="70a96-2254">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-2254">Core</span></span>

* <span data-ttu-id="70a96-2255">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="70a96-2255">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="70a96-2256">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2256">June 13, 2018</span></span>

<span data-ttu-id="70a96-2257">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="70a96-2257">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="70a96-2258">AKS</span><span class="sxs-lookup"><span data-stu-id="70a96-2258">AKS</span></span>

* <span data-ttu-id="70a96-2259">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="70a96-2259">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="70a96-2260">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="70a96-2260">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="70a96-2261">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="70a96-2261">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="70a96-2262">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="70a96-2262">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="70a96-2263">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="70a96-2263">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-2264">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-2264">AppService</span></span>

* <span data-ttu-id="70a96-2265">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="70a96-2265">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="70a96-2266">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2266">June 5, 2018</span></span>

<span data-ttu-id="70a96-2267">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="70a96-2267">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="70a96-2268">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="70a96-2268">Interactive</span></span>

* <span data-ttu-id="70a96-2269">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="70a96-2269">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="70a96-2270">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2270">June 5, 2018</span></span>

<span data-ttu-id="70a96-2271">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="70a96-2271">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="70a96-2272">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-2272">Core</span></span>

* <span data-ttu-id="70a96-2273">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="70a96-2273">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="70a96-2274">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="70a96-2274">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-2275">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-2275">ACR</span></span>

* <span data-ttu-id="70a96-2276">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="70a96-2276">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="70a96-2277">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2277">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="70a96-2278">AKS</span><span class="sxs-lookup"><span data-stu-id="70a96-2278">AKS</span></span>

* <span data-ttu-id="70a96-2279">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="70a96-2279">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="70a96-2280">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-2280">Batch</span></span>

* <span data-ttu-id="70a96-2281">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="70a96-2281">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="70a96-2282">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-2282">IOT</span></span>

* <span data-ttu-id="70a96-2283">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="70a96-2283">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="70a96-2284">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-2284">Network</span></span>

* <span data-ttu-id="70a96-2285">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2285">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="70a96-2286">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="70a96-2286">Policy Insights</span></span>

* <span data-ttu-id="70a96-2287">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="70a96-2287">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="70a96-2288">ARM</span><span class="sxs-lookup"><span data-stu-id="70a96-2288">ARM</span></span>

* <span data-ttu-id="70a96-2289">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2289">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-2290">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-2290">SQL</span></span>

* <span data-ttu-id="70a96-2291">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="70a96-2291">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="70a96-2292">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="70a96-2292">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="70a96-2293">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-2293">Storage</span></span>

* <span data-ttu-id="70a96-2294">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2294">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2295">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2295">VM</span></span>

* <span data-ttu-id="70a96-2296">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2296">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="70a96-2297">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2297">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="70a96-2298">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2298">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="70a96-2299">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2299">May 22, 2018</span></span>

<span data-ttu-id="70a96-2300">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="70a96-2300">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="70a96-2301">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-2301">Core</span></span>

* <span data-ttu-id="70a96-2302">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2302">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-2303">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-2303">ACS</span></span>

* <span data-ttu-id="70a96-2304">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2304">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="70a96-2305">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="70a96-2305">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-2306">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-2306">AppService</span></span>

* <span data-ttu-id="70a96-2307">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="70a96-2307">Improved generic update commands</span></span>
* <span data-ttu-id="70a96-2308">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2308">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="70a96-2309">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-2309">Container</span></span>

* <span data-ttu-id="70a96-2310">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="70a96-2310">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="70a96-2311">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70a96-2311">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="70a96-2312">Расширение</span><span class="sxs-lookup"><span data-stu-id="70a96-2312">Extension</span></span>

* <span data-ttu-id="70a96-2313">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="70a96-2313">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="70a96-2314">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="70a96-2314">Interactive</span></span>

* <span data-ttu-id="70a96-2315">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="70a96-2315">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="70a96-2316">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="70a96-2316">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="70a96-2317">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70a96-2317">KeyVault</span></span>

* <span data-ttu-id="70a96-2318">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="70a96-2318">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="70a96-2319">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-2319">Network</span></span>

* <span data-ttu-id="70a96-2320">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="70a96-2320">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="70a96-2321">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="70a96-2321">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-2322">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-2322">SQL</span></span>

* <span data-ttu-id="70a96-2323">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="70a96-2323">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="70a96-2324">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2324">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="70a96-2325">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2325">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="70a96-2326">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="70a96-2326">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="70a96-2327">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="70a96-2327">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="70a96-2328">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2328">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="70a96-2329">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2329">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="70a96-2330">`edition`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2330">`edition`.</span></span> <span data-ttu-id="70a96-2331">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2331">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="70a96-2332">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2332">`elasticPoolName`.</span></span> <span data-ttu-id="70a96-2333">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2333">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="70a96-2334">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="70a96-2334">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="70a96-2335">`edition`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2335">`edition`.</span></span> <span data-ttu-id="70a96-2336">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2336">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="70a96-2337">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2337">`dtu`.</span></span> <span data-ttu-id="70a96-2338">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2338">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="70a96-2339">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2339">`databaseDtuMin`.</span></span> <span data-ttu-id="70a96-2340">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2340">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="70a96-2341">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2341">`databaseDtuMax`.</span></span> <span data-ttu-id="70a96-2342">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2342">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="70a96-2343">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2343">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="70a96-2344">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2344">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-2345">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-2345">Storage</span></span>

* <span data-ttu-id="70a96-2346">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2346">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="70a96-2347">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2347">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2348">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2348">VM</span></span>

* <span data-ttu-id="70a96-2349">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2349">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="70a96-2350">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2350">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="70a96-2351">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2351">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="70a96-2352">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="70a96-2352">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="70a96-2353">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2353">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="70a96-2354">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2354">May 7, 2018</span></span>

<span data-ttu-id="70a96-2355">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="70a96-2355">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="70a96-2356">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-2356">Core</span></span>

* <span data-ttu-id="70a96-2357">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="70a96-2357">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="70a96-2358">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2358">Added limited support for positional arguments</span></span>
* <span data-ttu-id="70a96-2359">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2359">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="70a96-2360">#5591</span><span class="sxs-lookup"><span data-stu-id="70a96-2360">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="70a96-2361">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2361">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="70a96-2362">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="70a96-2362">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="70a96-2363">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="70a96-2363">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="70a96-2364">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2364">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="70a96-2365">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="70a96-2365">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-2366">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-2366">ACR</span></span>

* <span data-ttu-id="70a96-2367">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="70a96-2367">Added ACR Build commands</span></span>
* <span data-ttu-id="70a96-2368">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="70a96-2368">Improved resource not found error messages</span></span>
* <span data-ttu-id="70a96-2369">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="70a96-2369">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="70a96-2370">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="70a96-2370">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="70a96-2371">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="70a96-2371">Improved repository commands error messages</span></span>
* <span data-ttu-id="70a96-2372">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="70a96-2372">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-2373">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-2373">ACS</span></span>

* <span data-ttu-id="70a96-2374">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="70a96-2374">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="70a96-2375">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="70a96-2375">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="70a96-2376">AMS</span><span class="sxs-lookup"><span data-stu-id="70a96-2376">AMS</span></span>

* <span data-ttu-id="70a96-2377">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="70a96-2377">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-2378">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-2378">Appservice</span></span>

* <span data-ttu-id="70a96-2379">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="70a96-2379">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="70a96-2380">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2380">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="70a96-2381">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="70a96-2381">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="70a96-2382">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70a96-2382">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="70a96-2383">Batch AI</span><span class="sxs-lookup"><span data-stu-id="70a96-2383">Batch AI</span></span>

* <span data-ttu-id="70a96-2384">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="70a96-2384">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="70a96-2385">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="70a96-2385">Cognitive Services</span></span>

* <span data-ttu-id="70a96-2386">Исправлена опечатка в примере для `cognitiveservices account create` ([№ 5603](https://github.com/Azure/azure-cli/issues/5603)).</span><span class="sxs-lookup"><span data-stu-id="70a96-2386">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="70a96-2387">Потребление</span><span class="sxs-lookup"><span data-stu-id="70a96-2387">Consumption</span></span>

* <span data-ttu-id="70a96-2388">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="70a96-2388">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="70a96-2389">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-2389">Container</span></span>

* <span data-ttu-id="70a96-2390">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="70a96-2390">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="70a96-2391">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70a96-2391">Cosmos DB</span></span>

* <span data-ttu-id="70a96-2392">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70a96-2392">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="70a96-2393">DMS</span><span class="sxs-lookup"><span data-stu-id="70a96-2393">DMS</span></span>

* <span data-ttu-id="70a96-2394">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="70a96-2394">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="70a96-2395">Расширение</span><span class="sxs-lookup"><span data-stu-id="70a96-2395">Extension</span></span>

* <span data-ttu-id="70a96-2396">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="70a96-2396">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="70a96-2397">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="70a96-2397">Interactive</span></span>

* <span data-ttu-id="70a96-2398">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="70a96-2398">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="70a96-2399">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="70a96-2399">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="70a96-2400">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="70a96-2400">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="70a96-2401">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="70a96-2401">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="70a96-2402">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="70a96-2402">Lab</span></span>

* <span data-ttu-id="70a96-2403">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="70a96-2403">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="70a96-2404">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-2404">Network</span></span>

* <span data-ttu-id="70a96-2405">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="70a96-2405">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="70a96-2406">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-2406">Profile</span></span>

* <span data-ttu-id="70a96-2407">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2407">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="70a96-2408">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="70a96-2408">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="70a96-2409">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2409">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="70a96-2410">Redis</span><span class="sxs-lookup"><span data-stu-id="70a96-2410">Redis</span></span>

* <span data-ttu-id="70a96-2411">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2411">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="70a96-2412">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="70a96-2412">Deprecated `redis list-all`.</span></span> <span data-ttu-id="70a96-2413">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2413">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="70a96-2414">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2414">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="70a96-2415">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="70a96-2415">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="70a96-2416">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-2416">Role</span></span>

* <span data-ttu-id="70a96-2417">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="70a96-2417">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-2418">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-2418">Storage</span></span>

* <span data-ttu-id="70a96-2419">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="70a96-2419">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="70a96-2420">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="70a96-2420">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="70a96-2421">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="70a96-2421">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="70a96-2422">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="70a96-2422">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="70a96-2423">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="70a96-2423">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2424">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2424">VM</span></span>

* <span data-ttu-id="70a96-2425">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="70a96-2425">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="70a96-2426">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="70a96-2426">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="70a96-2427">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="70a96-2427">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="70a96-2428">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2428">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="70a96-2429">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="70a96-2429">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="70a96-2430">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="70a96-2430">Added write accelerator support</span></span>
* <span data-ttu-id="70a96-2431">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2431">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="70a96-2432">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="70a96-2432">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="70a96-2433">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="70a96-2433">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="70a96-2434">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2434">April 10, 2018</span></span>

<span data-ttu-id="70a96-2435">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="70a96-2435">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-2436">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-2436">ACR</span></span>

* <span data-ttu-id="70a96-2437">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="70a96-2437">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-2438">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-2438">ACS</span></span>

* <span data-ttu-id="70a96-2439">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="70a96-2439">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-2440">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-2440">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="70a96-2442">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="70a96-2442">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="70a96-2443">Batch AI</span><span class="sxs-lookup"><span data-stu-id="70a96-2443">BatchAI</span></span>

* <span data-ttu-id="70a96-2444">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="70a96-2444">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="70a96-2445">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="70a96-2445">Job level mounting</span></span>
  - <span data-ttu-id="70a96-2446">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2446">Environment variables with secret values</span></span>
  - <span data-ttu-id="70a96-2447">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="70a96-2447">Performance counters settings</span></span>
  - <span data-ttu-id="70a96-2448">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="70a96-2448">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="70a96-2449">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2449">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="70a96-2450">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="70a96-2450">Usage and limits reporting</span></span>
  - <span data-ttu-id="70a96-2451">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2451">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="70a96-2452">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2452">Support for custom images</span></span>
  - <span data-ttu-id="70a96-2453">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="70a96-2453">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="70a96-2454">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="70a96-2454">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="70a96-2455">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2455">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="70a96-2456">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="70a96-2456">National clouds are supported</span></span>
* <span data-ttu-id="70a96-2457">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="70a96-2457">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="70a96-2458">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="70a96-2458">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="70a96-2459">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="70a96-2459">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="70a96-2460">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="70a96-2460">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="70a96-2461">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="70a96-2461">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="70a96-2462">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="70a96-2462">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="70a96-2463">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2463">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="70a96-2464">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="70a96-2464">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="70a96-2465">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="70a96-2465">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="70a96-2466">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2466">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="70a96-2467">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="70a96-2467">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="70a96-2468">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2468">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="70a96-2469">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2469">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="70a96-2470">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="70a96-2470">Billing</span></span>

* <span data-ttu-id="70a96-2471">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="70a96-2471">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="70a96-2472">Потребление</span><span class="sxs-lookup"><span data-stu-id="70a96-2472">Consumption</span></span>

* <span data-ttu-id="70a96-2473">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2473">Added `marketplace` commands</span></span>
* <span data-ttu-id="70a96-2474">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2474">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="70a96-2475">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2475">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="70a96-2476">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2476">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="70a96-2477">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2477">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="70a96-2478">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2478">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="70a96-2479">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-2479">Container</span></span>

* <span data-ttu-id="70a96-2480">Добавлены параметры подключения тома репозитория Git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2480">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="70a96-2481">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="70a96-2481">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="70a96-2482">Расширение</span><span class="sxs-lookup"><span data-stu-id="70a96-2482">Extension</span></span>

* <span data-ttu-id="70a96-2483">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="70a96-2483">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="70a96-2484">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="70a96-2484">Interactive</span></span>

* <span data-ttu-id="70a96-2485">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="70a96-2485">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="70a96-2486">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="70a96-2486">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="70a96-2487">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2487">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="70a96-2488">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-2488">Network</span></span>

* <span data-ttu-id="70a96-2489">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2489">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="70a96-2490">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2490">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="70a96-2491">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="70a96-2491">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="70a96-2492">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="70a96-2492">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="70a96-2493">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="70a96-2493">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="70a96-2494">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2494">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="70a96-2495">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2495">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="70a96-2496">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="70a96-2496">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="70a96-2497">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-2497">Profile</span></span>

* <span data-ttu-id="70a96-2498">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2498">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="70a96-2499">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi` & `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2499">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="70a96-2500">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="70a96-2500">RDBMS</span></span>

* <span data-ttu-id="70a96-2501">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2501">Added `georestore` command</span></span>
* <span data-ttu-id="70a96-2502">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="70a96-2502">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-2503">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-2503">Resource</span></span>

* <span data-ttu-id="70a96-2504">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2504">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="70a96-2505">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2505">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-2506">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-2506">SQL</span></span>

* <span data-ttu-id="70a96-2507">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2507">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-2508">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-2508">Storage</span></span>

* <span data-ttu-id="70a96-2509">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="70a96-2509">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2510">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2510">VM</span></span>

* <span data-ttu-id="70a96-2511">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="70a96-2511">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="70a96-2512">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="70a96-2512">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="70a96-2514">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2514">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="70a96-2515">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="70a96-2515">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="70a96-2516">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="70a96-2516">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="70a96-2517">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="70a96-2517">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="70a96-2518">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2518">March 27, 2018</span></span>

<span data-ttu-id="70a96-2519">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="70a96-2519">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="70a96-2520">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-2520">Core</span></span>

* <span data-ttu-id="70a96-2521">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="70a96-2521">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-2522">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-2522">ACS</span></span>

* <span data-ttu-id="70a96-2523">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="70a96-2523">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-2524">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-2524">Appservice</span></span>

* <span data-ttu-id="70a96-2525">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2525">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="70a96-2526">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2526">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="70a96-2527">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="70a96-2527">Backup</span></span>

* <span data-ttu-id="70a96-2528">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2528">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="70a96-2529">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="70a96-2529">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="70a96-2530">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="70a96-2530">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="70a96-2531">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2531">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="70a96-2532">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-2532">Container</span></span>

* <span data-ttu-id="70a96-2533">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2533">Added `container exec` command.</span></span> <span data-ttu-id="70a96-2534">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70a96-2534">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="70a96-2535">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70a96-2535">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="70a96-2536">Расширение</span><span class="sxs-lookup"><span data-stu-id="70a96-2536">Extension</span></span>

* <span data-ttu-id="70a96-2537">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="70a96-2537">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="70a96-2538">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2538">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="70a96-2539">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-2539">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="70a96-2540">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="70a96-2540">Interactive</span></span>

* <span data-ttu-id="70a96-2541">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="70a96-2541">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="70a96-2542">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2542">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="70a96-2543">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="70a96-2543">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="70a96-2544">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="70a96-2544">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="70a96-2545">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="70a96-2545">Lab</span></span>

* <span data-ttu-id="70a96-2546">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2546">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-2547">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-2547">Monitor</span></span>

* <span data-ttu-id="70a96-2548">Добавлена поддержка аргументов `--top`, `--orderby` и `--namespace` для `metrics list` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="70a96-2548">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="70a96-2549">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="70a96-2549">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="70a96-2550">Добавлена поддержка `--namespace` для `metrics list-definitions` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="70a96-2550">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="70a96-2551">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-2551">Network</span></span>

* <span data-ttu-id="70a96-2552">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="70a96-2552">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="70a96-2553">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-2553">Profile</span></span>

* <span data-ttu-id="70a96-2554">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2554">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="70a96-2555">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="70a96-2555">RDBMS</span></span>

* <span data-ttu-id="70a96-2556">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="70a96-2556">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-2557">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-2557">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="70a96-2559">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-2559">Role</span></span>

* <span data-ttu-id="70a96-2560">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2560">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="70a96-2561">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="70a96-2561">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="70a96-2562">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="70a96-2562">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="70a96-2563">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2563">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="70a96-2564">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2564">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-2565">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-2565">Storage</span></span>

* <span data-ttu-id="70a96-2566">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="70a96-2566">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="70a96-2567">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="70a96-2567">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2568">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2568">VM</span></span>

* <span data-ttu-id="70a96-2569">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="70a96-2569">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="70a96-2570">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2570">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="70a96-2571">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="70a96-2571">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="70a96-2572">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="70a96-2572">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="70a96-2573">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2573">March 13, 2018</span></span>

<span data-ttu-id="70a96-2574">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="70a96-2574">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-2575">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-2575">ACR</span></span>

* <span data-ttu-id="70a96-2576">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2576">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="70a96-2577">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="70a96-2577">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="70a96-2578">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="70a96-2578">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-2579">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-2579">ACS</span></span>

* <span data-ttu-id="70a96-2580">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="70a96-2580">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="70a96-2581">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="70a96-2581">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="70a96-2582">Помощник</span><span class="sxs-lookup"><span data-stu-id="70a96-2582">Advisor</span></span>

* <span data-ttu-id="70a96-2583">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2583">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="70a96-2584">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2584">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="70a96-2585">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2585">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="70a96-2586">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2586">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="70a96-2587">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2587">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-2588">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-2588">Appservice</span></span>

* <span data-ttu-id="70a96-2589">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="70a96-2589">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="70a96-2590">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2590">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="70a96-2591">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="70a96-2591">Eventhubs</span></span>

* <span data-ttu-id="70a96-2592">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="70a96-2592">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="70a96-2593">Расширение</span><span class="sxs-lookup"><span data-stu-id="70a96-2593">Extension</span></span>

* <span data-ttu-id="70a96-2594">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="70a96-2594">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="70a96-2595">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="70a96-2595">Interactive</span></span>

* <span data-ttu-id="70a96-2596">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="70a96-2596">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="70a96-2597">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="70a96-2597">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="70a96-2598">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="70a96-2598">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="70a96-2599">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="70a96-2599">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-2600">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-2600">Monitor</span></span>

* <span data-ttu-id="70a96-2601">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="70a96-2601">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="70a96-2602">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2602">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="70a96-2603">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2603">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="70a96-2604">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2604">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="70a96-2605">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-2605">Network</span></span>

* <span data-ttu-id="70a96-2606">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2606">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="70a96-2607">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="70a96-2607">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="70a96-2608">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2608">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="70a96-2609">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2609">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="70a96-2610">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-2610">Profile</span></span>

* <span data-ttu-id="70a96-2611">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="70a96-2611">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="70a96-2612">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2612">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="70a96-2613">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="70a96-2613">RDBMS</span></span>

* <span data-ttu-id="70a96-2614">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="70a96-2614">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="70a96-2615">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="70a96-2615">Service Bus</span></span>

* <span data-ttu-id="70a96-2616">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="70a96-2616">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-2617">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-2617">Storage</span></span>

* <span data-ttu-id="70a96-2618">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="70a96-2618">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="70a96-2619">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="70a96-2619">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2620">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2620">VM</span></span>

* <span data-ttu-id="70a96-2621">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="70a96-2621">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="70a96-2622">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="70a96-2622">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="70a96-2623">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2623">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="70a96-2624">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="70a96-2624">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="70a96-2625">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="70a96-2625">February 27, 2018</span></span>

<span data-ttu-id="70a96-2626">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="70a96-2626">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="70a96-2627">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-2627">Core</span></span>

* <span data-ttu-id="70a96-2628">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="70a96-2628">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="70a96-2629">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="70a96-2629">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="70a96-2630">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2630">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-2631">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-2631">ACS</span></span>

* <span data-ttu-id="70a96-2632">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-2632">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="70a96-2633">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="70a96-2633">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="70a96-2634">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2634">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="70a96-2635">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2635">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-2636">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-2636">Appservice</span></span>

* <span data-ttu-id="70a96-2637">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="70a96-2637">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="70a96-2638">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="70a96-2638">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="70a96-2639">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="70a96-2639">Cognitive Services</span></span>

* <span data-ttu-id="70a96-2640">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="70a96-2640">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="70a96-2641">Потребление</span><span class="sxs-lookup"><span data-stu-id="70a96-2641">Consumption</span></span>

* <span data-ttu-id="70a96-2642">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="70a96-2642">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="70a96-2643">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="70a96-2643">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="70a96-2644">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-2644">Container</span></span>

* <span data-ttu-id="70a96-2645">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="70a96-2645">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="70a96-2646">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-2646">Network</span></span>

* <span data-ttu-id="70a96-2647">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2647">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-2648">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-2648">Resource</span></span>

* <span data-ttu-id="70a96-2649">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="70a96-2649">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="70a96-2650">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-2650">Role</span></span>

* <span data-ttu-id="70a96-2651">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="70a96-2651">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-2652">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-2652">SQL</span></span>

* <span data-ttu-id="70a96-2653">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2653">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-2654">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-2654">Storage</span></span>

* <span data-ttu-id="70a96-2655">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2655">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2656">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2656">VM</span></span>

* <span data-ttu-id="70a96-2657">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="70a96-2657">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="70a96-2658">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2658">February 13, 2018</span></span>

<span data-ttu-id="70a96-2659">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="70a96-2659">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="70a96-2660">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-2660">Core</span></span>

* <span data-ttu-id="70a96-2661">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="70a96-2661">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-2662">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-2662">ACS</span></span>

* <span data-ttu-id="70a96-2663">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="70a96-2663">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="70a96-2664">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2664">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="70a96-2665">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="70a96-2665">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="70a96-2666">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="70a96-2666">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="70a96-2667">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="70a96-2667">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="70a96-2668">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2668">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="70a96-2669">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="70a96-2669">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="70a96-2670">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2670">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-2671">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-2671">Appservice</span></span>

* <span data-ttu-id="70a96-2672">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="70a96-2672">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="70a96-2673">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2673">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="70a96-2674">CDN</span><span class="sxs-lookup"><span data-stu-id="70a96-2674">CDN</span></span>

* <span data-ttu-id="70a96-2675">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2675">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="70a96-2676">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-2676">Container</span></span>

* <span data-ttu-id="70a96-2677">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="70a96-2677">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="70a96-2678">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70a96-2678">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="70a96-2679">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70a96-2679">CosmosDB</span></span>

* <span data-ttu-id="70a96-2680">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="70a96-2680">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="70a96-2681">Расширение</span><span class="sxs-lookup"><span data-stu-id="70a96-2681">Extension</span></span>

* <span data-ttu-id="70a96-2682">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2682">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="70a96-2683">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2683">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="70a96-2684">Отзывы</span><span class="sxs-lookup"><span data-stu-id="70a96-2684">Feedback</span></span>

* <span data-ttu-id="70a96-2685">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="70a96-2685">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="70a96-2686">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="70a96-2686">Interactive</span></span>

* <span data-ttu-id="70a96-2687">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="70a96-2687">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="70a96-2688">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="70a96-2688">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="70a96-2689">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-2689">IoT</span></span>

* <span data-ttu-id="70a96-2690">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="70a96-2690">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="70a96-2691">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="70a96-2691">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="70a96-2692">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2692">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="70a96-2693">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="70a96-2693">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-2694">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-2694">Monitor</span></span>

* <span data-ttu-id="70a96-2695">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2695">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="70a96-2696">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-2696">Network</span></span>

* <span data-ttu-id="70a96-2697">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="70a96-2697">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="70a96-2698">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-2698">Profile</span></span>

* <span data-ttu-id="70a96-2699">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="70a96-2699">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-2700">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-2700">Resource</span></span>

* <span data-ttu-id="70a96-2701">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2701">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="70a96-2702">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-2702">Role</span></span>

* <span data-ttu-id="70a96-2703">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="70a96-2703">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-2704">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-2704">SQL</span></span>

* <span data-ttu-id="70a96-2705">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2705">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="70a96-2706">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2706">Added `sql db rename`</span></span>
* <span data-ttu-id="70a96-2707">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="70a96-2707">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-2708">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-2708">Storage</span></span>

* <span data-ttu-id="70a96-2709">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="70a96-2709">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2710">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2710">VM</span></span>

* <span data-ttu-id="70a96-2711">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="70a96-2711">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="70a96-2712">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="70a96-2712">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="70a96-2713">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="70a96-2713">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="70a96-2714">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2714">January 31, 2018</span></span>

<span data-ttu-id="70a96-2715">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="70a96-2715">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="70a96-2716">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-2716">Core</span></span>

* <span data-ttu-id="70a96-2717">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="70a96-2717">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="70a96-2718">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="70a96-2718">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="70a96-2719">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="70a96-2719">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="70a96-2720">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="70a96-2720">Use `--verbose` to see</span></span>
* <span data-ttu-id="70a96-2721">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="70a96-2721">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-2722">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-2722">ACS</span></span>

* <span data-ttu-id="70a96-2723">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2723">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="70a96-2724">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2724">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-2725">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-2725">Appservice</span></span>

* <span data-ttu-id="70a96-2726">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="70a96-2726">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="70a96-2727">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="70a96-2727">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="70a96-2728">CDN</span><span class="sxs-lookup"><span data-stu-id="70a96-2728">CDN</span></span>

* <span data-ttu-id="70a96-2729">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2729">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="70a96-2730">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70a96-2730">CosmosDB</span></span>

* <span data-ttu-id="70a96-2731">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="70a96-2731">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="70a96-2732">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="70a96-2732">Interactive</span></span>

* <span data-ttu-id="70a96-2733">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="70a96-2733">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="70a96-2734">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-2734">Network</span></span>

* <span data-ttu-id="70a96-2735">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2735">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="70a96-2736">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-2736">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="70a96-2737">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2737">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="70a96-2738">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2738">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="70a96-2739">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2739">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="70a96-2740">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="70a96-2740">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="70a96-2741">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="70a96-2741">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="70a96-2742">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="70a96-2742">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="70a96-2743">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2743">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="70a96-2744">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2744">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="70a96-2745">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-2745">Profile</span></span>

* <span data-ttu-id="70a96-2746">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="70a96-2746">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-2747">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-2747">Resource</span></span>

* <span data-ttu-id="70a96-2748">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="70a96-2748">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-2749">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-2749">Storage</span></span>

* <span data-ttu-id="70a96-2750">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="70a96-2750">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="70a96-2751">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="70a96-2751">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="70a96-2752">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2752">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="70a96-2753">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2753">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="70a96-2754">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="70a96-2754">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2755">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2755">VM</span></span>

* <span data-ttu-id="70a96-2756">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="70a96-2756">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="70a96-2757">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2757">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="70a96-2758">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="70a96-2758">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="70a96-2759">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2759">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="70a96-2760">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2760">January 17, 2018</span></span>

<span data-ttu-id="70a96-2761">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="70a96-2761">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-2762">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-2762">ACR</span></span>

* <span data-ttu-id="70a96-2763">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="70a96-2763">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="70a96-2764">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="70a96-2764">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-2765">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-2765">ACS</span></span>

* <span data-ttu-id="70a96-2766">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2766">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="70a96-2767">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="70a96-2767">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-2768">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-2768">Appservice</span></span>

* <span data-ttu-id="70a96-2769">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="70a96-2769">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="70a96-2770">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2770">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="70a96-2771">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2771">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="70a96-2772">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="70a96-2772">Backup</span></span>

* <span data-ttu-id="70a96-2773">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="70a96-2773">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="70a96-2774">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="70a96-2774">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="70a96-2775">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="70a96-2775">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="70a96-2776">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="70a96-2776">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="70a96-2777">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="70a96-2777">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="70a96-2778">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-2778">Batch</span></span>

* <span data-ttu-id="70a96-2779">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="70a96-2779">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="70a96-2780">Cloud</span><span class="sxs-lookup"><span data-stu-id="70a96-2780">Cloud</span></span>

* <span data-ttu-id="70a96-2781">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="70a96-2781">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="70a96-2782">Потребление</span><span class="sxs-lookup"><span data-stu-id="70a96-2782">Consumption</span></span>

* <span data-ttu-id="70a96-2783">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2783">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="70a96-2784">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-2784">Event Grid</span></span>

* <span data-ttu-id="70a96-2785">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2785">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="70a96-2786">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2786">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="70a96-2787">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2787">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="70a96-2788">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2788">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="70a96-2789">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2789">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="70a96-2790">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2790">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="70a96-2791">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2791">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="70a96-2792">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2792">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="70a96-2793">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="70a96-2793">Interactive</span></span>

* <span data-ttu-id="70a96-2794">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="70a96-2794">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="70a96-2795">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="70a96-2795">Fixed errors on startup</span></span>
* <span data-ttu-id="70a96-2796">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="70a96-2796">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="70a96-2797">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-2797">IoT</span></span>

* <span data-ttu-id="70a96-2798">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="70a96-2798">Added support for device provisioning service</span></span>
* <span data-ttu-id="70a96-2799">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="70a96-2799">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="70a96-2800">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="70a96-2800">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-2801">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-2801">Monitor</span></span>

* <span data-ttu-id="70a96-2802">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="70a96-2802">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="70a96-2803">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2803">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="70a96-2804">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="70a96-2804">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="70a96-2805">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-2805">Network</span></span>

* <span data-ttu-id="70a96-2806">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="70a96-2806">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="70a96-2807">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="70a96-2807">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="70a96-2808">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-2808">Profile</span></span>

* <span data-ttu-id="70a96-2809">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="70a96-2809">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="70a96-2810">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-2810">Role</span></span>

* <span data-ttu-id="70a96-2811">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2811">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="70a96-2812">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="70a96-2812">Service Fabric</span></span>

* <span data-ttu-id="70a96-2813">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="70a96-2813">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="70a96-2814">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="70a96-2814">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2815">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2815">VM</span></span>

* <span data-ttu-id="70a96-2816">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2816">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="70a96-2817">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="70a96-2817">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="70a96-2818">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2818">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="70a96-2819">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="70a96-2819">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="70a96-2820">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="70a96-2820">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="70a96-2821">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2821">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="70a96-2822">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2822">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="70a96-2823">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2823">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="70a96-2824">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2824">December 19, 2017</span></span>

<span data-ttu-id="70a96-2825">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="70a96-2825">Version 2.0.23</span></span>

* <span data-ttu-id="70a96-2826">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="70a96-2826">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="70a96-2827">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-2827">Container</span></span>

* <span data-ttu-id="70a96-2828">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70a96-2828">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="70a96-2829">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-2829">Network</span></span>

* <span data-ttu-id="70a96-2830">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="70a96-2830">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="70a96-2831">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="70a96-2831">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-2832">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-2832">Storage</span></span>

* <span data-ttu-id="70a96-2833">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="70a96-2833">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2834">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2834">VM</span></span>

* <span data-ttu-id="70a96-2835">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="70a96-2835">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="70a96-2836">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2836">December 5, 2017</span></span>

<span data-ttu-id="70a96-2837">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="70a96-2837">Version 2.0.22</span></span>

* <span data-ttu-id="70a96-2838">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2838">Removed `az component` commands.</span></span> <span data-ttu-id="70a96-2839">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2839">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="70a96-2840">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-2840">Core</span></span>
* <span data-ttu-id="70a96-2841">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="70a96-2841">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="70a96-2842">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="70a96-2842">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-2843">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-2843">ACS</span></span>

* <span data-ttu-id="70a96-2844">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2844">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="70a96-2845">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2845">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="70a96-2846">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="70a96-2846">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="70a96-2847">Помощник</span><span class="sxs-lookup"><span data-stu-id="70a96-2847">Advisor</span></span>

* <span data-ttu-id="70a96-2848">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="70a96-2848">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-2849">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-2849">Appservice</span></span>

* <span data-ttu-id="70a96-2850">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2850">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="70a96-2851">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="70a96-2851">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="70a96-2852">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2852">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="70a96-2853">Потребление</span><span class="sxs-lookup"><span data-stu-id="70a96-2853">Consumption</span></span>

* <span data-ttu-id="70a96-2854">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="70a96-2854">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="70a96-2855">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-2855">Container</span></span>

* <span data-ttu-id="70a96-2856">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="70a96-2856">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-2857">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-2857">Monitor</span></span>

* <span data-ttu-id="70a96-2858">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="70a96-2858">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-2859">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-2859">Resource</span></span>

* <span data-ttu-id="70a96-2860">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="70a96-2860">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="70a96-2861">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-2861">Role</span></span>

* <span data-ttu-id="70a96-2862">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2862">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="70a96-2863">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="70a96-2863">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="70a96-2864">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2864">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-2865">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-2865">SQL</span></span>

* <span data-ttu-id="70a96-2866">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2866">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="70a96-2867">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2867">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2868">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2868">VM</span></span>

* <span data-ttu-id="70a96-2869">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2869">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="70a96-2870">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2870">November 14, 2017</span></span>

<span data-ttu-id="70a96-2871">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="70a96-2871">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-2872">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-2872">ACR</span></span>

* <span data-ttu-id="70a96-2873">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="70a96-2873">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="70a96-2874">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-2874">ACS</span></span>

* <span data-ttu-id="70a96-2875">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="70a96-2875">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="70a96-2876">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="70a96-2876">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="70a96-2877">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2877">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="70a96-2878">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="70a96-2878">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="70a96-2879">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="70a96-2879">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-2880">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-2880">Appservice</span></span>

* <span data-ttu-id="70a96-2881">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="70a96-2881">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="70a96-2882">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2882">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="70a96-2883">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2883">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="70a96-2884">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2884">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="70a96-2885">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="70a96-2885">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="70a96-2886">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="70a96-2886">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="70a96-2887">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-2887">Batch</span></span>

* <span data-ttu-id="70a96-2888">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2888">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="70a96-2889">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="70a96-2889">Batchai</span></span>

* <span data-ttu-id="70a96-2890">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2890">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="70a96-2891">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2891">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="70a96-2892">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2892">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="70a96-2893">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2893">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="70a96-2894">Cloud</span><span class="sxs-lookup"><span data-stu-id="70a96-2894">Cloud</span></span>

* <span data-ttu-id="70a96-2895">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="70a96-2895">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="70a96-2896">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-2896">Container</span></span>

* <span data-ttu-id="70a96-2897">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2897">Added support to open multiple ports</span></span>
* <span data-ttu-id="70a96-2898">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70a96-2898">Added container group restart policy</span></span>
* <span data-ttu-id="70a96-2899">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="70a96-2899">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="70a96-2900">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="70a96-2900">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="70a96-2901">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="70a96-2901">Data Lake Analytics</span></span>

* <span data-ttu-id="70a96-2902">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="70a96-2902">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="70a96-2903">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="70a96-2903">Data Lake Store</span></span>

* <span data-ttu-id="70a96-2904">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="70a96-2904">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="70a96-2905">Расширение</span><span class="sxs-lookup"><span data-stu-id="70a96-2905">Extension</span></span>

* <span data-ttu-id="70a96-2906">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="70a96-2906">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="70a96-2907">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="70a96-2907">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="70a96-2908">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-2908">IoT</span></span>

* <span data-ttu-id="70a96-2909">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2909">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-2910">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-2910">Monitor</span></span>

* <span data-ttu-id="70a96-2911">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2911">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="70a96-2912">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-2912">Network</span></span>

* <span data-ttu-id="70a96-2913">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="70a96-2913">Added support for CAA DNS records</span></span>
* <span data-ttu-id="70a96-2914">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2914">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="70a96-2915">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="70a96-2915">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="70a96-2916">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2916">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="70a96-2917">Резервирование</span><span class="sxs-lookup"><span data-stu-id="70a96-2917">Reservations</span></span>

* <span data-ttu-id="70a96-2918">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="70a96-2918">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-2919">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-2919">Resource</span></span>

* <span data-ttu-id="70a96-2920">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2920">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-2921">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-2921">SQL</span></span>

* <span data-ttu-id="70a96-2922">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2922">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-2923">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-2923">Storage</span></span>

* <span data-ttu-id="70a96-2924">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-2924">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="70a96-2925">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="70a96-2925">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="70a96-2926">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2926">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="70a96-2927">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2927">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="70a96-2928">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2928">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="70a96-2929">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2929">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="70a96-2930">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2930">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2931">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2931">VM</span></span>

* <span data-ttu-id="70a96-2932">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2932">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="70a96-2933">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2933">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="70a96-2934">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2934">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="70a96-2935">Переименование `vm format-secret` в `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="70a96-2935">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="70a96-2936">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="70a96-2936">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="70a96-2937">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2937">October 24, 2017</span></span>

<span data-ttu-id="70a96-2938">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="70a96-2938">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="70a96-2939">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-2939">Core</span></span>

* <span data-ttu-id="70a96-2940">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="70a96-2940">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-2941">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-2941">ACR</span></span>

* <span data-ttu-id="70a96-2942">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="70a96-2942">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="70a96-2943">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="70a96-2943">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="70a96-2944">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="70a96-2944">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-2945">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-2945">ACS</span></span>

* <span data-ttu-id="70a96-2946">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="70a96-2946">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="70a96-2947">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="70a96-2947">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-2948">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-2948">Appservice</span></span>

* <span data-ttu-id="70a96-2949">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="70a96-2949">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="70a96-2950">Компонент</span><span class="sxs-lookup"><span data-stu-id="70a96-2950">Component</span></span>

* <span data-ttu-id="70a96-2951">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="70a96-2951">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-2952">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-2952">Monitor</span></span>

* <span data-ttu-id="70a96-2953">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2953">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-2954">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-2954">Resource</span></span>

* <span data-ttu-id="70a96-2955">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="70a96-2955">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="70a96-2956">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="70a96-2956">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2957">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-2957">VM</span></span>

* <span data-ttu-id="70a96-2958">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="70a96-2958">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="70a96-2959">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2959">October 9, 2017</span></span>

<span data-ttu-id="70a96-2960">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="70a96-2960">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="70a96-2961">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-2961">Core</span></span>

* <span data-ttu-id="70a96-2962">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="70a96-2962">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-2963">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-2963">Appservice</span></span>

* <span data-ttu-id="70a96-2964">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2964">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="70a96-2965">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-2965">Batch</span></span>

* <span data-ttu-id="70a96-2966">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="70a96-2966">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="70a96-2967">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="70a96-2967">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="70a96-2968">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="70a96-2968">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="70a96-2969">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2969">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="70a96-2970">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="70a96-2970">Batchai</span></span>

* <span data-ttu-id="70a96-2971">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="70a96-2971">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="70a96-2972">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70a96-2972">Keyvault</span></span>

* <span data-ttu-id="70a96-2973">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="70a96-2973">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="70a96-2974">(#4448)</span><span class="sxs-lookup"><span data-stu-id="70a96-2974">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="70a96-2975">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-2975">Network</span></span>

* <span data-ttu-id="70a96-2976">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="70a96-2976">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="70a96-2977">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="70a96-2977">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-2978">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-2978">Resource</span></span>

* <span data-ttu-id="70a96-2979">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2979">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="70a96-2980">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="70a96-2980">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="70a96-2981">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="70a96-2981">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="70a96-2982">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="70a96-2982">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-2983">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-2983">Sql</span></span>

* <span data-ttu-id="70a96-2984">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="70a96-2984">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="70a96-2985">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="70a96-2985">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="70a96-2986">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="70a96-2986">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-2987">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-2987">Storage</span></span>

* <span data-ttu-id="70a96-2988">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2988">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-2989">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="70a96-2989">Vm</span></span>

* <span data-ttu-id="70a96-2990">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="70a96-2990">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="70a96-2991">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2991">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="70a96-2992">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2992">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="70a96-2993">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-2993">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="70a96-2994">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="70a96-2994">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="70a96-2995">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-2995">September 22, 2017</span></span>

<span data-ttu-id="70a96-2996">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="70a96-2996">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-2997">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-2997">Resource</span></span>

* <span data-ttu-id="70a96-2998">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="70a96-2998">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="70a96-2999">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="70a96-2999">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="70a96-3000">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="70a96-3000">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="70a96-3001">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3001">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="70a96-3002">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-3002">Network</span></span>

* <span data-ttu-id="70a96-3003">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="70a96-3003">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="70a96-3004">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="70a96-3004">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="70a96-3005">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="70a96-3005">Added `asg` application security group commands</span></span>
* <span data-ttu-id="70a96-3006">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="70a96-3006">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="70a96-3007">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="70a96-3007">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="70a96-3008">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="70a96-3008">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="70a96-3009">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3009">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-3010">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-3010">Storage</span></span>

* <span data-ttu-id="70a96-3011">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="70a96-3011">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="70a96-3012">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="70a96-3012">Eventgrid</span></span>

* <span data-ttu-id="70a96-3013">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="70a96-3013">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-3014">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-3014">SQL</span></span>

* <span data-ttu-id="70a96-3015">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="70a96-3015">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="70a96-3016">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="70a96-3016">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="70a96-3017">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="70a96-3017">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="70a96-3018">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70a96-3018">Keyvault</span></span>

* <span data-ttu-id="70a96-3019">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="70a96-3019">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-3020">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-3020">VM</span></span>

* <span data-ttu-id="70a96-3021">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="70a96-3021">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="70a96-3022">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="70a96-3022">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="70a96-3023">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="70a96-3023">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="70a96-3024">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="70a96-3024">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="70a96-3025">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="70a96-3025">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="70a96-3026">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="70a96-3026">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-3027">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-3027">ACS</span></span>

* <span data-ttu-id="70a96-3028">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="70a96-3028">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-3029">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-3029">Appservice</span></span>

* <span data-ttu-id="70a96-3030">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="70a96-3030">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="70a96-3031">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="70a96-3031">Backup</span></span>

* <span data-ttu-id="70a96-3032">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="70a96-3032">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="70a96-3033">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-3033">September 11, 2017</span></span>

<span data-ttu-id="70a96-3034">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="70a96-3034">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="70a96-3035">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-3035">Core</span></span>

* <span data-ttu-id="70a96-3036">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="70a96-3036">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="70a96-3037">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="70a96-3037">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-3038">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-3038">Acs</span></span>

* <span data-ttu-id="70a96-3039">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3039">Added `acs list-locations` command</span></span>
* <span data-ttu-id="70a96-3040">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-3040">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-3041">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-3041">Appservice</span></span>

* <span data-ttu-id="70a96-3042">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="70a96-3042">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="70a96-3043">CDN</span><span class="sxs-lookup"><span data-stu-id="70a96-3043">CDN</span></span>

* <span data-ttu-id="70a96-3044">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3044">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="70a96-3045">Расширение</span><span class="sxs-lookup"><span data-stu-id="70a96-3045">Extension</span></span>

* <span data-ttu-id="70a96-3046">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="70a96-3046">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="70a96-3047">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70a96-3047">Keyvault</span></span>

* <span data-ttu-id="70a96-3048">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3048">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="70a96-3049">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-3049">Network</span></span>

* <span data-ttu-id="70a96-3050">Переименование `vnet list-private-access-services` в `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="70a96-3050">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="70a96-3051">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3051">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="70a96-3052">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3052">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="70a96-3053">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3053">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="70a96-3054">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3054">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-3055">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-3055">Resource</span></span>

* <span data-ttu-id="70a96-3056">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3056">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="70a96-3057">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3057">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="70a96-3058">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="70a96-3058">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="70a96-3059">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="70a96-3059">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-3060">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-3060">SQL</span></span>

* <span data-ttu-id="70a96-3061">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3061">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-3062">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-3062">VM</span></span>

* <span data-ttu-id="70a96-3063">Исправлено: Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="70a96-3063">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="70a96-3064">Исправлено: Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="70a96-3064">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="70a96-3065">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3065">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="70a96-3066">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="70a96-3066">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="70a96-3067">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="70a96-3067">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="70a96-3068">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-3068">August 31, 2017</span></span>

<span data-ttu-id="70a96-3069">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="70a96-3069">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="70a96-3070">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70a96-3070">Keyvault</span></span>

* <span data-ttu-id="70a96-3071">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3071">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="70a96-3072">Sf</span><span class="sxs-lookup"><span data-stu-id="70a96-3072">Sf</span></span>

* <span data-ttu-id="70a96-3073">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="70a96-3073">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-3074">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-3074">Storage</span></span>

* <span data-ttu-id="70a96-3075">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="70a96-3075">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="70a96-3076">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="70a96-3076">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="70a96-3077">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-3077">August 28, 2017</span></span>

<span data-ttu-id="70a96-3078">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="70a96-3078">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="70a96-3079">CLI</span><span class="sxs-lookup"><span data-stu-id="70a96-3079">CLI</span></span>

* <span data-ttu-id="70a96-3080">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="70a96-3080">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-3081">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-3081">ACS</span></span>

* <span data-ttu-id="70a96-3082">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="70a96-3082">Corrected preview regions</span></span>
* <span data-ttu-id="70a96-3083">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3083">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="70a96-3084">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="70a96-3084">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-3085">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-3085">Appservice</span></span>

* <span data-ttu-id="70a96-3086">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3086">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="70a96-3087">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3087">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="70a96-3088">Предоставлен параметр `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3088">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="70a96-3089">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="70a96-3089">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="70a96-3090">Исправлено: Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="70a96-3090">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="70a96-3091">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-3091">IoT</span></span>

* <span data-ttu-id="70a96-3092">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="70a96-3092">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="70a96-3093">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-3093">Network</span></span>

* <span data-ttu-id="70a96-3094">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3094">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="70a96-3095">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3095">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="70a96-3096">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3096">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="70a96-3097">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3097">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="70a96-3098">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3098">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="70a96-3099">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-3099">Profile</span></span>

* <span data-ttu-id="70a96-3100">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="70a96-3100">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="70a96-3101">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="70a96-3101">Service Fabric</span></span>

* <span data-ttu-id="70a96-3102">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="70a96-3102">Preview release</span></span>
* <span data-ttu-id="70a96-3103">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="70a96-3103">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="70a96-3104">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="70a96-3104">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="70a96-3105">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3105">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-3106">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-3106">Storage</span></span>

* <span data-ttu-id="70a96-3107">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="70a96-3107">Enabled setting blob tier</span></span>
* <span data-ttu-id="70a96-3108">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="70a96-3108">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="70a96-3109">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3109">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="70a96-3110">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="70a96-3110">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="70a96-3111">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3111">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="70a96-3112">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3112">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-3113">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-3113">VM</span></span>

* <span data-ttu-id="70a96-3114">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3114">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="70a96-3115">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3115">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="70a96-3116">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="70a96-3116">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="70a96-3117">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="70a96-3117">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="70a96-3118">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="70a96-3118">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="70a96-3119">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3119">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="70a96-3120">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-3120">August 15, 2017</span></span>

<span data-ttu-id="70a96-3121">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="70a96-3121">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-3122">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-3122">ACS</span></span>

* <span data-ttu-id="70a96-3123">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="70a96-3123">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-3124">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-3124">Appservice</span></span>

* <span data-ttu-id="70a96-3125">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="70a96-3125">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="70a96-3126">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-3126">Event Grid</span></span>

* <span data-ttu-id="70a96-3127">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="70a96-3127">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="70a96-3128">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-3128">August 11, 2017</span></span>

<span data-ttu-id="70a96-3129">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="70a96-3129">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-3130">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-3130">ACS</span></span>

* <span data-ttu-id="70a96-3131">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="70a96-3131">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="70a96-3132">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-3132">Batch</span></span>

* <span data-ttu-id="70a96-3133">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="70a96-3133">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="70a96-3134">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="70a96-3134">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="70a96-3135">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70a96-3135">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="70a96-3136">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="70a96-3136">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="70a96-3137">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="70a96-3137">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="70a96-3138">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="70a96-3138">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="70a96-3139">Компонент</span><span class="sxs-lookup"><span data-stu-id="70a96-3139">Component</span></span>

* <span data-ttu-id="70a96-3140">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="70a96-3140">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="70a96-3141">Контейнер</span><span class="sxs-lookup"><span data-stu-id="70a96-3141">Container</span></span>

* <span data-ttu-id="70a96-3142">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="70a96-3142">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="70a96-3143">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="70a96-3143">Data Lake Store</span></span>

* <span data-ttu-id="70a96-3144">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="70a96-3144">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="70a96-3145">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-3145">Event Grid</span></span>

* <span data-ttu-id="70a96-3146">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="70a96-3146">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="70a96-3147">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-3147">Network</span></span>

* <span data-ttu-id="70a96-3148">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="70a96-3148">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="70a96-3149">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3149">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="70a96-3150">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3150">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="70a96-3151">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3151">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="70a96-3152">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-3152">Profile</span></span>

* <span data-ttu-id="70a96-3153">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="70a96-3153">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-3154">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-3154">Storage</span></span>

* <span data-ttu-id="70a96-3155">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="70a96-3155">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-3156">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-3156">VM</span></span>

* <span data-ttu-id="70a96-3157">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="70a96-3157">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="70a96-3158">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3158">Exposed `list-skus` command</span></span>
* <span data-ttu-id="70a96-3159">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="70a96-3159">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="70a96-3160">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="70a96-3160">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="70a96-3161">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="70a96-3161">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="70a96-3162">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-3162">July 28, 2017</span></span>

<span data-ttu-id="70a96-3163">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="70a96-3163">Version 2.0.12</span></span>

* <span data-ttu-id="70a96-3164">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="70a96-3164">Added container commands</span></span>
* <span data-ttu-id="70a96-3165">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="70a96-3165">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="70a96-3166">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-3166">Core</span></span>

* <span data-ttu-id="70a96-3167">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="70a96-3167">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="70a96-3168">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="70a96-3168">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="70a96-3169">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="70a96-3169">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="70a96-3170">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="70a96-3170">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="70a96-3171">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="70a96-3171">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="70a96-3172">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="70a96-3172">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="70a96-3173">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="70a96-3173">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="70a96-3174">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="70a96-3174">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="70a96-3175">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="70a96-3175">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="70a96-3176">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="70a96-3176">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="70a96-3177">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="70a96-3177">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="70a96-3178">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="70a96-3178">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="70a96-3179">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="70a96-3179">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="70a96-3180">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="70a96-3180">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="70a96-3181">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="70a96-3181">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="70a96-3182">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="70a96-3182">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="70a96-3183">ACR</span><span class="sxs-lookup"><span data-stu-id="70a96-3183">ACR</span></span>

* <span data-ttu-id="70a96-3184">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="70a96-3184">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="70a96-3185">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="70a96-3185">Support SKU update for managed registries</span></span>
* <span data-ttu-id="70a96-3186">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="70a96-3186">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="70a96-3187">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="70a96-3187">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="70a96-3188">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="70a96-3188">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="70a96-3189">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="70a96-3189">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-3190">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-3190">ACS</span></span>

* <span data-ttu-id="70a96-3191">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="70a96-3191">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-3192">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="70a96-3192">Appservice</span></span>

* <span data-ttu-id="70a96-3193">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="70a96-3193">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="70a96-3194">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="70a96-3194">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="70a96-3195">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3195">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="70a96-3196">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="70a96-3196">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="70a96-3197">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="70a96-3197">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="70a96-3198">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="70a96-3198">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="70a96-3199">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="70a96-3199">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="70a96-3200">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="70a96-3200">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="70a96-3201">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="70a96-3201">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="70a96-3202">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3202">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="70a96-3203">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="70a96-3203">Batch</span></span>

* <span data-ttu-id="70a96-3204">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="70a96-3204">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="70a96-3205">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3205">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="70a96-3206">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3206">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="70a96-3207">CDN</span><span class="sxs-lookup"><span data-stu-id="70a96-3207">CDN</span></span>

* <span data-ttu-id="70a96-3208">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="70a96-3208">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="70a96-3209">Cloud</span><span class="sxs-lookup"><span data-stu-id="70a96-3209">Cloud</span></span>

* <span data-ttu-id="70a96-3210">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="70a96-3210">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="70a96-3211">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="70a96-3211">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="70a96-3212">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="70a96-3212">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="70a96-3213">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="70a96-3213">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="70a96-3214">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3214">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="70a96-3215">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70a96-3215">CosmosDB</span></span>

* <span data-ttu-id="70a96-3216">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="70a96-3216">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="70a96-3217">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="70a96-3217">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="70a96-3218">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="70a96-3218">Data Lake Analytics</span></span>

* <span data-ttu-id="70a96-3219">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3219">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="70a96-3220">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3220">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="70a96-3221">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3221">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="70a96-3222">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="70a96-3222">Data Lake Store</span></span>

* <span data-ttu-id="70a96-3223">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3223">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="70a96-3224">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="70a96-3224">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="70a96-3225">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3225">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="70a96-3226">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="70a96-3226">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="70a96-3227">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="70a96-3227">Interactive</span></span>

* <span data-ttu-id="70a96-3228">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="70a96-3228">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="70a96-3229">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="70a96-3229">Increased test coverage</span></span>
* <span data-ttu-id="70a96-3230">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="70a96-3230">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="70a96-3231">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="70a96-3231">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="70a96-3232">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="70a96-3232">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="70a96-3233">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="70a96-3233">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="70a96-3234">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="70a96-3234">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="70a96-3235">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3235">Added `--progress` flag</span></span>
* <span data-ttu-id="70a96-3236">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3236">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="70a96-3237">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="70a96-3237">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="70a96-3238">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="70a96-3238">IoT</span></span>

* <span data-ttu-id="70a96-3239">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="70a96-3239">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="70a96-3240">(3934).</span><span class="sxs-lookup"><span data-stu-id="70a96-3240">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="70a96-3241">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70a96-3241">Key vault</span></span>

* <span data-ttu-id="70a96-3242">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="70a96-3242">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="70a96-3243">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3243">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="70a96-3244">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="70a96-3244">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="70a96-3245">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3245">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="70a96-3246">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3246">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="70a96-3247">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="70a96-3247">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="70a96-3248">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="70a96-3248">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="70a96-3249">(3307).</span><span class="sxs-lookup"><span data-stu-id="70a96-3249">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="70a96-3250">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="70a96-3250">Lab</span></span>

* <span data-ttu-id="70a96-3251">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3251">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="70a96-3252">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3252">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-3253">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-3253">Monitor</span></span>

* <span data-ttu-id="70a96-3254">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="70a96-3254">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="70a96-3255">Переименование `monitor alert-rule-incidents list` в `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="70a96-3255">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="70a96-3256">Переименование `monitor alert-rule-incidents show` в `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="70a96-3256">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="70a96-3257">Переименование `monitor metric-defintions list` в `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="70a96-3257">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="70a96-3258">Переименование `monitor alert-rules` в `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="70a96-3258">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="70a96-3259">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="70a96-3259">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="70a96-3260">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="70a96-3260">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="70a96-3261">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="70a96-3261">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="70a96-3262">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="70a96-3262">`location` no longer required</span></span>
  * <span data-ttu-id="70a96-3263">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="70a96-3263">Add name and ID support for target</span></span>
  * <span data-ttu-id="70a96-3264">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="70a96-3264">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="70a96-3265">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="70a96-3265">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="70a96-3266">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="70a96-3266">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="70a96-3267">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="70a96-3267">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="70a96-3268">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3268">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="70a96-3269">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3269">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="70a96-3270">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-3270">Network</span></span>

* <span data-ttu-id="70a96-3271">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3271">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="70a96-3272">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3272">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="70a96-3273">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="70a96-3273">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="70a96-3274">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3274">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="70a96-3275">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3275">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="70a96-3276">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3276">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="70a96-3277">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3277">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="70a96-3278">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3278">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="70a96-3279">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3279">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="70a96-3280">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3280">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="70a96-3281">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3281">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="70a96-3282">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3282">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="70a96-3283">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3283">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="70a96-3284">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3284">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="70a96-3285">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3285">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="70a96-3286">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3286">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="70a96-3287">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="70a96-3287">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="70a96-3288">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3288">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="70a96-3289">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3289">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="70a96-3290">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3290">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="70a96-3291">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3291">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="70a96-3292">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3292">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="70a96-3293">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3293">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="70a96-3294">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="70a96-3294">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="70a96-3295">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="70a96-3295">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="70a96-3296">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="70a96-3296">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="70a96-3297">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="70a96-3297">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="70a96-3298">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-3298">Profile</span></span>

* <span data-ttu-id="70a96-3299">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="70a96-3299">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="70a96-3300">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="70a96-3300">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="70a96-3301">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="70a96-3301">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="70a96-3302">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="70a96-3302">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="70a96-3303">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="70a96-3303">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="70a96-3304">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="70a96-3304">RDBMS</span></span>

* <span data-ttu-id="70a96-3305">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="70a96-3305">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="70a96-3306">Исправлена проблема с обработкой `%s` из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="70a96-3306">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="70a96-3307">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="70a96-3307">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="70a96-3308">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="70a96-3308">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-3309">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-3309">Resource</span></span>

* <span data-ttu-id="70a96-3310">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3310">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="70a96-3311">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3311">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="70a96-3312">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3312">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="70a96-3313">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3313">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="70a96-3314">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="70a96-3314">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="70a96-3315">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3315">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="70a96-3316">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="70a96-3316">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="70a96-3317">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3317">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="70a96-3318">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-3318">Role</span></span>

* <span data-ttu-id="70a96-3319">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="70a96-3319">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="70a96-3320">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="70a96-3320">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="70a96-3321">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="70a96-3321">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="70a96-3322">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="70a96-3322">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="70a96-3323">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3323">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="70a96-3324">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="70a96-3324">Service Fabric</span></span>
* <span data-ttu-id="70a96-3325">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="70a96-3325">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="70a96-3326">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="70a96-3326">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="70a96-3327">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="70a96-3327">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-3328">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-3328">SQL</span></span>

* <span data-ttu-id="70a96-3329">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3329">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="70a96-3330">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3330">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="70a96-3331">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3331">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-3332">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-3332">Storage</span></span>

* <span data-ttu-id="70a96-3333">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="70a96-3333">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="70a96-3334">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="70a96-3334">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="70a96-3335">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="70a96-3335">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="70a96-3336">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="70a96-3336">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="70a96-3337">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="70a96-3337">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="70a96-3338">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="70a96-3338">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-3339">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-3339">VM</span></span>

* <span data-ttu-id="70a96-3340">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="70a96-3340">Support configuring nsg</span></span>
* <span data-ttu-id="70a96-3341">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="70a96-3341">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="70a96-3342">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="70a96-3342">Support managed service identities</span></span>
* <span data-ttu-id="70a96-3343">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3343">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="70a96-3344">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="70a96-3344">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="70a96-3345">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-3345">May 10, 2017</span></span>

<span data-ttu-id="70a96-3346">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="70a96-3346">Version 2.0.6</span></span>

* <span data-ttu-id="70a96-3347">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="70a96-3347">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="70a96-3348">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="70a96-3348">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="70a96-3349">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="70a96-3349">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="70a96-3350">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="70a96-3350">Include Cognitive Services module</span></span>
* <span data-ttu-id="70a96-3351">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="70a96-3351">Include Service Fabric module</span></span>
* <span data-ttu-id="70a96-3352">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="70a96-3352">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="70a96-3353">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="70a96-3353">Add support for CDN commands</span></span>
* <span data-ttu-id="70a96-3354">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="70a96-3354">Remove Container module</span></span>
* <span data-ttu-id="70a96-3355">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3355">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="70a96-3356">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3356">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="70a96-3357">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-3357">Core</span></span>

* <span data-ttu-id="70a96-3358">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="70a96-3358">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="70a96-3359">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([#2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3359">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="70a96-3360">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3360">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="70a96-3361">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3361">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="70a96-3362">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3362">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="70a96-3363">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3363">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="70a96-3364">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3364">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="70a96-3365">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3365">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="70a96-3366">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3366">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="70a96-3367">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="70a96-3367">core: Improved performance</span></span>
* <span data-ttu-id="70a96-3368">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="70a96-3368">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="70a96-3369">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="70a96-3369">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-3370">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-3370">ACS</span></span>

* <span data-ttu-id="70a96-3371">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="70a96-3371">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="70a96-3372">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="70a96-3372">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="70a96-3373">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="70a96-3373">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="70a96-3374">Удален профиль Windows перед вызовом метода PUT для команды scale ([#2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3374">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-3375">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-3375">AppService</span></span>

* <span data-ttu-id="70a96-3376">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="70a96-3376">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="70a96-3377">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="70a96-3377">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="70a96-3378">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="70a96-3378">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="70a96-3379">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="70a96-3379">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="70a96-3380">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="70a96-3380">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="70a96-3381">Включена поддержка настройки строк подключения ([#2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3381">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="70a96-3382">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="70a96-3382">support slot swap with preview</span></span>
* <span data-ttu-id="70a96-3383">Устранены ошибки из команд службы приложений ([#2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3383">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="70a96-3384">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([#2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3384">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="70a96-3385">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="70a96-3385">CosmosDB</span></span>

* <span data-ttu-id="70a96-3386">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="70a96-3386">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="70a96-3387">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="70a96-3387">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="70a96-3388">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="70a96-3388">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="70a96-3389">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="70a96-3389">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="70a96-3390">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="70a96-3390">Data Lake Analytics</span></span>

* <span data-ttu-id="70a96-3391">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="70a96-3391">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="70a96-3392">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="70a96-3392">Add support for new catalog item type: package.</span></span> <span data-ttu-id="70a96-3393">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3393">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="70a96-3394">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="70a96-3394">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="70a96-3395">Таблица</span><span class="sxs-lookup"><span data-stu-id="70a96-3395">Table</span></span>
  * <span data-ttu-id="70a96-3396">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="70a96-3396">Table valued function</span></span>
  * <span data-ttu-id="70a96-3397">Представление</span><span class="sxs-lookup"><span data-stu-id="70a96-3397">View</span></span>
  * <span data-ttu-id="70a96-3398">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="70a96-3398">Table Statistics.</span></span> <span data-ttu-id="70a96-3399">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="70a96-3399">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="70a96-3400">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="70a96-3400">Data Lake Store</span></span>

* <span data-ttu-id="70a96-3401">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="70a96-3401">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="70a96-3402">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3402">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="70a96-3403">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="70a96-3403">missed help for access show.</span></span> <span data-ttu-id="70a96-3404">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="70a96-3404">adding it.</span></span> <span data-ttu-id="70a96-3405">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="70a96-3405">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="70a96-3406">Поиск</span><span class="sxs-lookup"><span data-stu-id="70a96-3406">Find</span></span>

* <span data-ttu-id="70a96-3407">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="70a96-3407">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="70a96-3408">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="70a96-3408">KeyVault</span></span>

* <span data-ttu-id="70a96-3409">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="70a96-3409">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="70a96-3410">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="70a96-3410">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="70a96-3411">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="70a96-3411">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="70a96-3412">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="70a96-3412">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="70a96-3413">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3413">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="70a96-3414">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="70a96-3414">Lab</span></span>

* <span data-ttu-id="70a96-3415">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="70a96-3415">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="70a96-3416">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="70a96-3416">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="70a96-3417">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="70a96-3417">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="70a96-3418">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="70a96-3418">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="70a96-3419">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="70a96-3419">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="70a96-3420">Монитор</span><span class="sxs-lookup"><span data-stu-id="70a96-3420">Monitor</span></span>

* <span data-ttu-id="70a96-3421">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3421">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="70a96-3422">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3422">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="70a96-3423">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-3423">Network</span></span>

* <span data-ttu-id="70a96-3424">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3424">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="70a96-3425">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3425">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="70a96-3426">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="70a96-3426">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="70a96-3427">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="70a96-3427">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="70a96-3428">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="70a96-3428">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="70a96-3429">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="70a96-3429">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="70a96-3430">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="70a96-3430">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="70a96-3431">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="70a96-3431">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="70a96-3432">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3432">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="70a96-3433">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="70a96-3433">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="70a96-3434">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3434">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="70a96-3435">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3435">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="70a96-3436">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="70a96-3436">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="70a96-3437">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="70a96-3437">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="70a96-3438">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="70a96-3438">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="70a96-3439">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="70a96-3439">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="70a96-3440">Профиль</span><span class="sxs-lookup"><span data-stu-id="70a96-3440">Profile</span></span>

* <span data-ttu-id="70a96-3441">Включена поддержка входа при отсутствии подписок ([#2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3441">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="70a96-3442">Включена поддержка сокращенных имен параметров в команде az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3442">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="70a96-3443">Redis</span><span class="sxs-lookup"><span data-stu-id="70a96-3443">Redis</span></span>

* <span data-ttu-id="70a96-3444">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="70a96-3444">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="70a96-3445">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="70a96-3445">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="70a96-3446">Ресурс</span><span class="sxs-lookup"><span data-stu-id="70a96-3446">Resource</span></span>

* <span data-ttu-id="70a96-3447">Добавлены команды определения managedapp и managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3447">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="70a96-3448">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3448">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="70a96-3449">Включена поддержка создания универсального ресурса ([#2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3449">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="70a96-3450">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="70a96-3450">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="70a96-3451">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="70a96-3451">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="70a96-3452">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="70a96-3452">Add docs for az lock update.</span></span> <span data-ttu-id="70a96-3453">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="70a96-3453">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="70a96-3454">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="70a96-3454">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="70a96-3455">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="70a96-3455">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="70a96-3456">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="70a96-3456">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="70a96-3457">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="70a96-3457">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="70a96-3458">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([#2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3458">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="70a96-3459">Роль</span><span class="sxs-lookup"><span data-stu-id="70a96-3459">Role</span></span>

* <span data-ttu-id="70a96-3460">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([#2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3460">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="70a96-3461">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3461">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="70a96-3462">Роль: устранены проблемы при обновлении определения роли ([#2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3462">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="70a96-3463">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="70a96-3463">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="70a96-3464">SQL</span><span class="sxs-lookup"><span data-stu-id="70a96-3464">SQL</span></span>

* <span data-ttu-id="70a96-3465">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="70a96-3465">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="70a96-3466">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3466">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="70a96-3467">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-3467">Storage</span></span>

* <span data-ttu-id="70a96-3468">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3468">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="70a96-3469">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="70a96-3469">Add support for incremental blob copy</span></span>
* <span data-ttu-id="70a96-3470">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="70a96-3470">Add support for large block blob upload</span></span>
* <span data-ttu-id="70a96-3471">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="70a96-3471">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-3472">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-3472">VM</span></span>

* <span data-ttu-id="70a96-3473">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="70a96-3473">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="70a96-3474">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="70a96-3474">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="70a96-3475">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="70a96-3475">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="70a96-3476">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="70a96-3476">az vm/vmss disk</span></span>
  3. <span data-ttu-id="70a96-3477">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="70a96-3477">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="70a96-3478">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="70a96-3478">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="70a96-3479">vm/vmss: добавлена поддержка создания из образа Marketplace, для которого требуются сведения о плане ([#1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3479">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="70a96-3480">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-3480">April 3, 2017</span></span>

<span data-ttu-id="70a96-3481">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="70a96-3481">Version 2.0.2</span></span>

<span data-ttu-id="70a96-3482">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="70a96-3482">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="70a96-3483">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="70a96-3483">Core</span></span>

* <span data-ttu-id="70a96-3484">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-3484">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="70a96-3485">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3485">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="70a96-3486">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3486">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="70a96-3487">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3487">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="70a96-3488">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3488">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="70a96-3489">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="70a96-3489">Add prompting for missing template parameters.</span></span> <span data-ttu-id="70a96-3490">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3490">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="70a96-3491">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="70a96-3491">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="70a96-3492">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="70a96-3492">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="70a96-3493">ACS</span><span class="sxs-lookup"><span data-stu-id="70a96-3493">ACS</span></span>

* <span data-ttu-id="70a96-3494">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3494">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="70a96-3495">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="70a96-3495">Add support for ssh key password prompting.</span></span> <span data-ttu-id="70a96-3496">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3496">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="70a96-3497">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="70a96-3497">Add support for windows clusters.</span></span> <span data-ttu-id="70a96-3498">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3498">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="70a96-3499">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="70a96-3499">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="70a96-3500">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3500">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="70a96-3501">AppService</span><span class="sxs-lookup"><span data-stu-id="70a96-3501">AppService</span></span>

* <span data-ttu-id="70a96-3502">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3502">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="70a96-3503">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3503">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="70a96-3504">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3504">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="70a96-3505">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3505">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="70a96-3506">Data Lake</span><span class="sxs-lookup"><span data-stu-id="70a96-3506">DataLake</span></span>

* <span data-ttu-id="70a96-3507">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="70a96-3507">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="70a96-3508">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="70a96-3508">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="70a96-3509">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="70a96-3509">DocuemntDB</span></span>

* <span data-ttu-id="70a96-3510">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3510">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="70a96-3511">ВМ</span><span class="sxs-lookup"><span data-stu-id="70a96-3511">VM</span></span>

* <span data-ttu-id="70a96-3512">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3512">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="70a96-3513">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3513">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="70a96-3514">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3514">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="70a96-3515">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3515">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="70a96-3516">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3516">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="70a96-3517">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3517">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="70a96-3518">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="70a96-3518">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="70a96-3519">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="70a96-3519">February 27, 2017</span></span>

<span data-ttu-id="70a96-3520">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="70a96-3520">Version 2.0.0</span></span>

<span data-ttu-id="70a96-3521">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="70a96-3521">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="70a96-3522">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="70a96-3522">Container Service (acs)</span></span>
- <span data-ttu-id="70a96-3523">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="70a96-3523">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="70a96-3524">Сеть</span><span class="sxs-lookup"><span data-stu-id="70a96-3524">Networking</span></span>
- <span data-ttu-id="70a96-3525">Память</span><span class="sxs-lookup"><span data-stu-id="70a96-3525">Storage</span></span>

<span data-ttu-id="70a96-3526">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3526">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="70a96-3527">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="70a96-3527">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="70a96-3528">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="70a96-3528">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="70a96-3529">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="70a96-3529">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="70a96-3530">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="70a96-3530">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="70a96-3531">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="70a96-3531">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="70a96-3532">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="70a96-3532">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="70a96-3533">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="70a96-3533">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="70a96-3534">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="70a96-3534">Provide feedback from the command line with the `az feedback` command</span></span>
