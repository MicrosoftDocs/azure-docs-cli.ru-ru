---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 04/28/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 032039cc5a51f0d158fbd3616a30263df139f53b
ms.sourcegitcommit: 1e5d8f04091803d68ac6833d2e2af37a863486ac
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "82199399"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="2b0ed-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="2b0ed-103">Azure CLI release notes</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="2b0ed-104">28 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-104">April 28, 2020</span></span>

<span data-ttu-id="2b0ed-105">Версия 2.5.0</span><span class="sxs-lookup"><span data-stu-id="2b0ed-105">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-106">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-106">ACS</span></span>

* <span data-ttu-id="2b0ed-107">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az openshift create: удален параметр --vnet-peer.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-107">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="2b0ed-108">`az openshift create`: добавлены флаги для поддержки частного кластера.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-108">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="2b0ed-109">`az openshift`: обновление до версии API `2019-10-27-preview`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-109">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="2b0ed-110">`az openshift`: добавлена команда `update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-110">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="2b0ed-111">AKS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-111">AKS</span></span>

* <span data-ttu-id="2b0ed-112">`az aks create`: включена поддержка Windows.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-112">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-113">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-113">AppService</span></span>

* <span data-ttu-id="2b0ed-114">`az webapp deployment source config-zip`: удалена функция перевода в спящий режим после выполнения request.get().</span><span class="sxs-lookup"><span data-stu-id="2b0ed-114">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="2b0ed-115">ARM</span><span class="sxs-lookup"><span data-stu-id="2b0ed-115">ARM</span></span>

* <span data-ttu-id="2b0ed-116">Добавлены команды What-If развертывания шаблона.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-116">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="2b0ed-117">ARO</span><span class="sxs-lookup"><span data-stu-id="2b0ed-117">ARO</span></span>

* <span data-ttu-id="2b0ed-118">`az aro`: исправлены выходные данные таблицы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-118">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="2b0ed-119">CI</span><span class="sxs-lookup"><span data-stu-id="2b0ed-119">CI</span></span>

* <span data-ttu-id="2b0ed-120">Включена поддержка PyTest и прекращена поддержка Nose для автотестов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-120">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="2b0ed-121">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-121">Compute</span></span>

* <span data-ttu-id="2b0ed-122">`az vmss disk detach`: устранена проблема с NoneType для диска данных.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-122">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="2b0ed-123">`az vm availability-set list`: включена поддержка отображения списка виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-123">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="2b0ed-124">`az vm list-skus`: исправлена проблема с отображением формата таблицы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-124">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="2b0ed-125">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-125">KeyVault</span></span>

* <span data-ttu-id="2b0ed-126">Добавлен новый параметр `--enable-rbac-authorization` для использования во время создания или обновления.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-126">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-127">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-127">Monitor</span></span>

* <span data-ttu-id="2b0ed-128">Включена поддержка компонентов CMK в кластере LA.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-128">Support LA cluster CMK features</span></span>
* <span data-ttu-id="2b0ed-129">`az monitor log-analytics workspace linked-storage`: включена поддержка функций BYOS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-129">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-130">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-130">Network</span></span>

* <span data-ttu-id="2b0ed-131">`az network security-partner`: включена поддержка поставщика партнера по безопасности.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-131">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="2b0ed-132">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-132">Privatedns</span></span>

* <span data-ttu-id="2b0ed-133">Добавлена функция в частной зоне DNS для импорта и экспорта файла зоны.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-133">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="2b0ed-134">21 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-134">April 21, 2020</span></span>

<span data-ttu-id="2b0ed-135">Версия 2.4.0</span><span class="sxs-lookup"><span data-stu-id="2b0ed-135">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-136">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-136">ACR</span></span>

* <span data-ttu-id="2b0ed-137">`az acr run --cmd`: отключает переопределение рабочего каталога.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-137">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="2b0ed-138">Включена поддержка выделенной конечной точки данных.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-138">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="2b0ed-139">AKS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-139">AKS</span></span>

* <span data-ttu-id="2b0ed-140">`az aks list -o table` теперь показывает privateFqdn как FQDN для частных кластеров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-140">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="2b0ed-141">Добавлен параметр --uptime-sla.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-141">Add --uptime-sla</span></span>
* <span data-ttu-id="2b0ed-142">Обновлен пакет containerservice.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-142">Update containerservice package</span></span>
* <span data-ttu-id="2b0ed-143">Включена поддержка общедоступных IP-адресов узлов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-143">Add node public IP support</span></span>
* <span data-ttu-id="2b0ed-144">Исправлена опечатка в команде справки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-144">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="2b0ed-145">AppConfig</span><span class="sxs-lookup"><span data-stu-id="2b0ed-145">AppConfig</span></span>

* <span data-ttu-id="2b0ed-146">Разрешена ссылка на хранилище ключей для команд kv list и export.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-146">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="2b0ed-147">Исправлена ошибка при отображении значений ключей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-147">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-148">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-148">AppService</span></span>

* <span data-ttu-id="2b0ed-149">`az functionapp create`: изменен способ настройки linuxFxVersion для приложений-функций dotnet в Linux.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-149">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="2b0ed-150">Это должно исправить ошибку, препятствующую созданию приложений dotnet для использования в Linux.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-150">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="2b0ed-151">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az webapp create` Исправлена ошибка для сохранения существующих параметров AppSettings с помощью az webapp create.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-151">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="2b0ed-152">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az webapp up` Исправлена ошибка для создания группы ресурсов для команды az webapp up при использовании флага -g.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-152">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="2b0ed-153">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az webapp config` Исправлена ошибка для отображения значений для выходных данных не в формате JSON с помощью команды az webapp config connection-string list.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-153">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="2b0ed-154">ARM</span><span class="sxs-lookup"><span data-stu-id="2b0ed-154">ARM</span></span>

* <span data-ttu-id="2b0ed-155">`az deployment create/validate`: добавлен параметр `--no-prompt` для пропуска запроса отсутствующих параметров для шаблона ARM.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-155">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="2b0ed-156">`az deployment group/mg/sub/tenant validate`: включена поддержка комментариев в файле параметров развертывания.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-156">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="2b0ed-157">`az deployment`: удалено значение `is_preview` для параметра `--handle-extended-json-format`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-157">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="2b0ed-158">`az deployment group/mg/sub/tenant cancel`: включена поддержка отмены развертывания для шаблона ARM.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-158">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="2b0ed-159">`az deployment group/mg/sub/tenant validate`: улучшено отображение сообщения об ошибке при сбое проверки развертывания.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-159">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="2b0ed-160">`az deployment-scripts`: добавлена новая команда для DeploymentScripts.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-160">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="2b0ed-161">`az resource tag`: добавлен параметр `--is-incremental` для инкрементного добавления тегов к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-161">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="2b0ed-162">ARO</span><span class="sxs-lookup"><span data-stu-id="2b0ed-162">ARO</span></span>

* <span data-ttu-id="2b0ed-163">`az aro`:  добавлен модуль команды aro Azure RedHat OpenShift версии 4.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-163">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="2b0ed-164">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-164">Batch</span></span>

* <span data-ttu-id="2b0ed-165">Обновлен API пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-165">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="2b0ed-166">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-166">Compute</span></span>

* <span data-ttu-id="2b0ed-167">`az sig image-version create`: добавлен тип учетной записи хранения Premium_LRS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-167">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="2b0ed-168">`az vmss update`: устранена проблема с обновлением уведомления о завершении.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-168">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="2b0ed-169">`az vm/vmss create`: включена поддержка версии специализированного образа.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-169">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="2b0ed-170">API SIG версии 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="2b0ed-170">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="2b0ed-171">`az sig image-version create`: добавлен параметр --target-region-encryption.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-171">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="2b0ed-172">Исправлена ошибка, из-за которой тесты завершались сбоем при последовательном выполнении из-за дублирования имени хранилища ключей в глобальном кэше в памяти.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-172">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2b0ed-173">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-173">CosmosDB</span></span>

* <span data-ttu-id="2b0ed-174">Включена поддержка `az cosmosdb private-link-resource/private-endpoint-connection`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-174">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="2b0ed-175">IoT Central</span><span class="sxs-lookup"><span data-stu-id="2b0ed-175">IoT Central</span></span>

* <span data-ttu-id="2b0ed-176">Прекращена поддержка `az iotcentral`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-176">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="2b0ed-177">Добавлен модуль команды `az iot central`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-177">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-178">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-178">Monitor</span></span>

* <span data-ttu-id="2b0ed-179">Включена поддержка сценария приватного канала для монитора.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-179">Support private link scenario for monitor</span></span>
* <span data-ttu-id="2b0ed-180">Исправлен неправильный способ имитации в test_monitor_general_operations.py.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-180">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-181">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-181">Network</span></span>

* <span data-ttu-id="2b0ed-182">Прекращена поддержка SKU для команды public ip update.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-182">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="2b0ed-183">`az network private-endpoint`: включена поддержка закрытой группы зон DNS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-183">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="2b0ed-184">Включена функция локального контекста для параметра vnet/subnet.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-184">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="2b0ed-185">Исправлен неправильный пример использования в test_nw_flow_log_delete.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-185">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="2b0ed-186">Упаковка</span><span class="sxs-lookup"><span data-stu-id="2b0ed-186">Packaging</span></span>

* <span data-ttu-id="2b0ed-187">Прекращена поддержка пакета Ubuntu/Disco.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-187">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="2b0ed-188">RBAC</span><span class="sxs-lookup"><span data-stu-id="2b0ed-188">RBAC</span></span>

* <span data-ttu-id="2b0ed-189">`az ad app create/update`: включена поддержка параметра --optional-claims.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-189">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="2b0ed-190">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="2b0ed-190">RDBMS</span></span>

* <span data-ttu-id="2b0ed-191">Добавлены команды администратора Azure Active Directory для PostgreSQL и MySQL.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-191">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="2b0ed-192">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="2b0ed-192">Service Fabric</span></span>

* <span data-ttu-id="2b0ed-193">Исправление 12891: `az sf application update --application-parameters` удаляет старые параметры, отсутствующие в запросе.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-193">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="2b0ed-194">Исправление 12470: включена поддержка az sf create cluster, исправлены ошибки, связанные с устойчивостью и надежностью обновления, поиск VMSS выполняется корректно в коде при указании имени типа узла.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-194">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-195">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-195">SQL</span></span>

* <span data-ttu-id="2b0ed-196">Добавлены команды `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-196">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="2b0ed-197">`az sql midb`: обновление и отображение политик долгосрочного хранения, отображение и удаление долгосрочных резервных копий, восстановление долгосрочных резервных копий.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-197">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-198">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-198">Storage</span></span>

* <span data-ttu-id="2b0ed-199">Обновлена версия azure-mgmt-storage до 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-199">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="2b0ed-200">`az storage logging off`: включено отключение ведения журналов для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-200">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="2b0ed-201">`az storage account update`: включена автоматическая смена ключа для CMK.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-201">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="2b0ed-202">`az storage account encryption-scope create/update/list/show`: включена настройка области шифрования.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-202">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="2b0ed-203">`az storage container create`: добавлены параметры --default-encryption-scope и --deny-encryption-scope-override для настройки области шифрования на уровне контейнера.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-203">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="2b0ed-204">Опрос</span><span class="sxs-lookup"><span data-stu-id="2b0ed-204">Survey</span></span>

* <span data-ttu-id="2b0ed-205">Добавлен параметр для отключения ссылки опроса.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-205">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="2b0ed-206">01 апреля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-206">April 01, 2020</span></span>

<span data-ttu-id="2b0ed-207">Версия 2.3.1</span><span class="sxs-lookup"><span data-stu-id="2b0ed-207">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-208">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-208">ACR</span></span>

* <span data-ttu-id="2b0ed-209">Исправлена неправильная версия azure-mgmt-containerregistry для Linux.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-209">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="2b0ed-210">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-210">Profile</span></span>

* <span data-ttu-id="2b0ed-211">az login: Исправлена ошибка входа в облачных профилях, отличающихся от `latest`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-211">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="2b0ed-212">31 марта 2020 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-212">March 31, 2020</span></span>

<span data-ttu-id="2b0ed-213">Версия 2.3.0</span><span class="sxs-lookup"><span data-stu-id="2b0ed-213">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-214">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-214">ACR</span></span>

* <span data-ttu-id="2b0ed-215">az acr task update: исключение пустого указателя.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-215">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="2b0ed-216">`az acr import`: Отредактировано справочное сообщение и сообщение об ошибке для уточнения того, как использовать параметры --source и --registry.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-216">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="2b0ed-217">Добавлено средство проверки для аргумента registry_name.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-217">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="2b0ed-218">`az acr login`: удален флаг предпросмотра для --expose-token.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-218">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="2b0ed-219">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр ветви az acr task create/update.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-219">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="2b0ed-220">Клиент az acr task update теперь может независимо обновлять контекст, токен GitHub и триггеры.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-220">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="2b0ed-221">az acr agentpool: новая функция.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-221">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="2b0ed-222">AKS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-222">AKS</span></span>

* <span data-ttu-id="2b0ed-223">Исправлена ошибка с apiServerAccessProfile при обновлении --api-server-authorized-ip-ranges.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-223">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="2b0ed-224">Обновление AKS: при обновлении исходящие IP-адреса переопределяются с помощью входных значений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-224">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="2b0ed-225">Не создаются имена субъектов-служб для кластеров MSI и реализована поддержка присоединение ACR к кластерам MSI.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-225">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="2b0ed-226">AMS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-226">AMS</span></span>

* <span data-ttu-id="2b0ed-227">Исправление 12469: не удается добавить content-key-policy для FairPlay из-за проблем с параметром ask.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-227">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="2b0ed-228">AppConfig</span><span class="sxs-lookup"><span data-stu-id="2b0ed-228">AppConfig</span></span>

* <span data-ttu-id="2b0ed-229">Добавлен параметр --skip-keyvault для экспорта kv.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-229">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-230">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-230">AppService</span></span>

* <span data-ttu-id="2b0ed-231">Исправление 12509: удален тег, добавлявшийся по умолчанию при создании приложения с помощью az webapp up.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-231">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="2b0ed-232">az functionapp create: обновлено меню справки для --runtime-version и добавлено предупреждение, когда пользователь указывает параметр --runtime-version для DotNet.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-232">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="2b0ed-233">az functionapp create: изменен способ установки JavaVersion для приложений-функций Windows.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-233">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="2b0ed-234">ARM</span><span class="sxs-lookup"><span data-stu-id="2b0ed-234">ARM</span></span>

* <span data-ttu-id="2b0ed-235">az deployment create/validate: по умолчанию используется параметр --handle-extended-json-format.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-235">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="2b0ed-236">az lock create: в справочную документацию добавлены примеры создания подресурсов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-236">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="2b0ed-237">Список az deployment {group/mg/sub/tenant}: реализована поддержка фильтрации ProvisioningState.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-237">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="2b0ed-238">az deployment: исправлена ошибка синтаксического анализа комментария в последнем аргументе.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-238">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="2b0ed-239">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="2b0ed-239">Backup</span></span>

* <span data-ttu-id="2b0ed-240">Добавлена возможность восстановления нескольких файлов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-240">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="2b0ed-241">Добавлена возможность резервного копирования только дисков с ОС.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-241">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="2b0ed-242">Добавлен параметр restore-as-unmanaged-disk, позволяющий задать неуправляемое восстановление.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-242">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="2b0ed-243">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-243">Compute</span></span>

* <span data-ttu-id="2b0ed-244">az vm create: для --nsg-rule добавлен вариант NONE.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-244">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="2b0ed-245">az vmss create/update: удален тег предпросмотра для автоматического восстановления VMSS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-245">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="2b0ed-246">az vm update: реализована поддержка --workspace.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-246">az vm update: Support --workspace</span></span>
* <span data-ttu-id="2b0ed-247">Исправлена ошибка в коде инициализации VirtualMachineScaleSetExtension.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-247">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="2b0ed-248">Версия VMAccessAgent обновлена до 2.4.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-248">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="2b0ed-249">az vmss set-orchestration-service-state: реализована поддержка состояния службы оркестрации наборов VMSS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-249">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="2b0ed-250">Версия API диска обновлена до 2019-11-01.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-250">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="2b0ed-251">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-251">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="2b0ed-252">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-252">Cosmos DB</span></span>

* <span data-ttu-id="2b0ed-253">Добавлен отсутствовавший параметр --type для перенаправления в связи с устареванием.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-253">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="2b0ed-254">Docker</span><span class="sxs-lookup"><span data-stu-id="2b0ed-254">Docker</span></span>

* <span data-ttu-id="2b0ed-255">Обновление до Alpine 3.11 и Python 3.6.10.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-255">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="2b0ed-256">Расширение</span><span class="sxs-lookup"><span data-stu-id="2b0ed-256">Extension</span></span>

* <span data-ttu-id="2b0ed-257">Добавлена возможность загрузки расширений в системный путь через пакеты.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-257">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="2b0ed-258">HDInsight</span><span class="sxs-lookup"><span data-stu-id="2b0ed-258">HDInsight</span></span>

* <span data-ttu-id="2b0ed-259">(az hdinsight create:) Добавлена возможность указания клиентами минимальной поддерживаемой версии TLS с помощью параметра `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-259">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="2b0ed-260">Допустимые значения: 1.0,1.1,1.2.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-260">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="2b0ed-261">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-261">IoT</span></span>

* <span data-ttu-id="2b0ed-262">Добавлен параметр codeowner.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-262">Add codeowner</span></span>
* <span data-ttu-id="2b0ed-263">az iot hub create: номер SKU по умолчанию изменен с F1 на S1.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-263">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="2b0ed-264">iot hub: реализована поддержка IotHub в профиле 2019-03-01-hybrid.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-264">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="2b0ed-265">IoT Central</span><span class="sxs-lookup"><span data-stu-id="2b0ed-265">IoTCentral</span></span>

* <span data-ttu-id="2b0ed-266">Обновлены сведения об ошибках, шаблон приложения по умолчанию и сообщение с подсказкой.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-266">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="2b0ed-267">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-267">KeyVault</span></span>

* <span data-ttu-id="2b0ed-268">Реализована поддержка резервного копирования и восстановления сертификатов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-268">Support certificate backup/restore</span></span>
* <span data-ttu-id="2b0ed-269">keyvault create/update: добавлена поддержка параметра --retention-days.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-269">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="2b0ed-270">При перечислении больше не показываются управляемые ключи и секреты.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-270">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="2b0ed-271">az keyvault create: реализована поддержка `--network-acls`, `--network-acls-ips` и `--network-acls-vnets` для указания сетевых правил при создании хранилища.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-271">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="2b0ed-272">Блокировка</span><span class="sxs-lookup"><span data-stu-id="2b0ed-272">Lock</span></span>

* <span data-ttu-id="2b0ed-273">Исправлена ошибка с командой az lock delete, не работавшей с Microsoft.DocumentDB.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-273">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-274">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-274">Monitor</span></span>

* <span data-ttu-id="2b0ed-275">az monitor clone: добавлена возможность клонирования правил метрики из одного ресурса в другой.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-275">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="2b0ed-276">Исправлена ошибка IcM179210086: не удается создать настраиваемое оповещение для метрики Application Insights.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-276">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="2b0ed-277">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="2b0ed-277">NetAppFiles</span></span>

* <span data-ttu-id="2b0ed-278">az volume create: для томов защиты данных добавлены операции репликации (approve, suspend, resume, status, remove).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-278">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-279">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-279">Network</span></span>

* <span data-ttu-id="2b0ed-280">az network application-gateway waf-policy managed-rule rule-set add: добавлена поддержка Microsoft_BotManagerRuleSet.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-280">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="2b0ed-281">Журнал потоков наблюдателя за сетями: исправлены неправильные сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-281">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="2b0ed-282">Добавлена поддержка имен узлов в прослушивателе шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-282">support host names in application gateway listener</span></span>
* <span data-ttu-id="2b0ed-283">az network nat gateway: добавлена возможность создания пустого ресурса без общедоступного IP-адреса или общедоступного IP-префикса.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-283">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="2b0ed-284">Добавлена возможность создания VPN-шлюза.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-284">Support vpn gateway generation</span></span>
* <span data-ttu-id="2b0ed-285">Реализована поддержка `--if-none-match` для `az network dns record-set {} add-record`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-285">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="2b0ed-286">Упаковка</span><span class="sxs-lookup"><span data-stu-id="2b0ed-286">Packaging</span></span>

* <span data-ttu-id="2b0ed-287">Прекращена поддержка Python 3.5.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-287">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="2b0ed-288">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-288">Profile</span></span>

* <span data-ttu-id="2b0ed-289">az login: добавлен показ предупреждений об ошибках MFA.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-289">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="2b0ed-290">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="2b0ed-290">RDBMS</span></span>

* <span data-ttu-id="2b0ed-291">Добавлены команды управления ключами шифрования данных сервера для PostgreSQL и MySQL.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-291">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="2b0ed-292">10 марта 2020 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-292">March 10, 2020</span></span>

<span data-ttu-id="2b0ed-293">Версия 2.2.0</span><span class="sxs-lookup"><span data-stu-id="2b0ed-293">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-294">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-294">ACR</span></span>

* <span data-ttu-id="2b0ed-295">Исправлена команда `az acr login`, которая неправильно вызывала ошибку.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-295">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="2b0ed-296">Добавлена новая команда `az acr helm install-cli`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-296">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="2b0ed-297">Добавлена частная ссылка и включена поддержка CMK.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-297">Add private link and CMK support</span></span>
* <span data-ttu-id="2b0ed-298">Добавлена команда private-link-resource list.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-298">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="2b0ed-299">AKS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-299">AKS</span></span>

* <span data-ttu-id="2b0ed-300">Исправлена функция поиска AKS в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-300">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="2b0ed-301">az aks: устранены ошибки NoneType при мониторинге надстроек и пула агентов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-301">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="2b0ed-302">Добавлен параметр --nodepool-tags в пуле узлов при создании кластера Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-302">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="2b0ed-303">Добавлен параметр --tags при добавлении пула узлов в кластер или его обновлении.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-303">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="2b0ed-304">aks create: добавлен параметр `--enable-private-cluster`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-304">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="2b0ed-305">Добавлен параметр --nodepool-labels в пуле узлов при создании кластера Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-305">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="2b0ed-306">Добавлен параметр --labels при добавлении нового пула узлов в кластер Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-306">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="2b0ed-307">Добавлен отсутствующий символ / в URL-адрес панели мониторинга.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-307">add missing / in the dashboard url</span></span>
* <span data-ttu-id="2b0ed-308">Включена поддержка создания кластеров AKS для управляемых удостоверений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-308">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="2b0ed-309">az aks: включена проверка состояния сетевого подключаемого модуля: Azure или Kubenet.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-309">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="2b0ed-310">az aks: включена поддержка ключа сеанса AAD.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-310">az aks: Add aad session key support</span></span>
* <span data-ttu-id="2b0ed-311">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az aks: включена поддержка изменений MSI для GF и BF для omsagent (мониторинг контейнеров) (1)</span><span class="sxs-lookup"><span data-stu-id="2b0ed-311">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="2b0ed-312">az aks use-dev-spaces: добавлен параметр типа конечной точки в команду use-dev-spaces для настройки конечной точки, созданной в контроллере Azure Dev Spaces.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-312">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="2b0ed-313">AppConfig</span><span class="sxs-lookup"><span data-stu-id="2b0ed-313">AppConfig</span></span>

* <span data-ttu-id="2b0ed-314">Включена разблокировка с использованием kv set для добавления функции и ссылки на хранилище ключей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-314">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-315">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-315">AppService</span></span>

* <span data-ttu-id="2b0ed-316">az webapp create: устранена проблема с выполнением команды с параметром --runtime.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-316">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="2b0ed-317">az functionapp deployment source config-zip: добавлено сообщение об ошибке, если группа ресурсов или имя функции недействительны или не существуют.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-317">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="2b0ed-318">functionapp create: исправлено сообщение с предупреждением, которое появляется с `functionapp create` и в котором указан флаг `--functions_version`, но в имени флага ошибочно используется `_` вместо `-`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-318">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="2b0ed-319">az functionapp create: обновлен способ настройки linuxFxVersion и имени образа контейнера для приложений с функциями Linux.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-319">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="2b0ed-320">az functionapp deployment source config-zip: устранена проблема, вызванная изменением параметров приложения во время развертывания ZIP, что приводит к ошибкам 5xx во время развертывания.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-320">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="2b0ed-321">Исправление 5720946: не удается задать имя с помощью az webapp backup.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-321">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="2b0ed-322">ARM</span><span class="sxs-lookup"><span data-stu-id="2b0ed-322">ARM</span></span>

* <span data-ttu-id="2b0ed-323">az resource: улучшены примеры для модуля ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-323">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="2b0ed-324">az policy assignment list: Включена поддержка списков назначений политик в области группы управления.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-324">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="2b0ed-325">Добавлены команды `az deployment group` и `az deployment operation group` для развертывания шаблонов в группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-325">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="2b0ed-326">Это дубликат `az group deployment` и `az group deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-326">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="2b0ed-327">Добавлены команды `az deployment sub` и `az deployment operation sub` для развертывания шаблонов в области подписки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-327">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="2b0ed-328">Это дубликат `az deployment` и `az deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-328">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="2b0ed-329">Добавлены команды `az deployment mg` и `az deployment operation mg` для развертывания шаблонов в группах управления.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-329">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="2b0ed-330">Добавлены команды `az deployment tenant` и `az deployment operation tenant` для развертывания шаблонов в области арендатора.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-330">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="2b0ed-331">az policy assignment create: добавлено описание параметра `--location`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-331">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="2b0ed-332">az group deployment create: добавлен параметр `--aux-tenants` для включения поддержки перекрестных арендаторов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-332">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="2b0ed-333">CDN</span><span class="sxs-lookup"><span data-stu-id="2b0ed-333">CDN</span></span>

* <span data-ttu-id="2b0ed-334">Добавлены команды WAF CDN.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-334">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="2b0ed-335">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-335">Compute</span></span>

* <span data-ttu-id="2b0ed-336">az sig image-version: добавлен параметр --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="2b0ed-336">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="2b0ed-337">az ppg show: добавлен параметр --colocation-status, чтобы включить выборку состояния совместного размещения всех ресурсов в группе размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-337">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="2b0ed-338">az vmss create/update: включена поддержка автоматического исправления.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-338">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="2b0ed-339">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az image template: шаблон переименован в построитель.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-339">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="2b0ed-340">az image builder create: добавлен параметр --image-template.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-340">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="2b0ed-341">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-341">Cosmos DB</span></span>

* <span data-ttu-id="2b0ed-342">Добавлены командлеты хранимой процедуры SQL, определяемых пользователем функций и триггеров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-342">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="2b0ed-343">az cosmosdb create: добавлен параметр --key-uri для добавления сведений о шифровании хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-343">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="2b0ed-344">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-344">KeyVault</span></span>

* <span data-ttu-id="2b0ed-345">keyvault create: включена функция обратимого удаления по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-345">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-346">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-346">Monitor</span></span>

* <span data-ttu-id="2b0ed-347">az monitor metrics alert create: включена поддержка `~` в `--condition`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-347">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-348">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-348">Network</span></span>

* <span data-ttu-id="2b0ed-349">az network application-gateway rewrite-rule create: включена поддержка конфигурации URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-349">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="2b0ed-350">az network dns zone import: для параметра --zone-name в будущем можно будет не учитывать регистр.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-350">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="2b0ed-351">az network private-endpoint/private-link-service: удалена метка предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-351">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="2b0ed-352">az network bastion: включена поддержка бастиона.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-352">az network bastion: support bastion</span></span>
* <span data-ttu-id="2b0ed-353">az network vnet list-available-ips: включена поддержка списка доступных IP-адресов в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-353">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="2b0ed-354">az network watcher flow-log create/list/delete/update: добавлены новые команды для управления журналами потоков Наблюдателя и предоставлен параметр --location для явного определения Наблюдателя.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-354">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="2b0ed-355">az network watcher flow-log configure: поддержка прекращена.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-355">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="2b0ed-356">az network watcher flow-log show: включена поддержка параметров --location и --name для получения результатов в формате ARM; поддержка предыдущего форматированного вывода прекращена.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-356">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="2b0ed-357">Политика</span><span class="sxs-lookup"><span data-stu-id="2b0ed-357">Policy</span></span>

* <span data-ttu-id="2b0ed-358">az policy assignment create: исправлена ошибка, из-за которой автоматически генерируемое имя назначения политики превышало предельное значение.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-358">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="2b0ed-359">RBAC</span><span class="sxs-lookup"><span data-stu-id="2b0ed-359">RBAC</span></span>

* <span data-ttu-id="2b0ed-360">az ad group show: исправлено значение --group, обрабатываемое как проблема с регулярными выражениями.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-360">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="2b0ed-361">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="2b0ed-361">RDBMS</span></span>

* <span data-ttu-id="2b0ed-362">Обновлена версия пакета SDK azure-mgmt-rdbms до 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-362">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="2b0ed-363">az postgres private-endpoint-connection: включено управление подключениями частных конечных точек Postgres.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-363">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="2b0ed-364">az postgres private-link-resource: включено управление ресурсами частных ссылок Postgres.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-364">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="2b0ed-365">az mysql private-endpoint-connection: включено управление подключениями частных конечных точек MySQL.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-365">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="2b0ed-366">az mysql private-link-resource: включено управление ресурсами частных ссылок MySQL.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-366">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="2b0ed-367">az mariadb private-endpoint-connection: включено управление подключениями частных конечных точек MariaDB.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-367">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="2b0ed-368">az mariadb private-link-resource: включено управление ресурсами частных ссылок MariaDB.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-368">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="2b0ed-369">Обновление тестов частной конечной точки RDBMS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-369">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-370">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-370">SQL</span></span>

* <span data-ttu-id="2b0ed-371">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-371">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="2b0ed-372">(sql server create:) добавлен необязательный флаг включения и отключения доступа к общедоступным сетям в команду создания SQL Server.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-372">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="2b0ed-373">(sql server update:) внесены некоторые изменения для клиентов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-373">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="2b0ed-374">Добавлено свойство minimal_tls_version для MI и SQL DB.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-374">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-375">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-375">Storage</span></span>

* <span data-ttu-id="2b0ed-376">az storage blob delete-batch: исправлено неправильное поведение флага `--dryrun`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-376">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="2b0ed-377">az storage account network-rule add (исправление): добавлено требование того, чтобы операция была идемпотентной.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-377">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="2b0ed-378">az storage account create/update: включена поддержка предпочтения маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-378">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="2b0ed-379">Обновлена версия azure-mgmt-storage до 8.0.0.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-379">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="2b0ed-380">az storage container immutability create: добавлен параметр --allow-protected-append-write.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-380">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="2b0ed-381">az storage account private-link-resource list: включена поддержка вывода списка ресурсов частной ссылки для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-381">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="2b0ed-382">az storage account private-endpoint-connection approve/reject/show/delete: включена поддержка управления подключениями к частным конечным точкам.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-382">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="2b0ed-383">az storage account blob-service-properties update: добавлены параметры --enable-restore-policy и --restore-days.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-383">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="2b0ed-384">az storage blob restore: включена поддержка восстановления диапазонов BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-384">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="2b0ed-385">18 февраля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-385">February 18, 2020</span></span>

<span data-ttu-id="2b0ed-386">Версия 2.1.0</span><span class="sxs-lookup"><span data-stu-id="2b0ed-386">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-387">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-387">ACR</span></span>

* <span data-ttu-id="2b0ed-388">Добавлен новый аргумент `--expose-token` для `az acr login`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-388">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="2b0ed-389">Исправлены неправильные выходные данные `az acr task identity show -n Name -r Registry -o table`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-389">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="2b0ed-390">az acr login: отображение CLIError при наличии ошибок, возвращаемых командой docker.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-390">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-391">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-391">ACS</span></span>

* <span data-ttu-id="2b0ed-392">aks create/update: добавление проверки `--vnet-subnet-id`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-392">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="2b0ed-393">Aladdin</span><span class="sxs-lookup"><span data-stu-id="2b0ed-393">Aladdin</span></span>

* <span data-ttu-id="2b0ed-394">Выполнение синтаксического анализа созданных примеров в _help.py для команд.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-394">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="2b0ed-395">AMS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-395">AMS</span></span>

* <span data-ttu-id="2b0ed-396">az ams теперь предоставляется в общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="2b0ed-396">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="2b0ed-397">AppConfig</span><span class="sxs-lookup"><span data-stu-id="2b0ed-397">AppConfig</span></span>

* <span data-ttu-id="2b0ed-398">Исправлено справочное сообщение, чтобы исключить неподдерживаемый фильтр ключей или меток.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-398">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="2b0ed-399">Удален тег preview для большинства команд, кроме управляемого удостоверения и флагов функций.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-399">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="2b0ed-400">Добавлен управляемый ключ клиента при обновлении магазинов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-400">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-401">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-401">AppService</span></span>

* <span data-ttu-id="2b0ed-402">az webapp list-runtimes: исправлена ошибка для list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-402">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="2b0ed-403">Добавлена команда az webapp|functionapp config ssl create.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-403">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="2b0ed-404">Включена поддержка приложений-функций версии 3 и Node 12.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-404">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="2b0ed-405">ARM</span><span class="sxs-lookup"><span data-stu-id="2b0ed-405">ARM</span></span>

* <span data-ttu-id="2b0ed-406">az policy assignment create: исправлено сообщение об ошибке, если параметр `--policy` является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-406">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="2b0ed-407">az group deployment create: Устранена ошибка stat: path too long for Windows при использовании большого файла parameters.json.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-407">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="2b0ed-408">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="2b0ed-408">Backup</span></span>

* <span data-ttu-id="2b0ed-409">Исправлен поток восстановления на уровне элемента в OLR.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-409">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="2b0ed-410">Включена поддержка восстановления в виде файлов для баз данных SQL и SAP.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-410">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="2b0ed-411">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-411">Compute</span></span>

* <span data-ttu-id="2b0ed-412">vm/vmss/availability-set update: add --ppg: разрешено обновление ProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-412">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="2b0ed-413">vmss create: add --data-disk-iops and --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="2b0ed-413">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="2b0ed-414">az vm host: удален тег preview для `vm host` и `vm host group`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-414">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="2b0ed-415">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправление 10728. `az vm create`: автоматическое создание подсети, если указанные виртуальная сеть и подсеть не существуют.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-415">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="2b0ed-416">Повышена надежность списка образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-416">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="2b0ed-417">Eventhub</span><span class="sxs-lookup"><span data-stu-id="2b0ed-417">Eventhub</span></span>

* <span data-ttu-id="2b0ed-418">Включена поддержка Azure Stack для профиля 2019-03-01-hybrid.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-418">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="2b0ed-419">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-419">KeyVault</span></span>

* <span data-ttu-id="2b0ed-420">az keyvault key create: добавлено новое значение `import` для параметра `--ops`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-420">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="2b0ed-421">az keyvault key list-versions: включена поддержка параметров `--id` для определения ключей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-421">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="2b0ed-422">Включена поддержка подключений к частным конечным точкам.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-422">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-423">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-423">Network</span></span>

* <span data-ttu-id="2b0ed-424">Выполнена активация azure-mgmt-network 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-424">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="2b0ed-425">az network private-link-service update/create: включена поддержка --enable-proxy-protocol.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-425">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="2b0ed-426">Добавлена функция монитора подключения версии 2.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-426">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="2b0ed-427">Упаковка</span><span class="sxs-lookup"><span data-stu-id="2b0ed-427">Packaging</span></span>

* <span data-ttu-id="2b0ed-428">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка Python 2.7.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-428">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="2b0ed-429">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-429">Profile</span></span>

* <span data-ttu-id="2b0ed-430">Предварительный просмотр: В учетные записи подписок добавлены новые атрибуты `homeTenantId` и `managedByTenants`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-430">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="2b0ed-431">Чтобы изменения вступили в силу, повторно выполните команду `az login`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-431">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="2b0ed-432">az login: отображение предупреждения, если подписка связана с несколькими клиентами, но по умолчанию используется с первым из них</span><span class="sxs-lookup"><span data-stu-id="2b0ed-432">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="2b0ed-433">(чтобы выбрать определенный клиент при доступе к этой подписке, включите `--tenant` в `az login`).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-433">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-434">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-434">Role</span></span>

* <span data-ttu-id="2b0ed-435">az role assignment create: исправлена ошибка с кодом HTTP 400, возникающая при присвоении роли субъекту-службе по отображаемому имени.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-435">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-436">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-436">SQL</span></span>

* <span data-ttu-id="2b0ed-437">Обновлен командлет `az sql mi update` Управляемого экземпляра SQL (добавлены два новых параметра: tier и family).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-437">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-438">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-438">Storage</span></span>

* <span data-ttu-id="2b0ed-439">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az storage account create`: Тип учетной записи хранения по умолчанию изменен на StorageV2.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-439">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="2b0ed-440">4 февраля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-440">February 04, 2020</span></span>

<span data-ttu-id="2b0ed-441">Версия 2.0.81</span><span class="sxs-lookup"><span data-stu-id="2b0ed-441">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-442">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-442">ACS</span></span>

* <span data-ttu-id="2b0ed-443">Добавлена возможность задания выделенных исходящих портов и времени ожидания подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-443">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="2b0ed-444">Выполнено обновление до API версии 2019-11-01.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-444">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-445">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-445">ACR</span></span>

* <span data-ttu-id="2b0ed-446">[Критическое изменение] `az acr delete` будет выводить запрос.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-446">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="2b0ed-447">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда az acr task delete будет выводить запрос.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-447">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="2b0ed-448">Добавлена новая группа команд az acr taskrun show/list/delete для управления выполнением задач.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-448">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="2b0ed-449">AKS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-449">AKS</span></span>

* <span data-ttu-id="2b0ed-450">Каждый кластер получает отдельный субъект-службу для улучшения изоляции.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-450">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="2b0ed-451">AppConfig</span><span class="sxs-lookup"><span data-stu-id="2b0ed-451">AppConfig</span></span>

* <span data-ttu-id="2b0ed-452">Поддержка импорта ссылок на хранилище ключей из службы приложений и их экспорта в нее.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-452">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="2b0ed-453">Поддержка импорта и экспорта всех меток между файлами appconfig.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-453">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="2b0ed-454">Проверка имен ключей и функций перед настройкой и импортом.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-454">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="2b0ed-455">Предоставление изменений номера SKU в хранилище конфигураций.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-455">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="2b0ed-456">Новая группа команд для управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-456">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-457">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-457">AppService</span></span>

* <span data-ttu-id="2b0ed-458">Azure Stack: команды поверхности в профиле 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="2b0ed-458">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="2b0ed-459">functionapp: добавлена возможность создавать приложения-функции Java в Linux.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-459">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="2b0ed-460">ARM</span><span class="sxs-lookup"><span data-stu-id="2b0ed-460">ARM</span></span>

* <span data-ttu-id="2b0ed-461">Исправление ошибки 10246: аварийное завершение `az resource tag` в случае, если переданный параметр `--ids` являлся идентификатором группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-461">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="2b0ed-462">Исправление ошибки 11658: команда `az group export` не поддерживала параметры `--query` и `--output`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-462">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="2b0ed-463">Исправление ошибки 10279: код выхода `az group deployment validate` был равен 0, если проверка не пройдена.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-463">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="2b0ed-464">Исправление ошибки 9916: улучшено сообщение об ошибке из-за конфликта между тегом и другими условиями фильтра для команды `az resource list`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-464">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="2b0ed-465">Добавлен новый параметр `--managed-by` для добавления данных managedBy для команды `az group create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-465">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="2b0ed-466">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="2b0ed-466">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="2b0ed-467">Добавлена подгруппа `monitor` для управления мониторингом Log Analytics в кластере Azure Red Hat OpensShift.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-467">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="2b0ed-468">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="2b0ed-468">BotService</span></span>

* <span data-ttu-id="2b0ed-469">Исправление ошибки 11697: команда `az bot create` не являлась идемпотентной.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-469">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="2b0ed-470">Проверки исправления имен изменены для выполнения только в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-470">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="2b0ed-471">CDN</span><span class="sxs-lookup"><span data-stu-id="2b0ed-471">CDN</span></span>

* <span data-ttu-id="2b0ed-472">Добавлена поддержка функции rulesEngine.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-472">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="2b0ed-473">Добавлена новая группа команд cdn endpoint rule для управления правилами.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-473">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="2b0ed-474">Пакет azure-mgmt-cdn обновлен до версии 4.0.0 для использования API версии 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-474">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="2b0ed-475">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="2b0ed-475">Deployment Manager</span></span>

* <span data-ttu-id="2b0ed-476">Добавлена операция вывода списка всех ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-476">Add list operation for all resources.</span></span>
* <span data-ttu-id="2b0ed-477">Улучшен ресурс шага для нового типа шага.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-477">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="2b0ed-478">Пакет azure-mgmt-deploymentmanager обновлен для использования версии 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-478">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="2b0ed-479">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-479">IoT</span></span>

* <span data-ttu-id="2b0ed-480">Команды IoT hub Job объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-480">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="2b0ed-481">IoT Central</span><span class="sxs-lookup"><span data-stu-id="2b0ed-481">IoT Central</span></span>

* <span data-ttu-id="2b0ed-482">Добавлена поддержка создания и обновления приложений с новыми SKU: ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-482">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="2b0ed-483">Key Vault</span><span class="sxs-lookup"><span data-stu-id="2b0ed-483">Key Vault</span></span>

* <span data-ttu-id="2b0ed-484">Добавлена новая команда `az keyvault key download` для скачивания ключей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-484">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="2b0ed-485">Разное</span><span class="sxs-lookup"><span data-stu-id="2b0ed-485">Misc</span></span>

* <span data-ttu-id="2b0ed-486">Исправление ошибки 6371: поддержка завершения имен файлов и переменных среды в Bash.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-486">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-487">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-487">Network</span></span>

* <span data-ttu-id="2b0ed-488">Исправление ошибки 2092: для команды az network dns record-set add/remove добавлено предупреждение, отображаемое, если набор записей не найден.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-488">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="2b0ed-489">В будущем для подтверждения этого автоматического создания будет добавлен дополнительный аргумент.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-489">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="2b0ed-490">Политика</span><span class="sxs-lookup"><span data-stu-id="2b0ed-490">Policy</span></span>

* <span data-ttu-id="2b0ed-491">Добавлена новая команда `az policy metadata` для получения ресурсов метаданных расширенной политики.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-491">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="2b0ed-492">`az policy remediation create`: С помощью параметра `--resource-discovery-mode` можно указать, следует ли повторно оценить соответствие перед исправлением.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-492">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="2b0ed-493">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-493">Profile</span></span>

* <span data-ttu-id="2b0ed-494">`az account get-access-token`: Добавлен параметр `--tenant` для получения маркера для арендатора напрямую, без необходимости указывать подписку.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-494">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="2b0ed-495">RBAC</span><span class="sxs-lookup"><span data-stu-id="2b0ed-495">RBAC</span></span>

* <span data-ttu-id="2b0ed-496">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправление ошибки 11883: `az role assignment create`: пустая область приведет к ошибке.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-496">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="2b0ed-497">Безопасность</span><span class="sxs-lookup"><span data-stu-id="2b0ed-497">Security</span></span>

* <span data-ttu-id="2b0ed-498">Добавлены новые команды `az atp show` и `az atp update` для просмотра и настройки дополнительных параметров защиты от угроз для учетных записей хранения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-498">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-499">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-499">SQL</span></span>

* <span data-ttu-id="2b0ed-500">`sql dw create`: параметры `--zone-redundant` и `--read-replica-count` объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-500">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="2b0ed-501">Эти параметры не применяются к хранилищу данных.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-501">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="2b0ed-502">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql db create`: Значения WideWorldImportersStd и WideWorldImportersFull больше не являются задокументированным допустимыми значениями для команды az sql db create --sample-name.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-502">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="2b0ed-503">Эти примеры базы данных всегда будут приводить к сбою создания.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-503">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="2b0ed-504">Добавлены новые команды `sql db classification show/list/update/delete` и `sql db classification recommendation list/enable/disable` для управления классификациями конфиденциальности баз данных SQL.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-504">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="2b0ed-505">`az sql db audit-policy`: устранены пустые действия аудита и группы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-505">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-506">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-506">Storage</span></span>

* <span data-ttu-id="2b0ed-507">Добавлена новая группа команд `az storage share-rm` для использования поставщика ресурсов Microsoft.Storage в операциях управления файловыми ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-507">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="2b0ed-508">Исправление ошибки 11415: ошибка разрешения для `az storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-508">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="2b0ed-509">Добавлены интеграция AzCopy 10.3.3 и поддержка Win32.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-509">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="2b0ed-510">`az storage copy`: добавлены параметры `--include-path`, `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-510">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="2b0ed-511">`az storage remove`: параметры `--inlcude` и `--exclude` заменены параметрами `--include-path`, `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-511">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="2b0ed-512">`az storage sync`: добавлены параметры `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-512">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="2b0ed-513">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="2b0ed-513">ServiceFabric</span></span>

* <span data-ttu-id="2b0ed-514">Добавлены новые команды для управления приложениями и службами.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-514">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="2b0ed-515">13 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-515">January 13, 2020</span></span>

<span data-ttu-id="2b0ed-516">Версия 2.0.80</span><span class="sxs-lookup"><span data-stu-id="2b0ed-516">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="2b0ed-517">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-517">Compute</span></span>

* <span data-ttu-id="2b0ed-518">Обновление диска: добавлены параметры --disk-encryption-set и --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-518">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="2b0ed-519">Создание и обновление моментального снимка: добавлены параметры --disk-encryption-set и --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-519">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-520">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-520">Storage</span></span>

* <span data-ttu-id="2b0ed-521">Обновление azure-mgmt-storage до версии 7.1.0</span><span class="sxs-lookup"><span data-stu-id="2b0ed-521">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="2b0ed-522">`az storage account create`: добавлены параметры `--encryption-key-type-for-table` и `--encryption-key-type-for-queue` для включения поддержки службы шифрования таблиц и очередей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-522">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="2b0ed-523">7 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-523">January 07, 2020</span></span>

<span data-ttu-id="2b0ed-524">Версия 2.0.79</span><span class="sxs-lookup"><span data-stu-id="2b0ed-524">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-525">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-525">ACR</span></span>

* <span data-ttu-id="2b0ed-526">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --os для команд acr build, acr task create/update, acr run и acr pack.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-526">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="2b0ed-527">Вместо этого используется параметр --platform.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-527">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="2b0ed-528">AppConfig</span><span class="sxs-lookup"><span data-stu-id="2b0ed-528">AppConfig</span></span>

* <span data-ttu-id="2b0ed-529">Добавлена поддержка импорта и экспорта флагов функций.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-529">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="2b0ed-530">Добавлена новая команда az appconfig kv set-keyvault для создания ссылки на хранилище ключей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-530">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="2b0ed-531">Добавлена поддержка различных соглашений об именовании при экспорте флагов функций в файл.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-531">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-532">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-532">AppService</span></span>

* <span data-ttu-id="2b0ed-533">Устранена проблема № 7154: обновлена документация по команде <> — теперь в ней используются обратные, а не одинарные кавычки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-533">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="2b0ed-534">Устранена проблема № 11287 (webapp up): по умолчанию для приложения, созданного с использованием этого флага, должен быть включен SSL.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-534">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="2b0ed-535">Устранена проблема № 11592: добавлен флаг az webapp up для статических сайтов HTML.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-535">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="2b0ed-536">ARM</span><span class="sxs-lookup"><span data-stu-id="2b0ed-536">ARM</span></span>

* <span data-ttu-id="2b0ed-537">Исправлена ошибка с командой `az resource tag`: невозможно было обновить теги хранилища Служб восстановления.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-537">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="2b0ed-538">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="2b0ed-538">Backup</span></span>

* <span data-ttu-id="2b0ed-539">Добавлена новая команда backup protection undelete для включения функции обратимого удаления рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-539">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="2b0ed-540">Добавлен новый параметр --soft-delete-feature-state для команды set backup-properties.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-540">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="2b0ed-541">Добавлена поддержка исключения диска для рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-541">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="2b0ed-542">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-542">Compute</span></span>

* <span data-ttu-id="2b0ed-543">Исправлен сбой `vm create` в профиле Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-543">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="2b0ed-544">Добавлена поддержка определений списков и метрик запросов для виртуальной машины (vm monitor metrics tail/list-definitions).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-544">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="2b0ed-545">Добавлено новое действия повторного применения команды az vm</span><span class="sxs-lookup"><span data-stu-id="2b0ed-545">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="2b0ed-546">HDInsight</span><span class="sxs-lookup"><span data-stu-id="2b0ed-546">HDInsight</span></span>

* <span data-ttu-id="2b0ed-547">Включена поддержка создания кластера Kafka с помощью прокси-сервера Kafka RESTful.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-547">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="2b0ed-548">Обновление azure-mgmt-hdinsight до версии 1.3.0</span><span class="sxs-lookup"><span data-stu-id="2b0ed-548">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="2b0ed-549">Прочее</span><span class="sxs-lookup"><span data-stu-id="2b0ed-549">Misc.</span></span>

* <span data-ttu-id="2b0ed-550">Добавлена команда `az version show` предварительного просмотра для отображения версий модулей и расширений Azure CLI в формате JSON по умолчанию или в формате, настроенном с помощью параметра --output</span><span class="sxs-lookup"><span data-stu-id="2b0ed-550">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="2b0ed-551">Центры событий</span><span class="sxs-lookup"><span data-stu-id="2b0ed-551">Event Hubs</span></span>

* <span data-ttu-id="2b0ed-552">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az eventhubs eventhub update и az eventhubs eventhub create.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-552">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="2b0ed-553">Данный параметр недопустим для сущностей концентратора событий.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-553">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="2b0ed-554">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="2b0ed-554">Service Bus</span></span>

* <span data-ttu-id="2b0ed-555">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az servicebus topic create, az servicebus topic update, az servicebus queue create и az servicebus queue update.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-555">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="2b0ed-556">Этот параметр является недопустимым для разделов и очередей служебной шины.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-556">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="2b0ed-557">RBAC</span><span class="sxs-lookup"><span data-stu-id="2b0ed-557">RBAC</span></span>

* <span data-ttu-id="2b0ed-558">Устранена проблема № 11712: команда `az ad app/sp show` не возвращала код выхода 3, если приложение или субъект-служба не существует.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-558">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-559">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-559">Storage</span></span>

* <span data-ttu-id="2b0ed-560">`az storage account create`: удален флаг предварительного просмотра для параметра --enable-hierarchical-namespace.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-560">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="2b0ed-561">Хранилище azure-mgmt-storage обновлено до версии 7.0.0 для использования API версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-561">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="2b0ed-562">Добавлены новые параметры (`--enable-delete-retention` и `--delete-retention-days`) для поддержки управления политикой хранения удаленных свойств службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-562">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="2b0ed-563">17 декабря 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-563">December 17, 2019</span></span>

<span data-ttu-id="2b0ed-564">2.0.78</span><span class="sxs-lookup"><span data-stu-id="2b0ed-564">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-565">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-565">ACR</span></span>

* <span data-ttu-id="2b0ed-566">Добавлена поддержка локального контекста во время выполнения задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-566">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-567">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-567">ACS</span></span>

* <span data-ttu-id="2b0ed-568">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде az openshift create параметр `--workspace-resource-id` переименован на `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-568">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="2b0ed-569">AMS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-569">AMS</span></span>

* <span data-ttu-id="2b0ed-570">Команды show обновлены для возвращения ответа 3, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-570">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="2b0ed-571">AppConfig</span><span class="sxs-lookup"><span data-stu-id="2b0ed-571">AppConfig</span></span>

* <span data-ttu-id="2b0ed-572">Исправлена ошибка, возникающая при добавлении api-version в URL-адрес запроса.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-572">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="2b0ed-573">Имеющееся решение не работает с разбивкой на страницы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-573">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="2b0ed-574">Добавлена поддержка отображения языков, кроме английского, так как наша внутренняя служба поддерживает Юникод для глобализации.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-574">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-575">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-575">AppService</span></span>

* <span data-ttu-id="2b0ed-576">Устранена проблема № 11217 (webapp): теперь команда az webapp config ssl upload поддерживает параметр слота.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-576">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="2b0ed-577">Устранена проблема № 10965. Ошибка: Имя не может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-577">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="2b0ed-578">Разрешено удаление по IP-адресу и подсети.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-578">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="2b0ed-579">Добавлена поддержка импорта сертификатов из хранилища ключей: `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-579">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="2b0ed-580">ARM</span><span class="sxs-lookup"><span data-stu-id="2b0ed-580">ARM</span></span>

* <span data-ttu-id="2b0ed-581">Обновлен пакет ресурсов azure-mgmt-resource для использования версии 6.0.0</span><span class="sxs-lookup"><span data-stu-id="2b0ed-581">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="2b0ed-582">Добавлена межклиентская поддержка команды `az group deployment create` путем добавления нового параметра `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-582">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="2b0ed-583">Добавлен новый параметр `--metadata` для поддержки добавления метаданных определений наборов политик.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-583">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="2b0ed-584">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="2b0ed-584">Backup</span></span>

* <span data-ttu-id="2b0ed-585">Добавлена поддержка резервного копирования для рабочей нагрузки SQL и SAP HANA.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-585">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="2b0ed-586">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="2b0ed-586">BotService</span></span>

* <span data-ttu-id="2b0ed-587">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг --version из предварительной версии команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-587">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="2b0ed-588">Поддерживаются только боты пакетов SDK версии 4.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-588">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="2b0ed-589">Добавлена проверка доступности имени для команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-589">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="2b0ed-590">Добавлена поддержка обновления URL-адреса значка для бота с помощью команды az bot update.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-590">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="2b0ed-591">Добавлена поддержка обновления канала Direct Line с помощью команды az bot directline update.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-591">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="2b0ed-592">Добавлена поддержка флага --enable-enhanced-auth в команде az bot directline create.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-592">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="2b0ed-593">Следующие группы команд предоставляются в общедоступной, а не в предварительной версии: az bot authsetting.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-593">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="2b0ed-594">Следующие команды в az bot предоставляются в общедоступной, а не в предварительной версии: create, prepare-deploy, show, delete и update.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-594">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="2b0ed-595">Устранена проблема с командой az bot prepare-deploy, которая изменяла значение параметра --proj-file-path на нижний регистр (например, с Test.csproj на test.csproj).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-595">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="2b0ed-596">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-596">Compute</span></span>

* <span data-ttu-id="2b0ed-597">vmss create/update: добавлен параметр --scale-on-policy, который определяет, какие виртуальные машины выбираются для удаления при масштабировании VMSS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-597">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="2b0ed-598">vm/vmss update: добавлен параметр --priority.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-598">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="2b0ed-599">vm/vmss update: добавлен параметр --max-price.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-599">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="2b0ed-600">Добавлена группа команд для шифрования дисков (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-600">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="2b0ed-601">disk create: добавлены параметры --encryption-type и --disk-encryption-set.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-601">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="2b0ed-602">vm/vmss create. Добавлены параметры --os-disk-encryption-set и --data-disk-encryption-sets.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-602">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-603">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-603">Core</span></span>

* <span data-ttu-id="2b0ed-604">Удалена поддержка Python версии 3.4.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-604">Removed support for Python 3.4</span></span>
* <span data-ttu-id="2b0ed-605">Подключение к опросу HaTS в нескольких командах.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-605">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="2b0ed-606">DLS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-606">DLS</span></span>

* <span data-ttu-id="2b0ed-607">Обновлена версия пакета SDK для ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-607">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="2b0ed-608">Установка</span><span class="sxs-lookup"><span data-stu-id="2b0ed-608">Install</span></span>

* <span data-ttu-id="2b0ed-609">Добавлена поддержка установки скриптов Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-609">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="2b0ed-610">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-610">IOT</span></span>

* <span data-ttu-id="2b0ed-611">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --failover-region из команды manual-failover.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-611">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="2b0ed-612">Теперь она будет выполнять отработку отказа в назначенный геопарный дополнительный регион.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-612">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="2b0ed-613">Key Vault</span><span class="sxs-lookup"><span data-stu-id="2b0ed-613">Key Vault</span></span>

* <span data-ttu-id="2b0ed-614">Устранена проблема № 8095: (`az keyvault storage remove`): улучшено справочное сообщение.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-614">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="2b0ed-615">Устранена проблема № 8921 (`az keyvault key/secret/certificate list/list-deleted/list-versions`): исправлена ошибка проверки в параметре `--maxresults`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-615">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="2b0ed-616">Устранена проблема № 10512 (`az keyvault set-policy`): улучшено сообщение об ошибке, возвращаемое, если не указан ни один из параметров `--object-id`, `--spn` или `--upn`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-616">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="2b0ed-617">Устранена проблема № 10846 (`az keyvault secret show-deleted`): при указании значения `--id` значение `--name/-n` не требовалось.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-617">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="2b0ed-618">Устранена проблема № 11084: (`az keyvault secret download`): улучшено справочное сообщение параметра `--encoding`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-618">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-619">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-619">Network</span></span>

* <span data-ttu-id="2b0ed-620">az network application-gateway probe: добавлена поддержка параметра --port, позволяющего указать порт, который используется для проверки внутренних серверов при создании и обновлении.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-620">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="2b0ed-621">az network application-gateway url-path-map create/update: исправлена ошибка с `--waf-policy`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-621">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="2b0ed-622">az network application-gateway: добавлена поддержка параметра `--rewrite-rule-set`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-622">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="2b0ed-623">az network list-service-aliases: добавлена поддержка перечисления псевдонимов служб, которые можно использовать для политик конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-623">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="2b0ed-624">az network dns zone import: добавлена поддержка символа .@ в имени записи.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-624">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="2b0ed-625">Упаковка</span><span class="sxs-lookup"><span data-stu-id="2b0ed-625">Packaging</span></span>

* <span data-ttu-id="2b0ed-626">Снова добавлены сборки Edge для установки PIP.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-626">Added back edge builds for pip install</span></span>
* <span data-ttu-id="2b0ed-627">Добавлен пакет Ubuntu eoan.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-627">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="2b0ed-628">Политика</span><span class="sxs-lookup"><span data-stu-id="2b0ed-628">Policy</span></span>

* <span data-ttu-id="2b0ed-629">Добавлена поддержка API Политики версии 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-629">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="2b0ed-630">az policy set-definition: добавлена поддержка группирования в определениях наборов политик с помощью параметра `--definition-groups`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-630">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="2b0ed-631">Redis</span><span class="sxs-lookup"><span data-stu-id="2b0ed-631">Redis</span></span>

* <span data-ttu-id="2b0ed-632">В команду `az redis create` добавлена предварительная версия параметра `--replicas-per-master`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-632">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="2b0ed-633">Обновлена версия azure-mgmt-redis с 6.0.0 на 7.0.0 RC1.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-633">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="2b0ed-634">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="2b0ed-634">ServiceFabric</span></span>

* <span data-ttu-id="2b0ed-635">Исправлена логика добавления типа узла, а также устранена проблема № 10963: при добавлении нового типа узла с уровнем устойчивости Gold возникала ошибка CLI.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-635">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="2b0ed-636">Обновлена версия параметра ServiceFabricNodeVmExt до 1.1 в шаблоне создания.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-636">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-637">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-637">SQL</span></span>

* <span data-ttu-id="2b0ed-638">В команды create и update базы данных SQL добавлены параметры --read-scale и --read-replicas для поддержки управления масштабированием операций чтения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-638">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-639">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-639">Storage</span></span>

* <span data-ttu-id="2b0ed-640">Выпущена общедоступная версия больших файловых ресурсов для команды создания и обновления учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-640">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="2b0ed-641">Выпущена общедоступная версия поддержки маркера SAS для делегирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-641">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="2b0ed-642">Добавлены новые команды (`az storage account blob-service-properties show` и `az storage account blob-service-properties update --enable-change-feed`) для управления свойствами службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-642">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="2b0ed-643">[ОЖИДАЕТСЯ КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] `az storage copy`: символ `*` больше не поддерживается в качестве подстановочного знака в URL-адресе. Тем не менее новые параметры--include-pattern и--exclude-pattern будут добавлены с поддержкой подстановочных знаков `*`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-643">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="2b0ed-644">Устранена проблема № 11043: добавлена поддержка удаления всего контейнера или общего ресурса в команде `az storage remove`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-644">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="2b0ed-645">26 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-645">November 26, 2019</span></span>

<span data-ttu-id="2b0ed-646">Версия 2.0.77</span><span class="sxs-lookup"><span data-stu-id="2b0ed-646">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-647">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-647">ACR</span></span>

* <span data-ttu-id="2b0ed-648">Параметр `--branch`, используемый при обновлении или создании задачи ACR, объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-648">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="2b0ed-649">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="2b0ed-649">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="2b0ed-650">Добавлен флаг `--workspace-resource-id` для создания кластера Azure Red Hat Openshift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-650">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="2b0ed-651">Добавлен флаг `monitor_profile` для создания кластера Azure Red Hat OpenShift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-651">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="2b0ed-652">AKS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-652">AKS</span></span>

* <span data-ttu-id="2b0ed-653">Включена поддержка операции смены сертификата кластера с использованием команды az aks rotate-certs.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-653">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="2b0ed-654">AppConfig</span><span class="sxs-lookup"><span data-stu-id="2b0ed-654">AppConfig</span></span>

* <span data-ttu-id="2b0ed-655">Включена поддержка использования символа ":" для разделителя `as az appconfig kv import`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-655">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="2b0ed-656">Исправлена проблема с перечислением значений ключей с несколькими метками, включая метку NULL.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-656">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="2b0ed-657">Обновлен пакет SDK для плоскости управления, azure-mgmt-appconfiguration, до версии 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-657">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="2b0ed-658">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-658">AppService</span></span>

* <span data-ttu-id="2b0ed-659">Исправлена ошибка № 11100. Использование AttributeError для az webapp up при создании плана службы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-659">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="2b0ed-660">az webapp up. При принудительном создании или развертывании сайта для поддерживаемых языков значения по умолчанию не используются.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-660">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="2b0ed-661">Включена поддержка Среды службы приложений: az appservice ase show | list | list-addresses | list-plans | create | update | delete.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-661">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="2b0ed-662">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="2b0ed-662">Backup</span></span>

* <span data-ttu-id="2b0ed-663">Исправлена проблема в команде az backup policy list-associated-items.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-663">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="2b0ed-664">Добавлен необязательный параметр BackupManagementType.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-664">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="2b0ed-665">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-665">Compute</span></span>

* <span data-ttu-id="2b0ed-666">Обновлена версия API вычислений, дисков, моментальных снимков до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-666">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="2b0ed-667">vmss create. Улучшение для --orchestration-mode.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-667">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="2b0ed-668">sig image-definition create. Добавлен параметр --os-state для указания того, являются ли виртуальные машины, созданные в этом образе, универсальными или специализированными.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-668">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="2b0ed-669">sig image-definition create. Добавлен параметр --hyper-v-generation для указания создания гипервизора.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-669">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="2b0ed-670">sig image-version create. Включена поддержка параметров --os-snapshot и --data-snapshots.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-670">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="2b0ed-671">image create. Включена поддержка параметра --data-disk-caching для указания параметра кэширования для дисков данных.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-671">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="2b0ed-672">Обновлена версия пакета SDK для вычислений Python до 10.0.0.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-672">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="2b0ed-673">vm/vmss create. Добавлен фрагмент Spot в свойство перечисления Priority.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-673">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="2b0ed-674">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименование параметра --max-billing в --max-price для виртуальных машин и Масштабируемых наборов виртуальных машин в соответствии с командлетами Swagger и PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-674">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="2b0ed-675">vm monitor log show. Включена поддержка запроса журналов в связанной рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-675">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="2b0ed-676">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-676">IOT</span></span>

* <span data-ttu-id="2b0ed-677">Исправление № 2531. Добавлены вспомогательные аргументы для обновления концентратора.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-677">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="2b0ed-678">Исправление № 8323. Добавлены недостающие параметры для создания пользовательской конечной точки хранилища.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-678">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="2b0ed-679">Исправлена ошибка регрессии. Отменены изменения, переопределяющие конечную точку хранилища по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-679">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="2b0ed-680">Key Vault</span><span class="sxs-lookup"><span data-stu-id="2b0ed-680">Key Vault</span></span>

* <span data-ttu-id="2b0ed-681">Исправление № 11121. При использовании `az keyvault certificate list` для передачи `--include-pending` теперь не требуется значение `true` или `false`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-681">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="2b0ed-682">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="2b0ed-682">NetAppFiles</span></span>

* <span data-ttu-id="2b0ed-683">Обновлена версия azure-mgmt-netapp до 0.7.0, которая включает некоторые дополнительные свойства тома, связанные с предстоящими операциями репликации.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-683">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-684">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-684">Network</span></span>

* <span data-ttu-id="2b0ed-685">application-gateway waf-config. Не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-685">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="2b0ed-686">application-gateway waf-policy. Добавлены управляемые правила подгрупп для контроля управляемых наборов правил и правил исключения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-686">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="2b0ed-687">application-gateway waf-policy. Добавлен параметр политики подгруппы для управления глобальной конфигурацией политики WAF.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-687">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="2b0ed-688">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] application-gateway waf-policy. Переименовано правило подгруппы в пользовательское правило.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-688">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="2b0ed-689">application-gateway http-listener. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-689">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="2b0ed-690">application-gateway url-path-map rule. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-690">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="2b0ed-691">Упаковка</span><span class="sxs-lookup"><span data-stu-id="2b0ed-691">Packaging</span></span>

* <span data-ttu-id="2b0ed-692">Удалена команда az wrapper в Python.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-692">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="2b0ed-693">Включена поддержка Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-693">Added support for Python 3.8</span></span>
* <span data-ttu-id="2b0ed-694">Изменена версия на Python 3 для пакета RPM.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-694">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="2b0ed-695">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-695">Profile</span></span>

* <span data-ttu-id="2b0ed-696">Исправлена ошибка при выполнении `az login -u {} -p {}` с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-696">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="2b0ed-697">Исправлена ошибка с `SSLError` при выполнении `az login` за прокси-сервером с самозаверяющим корневым сертификатом.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-697">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="2b0ed-698">Исправлена ошибка № 10578. `az login` зависает при одновременном запуске нескольких экземпляров в Windows или WSL.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-698">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="2b0ed-699">Исправлена ошибка № 11059. Сбой выполнения `az login --allow-no-subscriptions`, если в клиенте есть подписки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-699">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="2b0ed-700">Исправлена ошибка № 11238. После переименования подписки вход с помощью MSI приведет к тому, что одна и та же подписка появится дважды.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-700">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="2b0ed-701">RBAC</span><span class="sxs-lookup"><span data-stu-id="2b0ed-701">RBAC</span></span>

* <span data-ttu-id="2b0ed-702">Исправлена ошибка № 10996. Исправлена ошибка с `--force-change-password-next-login` в `az ad user update`, если `--password` не указывается.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-702">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="2b0ed-703">Redis</span><span class="sxs-lookup"><span data-stu-id="2b0ed-703">Redis</span></span>

* <span data-ttu-id="2b0ed-704">Исправлена ошибка № 2902. Предотвращена настройка конфигураций памяти при обновлении кэша с номером SKU "Базовый".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-704">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="2b0ed-705">Резервирование</span><span class="sxs-lookup"><span data-stu-id="2b0ed-705">Reservations</span></span>

* <span data-ttu-id="2b0ed-706">Обновлена версия пакета SDK до 0.6.0</span><span class="sxs-lookup"><span data-stu-id="2b0ed-706">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="2b0ed-707">Добавлены сведения о плане выставления счетов после вызова Get-Catalogs.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-707">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="2b0ed-708">Добавлена новая команда `az reservations reservation-order calculate` для вычисления стоимости резервирования.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-708">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="2b0ed-709">Добавлена новая команда `az reservations reservation-order purchase` для приобретения нового резервирования.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-709">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="2b0ed-710">Rest</span><span class="sxs-lookup"><span data-stu-id="2b0ed-710">Rest</span></span>
* <span data-ttu-id="2b0ed-711">Изменена версия `az rest` на общедоступную.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-711">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-712">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-712">SQL</span></span>

* <span data-ttu-id="2b0ed-713">Обновлена версия azure-mgmt-sql до 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-713">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-714">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-714">Storage</span></span>

* <span data-ttu-id="2b0ed-715">storage account create. Добавлен параметр --enable-hierarchical-namespace для включения поддержки семантики файловой системы в службе больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-715">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="2b0ed-716">Удалено несвязанное исключение из сообщения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-716">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="2b0ed-717">Исправлены проблемы, из-за которых появлялось неверное сообщение об отсутствии нужных разрешений на выполнение требуемой операции</span><span class="sxs-lookup"><span data-stu-id="2b0ed-717">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="2b0ed-718">при блокировке правилами сети (AuthenticationFailed).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-718">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="2b0ed-719">4 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-719">November 4, 2019</span></span>

<span data-ttu-id="2b0ed-720">Версия 2.0.76</span><span class="sxs-lookup"><span data-stu-id="2b0ed-720">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-721">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-721">ACR</span></span>

* <span data-ttu-id="2b0ed-722">В команду `az acr pack build` добавлен параметр предварительной версии `--pack-image-tag`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-722">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="2b0ed-723">Добавлена поддержка включения аудита при создании реестра.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-723">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="2b0ed-724">Включена поддержка функции RBAC, распространяющаяся на репозиторий.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-724">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="2b0ed-725">AKS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-725">AKS</span></span>

* <span data-ttu-id="2b0ed-726">В команду `az aks create` добавлены `--enable-cluster-autoscaler`, `--min-count` и `--max-count`, что позволяет автоматически масштабировать кластер для пула узлов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-726">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="2b0ed-727">Добавлены указанные выше флаги, а также `--update-cluster-autoscaler` и `--disable-cluster-autoscaler` в команду `az aks update`, что позволяет обновлять средство автоматического масштабирования кластера.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-727">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="2b0ed-728">AppConfig</span><span class="sxs-lookup"><span data-stu-id="2b0ed-728">AppConfig</span></span>

* <span data-ttu-id="2b0ed-729">Добавлена группа команд функции appconfig для управления флагами функций, хранимыми в Конфигурации приложений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-729">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="2b0ed-730">Исправлена незначительная ошибка команды экспорта в файл appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-730">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="2b0ed-731">Прерывание чтения содержимого конечного файла во время экспорта.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-731">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-732">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-732">AppService</span></span>

* <span data-ttu-id="2b0ed-733">`az appservice plan create`: Добавлена поддержка определения persitescaling при создании плана appservice.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-733">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="2b0ed-734">Исправлена проблема, из-за которой операция webapp config ssl bind удаляла существующие теги из ресурса.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-734">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="2b0ed-735">Добавлен флаг `--build-remote` для `az functionapp deployment source config-zip` для включения поддержки действия удаленной сборки во время развертывания приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-735">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="2b0ed-736">Изменена версия узла по умолчанию для приложений-функций на ~10 для Windows</span><span class="sxs-lookup"><span data-stu-id="2b0ed-736">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="2b0ed-737">В `az functionapp create` добавлено свойство `--runtime-version`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-737">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="2b0ed-738">ARM</span><span class="sxs-lookup"><span data-stu-id="2b0ed-738">ARM</span></span>

* <span data-ttu-id="2b0ed-739">`az deployment/group deployment validate`: В `--handle-extended-json-format` добавлен параметр для включения поддержки многострочности и комментариев в шаблоне JSON при развертывании.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-739">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="2b0ed-740">Версия azure-mgmt-resource обновлена до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-740">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="2b0ed-741">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="2b0ed-741">Backup</span></span>

* <span data-ttu-id="2b0ed-742">Добавлена поддержка резервного копирования AzureFiles.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-742">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="2b0ed-743">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-743">Compute</span></span>

* <span data-ttu-id="2b0ed-744">`az vm create`: Добавлено предупреждение при одновременном определении ускоренной сети и существующей сетевой карты.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-744">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="2b0ed-745">`az vm create`: Добавлен параметр `--vmss` для определения существующего масштабируемого набора виртуальных машин, которому должна быть назначена виртуальная машина.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-745">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="2b0ed-746">`az vm/vmss create`: Добавлена локальная копия файла псевдонима изображения, к которой можно получить доступ в ограниченной сетевой среде.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-746">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="2b0ed-747">`az vmss create`: Добавлен параметр `--orchestration-mode` для определения того, как виртуальные машины управляются масштабируемым набором.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-747">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="2b0ed-748">`az vm/vmss update`: Добавлен параметр `--ultra-ssd-enabled`, чтобы разрешить обновление параметра Ultra SSD.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-748">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="2b0ed-749">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az vm extension set`: Исправлена ошибка, из-за которой пользователям не удавалось определять расширение на виртуальной машине с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-749">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="2b0ed-750">Добавлены новые команды `az vm image terms accept/cancel/show` для управления условиями использования образов Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-750">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="2b0ed-751">Расширение VMAccessForLinux обновлено до версии 1.5.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-751">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2b0ed-752">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-752">CosmosDB</span></span>

* <span data-ttu-id="2b0ed-753">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql container create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-753">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="2b0ed-754">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az gremlin graph create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-754">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="2b0ed-755">`az sql container create`: Добавлены команды `--unique-key-policy` и `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-755">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="2b0ed-756">`az sql container create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-756">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="2b0ed-757">`gremlin graph create`: Добавлена команда `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-757">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="2b0ed-758">`gremlin graph create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-758">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="2b0ed-759">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-759">Fixed typo in help message</span></span>
* <span data-ttu-id="2b0ed-760">База данных: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-760">database: Added deprecation information</span></span>
* <span data-ttu-id="2b0ed-761">Коллекция: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-761">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="2b0ed-762">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-762">IoT</span></span>

* <span data-ttu-id="2b0ed-763">Добавлен новый тип источника маршрутизации: DigitalTwinChangeEvents.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-763">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="2b0ed-764">Добавлены отсутствующие компоненты в `az iot hub create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-764">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="2b0ed-765">Key Vault</span><span class="sxs-lookup"><span data-stu-id="2b0ed-765">Key Vault</span></span>

* <span data-ttu-id="2b0ed-766">Исправлена непредвиденная ошибка с отсутствием файла сертификата.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-766">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="2b0ed-767">Исправлена ошибка с неработающей командой `az keyvault recover/purge`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-767">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="2b0ed-768">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="2b0ed-768">NetAppFiles</span></span>

* <span data-ttu-id="2b0ed-769">Пакет azure-mgmt-netapp обновлен до версии 0.6.0 для включения поддержки API версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-769">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="2b0ed-770">Эта новая версия API включает:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-770">This new API version includes:</span></span>

    - <span data-ttu-id="2b0ed-771">При создании тома с использованием `--protocol-types` допускается NFSv4.1 вместо NFSv4.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-771">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="2b0ed-772">Свойство политики экспорта томов теперь называется nfsv41, а не nfsv4.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-772">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="2b0ed-773">Параметр `--creation-token` для тома переименован в `--file-path`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-773">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="2b0ed-774">Дата создания моментального снимка теперь имеет значение Created.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-774">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-775">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-775">Network</span></span>

* <span data-ttu-id="2b0ed-776">`az network private-dns link vnet create/update`: Добавлена поддержка связывания виртуальных сетей между клиентами.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-776">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="2b0ed-777">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az network vnet subnet list`: Параметры `--resource-group` и `--vnet-name` теперь являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-777">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="2b0ed-778">`az network public-ip prefix create`: Включена поддержка определения версии IP-адреса (IPv4, IPv6) при создании.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-778">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="2b0ed-779">Версия azure-mgmt-network обновлена до 7.0.0 и версия api-version до 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-779">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="2b0ed-780">`az network vrouter`: Включена поддержка нового виртуального маршрутизатора службы и пиринга виртуальных маршрутизаторов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-780">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="2b0ed-781">`az network express-route gateway connection`: Добавлена поддержка параметра `--internet-security`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-781">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="2b0ed-782">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-782">Profile</span></span>

* <span data-ttu-id="2b0ed-783">Исправлена ошибка с неработающей командой `az account get-access-token --resource-type ms-graph`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-783">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="2b0ed-784">Удалено предупреждение из `az login`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-784">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="2b0ed-785">RBAC</span><span class="sxs-lookup"><span data-stu-id="2b0ed-785">RBAC</span></span>

* <span data-ttu-id="2b0ed-786">Исправление `az ad app update --id {} --display-name {}` не работает.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-786">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="2b0ed-787">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="2b0ed-787">ServiceFabric</span></span>

* <span data-ttu-id="2b0ed-788">`az sf cluster create`: Исправлена проблема путем изменения VMSS для вычислений с использованием файла template.json для Service Fabric Linux и Windows со стандартных дисков на управляемые.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-788">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-789">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-789">SQL</span></span>

* <span data-ttu-id="2b0ed-790">Добавлены параметры `--compute-model`, `--auto-pause-delay` и `--min-capacity` для включения поддержки операций CRUD для нового предложения Базы данных SQL: Модель бессерверных вычислений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-790">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-791">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-791">Storage</span></span>

* <span data-ttu-id="2b0ed-792">`az storage account create/update`: Добавлен параметр --enable-files-adds и группа аргументов свойств Azure Active Directory для включения поддержки аутентификации доменных служб Azure Active Directory для Файлов Azure.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-792">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="2b0ed-793">Расширена команда `az storage account keys list/renew` для включения поддержки перечисления или повторного создания ключей Kerberos для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-793">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="2b0ed-794">15 октября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-794">October 15, 2019</span></span>

<span data-ttu-id="2b0ed-795">Версия 2.0.75</span><span class="sxs-lookup"><span data-stu-id="2b0ed-795">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="2b0ed-796">AKS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-796">AKS</span></span>

* <span data-ttu-id="2b0ed-797">Для параметра `--load-balancer-sku` изменено значение по умолчанию на `standard`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-797">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="2b0ed-798">Для параметра `--vm-set-type` изменено значение по умолчанию на `virtualmachinescalesets`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-798">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="2b0ed-799">AMS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-799">AMS</span></span>

* <span data-ttu-id="2b0ed-800">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя `job start` изменено на `job create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-800">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="2b0ed-801">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В параметре `--ask` команды `content-key-policy create` вместо кодировки UTF8 теперь используется шестнадцатеричная строка из 32 символов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-801">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-802">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-802">AppService</span></span>

* <span data-ttu-id="2b0ed-803">Добавлены команды `webapp config access-restriction show|set|add|remove`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-803">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="2b0ed-804">Улучшена обработка ошибок в `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-804">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="2b0ed-805">Для `appservice plan update` добавлена поддержка номера SKU `Isolated`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-805">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="2b0ed-806">ARM</span><span class="sxs-lookup"><span data-stu-id="2b0ed-806">ARM</span></span>

* <span data-ttu-id="2b0ed-807">В `deployment create` добавлен параметр `--handle-extended-json-format` для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-807">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="2b0ed-808">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-808">Compute</span></span>

* <span data-ttu-id="2b0ed-809">Добавлен параметр `--enable-agent` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-809">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="2b0ed-810">Внесены изменения в `vm create`, позволяющие автоматически использовать номер SKU "Стандартный" для общедоступных IP-адресов при использовании зон.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-810">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="2b0ed-811">Внесены изменения в `vm create`, позволяющие автоматически создавать допустимое имя для виртуальной машины, если оно не задано.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-811">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="2b0ed-812">В `vmss create` добавлен параметр `--computer-name-prefix` для поддержки пользовательского префикса имени для виртуальных машин в VMSS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-812">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="2b0ed-813">В `vm create` добавлен параметр `--workspace` для автоматического включения рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-813">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="2b0ed-814">API коллекций обновлен до версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-814">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-815">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-815">Core</span></span>

* <span data-ttu-id="2b0ed-816">Добавлена проверка синтаксиса для параметра `--set` в универсальной команде обновления.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-816">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="2b0ed-817">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-817">IoT</span></span>

* <span data-ttu-id="2b0ed-818">Исправлена проблема, при которой `iot hub show` неправильно выдавал ошибку "Ресурс не найден".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-818">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-819">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-819">Monitor</span></span>

* <span data-ttu-id="2b0ed-820">В `monitor log-analytics workspace` добавлена поддержка CRUD.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-820">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-821">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-821">Network</span></span>

* <span data-ttu-id="2b0ed-822">В `network private-dns link vnet [create|update]` добавлена поддержка виртуального канала для клиентов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-822">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="2b0ed-823">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для `network vnet subnet list` теперь требуются параметры `--resource-group` и `--vnet-name`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-823">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-824">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-824">SQL</span></span>

* <span data-ttu-id="2b0ed-825">В `sql mi ad-admin` добавлены команды, которые поддерживают назначение администратора AAD в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-825">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-826">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-826">Storage</span></span>

* <span data-ttu-id="2b0ed-827">В `storage copy` добавлен параметр `--preserve-s2s-access-tier`, позволяющий сохранить уровень доступа во время копирования между службами.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-827">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="2b0ed-828">В `storage account [create|update]` добавлен параметр `--enable-large-file-share` для поддержки общих папок большого размера в учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-828">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="2b0ed-829">24 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-829">September 24, 2019</span></span>

<span data-ttu-id="2b0ed-830">Версия 2.0.74</span><span class="sxs-lookup"><span data-stu-id="2b0ed-830">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-831">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-831">ACR</span></span>

* <span data-ttu-id="2b0ed-832">В `acr config retention update` добавлен обязательный параметр `--type`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-832">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="2b0ed-833">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованный параметр `--name -n` изменен на `--registry -r ` для группы команд `acr config`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-833">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="2b0ed-834">AKS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-834">AKS</span></span>

* <span data-ttu-id="2b0ed-835">В команду `aks create` добавлен параметр `--load-balancer-sku`, позволяющий создать кластер AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-835">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="2b0ed-836">В команды `aks [create|update]` добавлены параметры `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` и `--load-balancer-outbound-ip-prefixes`, позволяющие обновлять профиль подсистемы балансировки нагрузки у кластера AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-836">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="2b0ed-837">В команду `aks create` добавлен параметр `--vm-set-type`, позволяющий указывать типы виртуальных машин в кластере AKS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-837">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="2b0ed-838">ARM</span><span class="sxs-lookup"><span data-stu-id="2b0ed-838">ARM</span></span>

* <span data-ttu-id="2b0ed-839">В команду `group deployment create` добавлен параметр `--handle-extended-json-format`, для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-839">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="2b0ed-840">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-840">Compute</span></span>

* <span data-ttu-id="2b0ed-841">В команды `vmss [create|update]` добавлен параметр `--terminate-notification-time`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-841">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="2b0ed-842">В команду `vmss update` добавлен параметр `--enable-terminate-notification`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-842">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="2b0ed-843">В команды `[vm|vmss] create` добавлены параметры `--priority,`, `--eviction-policy,` и `--max-billing`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-843">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="2b0ed-844">Изменена команда `disk create`, которая теперь позволяет указать точный размер отправки на диск.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-844">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="2b0ed-845">В `snapshot create` добавлена поддержка добавочных моментальных снимков для управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-845">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="2b0ed-846">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-846">Cosmos DB</span></span>

* <span data-ttu-id="2b0ed-847">В команду `cosmosdb keys list` добавлен параметр `--type <key-type>` для отображения ключей, ключей только для чтения или строк подключения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-847">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="2b0ed-848">Добавлена команда `cosmosdb keys regenerate`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-848">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="2b0ed-849">[УСТАРЕЛО] Команды `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` и `cosmosdb list-read-only-keys` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-849">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="2b0ed-850">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="2b0ed-850">EventGrid</span></span>

* <span data-ttu-id="2b0ed-851">Исправлен текст справки по конечной точке — дана ссылка на правильный параметр.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-851">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="2b0ed-852">Key Vault</span><span class="sxs-lookup"><span data-stu-id="2b0ed-852">Key Vault</span></span>

* <span data-ttu-id="2b0ed-853">Исправлена проблема, из-за которой вход с помощью клиента (`login -t`) мог приводить к сбою `keyvault create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-853">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-854">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-854">Monitor</span></span>

* <span data-ttu-id="2b0ed-855">Исправлена проблема с тем, что символ `:` являлся недопустимым в аргументе `--condition` для `monitor metrics alert create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-855">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="2b0ed-856">Политика</span><span class="sxs-lookup"><span data-stu-id="2b0ed-856">Policy</span></span>

* <span data-ttu-id="2b0ed-857">Добавлена поддержка API Политики версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-857">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="2b0ed-858">В команду `policy assignment create` добавлен параметр `--enforcement-mode`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-858">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-859">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-859">Storage</span></span>

* <span data-ttu-id="2b0ed-860">В команду `az storage copy` добавлен параметр `--blob-type`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-860">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="2b0ed-861">10 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-861">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-862">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-862">ACR</span></span>

* <span data-ttu-id="2b0ed-863">Добавлена группа команд `acr config retention` для настройки политики хранения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-863">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="2b0ed-864">AKS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-864">AKS</span></span>

* <span data-ttu-id="2b0ed-865">Добавлена возможность интеграции ACR с помощью следующих команд:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-865">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="2b0ed-866">В `aks [create|update]` добавлен параметр `--attach-acr` для подключения ACR к кластеру AKS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-866">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="2b0ed-867">В `aks update` добавлен параметр `--detach-acr` для отключения ACR от кластера AKS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-867">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="2b0ed-868">ARM</span><span class="sxs-lookup"><span data-stu-id="2b0ed-868">ARM</span></span>

* <span data-ttu-id="2b0ed-869">Добавлена возможность использования API версии 2019-05-10.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-869">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="2b0ed-870">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-870">Batch</span></span>

* <span data-ttu-id="2b0ed-871">Добавлены новые параметры конфигурации JSON в `--json-file` для `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-871">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="2b0ed-872">Добавлен параметр `MountConfigurations` для подключений файловой системы (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-872">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="2b0ed-873">Добавлено необязательное свойство `publicIPs` в `NetworkConfiguration` для общедоступных IP-адресов в пулах (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-873">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="2b0ed-874">В `--image` добавлена поддержка коллекций общих образов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-874">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="2b0ed-875">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `--start-task-wait-for-success` в `batch pool create` изменено на `true`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-875">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="2b0ed-876">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `Scope` в `AutoUserSpecification` задано как Pool (ранее `Task` на узлах Windows и `Pool` на узлах Linux).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-876">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="2b0ed-877">Этот аргумент можно задать только в конфигурации JSON с помощью `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-877">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="2b0ed-878">HDInsight</span><span class="sxs-lookup"><span data-stu-id="2b0ed-878">HDInsight</span></span>

* <span data-ttu-id="2b0ed-879">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="2b0ed-879">GA release</span></span>
* <span data-ttu-id="2b0ed-880">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--workernode-count/-c` в `az hdinsight resize` теперь является обязательным.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-880">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="2b0ed-881">Key Vault</span><span class="sxs-lookup"><span data-stu-id="2b0ed-881">Key Vault</span></span>

* <span data-ttu-id="2b0ed-882">Исправлена проблема, когда подсети не удавалось удалить из сетевых правил.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-882">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="2b0ed-883">Исправлена проблема, когда дублированные подсети и IP-адреса могли быть добавлены к сетевым правилам.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-883">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-884">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-884">Network</span></span>

* <span data-ttu-id="2b0ed-885">Добавлен параметр `--interval` в `network watcher flow-log` для выбора значения интервала анализа трафика.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-885">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="2b0ed-886">Добавлена команда `network application-gateway identity` для управления удостоверением шлюза.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-886">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="2b0ed-887">Добавлена возможность указать идентификатор Key Vault в команде `network application-gateway ssl-cert`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-887">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="2b0ed-888">Добавлена команда `network express-route peering peer-connection [show|list]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-888">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="2b0ed-889">Политика</span><span class="sxs-lookup"><span data-stu-id="2b0ed-889">Policy</span></span>

* <span data-ttu-id="2b0ed-890">Добавлена возможность использования API версии 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-890">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="2b0ed-891">27 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-891">August 27, 2019</span></span>

<span data-ttu-id="2b0ed-892">Версия 2.0.72</span><span class="sxs-lookup"><span data-stu-id="2b0ed-892">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-893">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-893">ACR</span></span>

* <span data-ttu-id="2b0ed-894">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка SKU `classic`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-894">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="2b0ed-895">Управление API</span><span class="sxs-lookup"><span data-stu-id="2b0ed-895">API Management</span></span>

* <span data-ttu-id="2b0ed-896">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена группа команд `apim`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-896">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-897">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-897">AppService</span></span>

* <span data-ttu-id="2b0ed-898">Исправлена проблема с командой `webapp webjob continuous start` при указании слота.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-898">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="2b0ed-899">Изменена команда `webapp up` для обнаружения и удаления папки `env` из файла, используемого для развертывания.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-899">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="2b0ed-900">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-900">Keyvault</span></span>

* <span data-ttu-id="2b0ed-901">Исправлена ошибка в команде `keyvault secret set`, которая игнорировала аргумент `--expires`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-901">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-902">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-902">Network</span></span>

* <span data-ttu-id="2b0ed-903">Добавлена поддержка IPv6-адресов для аргументов `--private-ip-address-version`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-903">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="2b0ed-904">Добавлены новые команды `network private-endpoint [create|update|list-types]` для управления закрытыми конечными точками.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-904">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="2b0ed-905">Добавлена группа команд для `network private-link-service`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-905">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="2b0ed-906">Добавлены аргументы `--private-endpoint-network-policies` и `--private-link-service-network-policies` для команды `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-906">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="2b0ed-907">RBAC</span><span class="sxs-lookup"><span data-stu-id="2b0ed-907">RBAC</span></span>

* <span data-ttu-id="2b0ed-908">Исправлена проблема с `ad app update --homepage`, когда домашнюю страницу нельзя было обновить.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-908">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="2b0ed-909">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="2b0ed-909">ServiceFabric</span></span>

* <span data-ttu-id="2b0ed-910">Добавлена поддержка имен Key Vault в смешанном регистре.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-910">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="2b0ed-911">Исправлена проблема с использованием сертификатов в Key Vault.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-911">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="2b0ed-912">Исправлена проблема с использованием файлов сертификатов PFX.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-912">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="2b0ed-913">Исправлена проблема с `sf cluster certificate add`, когда группа ресурсов Key Vault не была указана.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-913">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="2b0ed-914">Исправлена проблема с неработающей командой `sf cluster set`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-914">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="2b0ed-915">SignalR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-915">SignalR</span></span>

* <span data-ttu-id="2b0ed-916">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-916">Added new commands:</span></span>
  * <span data-ttu-id="2b0ed-917">`signalr cors`: Управление CORS SignalR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-917">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="2b0ed-918">`signalr restart`: Перезапуск службы SignalR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-918">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="2b0ed-919">`signalr update`: Обновление службы SignalR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-919">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="2b0ed-920">Добавлен аргумент `--service-mode` для команды `signalr create`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-920">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-921">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-921">Storage</span></span>

* <span data-ttu-id="2b0ed-922">Добавлена команда `storage account revoke-delegation-keys`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-922">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="2b0ed-923">13 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-923">August 13, 2019</span></span>

<span data-ttu-id="2b0ed-924">Версия 2.0.71</span><span class="sxs-lookup"><span data-stu-id="2b0ed-924">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-925">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-925">AppService</span></span>

* <span data-ttu-id="2b0ed-926">Исправлена проблема, из-за которой выполнение команд `webapp webjob continuous` для слотов завершалось сбоем.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-926">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="2b0ed-927">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="2b0ed-927">BotService</span></span>

* <span data-ttu-id="2b0ed-928">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка создания ботов на основе пакета SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-928">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="2b0ed-929">Cognitive Services:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-929">CognitiveServices</span></span>

* <span data-ttu-id="2b0ed-930">Добавлены команды `cognitiveservices account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-930">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="2b0ed-931">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-931">Cosmos DB</span></span>

* <span data-ttu-id="2b0ed-932">Удалено предупреждение при обновлении нескольких расположений для записи.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-932">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="2b0ed-933">Добавлены команды CRUD для ресурсов CosmosDB SQL, MongoDB, Cassandra, Gremlin и ресурсов таблиц, а также пропускной способности ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-933">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="2b0ed-934">HDInsight</span><span class="sxs-lookup"><span data-stu-id="2b0ed-934">HDInsight</span></span>

<span data-ttu-id="2b0ed-935">Этот выпуск содержит большое число критических изменений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-935">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="2b0ed-936">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-936">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="2b0ed-937">Переименование `--storage-default-container` в `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-937">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="2b0ed-938">Переименование `--storage-default-filesystem` в `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-938">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="2b0ed-939">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--name` для `application create`, чтобы представлять имя приложения вместо имени кластера.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-939">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="2b0ed-940">Добавлен аргумент `--cluster-name` для `application create`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-940">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="2b0ed-941">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-941">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="2b0ed-942">Переименование `--application-type` в `--type`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-942">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="2b0ed-943">Переименование `--marketplace-identifier` в `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-943">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="2b0ed-944">Переименование `--https-endpoint-access-mode` в `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-944">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="2b0ed-945">Переименован аргумент `--https-endpoint-destination-port` на `--destination-port`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-945">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="2b0ed-946">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-946">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="2b0ed-947">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Переименован аргумент `--target-instance-count` на `--workernode-count` для `hdinsight resize`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-947">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="2b0ed-948">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены все команды в группе `hdinsight script-action`, чтобы использовать параметр `--name` в качестве имени действия скрипта.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-948">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="2b0ed-949">Добавлен аргумент `--cluster-name` для всех команд `hdinsight script-action`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-949">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="2b0ed-950">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименован аргумент `--script-execution-id` на `--execution-id`для всех команд `hdinsight script-action`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-950">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="2b0ed-951">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `hdinsight script-action show` переименована в `hdinsight script-action show-execution-details`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-951">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="2b0ed-952">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Изменены параметры для `hdinsight script-action execute --roles`, чтобы они разделялись пробелами, а не запятыми.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-952">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="2b0ed-953">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--persisted` для `hdinsight script-action list`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-953">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="2b0ed-954">Изменен параметр `hdinsight create --cluster-configurations`, чтобы принимать путь к локальному файлу JSON или строке JSON.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-954">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="2b0ed-955">Добавлена команда `hdinsight script-action list-execution-history`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-955">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="2b0ed-956">Изменен параметр `hdinsight monitor enable --workspace`, чтобы принимать идентификатор или имя рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-956">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="2b0ed-957">Добавлен аргумент `hdinsight monitor enable --primary-key`, который требуется, если в качестве параметра указан идентификатор рабочей области.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-957">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="2b0ed-958">Добавлены дополнительные примеры и обновленные описания для справочных сообщений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-958">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="2b0ed-959">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="2b0ed-959">Interactive</span></span>

* <span data-ttu-id="2b0ed-960">Исправлена ошибка загрузки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-960">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="2b0ed-961">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="2b0ed-961">Kubernetes</span></span>

* <span data-ttu-id="2b0ed-962">Теперь используется `https`, если порт контейнера панели мониторинга использует `https`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-962">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-963">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-963">Network</span></span>

* <span data-ttu-id="2b0ed-964">Добавлен аргумент `--yes` для `network dns record-set cname delete`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-964">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="2b0ed-965">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-965">Profile</span></span>

* <span data-ttu-id="2b0ed-966">Добавлен аргумент `--resource-type` для `account get-access-token`, чтобы получать маркеры доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-966">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="2b0ed-967">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="2b0ed-967">ServiceFabric</span></span>

* <span data-ttu-id="2b0ed-968">Добавлены все поддерживаемые версии ОС для команды sf cluster create.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-968">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="2b0ed-969">Исправлена ошибка проверки основного сертификата.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-969">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-970">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-970">Storage</span></span>

* <span data-ttu-id="2b0ed-971">Добавлена команда `storage copy`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-971">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="2b0ed-972">30 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-972">July 30, 2019</span></span>

<span data-ttu-id="2b0ed-973">Версия 2.0.70</span><span class="sxs-lookup"><span data-stu-id="2b0ed-973">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-974">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-974">ACR</span></span>

* <span data-ttu-id="2b0ed-975">Исправлена проблема № 9952 (регрессия в команде `acr pack build`).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-975">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="2b0ed-976">Удалено имя образа построителя по умолчанию в `acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-976">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-977">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-977">Appservice</span></span>

* <span data-ttu-id="2b0ed-978">Команда `webapp config ssl` изменена для отображения сообщения, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-978">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="2b0ed-979">Исправлена проблема, когда команда `functionapp create` не принимала тип учетной записи хранения `Standard_RAGRS`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-979">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="2b0ed-980">Исправлена проблема, когда команда `webapp up` завершала работу со сбоем в случае выполнения со старой версией Python.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-980">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-981">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-981">Network</span></span>

* <span data-ttu-id="2b0ed-982">Удален недопустимый параметр `--ids` из `network nic ip-config add` (исправление проблемы № 9861).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-982">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="2b0ed-983">Исправлена проблема № 9604.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-983">Fixes #9604.</span></span> <span data-ttu-id="2b0ed-984">Добавлен параметр `--root-certs` в `network application-gateway http-settings [create|update]` для поддержки связанных с пользователем доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-984">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="2b0ed-985">Исправлен аргумент `--subscription` для `network dns record-set ns create` (проблема № 9965).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-985">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="2b0ed-986">RBAC</span><span class="sxs-lookup"><span data-stu-id="2b0ed-986">RBAC</span></span>

* <span data-ttu-id="2b0ed-987">Добавлена команда `user update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-987">Added `user update` command</span></span>
* <span data-ttu-id="2b0ed-988">[УСТАРЕЛО]`--upn-or-object-id` не рекомендуется использовать в связанных с пользователями командах.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-988">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="2b0ed-989">Вместо этого применяйте аргумент `--id`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-989">Use replacement argument `--id`</span></span>
* <span data-ttu-id="2b0ed-990">Добавлен аргумент `--id` в связанные с пользователями команды.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-990">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-991">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-991">SQL</span></span>

* <span data-ttu-id="2b0ed-992">Добавлены команды управления для ключей и предохранителя TDE управляемого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-992">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-993">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-993">Storage</span></span>

* <span data-ttu-id="2b0ed-994">Добавлена команда `storage remove`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-994">Added `storage remove` command</span></span>
* <span data-ttu-id="2b0ed-995">Исправлена проблема с `storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-995">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-996">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-996">VM</span></span>

* <span data-ttu-id="2b0ed-997">Изменена команда `list-skus` для использования новой версии API для вывода сведений о зонах.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-997">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="2b0ed-998">Изменено значение по умолчанию параметра `--single-placement-group` на `false` для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-998">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="2b0ed-999">Добавлена возможность выбирать номера SKU хранилища ZRS для `[snapshot|disk] create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-999">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="2b0ed-1000">Добавлена новая группа команд `vm host` для поддержки выделенных узлов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1000">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="2b0ed-1001">Добавлены параметры `--host` и `--host-group` в команде `vm create` для указания выделенного узла виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1001">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="2b0ed-1002">16 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1002">July 16, 2019</span></span>

<span data-ttu-id="2b0ed-1003">Версия 2.0.69</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1003">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-1004">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1004">Appservice</span></span>

* <span data-ttu-id="2b0ed-1005">Изменены команды `webapp identity`. Теперь они возвращают правильное сообщение об ошибке, если параметр ResourceGroupName или имя приложения недопустимы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1005">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="2b0ed-1006">Исправлена команда `webapp list`. Теперь она возвращает правильное значение для параметра numberOfSites, если не указан параметр ResourceGroup.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1006">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="2b0ed-1007">Исправлены побочные эффекты для команд `appservice plan create` и `webapp create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1007">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-1008">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1008">Core</span></span>

* <span data-ttu-id="2b0ed-1009">Исправлена ошибка, при которой отображался параметр `--subscription`, хотя он был неприменим.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1009">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="2b0ed-1010">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1010">Batch</span></span>

* <span data-ttu-id="2b0ed-1011">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `batch pool node-agent-skus list` заменена на `batch pool supported-images list`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1011">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="2b0ed-1012">Добавлена поддержка правил безопасности, которые блокируют сетевой доступ к пулу на основе исходного порта трафика при использовании параметра `--json-file` команды `batch pool create network`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1012">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="2b0ed-1013">Добавлена поддержка выполнения задачи в рабочей папке контейнера или рабочей папке задачи пакета при использовании параметра `--json-file` команды `batch task create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1013">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="2b0ed-1014">Исправлена ошибка в параметре `--application-package-references` команды `batch pool create`, которая позволяла работать только со значениями по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1014">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="2b0ed-1015">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1015">Eventhubs</span></span>

* <span data-ttu-id="2b0ed-1016">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1016">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="2b0ed-1017">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1017">RDBMS</span></span>

* <span data-ttu-id="2b0ed-1018">Добавлен необязательный параметр для указания номера SKU реплики в команде создания реплики.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1018">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="2b0ed-1019">Исправлена ошибка теста CI при создании реплики MySQL.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1019">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="2b0ed-1020">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1020">Relay</span></span>

* <span data-ttu-id="2b0ed-1021">Исправлена проблема с гибридным подключением при выключенной авторизации клиента ([8775](https://github.com/azure/azure-cli/issues/8775)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1021">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="2b0ed-1022">Добавлен параметр `--requires-transport-security` для команды `relay wcfrelay create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1022">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="2b0ed-1023">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1023">Servicebus</span></span>

* <span data-ttu-id="2b0ed-1024">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1024">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-1025">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1025">Storage</span></span>

* <span data-ttu-id="2b0ed-1026">Добавлена возможность обновления учетной записи хранения для AADDS в службе "Файлы".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1026">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="2b0ed-1027">Устранена проблема, описанная здесь: `storage blob service-properties update --set`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1027">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="2b0ed-1028">2 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1028">July 2, 2019</span></span>

<span data-ttu-id="2b0ed-1029">Версия 2.0.68</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1029">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-1030">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1030">Core</span></span>

* <span data-ttu-id="2b0ed-1031">Командные модули теперь объединены в один распространяемый пакет Python.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1031">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="2b0ed-1032">В результате этого прекращается непосредственное использование множества пакетов `azure-cli-` в PyPI.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1032">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="2b0ed-1033">Это также должно уменьшить размер установки и повлияет только на пользователей, которые выполняли установку непосредственно через `pip`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1033">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-1034">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1034">ACR</span></span>

* <span data-ttu-id="2b0ed-1035">В заданиях добавлена поддержка триггеров таймера.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1035">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-1036">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1036">Appservice</span></span>

* <span data-ttu-id="2b0ed-1037">Внесены изменения в `functionapp create` для включения Application Insights по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1037">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="2b0ed-1038">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена устаревшая команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1038">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="2b0ed-1039">Вместо нее используйте новую команду `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1039">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="2b0ed-1040">В `functionapp deployment config-zip` добавлена поддержка плана потребления приложения-функции Linux.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1040">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="2b0ed-1041">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1041">Cosmos DB</span></span>

* <span data-ttu-id="2b0ed-1042">Добавлена возможность отключения TTL.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1042">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="2b0ed-1043">DLS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1043">DLS</span></span>

* <span data-ttu-id="2b0ed-1044">Обновленная версия ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1044">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="2b0ed-1045">Отзывы</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1045">Feedback</span></span>

* <span data-ttu-id="2b0ed-1046">При сообщении о сбое при выполнении команды расширения `az feedback` теперь пытается открыть браузер по URL-адресу репозитория или проекта расширения из индекса.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1046">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="2b0ed-1047">HDInsight</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1047">HDInsight</span></span>

* <span data-ttu-id="2b0ed-1048">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя группы команд `oms` изменилось на `monitor`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1048">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="2b0ed-1049">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--http-password/-p` стал обязательным.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1049">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="2b0ed-1050">Добавлены средства заполнения для `--cluster-admin-account` и средство заполнения для параметров `cluster-users-group-dns`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1050">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="2b0ed-1051">Параметр `cluster-users-group-dns` стал обязательным, если присутствует `—esp`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1051">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="2b0ed-1052">Добавлено время ожидания для всех существующих средств автоматического заполнения аргументов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1052">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="2b0ed-1053">Добавлено время ожидания для преобразования имени ресурса в идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1053">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="2b0ed-1054">Внесены изменения в средства автоматического заполнения для выбора ресурсов из любой группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1054">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="2b0ed-1055">Это может быть группа ресурсов, отличная от той, которая указана с помощью `-g`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1055">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="2b0ed-1056">Добавлена поддержка параметров `--sub-domain-suffix` и `--disable_gateway_auth` в команде `hdinsight application create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1056">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="2b0ed-1057">Управляемые службы</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1057">Managed Services</span></span>

* <span data-ttu-id="2b0ed-1058">Командный модуль управляемых служб выпущен в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1058">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="2b0ed-1059">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1059">Profile</span></span>
* <span data-ttu-id="2b0ed-1060">Аргумент `--subscription` подавляется для команды выхода.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1060">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="2b0ed-1061">RBAC</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1061">RBAC</span></span>

* <span data-ttu-id="2b0ed-1062">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален аргумент `--password` для `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1062">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="2b0ed-1063">В команду `create` добавлен параметр `--assignee-principal-type` для устранения периодических сбоев из-за задержки репликации сервера AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1063">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="2b0ed-1064">Исправлен сбой в `ad signed-in-user` при перечислении собственных объектов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1064">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="2b0ed-1065">Исправлена проблема, при которой `ad sp` не удавалось найти нужное приложение в субъекте-службе.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1065">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="2b0ed-1066">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1066">RDBMS</span></span>

* <span data-ttu-id="2b0ed-1067">Добавлена поддержка репликации MariaDB.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1067">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-1068">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1068">SQL</span></span>

* <span data-ttu-id="2b0ed-1069">Описаны допустимые значения для `sql db create --sample-name`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1069">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-1070">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1070">Storage</span></span>

* <span data-ttu-id="2b0ed-1071">В `storage blob generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1071">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="2b0ed-1072">В `storage container generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1072">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="2b0ed-1073">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1073">VM</span></span>

* <span data-ttu-id="2b0ed-1074">Исправлена ошибка, при которой команда `vmss create` возвращала сообщение об ошибке при выполнении с `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1074">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="2b0ed-1075">Прекращена проверка `vmss create --single-placement-group` на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1075">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="2b0ed-1076">Команда не завершается сбоем, если для `--single-placement-group` задано значение `true`, а значение `--instance-count` больше 100 или указаны зоны доступности. Сама проверка теперь выполняется службой вычислений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1076">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="2b0ed-1077">Исправлена ошибка, при которой команда `[vm|vmss] extension image list` завершалась сбоем при указании `--latest`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1077">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="2b0ed-1078">18 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1078">June 18, 2019</span></span>

<span data-ttu-id="2b0ed-1079">Версия 2.0.67</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1079">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-1080">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1080">Core</span></span>

<span data-ttu-id="2b0ed-1081">В этом выпуске добавлен новый тег [Предварительная версия], который яснее дает понять, что группа команд, команда или аргумент находятся в состоянии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1081">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="2b0ed-1082">Ранее это указывалось в тексте справки или подразумевалось в номере версии командного модуля.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1082">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="2b0ed-1083">В будущем в интерфейсе командной строки номера версий отдельных пакетов не будут указываться.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1083">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="2b0ed-1084">Если команда доступна в предварительной версии, это также касается и всех ее аргументов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1084">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="2b0ed-1085">Если группа команд помечается как находящаяся в предварительной версии, значит все команды и аргументы также считаются доступными в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1085">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="2b0ed-1086">В результате этого изменения несколько групп команд могут "внезапно" оказаться в состоянии предварительной версии в этом выпуске.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1086">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="2b0ed-1087">В действительности большинство пакетов, которые находились в состоянии предварительной версии, в этом выпуске будут считаться общедоступными.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1087">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-1088">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1088">ACR</span></span>
* <span data-ttu-id="2b0ed-1089">Добавлена команда acr check-health.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1089">Added 'acr check-health' command</span></span>
* <span data-ttu-id="2b0ed-1090">Улучшена обработка ошибок с маркерами безопасности AAD и ошибок при получении внешних команд.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1090">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-1091">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1091">ACS</span></span>
* <span data-ttu-id="2b0ed-1092">Устаревшие команды ACS теперь скрыты в тексте справки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1092">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="2b0ed-1093">AMS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1093">AMS</span></span>
* <span data-ttu-id="2b0ed-1094">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в возврате строк времени ISO 8601 для archive-window-length и key-frame-interval-duration.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1094">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-1095">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1095">AppService</span></span>
* <span data-ttu-id="2b0ed-1096">Добавлена маршрутизация на основе расположение для `webapp deleted list` и `webapp deleted restore`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1096">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="2b0ed-1097">Исправлена проблема, при которой целевой URL-адрес веб-приложения ("Вы можете запустить приложение в...") не был активным в Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1097">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="2b0ed-1098">Устранена проблема, при которой создание приложений в некоторых SKU завершалось сбоем с ошибкой AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1098">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="2b0ed-1099">Добавлена предварительная проверка в `[appservice|webapp] create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1099">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="2b0ed-1100">Исправлено `[webapp|functionapp] traffic-routing` для использования правильного actionHostName.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1100">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="2b0ed-1101">Добавлена поддержка слотов для команд `functionapp`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1101">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="2b0ed-1102">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1102">Batch</span></span>
* <span data-ttu-id="2b0ed-1103">Исправлена регрессия проверки подлинности AAD, которую вызывал чрезмерный поток уведомлений об авторизации с помощью общего ключа.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1103">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="2b0ed-1104">Batch AI</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1104">BatchAI</span></span>
* <span data-ttu-id="2b0ed-1105">Команды BatchAI теперь признаны устаревшими и скрыты.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1105">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="2b0ed-1106">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1106">BotService</span></span>
* <span data-ttu-id="2b0ed-1107">Добавлены предупреждающие сообщения о прекращении поддержки и режиме обслуживания для команд, которые поддерживают пакет SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1107">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2b0ed-1108">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1108">CosmosDB</span></span>
* <span data-ttu-id="2b0ed-1109">[УСТАРЕЛО] использовать команду `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1109">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="2b0ed-1110">Добавлена команда `cosmosdb keys list`, заменяющая `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1110">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="2b0ed-1111">`cosmsodb create/update`: Добавлен новый формат для --location, который позволяет задавать свойство isZoneRedundant.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1111">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="2b0ed-1112">Нерекомендуемый старый формат.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1112">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="2b0ed-1113">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1113">EventGrid</span></span>
* <span data-ttu-id="2b0ed-1114">Добавлены команды `eventgrid domain` для операций CRUD домена.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1114">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="2b0ed-1115">Добавлены команды `eventgrid domain topic` для операций CRUD разделов домена.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1115">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="2b0ed-1116">В `eventgrid [topic|event-subscription] list` добавлен аргумент `--odata-query` для фильтрации результатов с использованием синтаксиса OData.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1116">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="2b0ed-1117">`event-subscription create/update`: Добавлена ServiceBusQueue в качестве новых значений для параметра `--endpoint-type`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1117">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="2b0ed-1118">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в прекращении поддержки `--included-event-types All` с `eventgrid event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1118">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="2b0ed-1119">HDInsight</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1119">HDInsight</span></span>
* <span data-ttu-id="2b0ed-1120">Добавлена поддержка параметра `--ssh-public-key` в команде `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1120">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="2b0ed-1121">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1121">IoT</span></span>
* <span data-ttu-id="2b0ed-1122">Добавлена поддержка для повторного создания ключей политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1122">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="2b0ed-1123">Добавлен пакет SDK и поддержка для службы подготовки репозитория DigitalTwin.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1123">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-1124">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1124">Network</span></span>
* <span data-ttu-id="2b0ed-1125">Добавлена поддержка зон для Шлюза NAT.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1125">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="2b0ed-1126">Добавлена команда `network list-service-tags`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1126">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="2b0ed-1127">Исправлена проблема с `dns zone import`, при которой пользователям не удавалось импортировать записи А с подстановочным знаком.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1127">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="2b0ed-1128">Исправлена проблема с `watcher flow-log configure`, при которой не удавалось включить ведение журнала потоков в определенных регионах.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1128">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-1129">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1129">Resource</span></span>
* <span data-ttu-id="2b0ed-1130">Добавлена команда `az rest` для вызовов REST.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1130">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="2b0ed-1131">Исправлена ошибка, возникавшая при использовании `policy assignment list` с группой ресурсов или уровнем подписки `--scope`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1131">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="2b0ed-1132">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1132">ServiceBus</span></span>
* <span data-ttu-id="2b0ed-1133">Устранена проблема № [9319](https://github.com/azure/azure-cli/issues/9319) с `servicebus topic create --max-size`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1133">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-1134">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1134">SQL</span></span>
* <span data-ttu-id="2b0ed-1135">Параметр `--location` стал необязательным для `sql [server|mi] create`. Если он не указан, используется расположение группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1135">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="2b0ed-1136">Исправлена ошибка "Объект NoneType не подлежит итерации" с `sql db list-editions --available`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1136">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="2b0ed-1137">SQLVm</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1137">SQLVm</span></span>
* <span data-ttu-id="2b0ed-1138">Критическое изменение. Для `sql vm create` теперь требуется параметр `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1138">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="2b0ed-1139">Внесены изменения, позволяющие задавать SKU образа SQL при создании или обновлении виртуальной машины SQL.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1139">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-1140">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1140">Storage</span></span>
* <span data-ttu-id="2b0ed-1141">Исправлена проблема с отсутствующим ключом учетной записи для `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1141">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="2b0ed-1142">Исправлена проблема с `storage blob sync` на платформе Linux.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1142">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-1143">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1143">VM</span></span>
* <span data-ttu-id="2b0ed-1144">[Предварительная версия] Добавлены команды `vm image template` для создания образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1144">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="2b0ed-1145">4 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1145">June 4, 2019</span></span>

<span data-ttu-id="2b0ed-1146">Версия 2.0.66</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1146">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-1147">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1147">Core</span></span>
* <span data-ttu-id="2b0ed-1148">Исправлена ошибка, из-за которой выполнение команды завершалось со сбоем, если параметр `--output yaml` использовался с параметром `--query`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1148">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-1149">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1149">ACR</span></span>
* <span data-ttu-id="2b0ed-1150">Добавлена группа команд acr pack для создания заданий быстрой сборки с помощью пакетов сборок.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1150">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-1151">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1151">ACS</span></span>
* <span data-ttu-id="2b0ed-1152">Разрешено включение и отключение надстройки панели мониторинга Kubernetes для AKS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1152">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="2b0ed-1153">Если подписку нельзя использовать с Azure Red Hat OpenShift, будет отображаться соответствующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1153">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="2b0ed-1154">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1154">Batch</span></span>
* <span data-ttu-id="2b0ed-1155">Улучшена обработка ошибок, если не выполнен вход в учетную запись \[[№ 9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[№ 8978](https://github.com/Azure/azure-cli/issues/8978)\].</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1155">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="2b0ed-1156">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1156">IoT</span></span>
* <span data-ttu-id="2b0ed-1157">Добавлена поддержка для перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1157">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-1158">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1158">Network</span></span>
* <span data-ttu-id="2b0ed-1159">Добавлены команды `network application-gateway waf-policy` для поддержки настраиваемых правил WAF.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1159">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="2b0ed-1160">Добавлены аргументы `--waf-policy` и `--max-capacity` для команды `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1160">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="2b0ed-1161">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1161">Resource</span></span>
* <span data-ttu-id="2b0ed-1162">Улучшен вывод сообщения команды `deployment create` при отсутствии TTY.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1162">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-1163">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1163">Role</span></span>
* <span data-ttu-id="2b0ed-1164">Обновлен текст справки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1164">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="2b0ed-1165">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1165">Compute</span></span>
* <span data-ttu-id="2b0ed-1166">Добавлена поддержка команды `vm create` для создания виртуальных машин из управляемого образа с номерами LUN дисков данных, которые не начинаются с 0 или для которых пропущены номера.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1166">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="2b0ed-1167">21 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1167">May 21, 2019</span></span>

<span data-ttu-id="2b0ed-1168">Версия 2.0.65</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1168">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-1169">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1169">Core</span></span>
* <span data-ttu-id="2b0ed-1170">Улучшена функция обратной связи при ошибках аутентификации.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1170">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="2b0ed-1171">Исправлена проблема, из-за которой интерфейс командной строки загружал расширения, которые не были совместимы с его базовой версией.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1171">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="2b0ed-1172">Исправлена проблема с запуском и неисправностью `clouds.config`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1172">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-1173">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1173">ACR</span></span>
* <span data-ttu-id="2b0ed-1174">Добавлена поддержка управляемых удостоверений в Задачи.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1174">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-1175">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1175">ACS</span></span>
* <span data-ttu-id="2b0ed-1176">Исправлена команда `openshift create`, используемая с пользовательским клиентом AAD.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1176">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-1177">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1177">AppService</span></span>
* <span data-ttu-id="2b0ed-1178">[УСТАРЕЛО] Команда `functionapp devops-build` устарела и будет удалена в следующем выпуске.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1178">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="2b0ed-1179">Внесено изменение в `functionapp devops-pipeline` для получения журнала сборки из Azure DevOps в режиме подробного протоколирования.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1179">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="2b0ed-1180">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален неподдерживаемый флаг `--use_local_settings` из команды `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1180">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="2b0ed-1181">Внесено изменение в `webapp up` для возврата выходных данных JSON, если `--logs` не используется.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1181">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="2b0ed-1182">Добавлена поддержка записи ресурсов по умолчанию в локальную конфигурацию для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1182">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="2b0ed-1183">Добавлена поддержка `webapp up` для повторного развертывания приложения без использования аргумента `--location`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1183">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="2b0ed-1184">Устранена проблема, из-за которой нельзя было создать для Linux номер SKU с планом службы приложений "Бесплатный".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1184">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="2b0ed-1185">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1185">BotService</span></span>
* <span data-ttu-id="2b0ed-1186">Внесено изменение для включения поддержки всех регистров в параметрах `--lang` для команд.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1186">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="2b0ed-1187">Обновлено описание модуля команды.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1187">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="2b0ed-1188">Потребление</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1188">Consumption</span></span>
* <span data-ttu-id="2b0ed-1189">Добавлен отсутствующий обязательный параметр при выполнении `consumption usage list --billing-period-name`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1189">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="2b0ed-1190">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1190">IoT</span></span>
* <span data-ttu-id="2b0ed-1191">Добавлена поддержка перечисления всех ключей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1191">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-1192">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1192">Network</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="2b0ed-1194">Добавлен аргумент `--nat-gateway` для `network vnet subnet [create|update]` для подключения к шлюзу NAT.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1194">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="2b0ed-1195">Исправлена проблема с `dns zone import`, из-за которой имена записей не сопоставлялись с типом записей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1195">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="2b0ed-1196">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1196">RDBMS</span></span>
* <span data-ttu-id="2b0ed-1197">Добавлена поддержка Postgres и MySQL для георепликации.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1197">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="2b0ed-1198">RBAC</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1198">RBAC</span></span>
* <span data-ttu-id="2b0ed-1199">Добавлена поддержка области группы управления для `role assignment`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1199">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-1200">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1200">Storage</span></span>
* <span data-ttu-id="2b0ed-1201">`storage blob sync`: добавьте команду синхронизации для хранилища BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1201">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="2b0ed-1202">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1202">Compute</span></span>
* <span data-ttu-id="2b0ed-1203">Добавлен параметр `--computer-name` для `vm create` для установки имени виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1203">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="2b0ed-1204">Переименован параметр `--ssh-key-value` в `--ssh-key-values` для `[vm|vmss] create` для приема нескольких значений пути или открытого ключа SSH.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1204">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="2b0ed-1205">__Примечание.__ Это **не** критическое изменение, благодаря которому `--ssh-key-value` будет правильно анализироваться, так как соответствует только `--ssh-key-values`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1205">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="2b0ed-1206">Внесено изменение в аргумент `ppg create` для `--type` — теперь он необязательный.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1206">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="2b0ed-1207">6 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1207">May 6, 2019</span></span>

<span data-ttu-id="2b0ed-1208">Версия 2.0.64</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1208">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-1209">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1209">ACS</span></span>
* <span data-ttu-id="2b0ed-1210">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--fqdn` из команд `openshift`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1210">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="2b0ed-1211">Внесено изменение для использования общедоступной версии API для Azure Red Hat Openshift.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1211">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="2b0ed-1212">Добавлен флаг `customer-admin-group-id` в `openshift create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1212">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="2b0ed-1213">[Общедоступная версия.] `(PREVIEW)` больше не используется для `aks create` в параметре `--network-policy`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1213">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-1214">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1214">Appservice</span></span>
* <span data-ttu-id="2b0ed-1215">[УСТАРЕЛО] Команда `functionapp devops-build` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1215">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="2b0ed-1216">Команда переименована в `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1216">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="2b0ed-1217">Исправлен процесс получения правильного имени пользователя для Cloud Shell, приводивший к ошибке выполнения `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1217">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="2b0ed-1218">Обновлена документация по `appservice plan --sku` в соответствии с поддерживаемыми планами службы приложений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1218">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="2b0ed-1219">Добавлены необязательные аргументы для группы ресурсов и план для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1219">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="2b0ed-1220">Добавлена поддержка `webapp ssh` в соответствии с переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1220">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="2b0ed-1221">Добавлена поддержка `appserviceplan create` для ценовой категории "Бесплатный" в Linux.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1221">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="2b0ed-1222">Внесено изменение в `webapp up` для перевода в спящий режим на 30 с после установки параметра приложения `SCM_DO_BUILD_DURING_DEPLOYMENT=true` для обработки холодного запуска Kudu.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1222">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="2b0ed-1223">Добавлена поддержка среды выполнения `powershell` для `functionapp create` в Windows.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1223">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="2b0ed-1224">Добавлена команда `create-remote-connection`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1224">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="2b0ed-1225">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1225">Batch</span></span>
* <span data-ttu-id="2b0ed-1226">Исправлена ошибка в проверяющем элементе управления для параметров `--application-package-references`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1226">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="2b0ed-1227">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1227">Botservice</span></span>
* <span data-ttu-id="2b0ed-1228">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` для создания пустого бота веб-приложения по умолчанию (т. е. бот не развертывается в Службе приложений).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1228">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="2b0ed-1229">Добавлен флаг `--echo` в `bot create` для использования старого поведения с `-v v4`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1229">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="2b0ed-1230">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено значение по умолчанию `--version` на `v4`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1230">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="2b0ed-1231">__ПРИМЕЧАНИЕ.__ `bot prepare-publish` по-прежнему использует старое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1231">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="2b0ed-1232">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `--lang` — значение `Csharp` больше не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1232">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="2b0ed-1233">Если команда требует `--lang`, который не указан, команда завершит работу с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1233">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="2b0ed-1234">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в аргументы `--appid` и `--password` для `bot create` — теперь они являются обязательными и их можно создать с помощью `ad app create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1234">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="2b0ed-1235">Добавлена проверка `--appid` и `--password`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1235">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="2b0ed-1236">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4`, чтобы не создавать или не использовать учетную запись хранения или Application Insights.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1236">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="2b0ed-1237">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v3`, чтобы требовать регион, где доступна служба Application Insights.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1237">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="2b0ed-1238">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot update`, чтобы влиять только на определенные свойства бота.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1238">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="2b0ed-1239">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в флаг `--lang` для принятия `Javascript` вместо `Node`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1239">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="2b0ed-1240">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`Node` больше не используется как допустимое значение `--lang`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1240">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="2b0ed-1241">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` — значение `SCM_DO_BUILD_DURING_DEPLOYMENT` больше не равно true.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1241">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="2b0ed-1242">Все развертывания через Kudu будут работать в соответствии с поведением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1242">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="2b0ed-1243">Внесено изменение в `bot download` для ботов без файлов `.bot`, чтобы создавать файл конфигурации для определенного языка со значениями из параметров приложения для бота.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1243">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="2b0ed-1244">В команду `bot prepare-deploy` добавлена поддержка параметра `Typescript`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1244">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="2b0ed-1245">Добавлено предупреждающее сообщение в `bot prepare-deploy` для ботов `Javascript` и `Typescript`, когда `--code-dir` не содержит `package.json`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1245">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="2b0ed-1246">Внесено изменение в `bot prepare-deploy` для возврата `true` при успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1246">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="2b0ed-1247">Включено ведение подробного журнала для `bot prepare-deploy`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1247">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="2b0ed-1248">Добавлены более доступные регионы Application Insights для `az bot create -v v3`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1248">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="2b0ed-1249">Configure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1249">Configure</span></span>
* <span data-ttu-id="2b0ed-1250">Добавлена поддержка конфигурации по умолчанию для аргумента на основе папки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1250">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="2b0ed-1251">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1251">Eventhubs</span></span>
* <span data-ttu-id="2b0ed-1252">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1252">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="2b0ed-1253">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1253">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-1254">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1254">Network</span></span>
* <span data-ttu-id="2b0ed-1255">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--cache` на `--defer` для `vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1255">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="2b0ed-1256">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1256">Policy Insights</span></span>
* <span data-ttu-id="2b0ed-1257">Добавлена поддержка `--expand PolicyEvaluationDetails` для результатов оценки политики запросов для ресурса.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1257">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-1258">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1258">Role</span></span>
* <span data-ttu-id="2b0ed-1259">[УСТАРЕЛО] Внесено изменение в `create-for-rbac` для скрытия аргумента --password (поддержка прекращается в мае 2019 г.).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1259">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="2b0ed-1260">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1260">Service Bus</span></span>
* <span data-ttu-id="2b0ed-1261">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1261">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="2b0ed-1262">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1262">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="2b0ed-1263">Внесено исправление в `topic [create|update]` — теперь `--max-size` поддерживает значения 10, 20, 40 и 80 ГБ для номера SKU ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1263">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-1264">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1264">SQL</span></span>
* <span data-ttu-id="2b0ed-1265">Добавлены команды `sql virtual-cluster [list|show|delete]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1265">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-1266">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1266">VM</span></span>
* <span data-ttu-id="2b0ed-1267">Добавлены параметры `--protect-from-scale-in` и `--protect-from-scale-set-actions` для `vmss update`, чтобы включать обновления политики защиты для экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1267">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="2b0ed-1268">Добавлены параметры `--instance-id` для `vmss update` для включения общего обновления экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1268">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="2b0ed-1269">Добавлен параметр `--instance-id` для команды `vmss wait`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1269">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="2b0ed-1270">Добавлена новая группа команд `ppg` для управления группами размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1270">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="2b0ed-1271">Добавлен параметр `--ppg` для `[vm|vmss] create` и `vm availability-set create` для управления PPG.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1271">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="2b0ed-1272">Добавлен параметр `--hyper-v-generation` для команды `image create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1272">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="2b0ed-1273">23 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1273">April 23, 2019</span></span>

<span data-ttu-id="2b0ed-1274">Версия 2.0.63</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1274">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-1275">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1275">ACS</span></span>
* <span data-ttu-id="2b0ed-1276">Внесено изменение в `aks get-credentials` для запроса на перезапись повторяющихся значений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1276">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="2b0ed-1277">Удалено описание `(PREVIEW)` из команд Dev Spaces aks use-dev-spaces и aks remove-dev-spaces.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1277">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="2b0ed-1278">AMS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1278">AMS</span></span>
* <span data-ttu-id="2b0ed-1279">Исправлена ошибка с обновлением фильтров ресурсов и учетных записей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1279">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-1280">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1280">AppService</span></span>
* <span data-ttu-id="2b0ed-1281">Добавлена поддержка ASE и времени ожидания для `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1281">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="2b0ed-1282">Добавлена возможность настройки непрерывной интеграции и развертывания в конвейере Azure DevOps из репозитория Github для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1282">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="2b0ed-1283">Добавлен аргумент `--github-pat` для `functionapp devops-build create` для получения личного маркера доступа Github.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1283">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="2b0ed-1284">Добавлен аргумент `--github-repository` для `functionapp devops-build create` для подключения репозитория Github, который содержит исходный код приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1284">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="2b0ed-1285">Исправлена проблема со сбоем `az webapp up --logs` и обновлением .Net Core до версии 2.1 по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1285">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="2b0ed-1286">Удалены ненужные параметры приложения-функции при создании приложения-функции с помощью плана потребления.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1286">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="2b0ed-1287">Внесены изменения в `webapp up`, чтобы строка ASP по умолчанию добавляла номера в конец для создания плана службы приложений на основе параметров SKU.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1287">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="2b0ed-1288">Добавлен параметр `-b` для `webapp up` для запуска приложения в браузере.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1288">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="2b0ed-1289">Внесены изменения в `webapp deployment source config zip` для обработки переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1289">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="2b0ed-1290">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1290">Deployment Manager</span></span>
* <span data-ttu-id="2b0ed-1291">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Создание и администрирование артефактов, которые поддерживают развертывания</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1291">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="2b0ed-1292">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1292">Lab</span></span>
* <span data-ttu-id="2b0ed-1293">Исправлена ошибка, которая приводила к неожиданному завершению работы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1293">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-1294">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1294">Network</span></span>
* <span data-ttu-id="2b0ed-1295">Добавлено автоматическое делегирование сервера имен для `dns zone create` в родительском объекте во время создания дочерней зоны.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1295">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-1296">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1296">Resource</span></span>
* <span data-ttu-id="2b0ed-1297">[УСТАРЕЛО] Не рекомендуются к использованию аргументы `--link-id`, `--target-id` и `--filter-string` для `resource link`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1297">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="2b0ed-1298">Используйте вместо них аргументы `--link`, `--target` и `--filter`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1298">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="2b0ed-1299">Исправлена проблема, из-за которой команды `resource link [create|update]` не работали.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1299">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="2b0ed-1300">Исправлена проблема, из-за которой удаление с помощью идентификатора ресурса приводило к сбою или ошибке.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1300">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-1301">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1301">SQL</span></span>
* <span data-ttu-id="2b0ed-1302">Добавлена поддержка пользовательского часового пояса в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1302">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="2b0ed-1303">Внесено изменение, чтобы разрешить использовать имя эластичного пула с `sql db update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1303">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="2b0ed-1304">В команду `sql server [create|update]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1304">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="2b0ed-1305">Добавлена команда `sql server wait`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1305">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-1306">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1306">Storage</span></span>
* <span data-ttu-id="2b0ed-1307">Устранена проблема с двойной кодировкой маркеров SAS в `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1307">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-1308">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1308">VM</span></span>
* <span data-ttu-id="2b0ed-1309">Добавлен флаг `--skip-shutdown` для `vm|vmss stop` для выключения виртуальных машин без завершения работы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1309">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="2b0ed-1310">Добавлен аргумент `--storage-account-type` для `sig image-version create` настройки типа учетной записи профиля публикации.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1310">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="2b0ed-1311">Добавлен аргумент `--target-regions` для `sig image-version create` для указания типов учетных записей хранения, связанных с регионами.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1311">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="2b0ed-1312">9 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1312">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-1313">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1313">Core</span></span>
* <span data-ttu-id="2b0ed-1314">Исправлена проблема, из-за которой для некоторых расширений отображалась версия `Unknown` и ее невозможно было обновить.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1314">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-1315">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1315">ACR</span></span>
* <span data-ttu-id="2b0ed-1316">Добавлена поддержка запуска образа без контекста.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1316">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="2b0ed-1317">AMS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1317">AMS</span></span>
* [УСТАРЕЛО]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="2b0ed-1320">Добавлена поддержка новых параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1320">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="2b0ed-1321">Добавлен новый параметр `--filters` для `ams streaming-locator create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1321">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-1322">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1322">AppService</span></span>
* <span data-ttu-id="2b0ed-1323">В команду `webapp up` добавлена поддержка параметра `--logs`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1323">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="2b0ed-1324">Исправлены ошибки в команде `functionapp devops-build create` при создании файла `azure-pipelines.yml`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1324">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="2b0ed-1325">Улучшена обработка и индикаторы ошибок с `unctionapp devops-build create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1325">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="2b0ed-1326">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--local-git` для команды `devops-build`. Обнаружение и обработка локального репозитория Git являются обязательными для создания конвейеров DevOps в Azure.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1326">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="2b0ed-1327">Добавлена поддержка создания плана функций Linux.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1327">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="2b0ed-1328">Добавлена возможность менять план для приложения-функции с помощью `functionapp update --plan`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1328">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="2b0ed-1329">Добавлена поддержка параметров горизонтального увеличения масштаба плана "Премиум" для Функций Azure.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1329">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="2b0ed-1330">CDN</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1330">CDN</span></span>
* <span data-ttu-id="2b0ed-1331">Добавлена поддержка `Microsoft_Standard` и `Standard_ChinaCdn`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1331">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="2b0ed-1332">Отзывы</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1332">Feedback</span></span>
* <span data-ttu-id="2b0ed-1333">Внесены изменения в `feedback` для отображения метаданных недавно выполненных команд.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1333">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="2b0ed-1334">Внесены изменения в `feedback`. Теперь при регистрации проблемы отображается запрос, в соответствии с которым пользователь должен открыть браузер и воспользоваться шаблоном проблемы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1334">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="2b0ed-1335">Внесены изменения в `feedback`. Теперь текст проблемы выводится при запуске с параметром --verbose.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1335">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-1336">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1336">Monitor</span></span>
* <span data-ttu-id="2b0ed-1337">Исправлена проблема, из-за которой у параметра count было недопустимое значение в `metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1337">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="2b0ed-1338">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1338">Network</span></span>
* <span data-ttu-id="2b0ed-1339">Исправлен формат таблицы, которая не отображалась с помощью `vnet-gateway list-bgp-peer-status`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1339">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="2b0ed-1340">Добавлены команды `list-request-headers` и `list-response-headers` для `application-gateway rewrite-rule`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1340">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="2b0ed-1341">Добавлена команда `list-server-variables` для `application-gateway rewrite-rule condition`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1341">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="2b0ed-1342">Исправлена проблема, из-за которой обновление состояния соединения на порту ExpressRoute вызывало неизвестное исключение атрибута `express-route port update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1342">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="2b0ed-1343">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1343">PrivateDNS</span></span>
* <span data-ttu-id="2b0ed-1344">Добавлена команда `network private-dns` для частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1344">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-1345">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1345">Resource</span></span>
* <span data-ttu-id="2b0ed-1346">Исправлена проблема с `deployment create` и `group deployment create`, из-за которой файл параметров с пустым набором параметров не работал.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1346">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-1347">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1347">Role</span></span>
* <span data-ttu-id="2b0ed-1348">Внесены исправления в `create-for-rbac`. Теперь `--years` обрабатывается правильно.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1348">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="2b0ed-1349">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `role assignment delete`. Теперь появляется запрос при удалении всех назначений в рамках подписки без дополнительных условий.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1349">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-1350">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1350">SQL</span></span>
* <span data-ttu-id="2b0ed-1351">Команда `sql mi [create|update]` обновлена с помощью свойств proxyOverride и publicDataEndpointEnabled.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1351">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-1352">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1352">Storage</span></span>
* <span data-ttu-id="2b0ed-1353">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален результат выполнения `storage blob delete`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1353">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="2b0ed-1354">В команду `storage blob generate-sas` добавлен параметр `--full-uri` для создания полного URI большого двоичного объекта с помощью SAS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1354">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="2b0ed-1355">В команду `storage file copy start` добавлен параметр `--file-snapshot` для копирования файла из моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1355">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="2b0ed-1356">Внесены изменения в `storage blob copy cancel`. Теперь вместо исключения для NoPendingCopyOperation отображается только сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1356">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="2b0ed-1357">26 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1357">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="2b0ed-1358">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1358">Core</span></span>
* <span data-ttu-id="2b0ed-1359">Устранены проблемы с несовместимостью расширений для разработки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1359">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="2b0ed-1360">Функция обработки ошибок теперь указывает клиентам на страницу проблем.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1360">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="2b0ed-1361">Cloud</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1361">Cloud</span></span>
* <span data-ttu-id="2b0ed-1362">Исправлена ошибка с сообщением о не найденной подписке в `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1362">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-1363">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1363">ACR</span></span>
* <span data-ttu-id="2b0ed-1364">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1364">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="2b0ed-1365">Добавлено `--auth-mode` в команды `acr build`, `acr run`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1365">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="2b0ed-1366">Добавлена команда acr task credential для управления учетными данными для задачи.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1366">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="2b0ed-1367">Добавлено --no-wait в команду `acr build`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1367">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-1368">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1368">AppService</span></span>
* <span data-ttu-id="2b0ed-1369">Исправлена ошибка с `webapp up`, из-за которой нельзя было правильно выполнить запуск из пустого каталога или скрипта неизвестного кода.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1369">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="2b0ed-1370">Исправлена ошибка, из-за которой не работали слоты для `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1370">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="2b0ed-1371">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1371">BOT Service</span></span>
* <span data-ttu-id="2b0ed-1372">Добавлено `bot prepare-deploy` для подготовки к развертыванию ботов с помощью `webapp`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1372">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="2b0ed-1373">Изменено `bot create --kind registration` для отображения пароля, если пароль не указан.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1373">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="2b0ed-1374">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--endpoint` в `bot create --kind registration` на пустую строку (по умолчанию) вместо запрашиваемой.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1374">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="2b0ed-1375">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1375">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="2b0ed-1376">CDN</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1376">CDN</span></span>
* <span data-ttu-id="2b0ed-1377">Добавлена поддержка параметра `--no-wait` в команде `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1377">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="2b0ed-1378">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено поведение кэширования строки запроса `cdn endpoint create` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1378">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="2b0ed-1379">IgnoreQueryString больше не используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1379">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="2b0ed-1380">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1380">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2b0ed-1381">Сosmos DB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1381">Cosmosdb</span></span>
* <span data-ttu-id="2b0ed-1382">Добавлена поддержка `--enable-multiple-write-locations` для обновления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1382">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="2b0ed-1383">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1383">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="2b0ed-1384">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1384">Interactive</span></span>
* <span data-ttu-id="2b0ed-1385">Исправлена несовместимость с интерактивным расширением, установленным с помощью azdev.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1385">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-1386">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1386">Monitor</span></span>
* <span data-ttu-id="2b0ed-1387">Внесено изменение, разрешающее использовать значение измерения `*` для `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1387">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-1388">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1388">Network</span></span>
* <span data-ttu-id="2b0ed-1389">Добавлена группа команд `rewrite-rule` для `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1389">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="2b0ed-1390">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1390">Profile</span></span>
* <span data-ttu-id="2b0ed-1391">Включена поддержка учетной записи уровня клиентов для управляемого удостоверения службы для `login`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1391">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="2b0ed-1392">Postgres</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1392">Postgres</span></span> 
* <span data-ttu-id="2b0ed-1393">Добавлены команды postgresql `replica` и команда `restart server`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1393">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="2b0ed-1394">Внесены изменения для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1394">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-1395">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1395">Resource</span></span>
* <span data-ttu-id="2b0ed-1396">Улучшены табличные выходные данные для `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1396">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="2b0ed-1397">Исправлена проблема с `deployment [create|validate]`, из-за которой secureObject типа не распознавался.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1397">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="2b0ed-1398">График</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1398">Graph</span></span>
* <span data-ttu-id="2b0ed-1399">Добавлена поддержка параметра `--end-date` в команде `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1399">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="2b0ed-1400">Добавлена поддержка разрешений для `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1400">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="2b0ed-1401">Исправлена проблема с `ad app permission list`, из-за которой отсутствовали разрешения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1401">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="2b0ed-1402">Изменено `ad sp delete` для пропуска удаления назначения роли, если текущая учетная запись не содержит подписок.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1402">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="2b0ed-1403">Изменено `ad app create` для использования `--identifier-uris` пустого списка (по умолчанию), если список не указан.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1403">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-1404">носителей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1404">storage</span></span>
* <span data-ttu-id="2b0ed-1405">Добавлено `--snapshot` для `storage file download-batch` для скачивания из моментального снимка общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1405">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="2b0ed-1406">Изменен индикатор выполнения `storage blob [download-batch|upload-batch]`, чтобы обобщить сведения и указать текущий большой двоичный объект.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1406">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="2b0ed-1407">Исправлена проблема с `storage account update` при обновлении параметров шифрования.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1407">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="2b0ed-1408">Исправлена проблема со сбоем `storage blob show` при использовании OAuth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1408">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-1409">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1409">VM</span></span>
* <span data-ttu-id="2b0ed-1410">Добавлена команда `image update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1410">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="2b0ed-1411">12 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1411">March 12, 2019</span></span>

<span data-ttu-id="2b0ed-1412">Версия 2.0.60</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1412">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-1413">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1413">Core</span></span>

* <span data-ttu-id="2b0ed-1414">Исправлена недопустимая ошибка в `cloud set` о том, что подписка не найдена.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1414">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-1415">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1415">ACR</span></span>

* <span data-ttu-id="2b0ed-1416">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1416">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-1417">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1417">ACS</span></span>

* <span data-ttu-id="2b0ed-1418">Внесены изменения, в соответствии с которыми параметр `--listen-address` для `aks browse` игнорируется, если он не поддерживается kubectl.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1418">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="2b0ed-1419">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1419">AppService</span></span>

* <span data-ttu-id="2b0ed-1420">Добавлено `[webapp|functionapp] deployment list-publishing-credentials` для получения URL-адреса публикации Kudu и связанных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1420">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="2b0ed-1421">Удалена ошибочная инструкция печати для `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1421">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="2b0ed-1422">Исправлено `functionapp` для настройки правильного образа для среды выполнения в планах службы приложений Linux.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1422">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="2b0ed-1423">Удален тег предварительной версии для `webapp up` и добавлены усовершенствования в команду.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1423">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="2b0ed-1424">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1424">Botservice</span></span>

* <span data-ttu-id="2b0ed-1425">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1425">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="2b0ed-1426">Добавлено `Microsoft-BotFramework-AppId` и `Microsoft-BotFramework-AppPassword` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1426">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="2b0ed-1427">Удалены одинарные кавычки из выходных данных команды `bot publish` в конце `bot create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1427">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="2b0ed-1428">Изменено `bot publish` для включения поддержки асинхронных операций.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1428">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="2b0ed-1429">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1429">Container</span></span>

* <span data-ttu-id="2b0ed-1430">Добавлен аргумент `--no-wait` для команды `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1430">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="2b0ed-1431">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1431">EventHub</span></span>

* <span data-ttu-id="2b0ed-1432">Добавлен флаг `--skip-empty-archives` для `eventhub create|update` для включения поддержки пустых архивов при записи.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1432">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="2b0ed-1433">Поиск</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1433">Find</span></span>

* <span data-ttu-id="2b0ed-1434">Основные обновления функций</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1434">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="2b0ed-1435">HDInsight</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1435">HDInsight</span></span>

* <span data-ttu-id="2b0ed-1436">Добавлен параметр `--storage-account-managed-identity` для `hdinsight create` для включения поддержки MSI ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1436">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-1437">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1437">Network</span></span>

* <span data-ttu-id="2b0ed-1438">Исправлена проблема с `vpn-connection update`, когда обновление VPN-подключения между шлюзами в разных подписках завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1438">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="2b0ed-1439">Rdbms</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1439">Rdbms</span></span>

* <span data-ttu-id="2b0ed-1440">Незначительные исправления для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1440">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-1441">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1441">Role</span></span>

* <span data-ttu-id="2b0ed-1442">Исправлено `role definition update` для использования идентификатора для правильного разрешения определения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1442">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="2b0ed-1443">Изменено `ad app credential reset` для исключения предположения о том, что субъект-служба приложения всегда существует.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1443">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="2b0ed-1444">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1444">Service Fabric</span></span>

* <span data-ttu-id="2b0ed-1445">Исправлена проблема с `sf cluster list` и невозможностью итерации.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1445">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="2b0ed-1446">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1446">February 26, 2019</span></span>

<span data-ttu-id="2b0ed-1447">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1447">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-1448">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1448">Core</span></span>

* <span data-ttu-id="2b0ed-1449">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1449">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-1450">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1450">ACR</span></span>

* <span data-ttu-id="2b0ed-1451">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1451">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="2b0ed-1452">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1452">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-1453">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1453">ACS</span></span>

* <span data-ttu-id="2b0ed-1454">Добавлен параметр `--listen-address` для команды `aks port-forward`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1454">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-1455">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1455">AppService</span></span>

* <span data-ttu-id="2b0ed-1456">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1456">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="2b0ed-1457">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1457">Batch</span></span>
* <span data-ttu-id="2b0ed-1458">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1458">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="2b0ed-1459">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1459">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="2b0ed-1460">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1460">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="2b0ed-1461">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1461">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="2b0ed-1462">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1462">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="2b0ed-1463">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1463">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2b0ed-1464">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1464">CosmosDB</span></span>

* <span data-ttu-id="2b0ed-1465">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1465">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="2b0ed-1466">Kusto</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1466">Kusto</span></span>

* <span data-ttu-id="2b0ed-1467">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1467">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-1468">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1468">Network</span></span>

* <span data-ttu-id="2b0ed-1469">Добавлен аргумент `--express-route-gateway-bypass` для команды `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1469">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="2b0ed-1470">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1470">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="2b0ed-1471">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1471">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="2b0ed-1472">Добавлен аргумент `--legacy-mode` в команду `express-route peering [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1472">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="2b0ed-1473">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1473">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="2b0ed-1474">Добавлен аргумент `--gateway-default-site` для команды `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1474">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="2b0ed-1475">Добавлены команды `ipsec-policy` для `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1475">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-1476">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1476">Resource</span></span>

* <span data-ttu-id="2b0ed-1477">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1477">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="2b0ed-1478">Добавлена поддержка файла параметров на основе URI для `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1478">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="2b0ed-1479">Добавлена поддержка определений и параметров на основе URI для `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1479">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="2b0ed-1480">Исправлена обработка параметров и правил для `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1480">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="2b0ed-1481">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1481">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-1482">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1482">Role</span></span>

* <span data-ttu-id="2b0ed-1483">Добавлена поддержка ролей приложений для `ad app [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1483">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-1484">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1484">VM</span></span>

* <span data-ttu-id="2b0ed-1485">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1485">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="2b0ed-1486">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1486">February 12, 2019</span></span>

<span data-ttu-id="2b0ed-1487">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1487">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-1488">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1488">Core</span></span>

* <span data-ttu-id="2b0ed-1489">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1489">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="2b0ed-1490">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1490">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-1491">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1491">ACR</span></span>
* <span data-ttu-id="2b0ed-1492">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1492">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="2b0ed-1493">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1493">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-1494">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1494">ACS</span></span>
* <span data-ttu-id="2b0ed-1495">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1495">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="2b0ed-1496">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1496">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="2b0ed-1497">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1497">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="2b0ed-1498">AMS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1498">AMS</span></span>
* <span data-ttu-id="2b0ed-1499">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1499">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="2b0ed-1500">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1500">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-1501">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1501">Appservice</span></span>
* <span data-ttu-id="2b0ed-1502">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1502">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="2b0ed-1503">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1503">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="2b0ed-1504">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1504">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="2b0ed-1505">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1505">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="2b0ed-1506">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1506">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="2b0ed-1507">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1507">Botservice</span></span>
* <span data-ttu-id="2b0ed-1508">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1508">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="2b0ed-1509">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1509">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="2b0ed-1510">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1510">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="2b0ed-1511">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1511">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="2b0ed-1512">[УСТАРЕЛО] Аргумент `--proj-name` не рекомендуется к использованию. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1512">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="2b0ed-1513">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1513">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="2b0ed-1514">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1514">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="2b0ed-1515">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1515">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="2b0ed-1516">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1516">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="2b0ed-1517">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1517">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="2b0ed-1518">Key Vault</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1518">Key Vault</span></span>
* <span data-ttu-id="2b0ed-1519">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1519">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-1520">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1520">Monitor</span></span>
* <span data-ttu-id="2b0ed-1521">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1521">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-1522">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1522">Network</span></span>
* <span data-ttu-id="2b0ed-1523">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1523">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="2b0ed-1524">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1524">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="2b0ed-1525">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1525">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="2b0ed-1526">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1526">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="2b0ed-1527">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1527">Policy Insights</span></span>
* <span data-ttu-id="2b0ed-1528">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1528">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="2b0ed-1529">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1529">RDBMS</span></span>
* <span data-ttu-id="2b0ed-1530">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1530">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="2b0ed-1531">Redis</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1531">Redis</span></span>
* <span data-ttu-id="2b0ed-1532">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1532">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="2b0ed-1533">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1533">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="2b0ed-1534">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1534">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="2b0ed-1535">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1535">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="2b0ed-1536">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1536">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="2b0ed-1537">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1537">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="2b0ed-1538">[УСТАРЕЛО] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1538">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-1539">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1539">Role</span></span>
* <span data-ttu-id="2b0ed-1540">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1540">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="2b0ed-1541">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1541">SQL VM</span></span>
* <span data-ttu-id="2b0ed-1542">[УСТАРЕЛО] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1542">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-1543">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1543">VM</span></span>
* <span data-ttu-id="2b0ed-1544">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1544">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="2b0ed-1545">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1545">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="2b0ed-1546">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1546">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="2b0ed-1547">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1547">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="2b0ed-1548">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1548">January 31, 2019</span></span>

<span data-ttu-id="2b0ed-1549">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1549">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-1550">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1550">Core</span></span>

* <span data-ttu-id="2b0ed-1551">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1551">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="2b0ed-1552">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1552">January 28, 2019</span></span>

<span data-ttu-id="2b0ed-1553">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1553">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-1554">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1554">ACR</span></span>
* <span data-ttu-id="2b0ed-1555">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1555">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-1556">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1556">ACS</span></span>
* <span data-ttu-id="2b0ed-1557">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1557">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="2b0ed-1558">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1558">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="2b0ed-1559">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1559">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="2b0ed-1560">AMS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1560">AMS</span></span>
* <span data-ttu-id="2b0ed-1561">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1561">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="2b0ed-1562">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1562">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-1563">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1563">Appservice</span></span>
* <span data-ttu-id="2b0ed-1564">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1564">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="2b0ed-1565">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1565">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="2b0ed-1566">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1566">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="2b0ed-1567">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1567">Container</span></span>
* <span data-ttu-id="2b0ed-1568">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1568">Added `container start` command</span></span>
* <span data-ttu-id="2b0ed-1569">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1569">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="2b0ed-1570">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1570">EventGrid</span></span>
* <span data-ttu-id="2b0ed-1571">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1571">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="2b0ed-1572">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1572">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="2b0ed-1573">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1573">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="2b0ed-1574">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1574">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="2b0ed-1575">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1575">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="2b0ed-1576">HDInsight</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1576">HDInsight</span></span>
* <span data-ttu-id="2b0ed-1577">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1577">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="2b0ed-1578">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1578">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="2b0ed-1579">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1579">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="2b0ed-1580">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1580">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="2b0ed-1581">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1581">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="2b0ed-1582">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1582">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="2b0ed-1583">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1583">IoT</span></span>
* <span data-ttu-id="2b0ed-1584">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1584">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="2b0ed-1585">Kusto</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1585">Kusto</span></span>
* <span data-ttu-id="2b0ed-1586">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1586">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-1587">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1587">Monitor</span></span>
* <span data-ttu-id="2b0ed-1588">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1588">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="2b0ed-1589">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1589">Profile</span></span>
* <span data-ttu-id="2b0ed-1590">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1590">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-1591">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1591">Network</span></span>
* <span data-ttu-id="2b0ed-1592">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1592">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="2b0ed-1593">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1593">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-1594">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1594">Resource</span></span>
* <span data-ttu-id="2b0ed-1595">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1595">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="2b0ed-1596">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1596">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="2b0ed-1597">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1597">SQL Virtual Machine</span></span>
* <span data-ttu-id="2b0ed-1598">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1598">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-1599">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1599">Storage</span></span>
* <span data-ttu-id="2b0ed-1600">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1600">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="2b0ed-1601">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1601">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-1602">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1602">VM</span></span>
* <span data-ttu-id="2b0ed-1603">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1603">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="2b0ed-1604">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1604">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="2b0ed-1605">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1605">January 15, 2019</span></span>

<span data-ttu-id="2b0ed-1606">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1606">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-1607">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1607">ACR</span></span>
* <span data-ttu-id="2b0ed-1608">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1608">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="2b0ed-1609">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1609">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="2b0ed-1610">[УСТАРЕЛО] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1610">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="2b0ed-1611">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1611">ACS</span></span>
* <span data-ttu-id="2b0ed-1612">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1612">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-1613">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1613">Appservice</span></span>
* <span data-ttu-id="2b0ed-1614">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1614">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="2b0ed-1615">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1615">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="2b0ed-1616">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1616">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="2b0ed-1617">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1617">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="2b0ed-1618">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1618">Botservice</span></span>
* <span data-ttu-id="2b0ed-1619">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1619">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="2b0ed-1620">Configure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1620">Configure</span></span>
* <span data-ttu-id="2b0ed-1621">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1621">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2b0ed-1622">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1622">CosmosDB</span></span>
* <span data-ttu-id="2b0ed-1623">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1623">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="2b0ed-1624">HDInsight</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1624">HDInsight</span></span>
* <span data-ttu-id="2b0ed-1625">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1625">Added commands for managing applications</span></span>
* <span data-ttu-id="2b0ed-1626">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1626">Added commands for managing script actions</span></span>
* <span data-ttu-id="2b0ed-1627">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1627">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="2b0ed-1628">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1628">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="2b0ed-1629">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1629">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-1630">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1630">Network</span></span>
* <span data-ttu-id="2b0ed-1631">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1631">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="2b0ed-1632">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1632">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="2b0ed-1633">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1633">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="2b0ed-1634">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1634">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-1635">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1635">Role</span></span>
* <span data-ttu-id="2b0ed-1636">[УСТАРЕЛО] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1636">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="2b0ed-1637">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1637">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="2b0ed-1638">Безопасность</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1638">Security</span></span>
* <span data-ttu-id="2b0ed-1639">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1639">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-1640">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1640">Storage</span></span>
* <span data-ttu-id="2b0ed-1641">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1641">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="2b0ed-1642">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1642">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="2b0ed-1643">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1643">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="2b0ed-1644">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1644">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="2b0ed-1645">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1645">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-1646">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1646">VM</span></span>
* <span data-ttu-id="2b0ed-1647">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1647">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="2b0ed-1648">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1648">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="2b0ed-1649">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1649">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="2b0ed-1650">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1650">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="2b0ed-1651">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1651">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="2b0ed-1652">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1652">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="2b0ed-1653">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1653">December 20, 2018</span></span>

<span data-ttu-id="2b0ed-1654">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1654">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="2b0ed-1655">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1655">Appservice</span></span>
* <span data-ttu-id="2b0ed-1656">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1656">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="2b0ed-1657">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1657">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="2b0ed-1658">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1658">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="2b0ed-1659">IoT Central</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1659">IoTCentral</span></span>
* <span data-ttu-id="2b0ed-1660">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1660">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-1661">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1661">Role</span></span>
* <span data-ttu-id="2b0ed-1662">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1662">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-1663">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1663">SQL</span></span>
* <span data-ttu-id="2b0ed-1664">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1664">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-1665">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1665">VM</span></span>
* <span data-ttu-id="2b0ed-1666">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1666">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="2b0ed-1667">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1667">December 18, 2018</span></span>

<span data-ttu-id="2b0ed-1668">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1668">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="2b0ed-1669">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1669">ACR</span></span>
* <span data-ttu-id="2b0ed-1670">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1670">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="2b0ed-1671">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1671">Condensed the table layout for task list</span></span>
* <span data-ttu-id="2b0ed-1672">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1672">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-1673">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1673">ACS</span></span>
* <span data-ttu-id="2b0ed-1674">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1674">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="2b0ed-1675">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1675">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="2b0ed-1676">[УСТАРЕЛО] Команды `az acs` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1676">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="2b0ed-1677">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1677">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="2b0ed-1678">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1678">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="2b0ed-1679">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1679">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-1680">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1680">Appservice</span></span>
* <span data-ttu-id="2b0ed-1681">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1681">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="2b0ed-1682">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1682">Botservice</span></span>
* <span data-ttu-id="2b0ed-1683">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1683">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="2b0ed-1684">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1684">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="2b0ed-1685">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1685">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="2b0ed-1686">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1686">Reduced Kudu network calls</span></span>
* <span data-ttu-id="2b0ed-1687">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1687">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="2b0ed-1688">Потребление</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1688">Consumption</span></span>
* <span data-ttu-id="2b0ed-1689">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1689">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2b0ed-1690">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1690">CosmosDB</span></span>
* <span data-ttu-id="2b0ed-1691">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1691">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="2b0ed-1692">Maps</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1692">Maps</span></span>
* <span data-ttu-id="2b0ed-1693">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1693">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-1694">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1694">Network</span></span>
* <span data-ttu-id="2b0ed-1695">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1695">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="2b0ed-1696">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1696">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-1697">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1697">Resource</span></span>
* <span data-ttu-id="2b0ed-1698">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1698">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="2b0ed-1699">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1699">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-1700">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1700">Storage</span></span>
*  <span data-ttu-id="2b0ed-1701">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1701">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-1702">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1702">VM</span></span>
* <span data-ttu-id="2b0ed-1703">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1703">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="2b0ed-1704">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1704">December 4, 2018</span></span>

<span data-ttu-id="2b0ed-1705">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1705">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="2b0ed-1706">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1706">Core</span></span>
* <span data-ttu-id="2b0ed-1707">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1707">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="2b0ed-1708">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1708">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-1709">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1709">Appservice</span></span>
* <span data-ttu-id="2b0ed-1710">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1710">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="2b0ed-1711">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1711">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-1712">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1712">Network</span></span>
* <span data-ttu-id="2b0ed-1713">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1713">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-1714">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1714">Role</span></span>
* <span data-ttu-id="2b0ed-1715">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1715">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="2b0ed-1716">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1716">VM</span></span>
* <span data-ttu-id="2b0ed-1717">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1717">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="2b0ed-1718">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1718">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="2b0ed-1719">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1719">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="2b0ed-1720">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1720">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="2b0ed-1721">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1721">November 20, 2018</span></span>

<span data-ttu-id="2b0ed-1722">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1722">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="2b0ed-1723">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1723">Core</span></span>
* <span data-ttu-id="2b0ed-1724">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1724">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-1725">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1725">ACR</span></span>
* <span data-ttu-id="2b0ed-1726">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1726">Added context token to task step</span></span>
* <span data-ttu-id="2b0ed-1727">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1727">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="2b0ed-1728">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1728">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-1729">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1729">Appservice</span></span>
* <span data-ttu-id="2b0ed-1730">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1730">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="2b0ed-1731">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1731">Updated the default `node_version`.</span></span> <span data-ttu-id="2b0ed-1732">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1732">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="2b0ed-1733">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1733">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="2b0ed-1734">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1734">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="2b0ed-1735">IotCentral</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1735">IotCentral</span></span>
* <span data-ttu-id="2b0ed-1736">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1736">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="2b0ed-1737">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1737">KeyVault</span></span>
* <span data-ttu-id="2b0ed-1738">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1738">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-1739">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1739">Network</span></span>
* <span data-ttu-id="2b0ed-1740">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1740">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="2b0ed-1741">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1741">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="2b0ed-1742">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1742">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="2b0ed-1743">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1743">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="2b0ed-1744">Rdbms</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1744">Rdbms</span></span>
* <span data-ttu-id="2b0ed-1745">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1745">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="2b0ed-1746">RBAC:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1746">Rbac</span></span>
* <span data-ttu-id="2b0ed-1747">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1747">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="2b0ed-1748">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1748">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="2b0ed-1749">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1749">Storage</span></span>
* <span data-ttu-id="2b0ed-1750">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1750">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="2b0ed-1751">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1751">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="2b0ed-1752">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1752">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="2b0ed-1753">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1753">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-1754">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1754">VM</span></span>
* <span data-ttu-id="2b0ed-1755">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1755">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="2b0ed-1756">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1756">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="2b0ed-1757">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1757">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="2b0ed-1758">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1758">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="2b0ed-1759">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1759">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="2b0ed-1760">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1760">Added `snapshot wait` command</span></span>
* <span data-ttu-id="2b0ed-1761">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1761">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="2b0ed-1762">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1762">November 6, 2018</span></span>

<span data-ttu-id="2b0ed-1763">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1763">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-1764">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1764">Core</span></span>
* <span data-ttu-id="2b0ed-1765">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1765">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-1766">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1766">ACR</span></span>
* <span data-ttu-id="2b0ed-1767">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1767">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="2b0ed-1768">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1768">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-1769">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1769">ACS</span></span>
* <span data-ttu-id="2b0ed-1770">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1770">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="2b0ed-1771">Помощник</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1771">Advisor</span></span>
* <span data-ttu-id="2b0ed-1772">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1772">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="2b0ed-1773">AMS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1773">AMS</span></span>
* <span data-ttu-id="2b0ed-1774">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1774">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="2b0ed-1775">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1775">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="2b0ed-1776">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1776">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="2b0ed-1777">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1777">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="2b0ed-1778">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1778">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="2b0ed-1779">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1779">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="2b0ed-1780">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1780">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="2b0ed-1781">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1781">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="2b0ed-1782">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1782">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="2b0ed-1783">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1783">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="2b0ed-1784">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1784">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="2b0ed-1785">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1785">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="2b0ed-1786">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1786">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="2b0ed-1787">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1787">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="2b0ed-1788">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1788">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="2b0ed-1789">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1789">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="2b0ed-1790">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1790">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-1791">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1791">AppService</span></span>
* <span data-ttu-id="2b0ed-1792">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1792">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="2b0ed-1793">Configure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1793">Configure</span></span>
* <span data-ttu-id="2b0ed-1794">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1794">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="2b0ed-1795">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1795">Container</span></span>
* <span data-ttu-id="2b0ed-1796">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1796">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="2b0ed-1797">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1797">EventHub</span></span>
* <span data-ttu-id="2b0ed-1798">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1798">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="2b0ed-1799">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1799">Interactive</span></span>
* <span data-ttu-id="2b0ed-1800">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1800">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-1801">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1801">Monitor</span></span>
* <span data-ttu-id="2b0ed-1802">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1802">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-1803">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1803">Network</span></span>
* <span data-ttu-id="2b0ed-1804">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1804">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="2b0ed-1805">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1805">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="2b0ed-1806">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1806">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="2b0ed-1807">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1807">Profile</span></span>
* <span data-ttu-id="2b0ed-1808">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1808">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="2b0ed-1809">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1809">RDBMS</span></span>
* <span data-ttu-id="2b0ed-1810">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1810">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-1811">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1811">Resource</span></span>
* <span data-ttu-id="2b0ed-1812">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1812">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-1813">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1813">Role</span></span>
* <span data-ttu-id="2b0ed-1814">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1814">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="2b0ed-1815">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1815">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="2b0ed-1816">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1816">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-1817">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1817">Storage</span></span>
* <span data-ttu-id="2b0ed-1818">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1818">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-1819">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1819">VM</span></span>
* <span data-ttu-id="2b0ed-1820">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1820">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="2b0ed-1821">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1821">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="2b0ed-1822">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1822">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="2b0ed-1823">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1823">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="2b0ed-1824">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1824">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="2b0ed-1825">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1825">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="2b0ed-1826">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1826">October 23, 2018</span></span>

<span data-ttu-id="2b0ed-1827">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1827">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-1828">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1828">Core</span></span>
* <span data-ttu-id="2b0ed-1829">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1829">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="2b0ed-1830">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1830">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-1831">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1831">ACR</span></span>
* <span data-ttu-id="2b0ed-1832">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1832">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="2b0ed-1833">CDN</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1833">CDN</span></span>
* <span data-ttu-id="2b0ed-1834">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1834">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="2b0ed-1835">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1835">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="2b0ed-1836">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1836">Container</span></span>
* <span data-ttu-id="2b0ed-1837">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1837">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="2b0ed-1838">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1838">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="2b0ed-1839">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1839">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="2b0ed-1840">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1840">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="2b0ed-1841">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1841">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="2b0ed-1842">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1842">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="2b0ed-1843">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1843">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2b0ed-1844">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1844">CosmosDB</span></span>
* <span data-ttu-id="2b0ed-1845">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1845">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="2b0ed-1846">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1846">Interactive</span></span>
* <span data-ttu-id="2b0ed-1847">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1847">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="2b0ed-1848">IoT Central</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1848">IoT Central</span></span>
* <span data-ttu-id="2b0ed-1849">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1849">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="2b0ed-1850">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1850">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-1851">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1851">Monitor</span></span>
* <span data-ttu-id="2b0ed-1852">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1852">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="2b0ed-1853">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1853">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="2b0ed-1854">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1854">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="2b0ed-1855">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1855">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="2b0ed-1856">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1856">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="2b0ed-1857">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1857">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="2b0ed-1858">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1858">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="2b0ed-1859">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1859">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="2b0ed-1860">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1860">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="2b0ed-1861">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1861">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-1862">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1862">Network</span></span>
* <span data-ttu-id="2b0ed-1863">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1863">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="2b0ed-1864">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1864">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="2b0ed-1865">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1865">ServiceBus</span></span>
* <span data-ttu-id="2b0ed-1866">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1866">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-1867">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1867">SQL</span></span>
* <span data-ttu-id="2b0ed-1868">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1868">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-1869">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1869">Storage</span></span>
* <span data-ttu-id="2b0ed-1870">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1870">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="2b0ed-1871">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1871">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-1872">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1872">VM</span></span>
* <span data-ttu-id="2b0ed-1873">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1873">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="2b0ed-1874">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1874">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="2b0ed-1875">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1875">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="2b0ed-1876">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1876">October 16, 2018</span></span>

<span data-ttu-id="2b0ed-1877">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1877">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-1878">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1878">VM</span></span>
* <span data-ttu-id="2b0ed-1879">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1879">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="2b0ed-1880">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1880">October 9, 2018</span></span>

<span data-ttu-id="2b0ed-1881">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1881">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-1882">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1882">Core</span></span>
* <span data-ttu-id="2b0ed-1883">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1883">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-1884">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1884">ACR</span></span>
* <span data-ttu-id="2b0ed-1885">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1885">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-1886">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1886">ACS</span></span>
* <span data-ttu-id="2b0ed-1887">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1887">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="2b0ed-1888">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1888">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="2b0ed-1889">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1889">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="2b0ed-1890">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1890">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="2b0ed-1891">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1891">Container</span></span>
* <span data-ttu-id="2b0ed-1892">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1892">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="2b0ed-1893">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1893">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="2b0ed-1894">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1894">Event Hub</span></span>
* <span data-ttu-id="2b0ed-1895">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1895">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="2b0ed-1896">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1896">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="2b0ed-1897">Модули</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1897">Extensions</span></span>
* <span data-ttu-id="2b0ed-1898">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1898">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="2b0ed-1899">HDInsight</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1899">HDInsight</span></span>
* <span data-ttu-id="2b0ed-1900">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1900">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="2b0ed-1901">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1901">IoT</span></span>
* <span data-ttu-id="2b0ed-1902">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1902">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="2b0ed-1903">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1903">KeyVault</span></span>
* <span data-ttu-id="2b0ed-1904">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1904">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-1905">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1905">Network</span></span>
* <span data-ttu-id="2b0ed-1906">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1906">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="2b0ed-1907">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1907">See #6052</span></span>
* <span data-ttu-id="2b0ed-1908">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1908">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="2b0ed-1909">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1909">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="2b0ed-1910">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1910">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="2b0ed-1911">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1911">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="2b0ed-1912">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1912">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="2b0ed-1913">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1913">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-1914">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1914">Role</span></span>
* <span data-ttu-id="2b0ed-1915">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1915">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="2b0ed-1916">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1916">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="2b0ed-1917">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1917">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="2b0ed-1918">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1918">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="2b0ed-1919">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1919">Service Bus</span></span>
* <span data-ttu-id="2b0ed-1920">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1920">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-1921">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1921">VM</span></span>
* <span data-ttu-id="2b0ed-1922">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1922">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="2b0ed-1923">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1923">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="2b0ed-1924">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1924">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="2b0ed-1925">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1925">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="2b0ed-1926">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1926">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="2b0ed-1927">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1927">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="2b0ed-1928">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1928">September 21, 2018</span></span>

<span data-ttu-id="2b0ed-1929">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1929">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-1930">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1930">ACR</span></span>
* <span data-ttu-id="2b0ed-1931">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1931">Added ACR Task commands</span></span>
* <span data-ttu-id="2b0ed-1932">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1932">Added quick run command</span></span>
* <span data-ttu-id="2b0ed-1933">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1933">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="2b0ed-1934">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1934">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="2b0ed-1935">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1935">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="2b0ed-1936">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1936">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-1937">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1937">ACS</span></span>
* <span data-ttu-id="2b0ed-1938">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1938">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="2b0ed-1939">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1939">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-1940">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1940">AppService</span></span>

* <span data-ttu-id="2b0ed-1941">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1941">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="2b0ed-1942">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1942">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="2b0ed-1943">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1943">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="2b0ed-1944">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1944">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="2b0ed-1945">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1945">Batch</span></span>
* <span data-ttu-id="2b0ed-1946">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1946">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="2b0ed-1947">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1947">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="2b0ed-1948">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1948">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="2b0ed-1949">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1949">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="2b0ed-1950">Batch AI</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1950">Batch AI</span></span> 
* <span data-ttu-id="2b0ed-1951">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1951">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="2b0ed-1952">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1952">Cognitive Services</span></span>
* <span data-ttu-id="2b0ed-1953">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1953">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="2b0ed-1954">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1954">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="2b0ed-1955">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1955">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="2b0ed-1956">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1956">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="2b0ed-1957">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1957">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="2b0ed-1958">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1958">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="2b0ed-1959">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1959">Container</span></span>
* <span data-ttu-id="2b0ed-1960">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1960">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="2b0ed-1961">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1961">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="2b0ed-1962">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1962">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="2b0ed-1963">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1963">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="2b0ed-1964">Data Lake</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1964">Datalake</span></span>
* <span data-ttu-id="2b0ed-1965">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1965">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="2b0ed-1966">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1966">Interactive Shell</span></span>
* <span data-ttu-id="2b0ed-1967">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1967">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="2b0ed-1968">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1968">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="2b0ed-1969">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1969">IoT</span></span>
* <span data-ttu-id="2b0ed-1970">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1970">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="2b0ed-1971">Key Vault</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1971">Key Vault</span></span>
* <span data-ttu-id="2b0ed-1972">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1972">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-1973">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1973">Network</span></span>
* <span data-ttu-id="2b0ed-1974">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1974">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="2b0ed-1975">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1975">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="2b0ed-1976">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1976">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="2b0ed-1977">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1977">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="2b0ed-1978">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1978">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="2b0ed-1979">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1979">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="2b0ed-1980">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1980">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="2b0ed-1981">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1981">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="2b0ed-1982">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1982">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="2b0ed-1983">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1983">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="2b0ed-1984">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1984">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="2b0ed-1985">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1985">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="2b0ed-1986">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1986">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="2b0ed-1987">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1987">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="2b0ed-1988">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1988">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="2b0ed-1989">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1989">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="2b0ed-1990">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1990">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="2b0ed-1991">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1991">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="2b0ed-1992">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1992">RDBMS</span></span>
* <span data-ttu-id="2b0ed-1993">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1993">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="2b0ed-1994">резервирование.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1994">Reservation</span></span>
* <span data-ttu-id="2b0ed-1995">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1995">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="2b0ed-1996">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1996">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="2b0ed-1997">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1997">Manage App</span></span>
* <span data-ttu-id="2b0ed-1998">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1998">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="2b0ed-1999">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-1999">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-2000">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2000">Role</span></span>
* <span data-ttu-id="2b0ed-2001">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2001">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="2b0ed-2002">SignalR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2002">SignalR</span></span>
* <span data-ttu-id="2b0ed-2003">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2003">First release</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-2004">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2004">Storage</span></span>
* <span data-ttu-id="2b0ed-2005">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2005">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="2b0ed-2006">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2006">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2007">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2007">VM</span></span>
* <span data-ttu-id="2b0ed-2008">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2008">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="2b0ed-2009">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2009">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="2b0ed-2010">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2010">August 28, 2018</span></span>

<span data-ttu-id="2b0ed-2011">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2011">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-2012">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2012">Core</span></span>

* <span data-ttu-id="2b0ed-2013">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2013">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="2b0ed-2014">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2014">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-2015">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2015">ACR</span></span>

* <span data-ttu-id="2b0ed-2016">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2016">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="2b0ed-2017">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2017">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-2018">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2018">ACS</span></span>

* <span data-ttu-id="2b0ed-2019">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2019">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="2b0ed-2020">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2020">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-2021">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2021">AppService</span></span>

* <span data-ttu-id="2b0ed-2022">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2022">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="2b0ed-2023">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2023">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="2b0ed-2024">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2024">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="2b0ed-2025">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2025">Backup</span></span>

* <span data-ttu-id="2b0ed-2026">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2026">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="2b0ed-2027">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2027">Bot Service</span></span>

* <span data-ttu-id="2b0ed-2028">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2028">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="2b0ed-2029">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2029">Cognitive Services</span></span>

* <span data-ttu-id="2b0ed-2030">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2030">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="2b0ed-2031">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2031">IoT</span></span>

* <span data-ttu-id="2b0ed-2032">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2032">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-2033">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2033">Monitor</span></span>

* <span data-ttu-id="2b0ed-2034">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2034">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="2b0ed-2035">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2035">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-2036">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2036">Network</span></span>

* <span data-ttu-id="2b0ed-2037">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2037">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-2038">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2038">Resource</span></span>

* <span data-ttu-id="2b0ed-2039">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2039">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-2040">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2040">Storage</span></span>

* <span data-ttu-id="2b0ed-2041">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2041">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2042">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2042">VM</span></span>

* <span data-ttu-id="2b0ed-2043">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2043">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="2b0ed-2044">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2044">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="2b0ed-2045">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2045">Auguest 14, 2018</span></span>

<span data-ttu-id="2b0ed-2046">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2046">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-2047">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2047">Core</span></span>

* <span data-ttu-id="2b0ed-2048">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2048">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="2b0ed-2049">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2049">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="2b0ed-2050">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2050">Telemetry</span></span>

* <span data-ttu-id="2b0ed-2051">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2051">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-2052">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2052">ACR</span></span>

* <span data-ttu-id="2b0ed-2053">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2053">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="2b0ed-2054">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2054">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-2055">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2055">ACS</span></span>

* <span data-ttu-id="2b0ed-2056">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2056">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="2b0ed-2057">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2057">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="2b0ed-2058">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2058">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="2b0ed-2059">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2059">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="2b0ed-2060">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2060">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="2b0ed-2061">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2061">AppService</span></span>

* <span data-ttu-id="2b0ed-2062">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2062">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="2b0ed-2063">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2063">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="2b0ed-2064">Batch AI</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2064">BatchAI</span></span>

* <span data-ttu-id="2b0ed-2065">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2065">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="2b0ed-2066">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2066">Container</span></span>

* <span data-ttu-id="2b0ed-2067">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2067">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="2b0ed-2068">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2068">IoT</span></span>

* <span data-ttu-id="2b0ed-2069">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2069">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="2b0ed-2070">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2070">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="2b0ed-2071">IoT Central</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2071">Iot Central</span></span>

* <span data-ttu-id="2b0ed-2072">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2072">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="2b0ed-2073">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2073">KeyVault</span></span>


* <span data-ttu-id="2b0ed-2074">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2074">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="2b0ed-2075">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2075">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="2b0ed-2076">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2076">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="2b0ed-2077">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2077">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="2b0ed-2078">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2078">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="2b0ed-2079">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2079">Relay</span></span>

* <span data-ttu-id="2b0ed-2080">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2080">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-2081">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2081">Sql</span></span>

* <span data-ttu-id="2b0ed-2082">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2082">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-2083">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2083">Storage</span></span>

* <span data-ttu-id="2b0ed-2084">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2084">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="2b0ed-2085">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2085">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="2b0ed-2086">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2086">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="2b0ed-2087">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2087">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="2b0ed-2088">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2088">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2089">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2089">VM</span></span>

* <span data-ttu-id="2b0ed-2090">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2090">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="2b0ed-2091">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2091">July 31, 2018</span></span>

<span data-ttu-id="2b0ed-2092">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2092">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-2093">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2093">ACR</span></span>

* <span data-ttu-id="2b0ed-2094">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2094">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="2b0ed-2095">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2095">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-2096">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2096">ACS</span></span>

* <span data-ttu-id="2b0ed-2097">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2097">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="2b0ed-2098">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2098">Batch</span></span>

* <span data-ttu-id="2b0ed-2099">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2099">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="2b0ed-2100">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2100">Container</span></span>

* <span data-ttu-id="2b0ed-2101">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2101">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-2102">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2102">Network</span></span>

* <span data-ttu-id="2b0ed-2103">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2103">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="2b0ed-2104">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2104">Resource</span></span>

* <span data-ttu-id="2b0ed-2105">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2105">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="2b0ed-2106">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2106">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-2107">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2107">Role</span></span>

* <span data-ttu-id="2b0ed-2108">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2108">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="2b0ed-2109">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2109">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="2b0ed-2110">Поиск</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2110">Search</span></span>

* <span data-ttu-id="2b0ed-2111">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2111">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="2b0ed-2112">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2112">Service Bus</span></span>

* <span data-ttu-id="2b0ed-2113">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2113">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="2b0ed-2114">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2114">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="2b0ed-2115">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2115">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="2b0ed-2116">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2116">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-2117">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2117">Storage</span></span>

* <span data-ttu-id="2b0ed-2118">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2118">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="2b0ed-2119">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2119">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2120">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2120">VM</span></span>

* <span data-ttu-id="2b0ed-2121">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2121">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="2b0ed-2122">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2122">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="2b0ed-2123">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2123">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="2b0ed-2124">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2124">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="2b0ed-2125">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2125">July 18, 2018</span></span>

<span data-ttu-id="2b0ed-2126">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2126">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-2127">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2127">Core</span></span>

* <span data-ttu-id="2b0ed-2128">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2128">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="2b0ed-2129">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2129">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="2b0ed-2130">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2130">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-2131">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2131">ACR</span></span>

* <span data-ttu-id="2b0ed-2132">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2132">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="2b0ed-2133">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2133">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="2b0ed-2134">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2134">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="2b0ed-2135">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2135">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-2136">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2136">ACS</span></span>

* <span data-ttu-id="2b0ed-2137">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2137">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-2138">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2138">AppService</span></span>

* <span data-ttu-id="2b0ed-2139">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2139">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="2b0ed-2140">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2140">Batch</span></span>

* <span data-ttu-id="2b0ed-2141">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2141">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="2b0ed-2142">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2142">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="2b0ed-2143">Batch AI</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2143">Batch AI</span></span>

* <span data-ttu-id="2b0ed-2144">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2144">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="2b0ed-2145">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2145">Container</span></span>

* <span data-ttu-id="2b0ed-2146">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2146">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="2b0ed-2147">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2147">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-2148">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2148">Network</span></span>

* <span data-ttu-id="2b0ed-2149">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2149">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="2b0ed-2150">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2150">Added `network nic wait`</span></span>
* <span data-ttu-id="2b0ed-2151">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2151">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="2b0ed-2152">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2152">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="2b0ed-2153">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2153">Resource</span></span>

* <span data-ttu-id="2b0ed-2154">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2154">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="2b0ed-2155">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2155">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="2b0ed-2156">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2156">Added `deployment wait` command</span></span>
* <span data-ttu-id="2b0ed-2157">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2157">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-2158">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2158">SQL</span></span>

* <span data-ttu-id="2b0ed-2159">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2159">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="2b0ed-2160">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2160">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="2b0ed-2161">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2161">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-2162">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2162">Storage</span></span>

* <span data-ttu-id="2b0ed-2163">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2163">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2164">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2164">VM</span></span>

* <span data-ttu-id="2b0ed-2165">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2165">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="2b0ed-2166">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2166">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="2b0ed-2167">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2167">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="2b0ed-2168">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2168">July 3, 2018</span></span>

<span data-ttu-id="2b0ed-2169">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2169">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="2b0ed-2170">AKS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2170">AKS</span></span>

* <span data-ttu-id="2b0ed-2171">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2171">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="2b0ed-2172">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2172">July 3, 2018</span></span>

<span data-ttu-id="2b0ed-2173">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2173">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-2174">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2174">Core</span></span>

* <span data-ttu-id="2b0ed-2175">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2175">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-2176">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2176">ACR</span></span>

* <span data-ttu-id="2b0ed-2177">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2177">Added polling build status</span></span>
* <span data-ttu-id="2b0ed-2178">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2178">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="2b0ed-2179">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2179">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-2180">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2180">ACS</span></span>

* <span data-ttu-id="2b0ed-2181">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2181">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="2b0ed-2182">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2182">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="2b0ed-2183">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2183">Updated options for `aks browse` command.</span></span> <span data-ttu-id="2b0ed-2184">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2184">Added `--listen-port` support</span></span>
* <span data-ttu-id="2b0ed-2185">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2185">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="2b0ed-2186">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2186">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="2b0ed-2187">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2187">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-2188">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2188">AppService</span></span>

* <span data-ttu-id="2b0ed-2189">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2189">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="2b0ed-2190">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2190">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="2b0ed-2191">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2191">Backup</span></span>

* <span data-ttu-id="2b0ed-2192">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2192">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="2b0ed-2193">Batch AI</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2193">BatchAI</span></span>

* <span data-ttu-id="2b0ed-2194">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2194">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="2b0ed-2195">Cloud</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2195">Cloud</span></span>

* <span data-ttu-id="2b0ed-2196">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2196">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="2b0ed-2197">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2197">Container</span></span>

* <span data-ttu-id="2b0ed-2198">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2198">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="2b0ed-2199">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2199">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="2b0ed-2200">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2200">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="2b0ed-2201">Расширение</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2201">Extension</span></span>

* <span data-ttu-id="2b0ed-2202">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2202">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-2203">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2203">Network</span></span>

* <span data-ttu-id="2b0ed-2204">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2204">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="2b0ed-2205">Rdbms</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2205">Rdbms</span></span>

* <span data-ttu-id="2b0ed-2206">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2206">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-2207">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2207">Resource</span></span>

* <span data-ttu-id="2b0ed-2208">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2208">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2209">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2209">VM</span></span>

* <span data-ttu-id="2b0ed-2210">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2210">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="2b0ed-2211">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2211">June 25, 2018</span></span>

<span data-ttu-id="2b0ed-2212">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2212">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="2b0ed-2213">CLI</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2213">CLI</span></span>

* <span data-ttu-id="2b0ed-2214">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2214">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="2b0ed-2215">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2215">June 19, 2018</span></span>

<span data-ttu-id="2b0ed-2216">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2216">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-2217">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2217">Core</span></span>

* <span data-ttu-id="2b0ed-2218">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2218">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-2219">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2219">ACR</span></span>

* <span data-ttu-id="2b0ed-2220">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2220">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="2b0ed-2221">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2221">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-2222">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2222">ACS</span></span>

* <span data-ttu-id="2b0ed-2223">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2223">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="2b0ed-2224">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2224">Added `--update` support</span></span>
* <span data-ttu-id="2b0ed-2225">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2225">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="2b0ed-2226">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2226">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="2b0ed-2227">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2227">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="2b0ed-2228">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2228">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="2b0ed-2229">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2229">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="2b0ed-2230">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2230">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-2231">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2231">AppService</span></span>

* <span data-ttu-id="2b0ed-2232">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2232">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="2b0ed-2233">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2233">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="2b0ed-2234">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2234">Batch</span></span>

* <span data-ttu-id="2b0ed-2235">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2235">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="2b0ed-2236">Batch AI</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2236">Batch AI</span></span>

* <span data-ttu-id="2b0ed-2237">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2237">Added support for workspaces.</span></span> <span data-ttu-id="2b0ed-2238">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2238">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="2b0ed-2239">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2239">Added support for experiments.</span></span> <span data-ttu-id="2b0ed-2240">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2240">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="2b0ed-2241">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2241">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="2b0ed-2242">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2242">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="2b0ed-2243">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2243">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="2b0ed-2244">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2244">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="2b0ed-2245">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2245">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="2b0ed-2246">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2246">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="2b0ed-2247">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2247">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="2b0ed-2248">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2248">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="2b0ed-2249">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2249">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="2b0ed-2250">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2250">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="2b0ed-2251">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2251">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="2b0ed-2252">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2252">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="2b0ed-2253">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2253">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="2b0ed-2254">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2254">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="2b0ed-2255">[`--config`, `-c`] переименовано в [`--config-file`, `-f`].</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2255">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="2b0ed-2256">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2256">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="2b0ed-2257">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2257">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="2b0ed-2258">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2258">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="2b0ed-2259">Maps</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2259">Maps</span></span>

* <span data-ttu-id="2b0ed-2260">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2260">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-2261">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2261">Network</span></span>

* <span data-ttu-id="2b0ed-2262">Добавлена поддержка `https` в `network lb probe create` ([№ 6571](https://github.com/Azure/azure-cli/issues/6571)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2262">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="2b0ed-2263">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2263">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="2b0ed-2264">#6502</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2264">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="2b0ed-2265">Резервирование</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2265">Reservations</span></span>

* <span data-ttu-id="2b0ed-2266">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2266">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="2b0ed-2267">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2267">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="2b0ed-2268">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2268">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="2b0ed-2269">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2269">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="2b0ed-2270">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2270">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="2b0ed-2271">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2271">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-2272">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2272">Role</span></span>

* <span data-ttu-id="2b0ed-2273">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2273">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-2274">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2274">SQL</span></span>

* <span data-ttu-id="2b0ed-2275">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2275">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-2276">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2276">Storage</span></span>

* <span data-ttu-id="2b0ed-2277">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2277">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2278">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2278">VM</span></span>

* <span data-ttu-id="2b0ed-2279">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2279">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="2b0ed-2280">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2280">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="2b0ed-2281">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2281">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="2b0ed-2282">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2282">June 13, 2018</span></span>

<span data-ttu-id="2b0ed-2283">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2283">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-2284">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2284">Core</span></span>

* <span data-ttu-id="2b0ed-2285">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2285">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="2b0ed-2286">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2286">June 13, 2018</span></span>

<span data-ttu-id="2b0ed-2287">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2287">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="2b0ed-2288">AKS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2288">AKS</span></span>

* <span data-ttu-id="2b0ed-2289">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2289">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="2b0ed-2290">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2290">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="2b0ed-2291">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2291">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="2b0ed-2292">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2292">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="2b0ed-2293">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2293">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-2294">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2294">AppService</span></span>

* <span data-ttu-id="2b0ed-2295">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2295">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="2b0ed-2296">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2296">June 5, 2018</span></span>

<span data-ttu-id="2b0ed-2297">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2297">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="2b0ed-2298">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2298">Interactive</span></span>

* <span data-ttu-id="2b0ed-2299">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2299">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="2b0ed-2300">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2300">June 5, 2018</span></span>

<span data-ttu-id="2b0ed-2301">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2301">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-2302">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2302">Core</span></span>

* <span data-ttu-id="2b0ed-2303">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2303">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="2b0ed-2304">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2304">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-2305">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2305">ACR</span></span>

* <span data-ttu-id="2b0ed-2306">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2306">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="2b0ed-2307">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2307">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="2b0ed-2308">AKS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2308">AKS</span></span>

* <span data-ttu-id="2b0ed-2309">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2309">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="2b0ed-2310">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2310">Batch</span></span>

* <span data-ttu-id="2b0ed-2311">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2311">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="2b0ed-2312">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2312">IOT</span></span>

* <span data-ttu-id="2b0ed-2313">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2313">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-2314">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2314">Network</span></span>

* <span data-ttu-id="2b0ed-2315">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2315">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="2b0ed-2316">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2316">Policy Insights</span></span>

* <span data-ttu-id="2b0ed-2317">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2317">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="2b0ed-2318">ARM</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2318">ARM</span></span>

* <span data-ttu-id="2b0ed-2319">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2319">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-2320">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2320">SQL</span></span>

* <span data-ttu-id="2b0ed-2321">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2321">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="2b0ed-2322">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2322">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="2b0ed-2323">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2323">Storage</span></span>

* <span data-ttu-id="2b0ed-2324">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2324">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2325">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2325">VM</span></span>

* <span data-ttu-id="2b0ed-2326">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2326">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="2b0ed-2327">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2327">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="2b0ed-2328">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2328">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="2b0ed-2329">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2329">May 22, 2018</span></span>

<span data-ttu-id="2b0ed-2330">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2330">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-2331">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2331">Core</span></span>

* <span data-ttu-id="2b0ed-2332">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2332">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-2333">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2333">ACS</span></span>

* <span data-ttu-id="2b0ed-2334">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2334">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="2b0ed-2335">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2335">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-2336">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2336">AppService</span></span>

* <span data-ttu-id="2b0ed-2337">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2337">Improved generic update commands</span></span>
* <span data-ttu-id="2b0ed-2338">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2338">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="2b0ed-2339">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2339">Container</span></span>

* <span data-ttu-id="2b0ed-2340">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2340">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="2b0ed-2341">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2341">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="2b0ed-2342">Расширение</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2342">Extension</span></span>

* <span data-ttu-id="2b0ed-2343">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2343">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="2b0ed-2344">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2344">Interactive</span></span>

* <span data-ttu-id="2b0ed-2345">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2345">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="2b0ed-2346">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2346">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="2b0ed-2347">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2347">KeyVault</span></span>

* <span data-ttu-id="2b0ed-2348">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2348">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-2349">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2349">Network</span></span>

* <span data-ttu-id="2b0ed-2350">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2350">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="2b0ed-2351">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2351">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-2352">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2352">SQL</span></span>

* <span data-ttu-id="2b0ed-2353">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2353">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="2b0ed-2354">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2354">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="2b0ed-2355">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2355">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="2b0ed-2356">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2356">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="2b0ed-2357">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2357">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="2b0ed-2358">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2358">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="2b0ed-2359">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2359">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="2b0ed-2360">`edition`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2360">`edition`.</span></span> <span data-ttu-id="2b0ed-2361">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2361">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="2b0ed-2362">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2362">`elasticPoolName`.</span></span> <span data-ttu-id="2b0ed-2363">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2363">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="2b0ed-2364">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2364">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="2b0ed-2365">`edition`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2365">`edition`.</span></span> <span data-ttu-id="2b0ed-2366">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2366">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="2b0ed-2367">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2367">`dtu`.</span></span> <span data-ttu-id="2b0ed-2368">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2368">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="2b0ed-2369">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2369">`databaseDtuMin`.</span></span> <span data-ttu-id="2b0ed-2370">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2370">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="2b0ed-2371">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2371">`databaseDtuMax`.</span></span> <span data-ttu-id="2b0ed-2372">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2372">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="2b0ed-2373">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2373">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="2b0ed-2374">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2374">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-2375">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2375">Storage</span></span>

* <span data-ttu-id="2b0ed-2376">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2376">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="2b0ed-2377">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2377">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2378">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2378">VM</span></span>

* <span data-ttu-id="2b0ed-2379">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2379">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="2b0ed-2380">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2380">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="2b0ed-2381">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2381">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="2b0ed-2382">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2382">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="2b0ed-2383">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2383">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="2b0ed-2384">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2384">May 7, 2018</span></span>

<span data-ttu-id="2b0ed-2385">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2385">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-2386">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2386">Core</span></span>

* <span data-ttu-id="2b0ed-2387">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2387">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="2b0ed-2388">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2388">Added limited support for positional arguments</span></span>
* <span data-ttu-id="2b0ed-2389">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2389">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="2b0ed-2390">#5591</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2390">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="2b0ed-2391">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2391">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="2b0ed-2392">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2392">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="2b0ed-2393">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2393">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="2b0ed-2394">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2394">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="2b0ed-2395">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2395">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-2396">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2396">ACR</span></span>

* <span data-ttu-id="2b0ed-2397">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2397">Added ACR Build commands</span></span>
* <span data-ttu-id="2b0ed-2398">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2398">Improved resource not found error messages</span></span>
* <span data-ttu-id="2b0ed-2399">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2399">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="2b0ed-2400">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2400">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="2b0ed-2401">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2401">Improved repository commands error messages</span></span>
* <span data-ttu-id="2b0ed-2402">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2402">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-2403">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2403">ACS</span></span>

* <span data-ttu-id="2b0ed-2404">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2404">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="2b0ed-2405">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2405">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="2b0ed-2406">AMS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2406">AMS</span></span>

* <span data-ttu-id="2b0ed-2407">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2407">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-2408">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2408">Appservice</span></span>

* <span data-ttu-id="2b0ed-2409">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2409">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="2b0ed-2410">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2410">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="2b0ed-2411">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2411">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="2b0ed-2412">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2412">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="2b0ed-2413">Batch AI</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2413">Batch AI</span></span>

* <span data-ttu-id="2b0ed-2414">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2414">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="2b0ed-2415">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2415">Cognitive Services</span></span>

* <span data-ttu-id="2b0ed-2416">Исправлена опечатка в примере для `cognitiveservices account create` ([№ 5603](https://github.com/Azure/azure-cli/issues/5603)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2416">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="2b0ed-2417">Потребление</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2417">Consumption</span></span>

* <span data-ttu-id="2b0ed-2418">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2418">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="2b0ed-2419">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2419">Container</span></span>

* <span data-ttu-id="2b0ed-2420">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2420">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="2b0ed-2421">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2421">Cosmos DB</span></span>

* <span data-ttu-id="2b0ed-2422">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2422">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="2b0ed-2423">DMS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2423">DMS</span></span>

* <span data-ttu-id="2b0ed-2424">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2424">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="2b0ed-2425">Расширение</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2425">Extension</span></span>

* <span data-ttu-id="2b0ed-2426">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2426">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="2b0ed-2427">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2427">Interactive</span></span>

* <span data-ttu-id="2b0ed-2428">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2428">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="2b0ed-2429">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2429">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="2b0ed-2430">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2430">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="2b0ed-2431">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2431">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="2b0ed-2432">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2432">Lab</span></span>

* <span data-ttu-id="2b0ed-2433">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2433">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-2434">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2434">Network</span></span>

* <span data-ttu-id="2b0ed-2435">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2435">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="2b0ed-2436">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2436">Profile</span></span>

* <span data-ttu-id="2b0ed-2437">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2437">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="2b0ed-2438">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2438">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="2b0ed-2439">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2439">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="2b0ed-2440">Redis</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2440">Redis</span></span>

* <span data-ttu-id="2b0ed-2441">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2441">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="2b0ed-2442">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2442">Deprecated `redis list-all`.</span></span> <span data-ttu-id="2b0ed-2443">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2443">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="2b0ed-2444">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2444">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="2b0ed-2445">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2445">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-2446">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2446">Role</span></span>

* <span data-ttu-id="2b0ed-2447">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2447">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-2448">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2448">Storage</span></span>

* <span data-ttu-id="2b0ed-2449">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2449">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="2b0ed-2450">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2450">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="2b0ed-2451">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2451">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="2b0ed-2452">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2452">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="2b0ed-2453">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2453">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2454">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2454">VM</span></span>

* <span data-ttu-id="2b0ed-2455">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2455">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="2b0ed-2456">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2456">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="2b0ed-2457">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2457">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="2b0ed-2458">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2458">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="2b0ed-2459">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2459">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="2b0ed-2460">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2460">Added write accelerator support</span></span>
* <span data-ttu-id="2b0ed-2461">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2461">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="2b0ed-2462">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2462">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="2b0ed-2463">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2463">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="2b0ed-2464">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2464">April 10, 2018</span></span>

<span data-ttu-id="2b0ed-2465">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2465">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-2466">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2466">ACR</span></span>

* <span data-ttu-id="2b0ed-2467">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2467">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-2468">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2468">ACS</span></span>

* <span data-ttu-id="2b0ed-2469">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2469">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-2470">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2470">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="2b0ed-2472">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2472">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="2b0ed-2473">Batch AI</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2473">BatchAI</span></span>

* <span data-ttu-id="2b0ed-2474">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2474">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="2b0ed-2475">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2475">Job level mounting</span></span>
  - <span data-ttu-id="2b0ed-2476">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2476">Environment variables with secret values</span></span>
  - <span data-ttu-id="2b0ed-2477">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2477">Performance counters settings</span></span>
  - <span data-ttu-id="2b0ed-2478">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2478">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="2b0ed-2479">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2479">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="2b0ed-2480">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2480">Usage and limits reporting</span></span>
  - <span data-ttu-id="2b0ed-2481">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2481">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="2b0ed-2482">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2482">Support for custom images</span></span>
  - <span data-ttu-id="2b0ed-2483">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2483">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="2b0ed-2484">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2484">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="2b0ed-2485">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2485">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="2b0ed-2486">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2486">National clouds are supported</span></span>
* <span data-ttu-id="2b0ed-2487">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2487">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="2b0ed-2488">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2488">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="2b0ed-2489">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2489">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="2b0ed-2490">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2490">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="2b0ed-2491">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2491">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="2b0ed-2492">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2492">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="2b0ed-2493">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2493">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="2b0ed-2494">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2494">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="2b0ed-2495">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2495">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="2b0ed-2496">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2496">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="2b0ed-2497">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2497">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="2b0ed-2498">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2498">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="2b0ed-2499">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2499">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="2b0ed-2500">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2500">Billing</span></span>

* <span data-ttu-id="2b0ed-2501">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2501">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="2b0ed-2502">Потребление</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2502">Consumption</span></span>

* <span data-ttu-id="2b0ed-2503">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2503">Added `marketplace` commands</span></span>
* <span data-ttu-id="2b0ed-2504">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2504">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="2b0ed-2505">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2505">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="2b0ed-2506">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2506">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="2b0ed-2507">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2507">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="2b0ed-2508">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2508">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="2b0ed-2509">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2509">Container</span></span>

* <span data-ttu-id="2b0ed-2510">Добавлены параметры подключения тома репозитория Git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2510">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="2b0ed-2511">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2511">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="2b0ed-2512">Расширение</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2512">Extension</span></span>

* <span data-ttu-id="2b0ed-2513">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2513">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="2b0ed-2514">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2514">Interactive</span></span>

* <span data-ttu-id="2b0ed-2515">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2515">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="2b0ed-2516">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2516">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="2b0ed-2517">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2517">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-2518">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2518">Network</span></span>

* <span data-ttu-id="2b0ed-2519">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2519">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="2b0ed-2520">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2520">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="2b0ed-2521">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2521">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="2b0ed-2522">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2522">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="2b0ed-2523">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2523">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="2b0ed-2524">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2524">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="2b0ed-2525">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2525">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="2b0ed-2526">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2526">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="2b0ed-2527">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2527">Profile</span></span>

* <span data-ttu-id="2b0ed-2528">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2528">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="2b0ed-2529">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi` & `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2529">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="2b0ed-2530">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2530">RDBMS</span></span>

* <span data-ttu-id="2b0ed-2531">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2531">Added `georestore` command</span></span>
* <span data-ttu-id="2b0ed-2532">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2532">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-2533">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2533">Resource</span></span>

* <span data-ttu-id="2b0ed-2534">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2534">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="2b0ed-2535">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2535">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-2536">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2536">SQL</span></span>

* <span data-ttu-id="2b0ed-2537">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2537">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-2538">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2538">Storage</span></span>

* <span data-ttu-id="2b0ed-2539">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2539">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2540">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2540">VM</span></span>

* <span data-ttu-id="2b0ed-2541">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2541">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="2b0ed-2542">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2542">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="2b0ed-2544">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2544">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="2b0ed-2545">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2545">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="2b0ed-2546">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2546">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="2b0ed-2547">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2547">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="2b0ed-2548">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2548">March 27, 2018</span></span>

<span data-ttu-id="2b0ed-2549">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2549">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-2550">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2550">Core</span></span>

* <span data-ttu-id="2b0ed-2551">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2551">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-2552">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2552">ACS</span></span>

* <span data-ttu-id="2b0ed-2553">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2553">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-2554">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2554">Appservice</span></span>

* <span data-ttu-id="2b0ed-2555">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2555">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="2b0ed-2556">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2556">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="2b0ed-2557">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2557">Backup</span></span>

* <span data-ttu-id="2b0ed-2558">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2558">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="2b0ed-2559">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2559">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="2b0ed-2560">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2560">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="2b0ed-2561">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2561">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="2b0ed-2562">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2562">Container</span></span>

* <span data-ttu-id="2b0ed-2563">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2563">Added `container exec` command.</span></span> <span data-ttu-id="2b0ed-2564">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2564">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="2b0ed-2565">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2565">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="2b0ed-2566">Расширение</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2566">Extension</span></span>

* <span data-ttu-id="2b0ed-2567">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2567">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="2b0ed-2568">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2568">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="2b0ed-2569">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2569">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="2b0ed-2570">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2570">Interactive</span></span>

* <span data-ttu-id="2b0ed-2571">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2571">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="2b0ed-2572">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2572">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="2b0ed-2573">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2573">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="2b0ed-2574">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2574">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="2b0ed-2575">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2575">Lab</span></span>

* <span data-ttu-id="2b0ed-2576">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2576">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-2577">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2577">Monitor</span></span>

* <span data-ttu-id="2b0ed-2578">Добавлена поддержка аргументов `--top`, `--orderby` и `--namespace` для `metrics list` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2578">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="2b0ed-2579">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2579">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="2b0ed-2580">Добавлена поддержка `--namespace` для `metrics list-definitions` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2580">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-2581">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2581">Network</span></span>

* <span data-ttu-id="2b0ed-2582">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2582">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="2b0ed-2583">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2583">Profile</span></span>

* <span data-ttu-id="2b0ed-2584">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2584">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="2b0ed-2585">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2585">RDBMS</span></span>

* <span data-ttu-id="2b0ed-2586">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2586">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-2587">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2587">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="2b0ed-2589">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2589">Role</span></span>

* <span data-ttu-id="2b0ed-2590">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2590">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="2b0ed-2591">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2591">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="2b0ed-2592">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2592">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="2b0ed-2593">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2593">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="2b0ed-2594">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2594">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-2595">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2595">Storage</span></span>

* <span data-ttu-id="2b0ed-2596">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2596">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="2b0ed-2597">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2597">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2598">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2598">VM</span></span>

* <span data-ttu-id="2b0ed-2599">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2599">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="2b0ed-2600">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2600">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="2b0ed-2601">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2601">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="2b0ed-2602">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2602">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="2b0ed-2603">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2603">March 13, 2018</span></span>

<span data-ttu-id="2b0ed-2604">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2604">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-2605">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2605">ACR</span></span>

* <span data-ttu-id="2b0ed-2606">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2606">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="2b0ed-2607">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2607">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="2b0ed-2608">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2608">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-2609">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2609">ACS</span></span>

* <span data-ttu-id="2b0ed-2610">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2610">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="2b0ed-2611">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2611">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="2b0ed-2612">Помощник</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2612">Advisor</span></span>

* <span data-ttu-id="2b0ed-2613">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2613">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="2b0ed-2614">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2614">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="2b0ed-2615">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2615">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="2b0ed-2616">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2616">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="2b0ed-2617">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2617">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-2618">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2618">Appservice</span></span>

* <span data-ttu-id="2b0ed-2619">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2619">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="2b0ed-2620">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2620">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="2b0ed-2621">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2621">Eventhubs</span></span>

* <span data-ttu-id="2b0ed-2622">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2622">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="2b0ed-2623">Расширение</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2623">Extension</span></span>

* <span data-ttu-id="2b0ed-2624">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2624">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="2b0ed-2625">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2625">Interactive</span></span>

* <span data-ttu-id="2b0ed-2626">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2626">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="2b0ed-2627">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2627">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="2b0ed-2628">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2628">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="2b0ed-2629">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2629">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-2630">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2630">Monitor</span></span>

* <span data-ttu-id="2b0ed-2631">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2631">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="2b0ed-2632">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2632">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="2b0ed-2633">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2633">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="2b0ed-2634">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2634">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-2635">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2635">Network</span></span>

* <span data-ttu-id="2b0ed-2636">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2636">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="2b0ed-2637">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2637">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="2b0ed-2638">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2638">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="2b0ed-2639">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2639">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="2b0ed-2640">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2640">Profile</span></span>

* <span data-ttu-id="2b0ed-2641">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2641">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="2b0ed-2642">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2642">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="2b0ed-2643">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2643">RDBMS</span></span>

* <span data-ttu-id="2b0ed-2644">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2644">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="2b0ed-2645">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2645">Service Bus</span></span>

* <span data-ttu-id="2b0ed-2646">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2646">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-2647">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2647">Storage</span></span>

* <span data-ttu-id="2b0ed-2648">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2648">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="2b0ed-2649">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2649">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2650">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2650">VM</span></span>

* <span data-ttu-id="2b0ed-2651">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2651">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="2b0ed-2652">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2652">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="2b0ed-2653">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2653">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="2b0ed-2654">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2654">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="2b0ed-2655">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2655">February 27, 2018</span></span>

<span data-ttu-id="2b0ed-2656">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2656">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-2657">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2657">Core</span></span>

* <span data-ttu-id="2b0ed-2658">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2658">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="2b0ed-2659">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2659">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="2b0ed-2660">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2660">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-2661">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2661">ACS</span></span>

* <span data-ttu-id="2b0ed-2662">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2662">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="2b0ed-2663">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2663">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="2b0ed-2664">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2664">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="2b0ed-2665">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2665">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-2666">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2666">Appservice</span></span>

* <span data-ttu-id="2b0ed-2667">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2667">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="2b0ed-2668">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2668">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="2b0ed-2669">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2669">Cognitive Services</span></span>

* <span data-ttu-id="2b0ed-2670">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2670">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="2b0ed-2671">Потребление</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2671">Consumption</span></span>

* <span data-ttu-id="2b0ed-2672">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2672">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="2b0ed-2673">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2673">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="2b0ed-2674">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2674">Container</span></span>

* <span data-ttu-id="2b0ed-2675">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2675">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-2676">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2676">Network</span></span>

* <span data-ttu-id="2b0ed-2677">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2677">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-2678">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2678">Resource</span></span>

* <span data-ttu-id="2b0ed-2679">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2679">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-2680">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2680">Role</span></span>

* <span data-ttu-id="2b0ed-2681">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2681">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-2682">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2682">SQL</span></span>

* <span data-ttu-id="2b0ed-2683">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2683">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-2684">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2684">Storage</span></span>

* <span data-ttu-id="2b0ed-2685">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2685">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2686">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2686">VM</span></span>

* <span data-ttu-id="2b0ed-2687">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2687">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="2b0ed-2688">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2688">February 13, 2018</span></span>

<span data-ttu-id="2b0ed-2689">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2689">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-2690">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2690">Core</span></span>

* <span data-ttu-id="2b0ed-2691">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2691">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-2692">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2692">ACS</span></span>

* <span data-ttu-id="2b0ed-2693">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2693">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="2b0ed-2694">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2694">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="2b0ed-2695">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2695">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="2b0ed-2696">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2696">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="2b0ed-2697">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2697">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="2b0ed-2698">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2698">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="2b0ed-2699">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2699">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="2b0ed-2700">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2700">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-2701">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2701">Appservice</span></span>

* <span data-ttu-id="2b0ed-2702">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2702">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="2b0ed-2703">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2703">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="2b0ed-2704">CDN</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2704">CDN</span></span>

* <span data-ttu-id="2b0ed-2705">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2705">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="2b0ed-2706">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2706">Container</span></span>

* <span data-ttu-id="2b0ed-2707">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2707">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="2b0ed-2708">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2708">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2b0ed-2709">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2709">CosmosDB</span></span>

* <span data-ttu-id="2b0ed-2710">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2710">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="2b0ed-2711">Расширение</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2711">Extension</span></span>

* <span data-ttu-id="2b0ed-2712">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2712">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="2b0ed-2713">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2713">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="2b0ed-2714">Отзывы</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2714">Feedback</span></span>

* <span data-ttu-id="2b0ed-2715">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2715">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="2b0ed-2716">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2716">Interactive</span></span>

* <span data-ttu-id="2b0ed-2717">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2717">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="2b0ed-2718">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2718">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="2b0ed-2719">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2719">IoT</span></span>

* <span data-ttu-id="2b0ed-2720">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2720">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="2b0ed-2721">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2721">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="2b0ed-2722">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2722">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="2b0ed-2723">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2723">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-2724">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2724">Monitor</span></span>

* <span data-ttu-id="2b0ed-2725">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2725">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-2726">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2726">Network</span></span>

* <span data-ttu-id="2b0ed-2727">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2727">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="2b0ed-2728">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2728">Profile</span></span>

* <span data-ttu-id="2b0ed-2729">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2729">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-2730">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2730">Resource</span></span>

* <span data-ttu-id="2b0ed-2731">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2731">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-2732">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2732">Role</span></span>

* <span data-ttu-id="2b0ed-2733">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2733">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-2734">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2734">SQL</span></span>

* <span data-ttu-id="2b0ed-2735">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2735">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="2b0ed-2736">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2736">Added `sql db rename`</span></span>
* <span data-ttu-id="2b0ed-2737">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2737">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-2738">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2738">Storage</span></span>

* <span data-ttu-id="2b0ed-2739">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2739">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2740">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2740">VM</span></span>

* <span data-ttu-id="2b0ed-2741">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2741">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="2b0ed-2742">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2742">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="2b0ed-2743">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2743">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="2b0ed-2744">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2744">January 31, 2018</span></span>

<span data-ttu-id="2b0ed-2745">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2745">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-2746">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2746">Core</span></span>

* <span data-ttu-id="2b0ed-2747">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2747">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="2b0ed-2748">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2748">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="2b0ed-2749">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2749">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="2b0ed-2750">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2750">Use `--verbose` to see</span></span>
* <span data-ttu-id="2b0ed-2751">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2751">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-2752">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2752">ACS</span></span>

* <span data-ttu-id="2b0ed-2753">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2753">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="2b0ed-2754">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2754">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-2755">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2755">Appservice</span></span>

* <span data-ttu-id="2b0ed-2756">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2756">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="2b0ed-2757">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2757">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="2b0ed-2758">CDN</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2758">CDN</span></span>

* <span data-ttu-id="2b0ed-2759">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2759">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2b0ed-2760">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2760">CosmosDB</span></span>

* <span data-ttu-id="2b0ed-2761">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2761">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="2b0ed-2762">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2762">Interactive</span></span>

* <span data-ttu-id="2b0ed-2763">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2763">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-2764">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2764">Network</span></span>

* <span data-ttu-id="2b0ed-2765">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2765">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="2b0ed-2766">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2766">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="2b0ed-2767">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2767">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="2b0ed-2768">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2768">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="2b0ed-2769">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2769">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="2b0ed-2770">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2770">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="2b0ed-2771">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2771">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="2b0ed-2772">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2772">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="2b0ed-2773">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2773">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="2b0ed-2774">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2774">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="2b0ed-2775">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2775">Profile</span></span>

* <span data-ttu-id="2b0ed-2776">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2776">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-2777">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2777">Resource</span></span>

* <span data-ttu-id="2b0ed-2778">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2778">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-2779">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2779">Storage</span></span>

* <span data-ttu-id="2b0ed-2780">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2780">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="2b0ed-2781">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2781">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="2b0ed-2782">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2782">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="2b0ed-2783">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2783">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="2b0ed-2784">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2784">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2785">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2785">VM</span></span>

* <span data-ttu-id="2b0ed-2786">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2786">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="2b0ed-2787">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2787">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="2b0ed-2788">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2788">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="2b0ed-2789">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2789">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="2b0ed-2790">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2790">January 17, 2018</span></span>

<span data-ttu-id="2b0ed-2791">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2791">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-2792">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2792">ACR</span></span>

* <span data-ttu-id="2b0ed-2793">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2793">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="2b0ed-2794">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2794">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-2795">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2795">ACS</span></span>

* <span data-ttu-id="2b0ed-2796">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2796">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="2b0ed-2797">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2797">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-2798">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2798">Appservice</span></span>

* <span data-ttu-id="2b0ed-2799">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2799">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="2b0ed-2800">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2800">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="2b0ed-2801">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2801">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="2b0ed-2802">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2802">Backup</span></span>

* <span data-ttu-id="2b0ed-2803">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2803">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="2b0ed-2804">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2804">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="2b0ed-2805">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2805">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="2b0ed-2806">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2806">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="2b0ed-2807">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2807">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="2b0ed-2808">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2808">Batch</span></span>

* <span data-ttu-id="2b0ed-2809">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2809">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="2b0ed-2810">Cloud</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2810">Cloud</span></span>

* <span data-ttu-id="2b0ed-2811">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2811">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="2b0ed-2812">Потребление</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2812">Consumption</span></span>

* <span data-ttu-id="2b0ed-2813">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2813">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="2b0ed-2814">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2814">Event Grid</span></span>

* <span data-ttu-id="2b0ed-2815">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2815">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="2b0ed-2816">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2816">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="2b0ed-2817">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2817">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="2b0ed-2818">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2818">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="2b0ed-2819">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2819">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="2b0ed-2820">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2820">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="2b0ed-2821">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2821">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="2b0ed-2822">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2822">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="2b0ed-2823">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2823">Interactive</span></span>

* <span data-ttu-id="2b0ed-2824">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2824">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="2b0ed-2825">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2825">Fixed errors on startup</span></span>
* <span data-ttu-id="2b0ed-2826">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2826">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="2b0ed-2827">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2827">IoT</span></span>

* <span data-ttu-id="2b0ed-2828">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2828">Added support for device provisioning service</span></span>
* <span data-ttu-id="2b0ed-2829">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2829">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="2b0ed-2830">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2830">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-2831">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2831">Monitor</span></span>

* <span data-ttu-id="2b0ed-2832">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2832">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="2b0ed-2833">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2833">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="2b0ed-2834">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2834">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-2835">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2835">Network</span></span>

* <span data-ttu-id="2b0ed-2836">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2836">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="2b0ed-2837">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2837">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="2b0ed-2838">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2838">Profile</span></span>

* <span data-ttu-id="2b0ed-2839">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2839">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-2840">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2840">Role</span></span>

* <span data-ttu-id="2b0ed-2841">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2841">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="2b0ed-2842">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2842">Service Fabric</span></span>

* <span data-ttu-id="2b0ed-2843">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2843">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="2b0ed-2844">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2844">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2845">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2845">VM</span></span>

* <span data-ttu-id="2b0ed-2846">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2846">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="2b0ed-2847">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2847">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="2b0ed-2848">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2848">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="2b0ed-2849">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2849">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="2b0ed-2850">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2850">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="2b0ed-2851">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2851">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="2b0ed-2852">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2852">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="2b0ed-2853">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2853">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="2b0ed-2854">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2854">December 19, 2017</span></span>

<span data-ttu-id="2b0ed-2855">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2855">Version 2.0.23</span></span>

* <span data-ttu-id="2b0ed-2856">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2856">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="2b0ed-2857">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2857">Container</span></span>

* <span data-ttu-id="2b0ed-2858">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2858">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-2859">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2859">Network</span></span>

* <span data-ttu-id="2b0ed-2860">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2860">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="2b0ed-2861">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2861">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-2862">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2862">Storage</span></span>

* <span data-ttu-id="2b0ed-2863">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2863">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2864">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2864">VM</span></span>

* <span data-ttu-id="2b0ed-2865">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2865">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="2b0ed-2866">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2866">December 5, 2017</span></span>

<span data-ttu-id="2b0ed-2867">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2867">Version 2.0.22</span></span>

* <span data-ttu-id="2b0ed-2868">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2868">Removed `az component` commands.</span></span> <span data-ttu-id="2b0ed-2869">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2869">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-2870">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2870">Core</span></span>
* <span data-ttu-id="2b0ed-2871">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2871">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="2b0ed-2872">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2872">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-2873">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2873">ACS</span></span>

* <span data-ttu-id="2b0ed-2874">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2874">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="2b0ed-2875">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2875">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="2b0ed-2876">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2876">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="2b0ed-2877">Помощник</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2877">Advisor</span></span>

* <span data-ttu-id="2b0ed-2878">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2878">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-2879">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2879">Appservice</span></span>

* <span data-ttu-id="2b0ed-2880">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2880">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="2b0ed-2881">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2881">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="2b0ed-2882">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2882">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="2b0ed-2883">Потребление</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2883">Consumption</span></span>

* <span data-ttu-id="2b0ed-2884">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2884">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="2b0ed-2885">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2885">Container</span></span>

* <span data-ttu-id="2b0ed-2886">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2886">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-2887">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2887">Monitor</span></span>

* <span data-ttu-id="2b0ed-2888">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2888">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-2889">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2889">Resource</span></span>

* <span data-ttu-id="2b0ed-2890">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2890">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-2891">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2891">Role</span></span>

* <span data-ttu-id="2b0ed-2892">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2892">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="2b0ed-2893">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2893">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="2b0ed-2894">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2894">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-2895">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2895">SQL</span></span>

* <span data-ttu-id="2b0ed-2896">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2896">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="2b0ed-2897">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2897">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2898">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2898">VM</span></span>

* <span data-ttu-id="2b0ed-2899">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2899">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="2b0ed-2900">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2900">November 14, 2017</span></span>

<span data-ttu-id="2b0ed-2901">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2901">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-2902">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2902">ACR</span></span>

* <span data-ttu-id="2b0ed-2903">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2903">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="2b0ed-2904">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2904">ACS</span></span>

* <span data-ttu-id="2b0ed-2905">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2905">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="2b0ed-2906">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2906">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="2b0ed-2907">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2907">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="2b0ed-2908">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2908">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="2b0ed-2909">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2909">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-2910">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2910">Appservice</span></span>

* <span data-ttu-id="2b0ed-2911">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2911">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="2b0ed-2912">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2912">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="2b0ed-2913">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2913">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="2b0ed-2914">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2914">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="2b0ed-2915">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2915">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="2b0ed-2916">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2916">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="2b0ed-2917">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2917">Batch</span></span>

* <span data-ttu-id="2b0ed-2918">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2918">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="2b0ed-2919">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2919">Batchai</span></span>

* <span data-ttu-id="2b0ed-2920">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2920">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="2b0ed-2921">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2921">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="2b0ed-2922">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2922">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="2b0ed-2923">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2923">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="2b0ed-2924">Cloud</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2924">Cloud</span></span>

* <span data-ttu-id="2b0ed-2925">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2925">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="2b0ed-2926">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2926">Container</span></span>

* <span data-ttu-id="2b0ed-2927">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2927">Added support to open multiple ports</span></span>
* <span data-ttu-id="2b0ed-2928">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2928">Added container group restart policy</span></span>
* <span data-ttu-id="2b0ed-2929">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2929">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="2b0ed-2930">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2930">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="2b0ed-2931">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2931">Data Lake Analytics</span></span>

* <span data-ttu-id="2b0ed-2932">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2932">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="2b0ed-2933">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2933">Data Lake Store</span></span>

* <span data-ttu-id="2b0ed-2934">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2934">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="2b0ed-2935">Расширение</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2935">Extension</span></span>

* <span data-ttu-id="2b0ed-2936">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2936">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="2b0ed-2937">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2937">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="2b0ed-2938">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2938">IoT</span></span>

* <span data-ttu-id="2b0ed-2939">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2939">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-2940">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2940">Monitor</span></span>

* <span data-ttu-id="2b0ed-2941">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2941">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-2942">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2942">Network</span></span>

* <span data-ttu-id="2b0ed-2943">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2943">Added support for CAA DNS records</span></span>
* <span data-ttu-id="2b0ed-2944">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2944">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="2b0ed-2945">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2945">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="2b0ed-2946">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2946">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="2b0ed-2947">Резервирование</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2947">Reservations</span></span>

* <span data-ttu-id="2b0ed-2948">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2948">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-2949">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2949">Resource</span></span>

* <span data-ttu-id="2b0ed-2950">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2950">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-2951">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2951">SQL</span></span>

* <span data-ttu-id="2b0ed-2952">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2952">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-2953">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2953">Storage</span></span>

* <span data-ttu-id="2b0ed-2954">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2954">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="2b0ed-2955">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2955">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="2b0ed-2956">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2956">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="2b0ed-2957">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2957">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="2b0ed-2958">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2958">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="2b0ed-2959">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2959">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="2b0ed-2960">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2960">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2961">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2961">VM</span></span>

* <span data-ttu-id="2b0ed-2962">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2962">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="2b0ed-2963">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2963">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="2b0ed-2964">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2964">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="2b0ed-2965">Переименование `vm format-secret` в `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2965">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="2b0ed-2966">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2966">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="2b0ed-2967">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2967">October 24, 2017</span></span>

<span data-ttu-id="2b0ed-2968">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2968">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-2969">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2969">Core</span></span>

* <span data-ttu-id="2b0ed-2970">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2970">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-2971">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2971">ACR</span></span>

* <span data-ttu-id="2b0ed-2972">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2972">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="2b0ed-2973">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2973">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="2b0ed-2974">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2974">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-2975">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2975">ACS</span></span>

* <span data-ttu-id="2b0ed-2976">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2976">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="2b0ed-2977">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2977">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-2978">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2978">Appservice</span></span>

* <span data-ttu-id="2b0ed-2979">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2979">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="2b0ed-2980">Компонент</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2980">Component</span></span>

* <span data-ttu-id="2b0ed-2981">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2981">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-2982">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2982">Monitor</span></span>

* <span data-ttu-id="2b0ed-2983">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2983">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-2984">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2984">Resource</span></span>

* <span data-ttu-id="2b0ed-2985">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2985">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="2b0ed-2986">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2986">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-2987">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2987">VM</span></span>

* <span data-ttu-id="2b0ed-2988">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2988">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="2b0ed-2989">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2989">October 9, 2017</span></span>

<span data-ttu-id="2b0ed-2990">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2990">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-2991">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2991">Core</span></span>

* <span data-ttu-id="2b0ed-2992">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2992">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-2993">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2993">Appservice</span></span>

* <span data-ttu-id="2b0ed-2994">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2994">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="2b0ed-2995">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2995">Batch</span></span>

* <span data-ttu-id="2b0ed-2996">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2996">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="2b0ed-2997">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2997">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="2b0ed-2998">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2998">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="2b0ed-2999">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-2999">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="2b0ed-3000">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3000">Batchai</span></span>

* <span data-ttu-id="2b0ed-3001">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3001">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="2b0ed-3002">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3002">Keyvault</span></span>

* <span data-ttu-id="2b0ed-3003">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3003">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="2b0ed-3004">(#4448)</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3004">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="2b0ed-3005">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3005">Network</span></span>

* <span data-ttu-id="2b0ed-3006">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3006">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="2b0ed-3007">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3007">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-3008">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3008">Resource</span></span>

* <span data-ttu-id="2b0ed-3009">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3009">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="2b0ed-3010">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3010">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="2b0ed-3011">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3011">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="2b0ed-3012">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3012">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-3013">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3013">Sql</span></span>

* <span data-ttu-id="2b0ed-3014">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3014">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="2b0ed-3015">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3015">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="2b0ed-3016">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3016">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-3017">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3017">Storage</span></span>

* <span data-ttu-id="2b0ed-3018">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3018">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-3019">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3019">Vm</span></span>

* <span data-ttu-id="2b0ed-3020">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3020">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="2b0ed-3021">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3021">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="2b0ed-3022">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3022">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="2b0ed-3023">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3023">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="2b0ed-3024">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3024">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="2b0ed-3025">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3025">September 22, 2017</span></span>

<span data-ttu-id="2b0ed-3026">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3026">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-3027">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3027">Resource</span></span>

* <span data-ttu-id="2b0ed-3028">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3028">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="2b0ed-3029">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3029">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="2b0ed-3030">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3030">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="2b0ed-3031">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3031">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-3032">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3032">Network</span></span>

* <span data-ttu-id="2b0ed-3033">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3033">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="2b0ed-3034">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3034">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="2b0ed-3035">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3035">Added `asg` application security group commands</span></span>
* <span data-ttu-id="2b0ed-3036">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3036">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="2b0ed-3037">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3037">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="2b0ed-3038">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3038">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="2b0ed-3039">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3039">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-3040">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3040">Storage</span></span>

* <span data-ttu-id="2b0ed-3041">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3041">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="2b0ed-3042">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3042">Eventgrid</span></span>

* <span data-ttu-id="2b0ed-3043">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3043">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-3044">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3044">SQL</span></span>

* <span data-ttu-id="2b0ed-3045">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3045">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="2b0ed-3046">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3046">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="2b0ed-3047">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3047">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="2b0ed-3048">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3048">Keyvault</span></span>

* <span data-ttu-id="2b0ed-3049">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3049">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-3050">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3050">VM</span></span>

* <span data-ttu-id="2b0ed-3051">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3051">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="2b0ed-3052">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3052">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="2b0ed-3053">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3053">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="2b0ed-3054">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3054">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="2b0ed-3055">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3055">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="2b0ed-3056">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3056">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-3057">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3057">ACS</span></span>

* <span data-ttu-id="2b0ed-3058">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3058">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-3059">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3059">Appservice</span></span>

* <span data-ttu-id="2b0ed-3060">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3060">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="2b0ed-3061">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3061">Backup</span></span>

* <span data-ttu-id="2b0ed-3062">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3062">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="2b0ed-3063">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3063">September 11, 2017</span></span>

<span data-ttu-id="2b0ed-3064">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3064">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="2b0ed-3065">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3065">Core</span></span>

* <span data-ttu-id="2b0ed-3066">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3066">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="2b0ed-3067">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3067">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-3068">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3068">Acs</span></span>

* <span data-ttu-id="2b0ed-3069">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3069">Added `acs list-locations` command</span></span>
* <span data-ttu-id="2b0ed-3070">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3070">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-3071">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3071">Appservice</span></span>

* <span data-ttu-id="2b0ed-3072">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3072">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="2b0ed-3073">CDN</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3073">CDN</span></span>

* <span data-ttu-id="2b0ed-3074">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3074">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="2b0ed-3075">Расширение</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3075">Extension</span></span>

* <span data-ttu-id="2b0ed-3076">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3076">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="2b0ed-3077">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3077">Keyvault</span></span>

* <span data-ttu-id="2b0ed-3078">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3078">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-3079">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3079">Network</span></span>

* <span data-ttu-id="2b0ed-3080">Переименование `vnet list-private-access-services` в `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3080">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="2b0ed-3081">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3081">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="2b0ed-3082">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3082">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="2b0ed-3083">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3083">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="2b0ed-3084">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3084">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-3085">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3085">Resource</span></span>

* <span data-ttu-id="2b0ed-3086">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3086">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="2b0ed-3087">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3087">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="2b0ed-3088">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3088">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="2b0ed-3089">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3089">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-3090">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3090">SQL</span></span>

* <span data-ttu-id="2b0ed-3091">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3091">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-3092">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3092">VM</span></span>

* <span data-ttu-id="2b0ed-3093">Исправлено: Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3093">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="2b0ed-3094">Исправлено: Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3094">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="2b0ed-3095">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3095">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="2b0ed-3096">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3096">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="2b0ed-3097">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3097">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="2b0ed-3098">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3098">August 31, 2017</span></span>

<span data-ttu-id="2b0ed-3099">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3099">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="2b0ed-3100">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3100">Keyvault</span></span>

* <span data-ttu-id="2b0ed-3101">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3101">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="2b0ed-3102">Sf</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3102">Sf</span></span>

* <span data-ttu-id="2b0ed-3103">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3103">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-3104">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3104">Storage</span></span>

* <span data-ttu-id="2b0ed-3105">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3105">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="2b0ed-3106">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3106">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="2b0ed-3107">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3107">August 28, 2017</span></span>

<span data-ttu-id="2b0ed-3108">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3108">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="2b0ed-3109">CLI</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3109">CLI</span></span>

* <span data-ttu-id="2b0ed-3110">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3110">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-3111">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3111">ACS</span></span>

* <span data-ttu-id="2b0ed-3112">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3112">Corrected preview regions</span></span>
* <span data-ttu-id="2b0ed-3113">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3113">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="2b0ed-3114">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3114">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-3115">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3115">Appservice</span></span>

* <span data-ttu-id="2b0ed-3116">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3116">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="2b0ed-3117">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3117">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="2b0ed-3118">Предоставлен параметр `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3118">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="2b0ed-3119">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3119">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="2b0ed-3120">Исправлено: Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3120">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="2b0ed-3121">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3121">IoT</span></span>

* <span data-ttu-id="2b0ed-3122">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3122">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-3123">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3123">Network</span></span>

* <span data-ttu-id="2b0ed-3124">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3124">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="2b0ed-3125">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3125">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="2b0ed-3126">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3126">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="2b0ed-3127">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3127">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="2b0ed-3128">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3128">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="2b0ed-3129">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3129">Profile</span></span>

* <span data-ttu-id="2b0ed-3130">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3130">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="2b0ed-3131">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3131">Service Fabric</span></span>

* <span data-ttu-id="2b0ed-3132">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3132">Preview release</span></span>
* <span data-ttu-id="2b0ed-3133">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3133">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="2b0ed-3134">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3134">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="2b0ed-3135">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3135">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-3136">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3136">Storage</span></span>

* <span data-ttu-id="2b0ed-3137">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3137">Enabled setting blob tier</span></span>
* <span data-ttu-id="2b0ed-3138">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3138">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="2b0ed-3139">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3139">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="2b0ed-3140">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3140">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="2b0ed-3141">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3141">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="2b0ed-3142">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3142">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-3143">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3143">VM</span></span>

* <span data-ttu-id="2b0ed-3144">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3144">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="2b0ed-3145">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3145">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="2b0ed-3146">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3146">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="2b0ed-3147">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3147">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="2b0ed-3148">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3148">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="2b0ed-3149">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3149">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="2b0ed-3150">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3150">August 15, 2017</span></span>

<span data-ttu-id="2b0ed-3151">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3151">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-3152">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3152">ACS</span></span>

* <span data-ttu-id="2b0ed-3153">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3153">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-3154">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3154">Appservice</span></span>

* <span data-ttu-id="2b0ed-3155">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3155">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="2b0ed-3156">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3156">Event Grid</span></span>

* <span data-ttu-id="2b0ed-3157">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3157">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="2b0ed-3158">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3158">August 11, 2017</span></span>

<span data-ttu-id="2b0ed-3159">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3159">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-3160">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3160">ACS</span></span>

* <span data-ttu-id="2b0ed-3161">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3161">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="2b0ed-3162">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3162">Batch</span></span>

* <span data-ttu-id="2b0ed-3163">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3163">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="2b0ed-3164">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3164">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="2b0ed-3165">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3165">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="2b0ed-3166">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3166">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="2b0ed-3167">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3167">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="2b0ed-3168">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3168">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="2b0ed-3169">Компонент</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3169">Component</span></span>

* <span data-ttu-id="2b0ed-3170">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3170">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="2b0ed-3171">Контейнер</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3171">Container</span></span>

* <span data-ttu-id="2b0ed-3172">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3172">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="2b0ed-3173">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3173">Data Lake Store</span></span>

* <span data-ttu-id="2b0ed-3174">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3174">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="2b0ed-3175">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3175">Event Grid</span></span>

* <span data-ttu-id="2b0ed-3176">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3176">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-3177">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3177">Network</span></span>

* <span data-ttu-id="2b0ed-3178">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3178">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="2b0ed-3179">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3179">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="2b0ed-3180">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3180">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="2b0ed-3181">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3181">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="2b0ed-3182">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3182">Profile</span></span>

* <span data-ttu-id="2b0ed-3183">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3183">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-3184">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3184">Storage</span></span>

* <span data-ttu-id="2b0ed-3185">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3185">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-3186">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3186">VM</span></span>

* <span data-ttu-id="2b0ed-3187">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3187">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="2b0ed-3188">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3188">Exposed `list-skus` command</span></span>
* <span data-ttu-id="2b0ed-3189">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3189">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="2b0ed-3190">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3190">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="2b0ed-3191">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3191">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="2b0ed-3192">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3192">July 28, 2017</span></span>

<span data-ttu-id="2b0ed-3193">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3193">Version 2.0.12</span></span>

* <span data-ttu-id="2b0ed-3194">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3194">Added container commands</span></span>
* <span data-ttu-id="2b0ed-3195">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3195">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="2b0ed-3196">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3196">Core</span></span>

* <span data-ttu-id="2b0ed-3197">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3197">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="2b0ed-3198">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3198">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="2b0ed-3199">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3199">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="2b0ed-3200">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3200">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="2b0ed-3201">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3201">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="2b0ed-3202">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3202">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="2b0ed-3203">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3203">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="2b0ed-3204">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3204">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="2b0ed-3205">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3205">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="2b0ed-3206">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3206">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="2b0ed-3207">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3207">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="2b0ed-3208">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3208">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="2b0ed-3209">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3209">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="2b0ed-3210">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3210">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="2b0ed-3211">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3211">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="2b0ed-3212">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3212">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="2b0ed-3213">ACR</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3213">ACR</span></span>

* <span data-ttu-id="2b0ed-3214">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3214">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="2b0ed-3215">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3215">Support SKU update for managed registries</span></span>
* <span data-ttu-id="2b0ed-3216">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3216">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="2b0ed-3217">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3217">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="2b0ed-3218">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3218">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="2b0ed-3219">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3219">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-3220">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3220">ACS</span></span>

* <span data-ttu-id="2b0ed-3221">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3221">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-3222">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3222">Appservice</span></span>

* <span data-ttu-id="2b0ed-3223">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3223">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="2b0ed-3224">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3224">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="2b0ed-3225">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3225">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="2b0ed-3226">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3226">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="2b0ed-3227">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3227">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="2b0ed-3228">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3228">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="2b0ed-3229">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3229">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="2b0ed-3230">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3230">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="2b0ed-3231">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3231">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="2b0ed-3232">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3232">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="2b0ed-3233">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3233">Batch</span></span>

* <span data-ttu-id="2b0ed-3234">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3234">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="2b0ed-3235">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3235">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="2b0ed-3236">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3236">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="2b0ed-3237">CDN</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3237">CDN</span></span>

* <span data-ttu-id="2b0ed-3238">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3238">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="2b0ed-3239">Cloud</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3239">Cloud</span></span>

* <span data-ttu-id="2b0ed-3240">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3240">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="2b0ed-3241">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3241">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="2b0ed-3242">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3242">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="2b0ed-3243">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3243">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="2b0ed-3244">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3244">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2b0ed-3245">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3245">CosmosDB</span></span>

* <span data-ttu-id="2b0ed-3246">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3246">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="2b0ed-3247">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3247">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="2b0ed-3248">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3248">Data Lake Analytics</span></span>

* <span data-ttu-id="2b0ed-3249">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3249">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="2b0ed-3250">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3250">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="2b0ed-3251">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3251">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="2b0ed-3252">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3252">Data Lake Store</span></span>

* <span data-ttu-id="2b0ed-3253">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3253">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="2b0ed-3254">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3254">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="2b0ed-3255">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3255">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="2b0ed-3256">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3256">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="2b0ed-3257">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3257">Interactive</span></span>

* <span data-ttu-id="2b0ed-3258">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3258">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="2b0ed-3259">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3259">Increased test coverage</span></span>
* <span data-ttu-id="2b0ed-3260">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3260">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="2b0ed-3261">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3261">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="2b0ed-3262">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3262">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="2b0ed-3263">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3263">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="2b0ed-3264">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3264">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="2b0ed-3265">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3265">Added `--progress` flag</span></span>
* <span data-ttu-id="2b0ed-3266">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3266">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="2b0ed-3267">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3267">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="2b0ed-3268">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3268">IoT</span></span>

* <span data-ttu-id="2b0ed-3269">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3269">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="2b0ed-3270">(3934).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3270">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="2b0ed-3271">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3271">Key vault</span></span>

* <span data-ttu-id="2b0ed-3272">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3272">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="2b0ed-3273">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3273">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="2b0ed-3274">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3274">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="2b0ed-3275">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3275">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="2b0ed-3276">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3276">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="2b0ed-3277">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3277">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="2b0ed-3278">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3278">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="2b0ed-3279">(3307).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3279">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="2b0ed-3280">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3280">Lab</span></span>

* <span data-ttu-id="2b0ed-3281">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3281">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="2b0ed-3282">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3282">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-3283">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3283">Monitor</span></span>

* <span data-ttu-id="2b0ed-3284">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3284">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="2b0ed-3285">Переименование `monitor alert-rule-incidents list` в `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3285">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="2b0ed-3286">Переименование `monitor alert-rule-incidents show` в `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3286">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="2b0ed-3287">Переименование `monitor metric-defintions list` в `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3287">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="2b0ed-3288">Переименование `monitor alert-rules` в `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3288">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="2b0ed-3289">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3289">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="2b0ed-3290">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3290">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="2b0ed-3291">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3291">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="2b0ed-3292">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3292">`location` no longer required</span></span>
  * <span data-ttu-id="2b0ed-3293">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3293">Add name and ID support for target</span></span>
  * <span data-ttu-id="2b0ed-3294">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3294">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="2b0ed-3295">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3295">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="2b0ed-3296">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3296">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="2b0ed-3297">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3297">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="2b0ed-3298">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3298">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="2b0ed-3299">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3299">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-3300">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3300">Network</span></span>

* <span data-ttu-id="2b0ed-3301">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3301">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="2b0ed-3302">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3302">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="2b0ed-3303">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3303">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="2b0ed-3304">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3304">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="2b0ed-3305">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3305">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="2b0ed-3306">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3306">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="2b0ed-3307">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3307">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="2b0ed-3308">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3308">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="2b0ed-3309">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3309">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="2b0ed-3310">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3310">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="2b0ed-3311">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3311">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="2b0ed-3312">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3312">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="2b0ed-3313">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3313">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="2b0ed-3314">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3314">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="2b0ed-3315">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3315">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="2b0ed-3316">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3316">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="2b0ed-3317">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3317">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="2b0ed-3318">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3318">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="2b0ed-3319">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3319">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="2b0ed-3320">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3320">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="2b0ed-3321">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3321">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="2b0ed-3322">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3322">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="2b0ed-3323">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3323">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="2b0ed-3324">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3324">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="2b0ed-3325">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3325">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="2b0ed-3326">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3326">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="2b0ed-3327">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3327">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="2b0ed-3328">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3328">Profile</span></span>

* <span data-ttu-id="2b0ed-3329">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3329">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="2b0ed-3330">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3330">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="2b0ed-3331">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3331">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="2b0ed-3332">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3332">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="2b0ed-3333">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3333">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="2b0ed-3334">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3334">RDBMS</span></span>

* <span data-ttu-id="2b0ed-3335">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3335">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="2b0ed-3336">Исправлена проблема с обработкой `%s` из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3336">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="2b0ed-3337">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3337">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="2b0ed-3338">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3338">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-3339">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3339">Resource</span></span>

* <span data-ttu-id="2b0ed-3340">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3340">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="2b0ed-3341">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3341">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="2b0ed-3342">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3342">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="2b0ed-3343">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3343">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="2b0ed-3344">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3344">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="2b0ed-3345">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3345">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="2b0ed-3346">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3346">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="2b0ed-3347">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3347">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-3348">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3348">Role</span></span>

* <span data-ttu-id="2b0ed-3349">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3349">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="2b0ed-3350">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3350">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="2b0ed-3351">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3351">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="2b0ed-3352">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3352">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="2b0ed-3353">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3353">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="2b0ed-3354">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3354">Service Fabric</span></span>
* <span data-ttu-id="2b0ed-3355">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3355">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="2b0ed-3356">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3356">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="2b0ed-3357">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3357">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-3358">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3358">SQL</span></span>

* <span data-ttu-id="2b0ed-3359">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3359">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="2b0ed-3360">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3360">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="2b0ed-3361">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3361">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-3362">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3362">Storage</span></span>

* <span data-ttu-id="2b0ed-3363">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3363">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="2b0ed-3364">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3364">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="2b0ed-3365">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3365">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="2b0ed-3366">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3366">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="2b0ed-3367">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3367">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="2b0ed-3368">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3368">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-3369">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3369">VM</span></span>

* <span data-ttu-id="2b0ed-3370">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3370">Support configuring nsg</span></span>
* <span data-ttu-id="2b0ed-3371">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3371">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="2b0ed-3372">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3372">Support managed service identities</span></span>
* <span data-ttu-id="2b0ed-3373">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3373">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="2b0ed-3374">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3374">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="2b0ed-3375">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3375">May 10, 2017</span></span>

<span data-ttu-id="2b0ed-3376">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3376">Version 2.0.6</span></span>

* <span data-ttu-id="2b0ed-3377">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3377">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="2b0ed-3378">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3378">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="2b0ed-3379">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3379">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="2b0ed-3380">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3380">Include Cognitive Services module</span></span>
* <span data-ttu-id="2b0ed-3381">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3381">Include Service Fabric module</span></span>
* <span data-ttu-id="2b0ed-3382">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3382">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="2b0ed-3383">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3383">Add support for CDN commands</span></span>
* <span data-ttu-id="2b0ed-3384">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3384">Remove Container module</span></span>
* <span data-ttu-id="2b0ed-3385">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3385">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="2b0ed-3386">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3386">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="2b0ed-3387">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3387">Core</span></span>

* <span data-ttu-id="2b0ed-3388">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3388">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="2b0ed-3389">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([#2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3389">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="2b0ed-3390">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3390">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="2b0ed-3391">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3391">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="2b0ed-3392">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3392">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="2b0ed-3393">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3393">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="2b0ed-3394">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3394">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="2b0ed-3395">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3395">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="2b0ed-3396">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3396">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="2b0ed-3397">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3397">core: Improved performance</span></span>
* <span data-ttu-id="2b0ed-3398">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3398">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="2b0ed-3399">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3399">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-3400">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3400">ACS</span></span>

* <span data-ttu-id="2b0ed-3401">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3401">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="2b0ed-3402">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3402">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="2b0ed-3403">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3403">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="2b0ed-3404">Удален профиль Windows перед вызовом метода PUT для команды scale ([#2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3404">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-3405">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3405">AppService</span></span>

* <span data-ttu-id="2b0ed-3406">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3406">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="2b0ed-3407">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3407">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="2b0ed-3408">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3408">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="2b0ed-3409">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3409">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="2b0ed-3410">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3410">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="2b0ed-3411">Включена поддержка настройки строк подключения ([#2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3411">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="2b0ed-3412">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3412">support slot swap with preview</span></span>
* <span data-ttu-id="2b0ed-3413">Устранены ошибки из команд службы приложений ([#2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3413">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="2b0ed-3414">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([#2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3414">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="2b0ed-3415">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3415">CosmosDB</span></span>

* <span data-ttu-id="2b0ed-3416">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3416">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="2b0ed-3417">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3417">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="2b0ed-3418">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3418">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="2b0ed-3419">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3419">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="2b0ed-3420">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3420">Data Lake Analytics</span></span>

* <span data-ttu-id="2b0ed-3421">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3421">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="2b0ed-3422">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3422">Add support for new catalog item type: package.</span></span> <span data-ttu-id="2b0ed-3423">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3423">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="2b0ed-3424">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3424">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="2b0ed-3425">Таблица</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3425">Table</span></span>
  * <span data-ttu-id="2b0ed-3426">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3426">Table valued function</span></span>
  * <span data-ttu-id="2b0ed-3427">Представление</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3427">View</span></span>
  * <span data-ttu-id="2b0ed-3428">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3428">Table Statistics.</span></span> <span data-ttu-id="2b0ed-3429">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3429">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="2b0ed-3430">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3430">Data Lake Store</span></span>

* <span data-ttu-id="2b0ed-3431">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3431">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="2b0ed-3432">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3432">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="2b0ed-3433">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3433">missed help for access show.</span></span> <span data-ttu-id="2b0ed-3434">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3434">adding it.</span></span> <span data-ttu-id="2b0ed-3435">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3435">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="2b0ed-3436">Поиск</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3436">Find</span></span>

* <span data-ttu-id="2b0ed-3437">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3437">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="2b0ed-3438">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3438">KeyVault</span></span>

* <span data-ttu-id="2b0ed-3439">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3439">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="2b0ed-3440">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3440">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="2b0ed-3441">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3441">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="2b0ed-3442">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3442">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="2b0ed-3443">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3443">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="2b0ed-3444">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3444">Lab</span></span>

* <span data-ttu-id="2b0ed-3445">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3445">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="2b0ed-3446">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3446">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="2b0ed-3447">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3447">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="2b0ed-3448">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3448">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="2b0ed-3449">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3449">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="2b0ed-3450">Монитор</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3450">Monitor</span></span>

* <span data-ttu-id="2b0ed-3451">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3451">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="2b0ed-3452">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3452">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="2b0ed-3453">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3453">Network</span></span>

* <span data-ttu-id="2b0ed-3454">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3454">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="2b0ed-3455">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3455">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="2b0ed-3456">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3456">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="2b0ed-3457">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3457">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="2b0ed-3458">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3458">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="2b0ed-3459">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3459">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="2b0ed-3460">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3460">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="2b0ed-3461">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3461">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="2b0ed-3462">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3462">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="2b0ed-3463">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3463">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="2b0ed-3464">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3464">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="2b0ed-3465">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3465">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="2b0ed-3466">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3466">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="2b0ed-3467">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3467">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="2b0ed-3468">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3468">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="2b0ed-3469">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3469">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="2b0ed-3470">Профиль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3470">Profile</span></span>

* <span data-ttu-id="2b0ed-3471">Включена поддержка входа при отсутствии подписок ([#2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3471">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="2b0ed-3472">Включена поддержка сокращенных имен параметров в команде az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3472">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="2b0ed-3473">Redis</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3473">Redis</span></span>

* <span data-ttu-id="2b0ed-3474">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3474">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="2b0ed-3475">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3475">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="2b0ed-3476">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3476">Resource</span></span>

* <span data-ttu-id="2b0ed-3477">Добавлены команды определения managedapp и managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3477">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="2b0ed-3478">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3478">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="2b0ed-3479">Включена поддержка создания универсального ресурса ([#2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3479">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="2b0ed-3480">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3480">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="2b0ed-3481">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3481">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="2b0ed-3482">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3482">Add docs for az lock update.</span></span> <span data-ttu-id="2b0ed-3483">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3483">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="2b0ed-3484">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3484">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="2b0ed-3485">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3485">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="2b0ed-3486">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3486">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="2b0ed-3487">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3487">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="2b0ed-3488">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([#2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3488">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="2b0ed-3489">Роль</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3489">Role</span></span>

* <span data-ttu-id="2b0ed-3490">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([#2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3490">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="2b0ed-3491">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3491">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="2b0ed-3492">Роль: устранены проблемы при обновлении определения роли ([#2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3492">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="2b0ed-3493">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3493">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="2b0ed-3494">SQL</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3494">SQL</span></span>

* <span data-ttu-id="2b0ed-3495">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3495">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="2b0ed-3496">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3496">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="2b0ed-3497">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3497">Storage</span></span>

* <span data-ttu-id="2b0ed-3498">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3498">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="2b0ed-3499">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3499">Add support for incremental blob copy</span></span>
* <span data-ttu-id="2b0ed-3500">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3500">Add support for large block blob upload</span></span>
* <span data-ttu-id="2b0ed-3501">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3501">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-3502">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3502">VM</span></span>

* <span data-ttu-id="2b0ed-3503">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3503">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="2b0ed-3504">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3504">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="2b0ed-3505">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3505">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="2b0ed-3506">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3506">az vm/vmss disk</span></span>
  3. <span data-ttu-id="2b0ed-3507">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3507">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="2b0ed-3508">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3508">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="2b0ed-3509">vm/vmss: добавлена поддержка создания из образа Marketplace, для которого требуются сведения о плане ([#1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3509">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="2b0ed-3510">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3510">April 3, 2017</span></span>

<span data-ttu-id="2b0ed-3511">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3511">Version 2.0.2</span></span>

<span data-ttu-id="2b0ed-3512">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3512">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="2b0ed-3513">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3513">Core</span></span>

* <span data-ttu-id="2b0ed-3514">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3514">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="2b0ed-3515">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3515">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="2b0ed-3516">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3516">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="2b0ed-3517">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3517">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="2b0ed-3518">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3518">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="2b0ed-3519">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3519">Add prompting for missing template parameters.</span></span> <span data-ttu-id="2b0ed-3520">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3520">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="2b0ed-3521">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3521">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="2b0ed-3522">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3522">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="2b0ed-3523">ACS</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3523">ACS</span></span>

* <span data-ttu-id="2b0ed-3524">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3524">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="2b0ed-3525">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3525">Add support for ssh key password prompting.</span></span> <span data-ttu-id="2b0ed-3526">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3526">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="2b0ed-3527">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3527">Add support for windows clusters.</span></span> <span data-ttu-id="2b0ed-3528">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3528">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="2b0ed-3529">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3529">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="2b0ed-3530">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3530">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="2b0ed-3531">AppService</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3531">AppService</span></span>

* <span data-ttu-id="2b0ed-3532">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3532">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="2b0ed-3533">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3533">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="2b0ed-3534">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3534">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="2b0ed-3535">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3535">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="2b0ed-3536">Data Lake</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3536">DataLake</span></span>

* <span data-ttu-id="2b0ed-3537">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3537">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="2b0ed-3538">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3538">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="2b0ed-3539">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3539">DocuemntDB</span></span>

* <span data-ttu-id="2b0ed-3540">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3540">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="2b0ed-3541">ВМ</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3541">VM</span></span>

* <span data-ttu-id="2b0ed-3542">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3542">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="2b0ed-3543">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3543">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="2b0ed-3544">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3544">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="2b0ed-3545">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3545">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="2b0ed-3546">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3546">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="2b0ed-3547">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3547">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="2b0ed-3548">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3548">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="2b0ed-3549">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3549">February 27, 2017</span></span>

<span data-ttu-id="2b0ed-3550">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3550">Version 2.0.0</span></span>

<span data-ttu-id="2b0ed-3551">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3551">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="2b0ed-3552">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3552">Container Service (acs)</span></span>
- <span data-ttu-id="2b0ed-3553">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3553">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="2b0ed-3554">Сеть</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3554">Networking</span></span>
- <span data-ttu-id="2b0ed-3555">Память</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3555">Storage</span></span>

<span data-ttu-id="2b0ed-3556">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3556">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="2b0ed-3557">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3557">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="2b0ed-3558">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3558">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="2b0ed-3559">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3559">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="2b0ed-3560">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3560">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="2b0ed-3561">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3561">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="2b0ed-3562">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3562">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="2b0ed-3563">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3563">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="2b0ed-3564">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="2b0ed-3564">Provide feedback from the command line with the `az feedback` command</span></span>
