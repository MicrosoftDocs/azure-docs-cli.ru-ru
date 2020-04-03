---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 03/31/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: aed043bcb900937a405fd71dafe24016fa0972d7
ms.sourcegitcommit: b5ecfc168489cd0d96462d6decf83e8b26a10194
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2020
ms.locfileid: "80417815"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="ec6b9-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="ec6b9-103">Azure CLI release notes</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="ec6b9-104">31 марта 2020 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-104">March 31, 2020</span></span>

<span data-ttu-id="ec6b9-105">Версия 2.3.0</span><span class="sxs-lookup"><span data-stu-id="ec6b9-105">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-106">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-106">ACR</span></span>

* <span data-ttu-id="ec6b9-107">az acr task update: исключение пустого указателя.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-107">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="ec6b9-108">`az acr import`: Отредактировано справочное сообщение и сообщение об ошибке для уточнения того, как использовать параметры --source и --registry.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-108">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="ec6b9-109">Добавлено средство проверки для аргумента registry_name.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-109">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="ec6b9-110">`az acr login`: удален флаг предпросмотра для --expose-token.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-110">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="ec6b9-111">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр ветви az acr task create/update.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-111">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="ec6b9-112">Клиент az acr task update теперь может независимо обновлять контекст, токен GitHub и триггеры.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-112">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="ec6b9-113">az acr agentpool: новая функция.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-113">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="ec6b9-114">AKS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-114">AKS</span></span>

* <span data-ttu-id="ec6b9-115">Исправлена ошибка с apiServerAccessProfile при обновлении --api-server-authorized-ip-ranges.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-115">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="ec6b9-116">Обновление AKS: при обновлении исходящие IP-адреса переопределяются с помощью входных значений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-116">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="ec6b9-117">Не создаются имена субъектов-служб для кластеров MSI и реализована поддержка присоединение ACR к кластерам MSI.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-117">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="ec6b9-118">AMS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-118">AMS</span></span>

* <span data-ttu-id="ec6b9-119">Исправление 12469: не удается добавить content-key-policy для FairPlay из-за проблем с параметром ask.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-119">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="ec6b9-120">AppConfig</span><span class="sxs-lookup"><span data-stu-id="ec6b9-120">AppConfig</span></span>

* <span data-ttu-id="ec6b9-121">Добавлен параметр --skip-keyvault для экспорта kv.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-121">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-122">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-122">AppService</span></span>

* <span data-ttu-id="ec6b9-123">Исправление 12509: удален тег, добавлявшийся по умолчанию при создании приложения с помощью az webapp up.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-123">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="ec6b9-124">az functionapp create: обновлено меню справки для --runtime-version и добавлено предупреждение, когда пользователь указывает параметр --runtime-version для DotNet.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-124">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="ec6b9-125">az functionapp create: изменен способ установки JavaVersion для приложений-функций Windows.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-125">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="ec6b9-126">ARM</span><span class="sxs-lookup"><span data-stu-id="ec6b9-126">ARM</span></span>

* <span data-ttu-id="ec6b9-127">az deployment create/validate: по умолчанию используется параметр --handle-extended-json-format.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-127">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="ec6b9-128">az lock create: в справочную документацию добавлены примеры создания подресурсов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-128">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="ec6b9-129">Список az deployment {group/mg/sub/tenant}: реализована поддержка фильтрации ProvisioningState.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-129">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="ec6b9-130">az deployment: исправлена ошибка синтаксического анализа комментария в последнем аргументе.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-130">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="ec6b9-131">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="ec6b9-131">Backup</span></span>

* <span data-ttu-id="ec6b9-132">Добавлена возможность восстановления нескольких файлов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-132">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="ec6b9-133">Добавлена возможность резервного копирования только дисков с ОС.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-133">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="ec6b9-134">Добавлен параметр restore-as-unmanaged-disk, позволяющий задать неуправляемое восстановление.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-134">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="ec6b9-135">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-135">Compute</span></span>

* <span data-ttu-id="ec6b9-136">az vm create: для --nsg-rule добавлен вариант NONE.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-136">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="ec6b9-137">az vmss create/update: удален тег предпросмотра для автоматического восстановления VMSS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-137">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="ec6b9-138">az vm update: реализована поддержка --workspace.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-138">az vm update: Support --workspace</span></span>
* <span data-ttu-id="ec6b9-139">Исправлена ошибка в коде инициализации VirtualMachineScaleSetExtension.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-139">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="ec6b9-140">Версия VMAccessAgent обновлена до 2.4.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-140">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="ec6b9-141">az vmss set-orchestration-service-state: реализована поддержка состояния службы оркестрации наборов VMSS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-141">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="ec6b9-142">Версия API диска обновлена до 2019-11-01.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-142">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="ec6b9-143">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-143">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="ec6b9-144">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ec6b9-144">Cosmos DB</span></span>

* <span data-ttu-id="ec6b9-145">Добавлен отсутствовавший параметр --type для перенаправления в связи с устареванием.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-145">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="ec6b9-146">Docker</span><span class="sxs-lookup"><span data-stu-id="ec6b9-146">Docker</span></span>

* <span data-ttu-id="ec6b9-147">Обновление до Alpine 3.11 и Python 3.6.10.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-147">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="ec6b9-148">Расширение</span><span class="sxs-lookup"><span data-stu-id="ec6b9-148">Extension</span></span>

* <span data-ttu-id="ec6b9-149">Добавлена возможность загрузки расширений в системный путь через пакеты.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-149">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="ec6b9-150">HDInsight</span><span class="sxs-lookup"><span data-stu-id="ec6b9-150">HDInsight</span></span>

* <span data-ttu-id="ec6b9-151">(az hdinsight create:) Добавлена возможность указания клиентами минимальной поддерживаемой версии TLS с помощью параметра `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-151">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="ec6b9-152">Допустимые значения: 1.0,1.1,1.2.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-152">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="ec6b9-153">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-153">IoT</span></span>

* <span data-ttu-id="ec6b9-154">Добавлен параметр codeowner.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-154">Add codeowner</span></span>
* <span data-ttu-id="ec6b9-155">az iot hub create: номер SKU по умолчанию изменен с F1 на S1.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-155">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="ec6b9-156">iot hub: реализована поддержка IotHub в профиле 2019-03-01-hybrid.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-156">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="ec6b9-157">IoT Central</span><span class="sxs-lookup"><span data-stu-id="ec6b9-157">IoTCentral</span></span>

* <span data-ttu-id="ec6b9-158">Обновлены сведения об ошибках, шаблон приложения по умолчанию и сообщение с подсказкой.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-158">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="ec6b9-159">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-159">KeyVault</span></span>

* <span data-ttu-id="ec6b9-160">Реализована поддержка резервного копирования и восстановления сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-160">Support certificate backup/restore</span></span>
* <span data-ttu-id="ec6b9-161">keyvault create/update: добавлена поддержка параметра --retention-days.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-161">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="ec6b9-162">При перечислении больше не показываются управляемые ключи и секреты.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-162">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="ec6b9-163">az keyvault create: реализована поддержка `--network-acls`, `--network-acls-ips` и `--network-acls-vnets` для указания сетевых правил при создании хранилища.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-163">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="ec6b9-164">Блокировка</span><span class="sxs-lookup"><span data-stu-id="ec6b9-164">Lock</span></span>

* <span data-ttu-id="ec6b9-165">Исправлена ошибка с командой az lock delete, не работавшей с Microsoft.DocumentDB.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-165">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-166">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-166">Monitor</span></span>

* <span data-ttu-id="ec6b9-167">az monitor clone: добавлена возможность клонирования правил метрики из одного ресурса в другой.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-167">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="ec6b9-168">Исправлена ошибка IcM179210086: не удается создать настраиваемое оповещение для метрики Application Insights.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-168">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="ec6b9-169">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="ec6b9-169">NetAppFiles</span></span>

* <span data-ttu-id="ec6b9-170">az volume create: для томов защиты данных добавлены операции репликации (approve, suspend, resume, status, remove).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-170">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-171">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-171">Network</span></span>

* <span data-ttu-id="ec6b9-172">az network application-gateway waf-policy managed-rule rule-set add: добавлена поддержка Microsoft_BotManagerRuleSet.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-172">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="ec6b9-173">Журнал потоков наблюдателя за сетями: исправлены неправильные сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-173">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="ec6b9-174">Добавлена поддержка имен узлов в прослушивателе шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-174">support host names in application gateway listener</span></span>
* <span data-ttu-id="ec6b9-175">az network nat gateway: добавлена возможность создания пустого ресурса без общедоступного IP-адреса или общедоступного IP-префикса.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-175">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="ec6b9-176">Добавлена возможность создания VPN-шлюза.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-176">Support vpn gateway generation</span></span>
* <span data-ttu-id="ec6b9-177">Реализована поддержка `--if-none-match` для `az network dns record-set {} add-record`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-177">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="ec6b9-178">Упаковка</span><span class="sxs-lookup"><span data-stu-id="ec6b9-178">Packaging</span></span>

* <span data-ttu-id="ec6b9-179">Прекращена поддержка Python 3.5.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-179">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="ec6b9-180">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-180">Profile</span></span>

* <span data-ttu-id="ec6b9-181">az login: добавлен показ предупреждений об ошибках MFA.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-181">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="ec6b9-182">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ec6b9-182">RDBMS</span></span>

* <span data-ttu-id="ec6b9-183">Добавлены команды управления ключами шифрования данных сервера для PostgreSQL и MySQL.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-183">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="ec6b9-184">10 марта 2020 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-184">March 10, 2020</span></span>

<span data-ttu-id="ec6b9-185">Версия 2.2.0</span><span class="sxs-lookup"><span data-stu-id="ec6b9-185">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-186">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-186">ACR</span></span>

* <span data-ttu-id="ec6b9-187">Исправлена команда `az acr login`, которая неправильно вызывала ошибку.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-187">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="ec6b9-188">Добавлена новая команда `az acr helm install-cli`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-188">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="ec6b9-189">Добавлена частная ссылка и включена поддержка CMK.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-189">Add private link and CMK support</span></span>
* <span data-ttu-id="ec6b9-190">Добавлена команда private-link-resource list.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-190">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="ec6b9-191">AKS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-191">AKS</span></span>

* <span data-ttu-id="ec6b9-192">Исправлена функция поиска AKS в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-192">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="ec6b9-193">az aks: устранены ошибки NoneType при мониторинге надстроек и пула агентов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-193">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="ec6b9-194">Добавлен параметр --nodepool-tags в пуле узлов при создании кластера Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-194">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="ec6b9-195">Добавлен параметр --tags при добавлении пула узлов в кластер или его обновлении.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-195">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="ec6b9-196">aks create: добавлен параметр `--enable-private-cluster`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-196">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="ec6b9-197">Добавлен параметр --nodepool-labels в пуле узлов при создании кластера Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-197">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="ec6b9-198">Добавлен параметр --labels при добавлении нового пула узлов в кластер Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-198">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="ec6b9-199">Добавлен отсутствующий символ / в URL-адрес панели мониторинга.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-199">add missing / in the dashboard url</span></span>
* <span data-ttu-id="ec6b9-200">Включена поддержка создания кластеров AKS для управляемых удостоверений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-200">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="ec6b9-201">az aks: включена проверка состояния сетевого подключаемого модуля: Azure или Kubenet.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-201">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="ec6b9-202">az aks: включена поддержка ключа сеанса AAD.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-202">az aks: Add aad session key support</span></span>
* <span data-ttu-id="ec6b9-203">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az aks: включена поддержка изменений MSI для GF и BF для omsagent (мониторинг контейнеров) (1)</span><span class="sxs-lookup"><span data-stu-id="ec6b9-203">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="ec6b9-204">az aks use-dev-spaces: добавлен параметр типа конечной точки в команду use-dev-spaces для настройки конечной точки, созданной в контроллере Azure Dev Spaces.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-204">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="ec6b9-205">AppConfig</span><span class="sxs-lookup"><span data-stu-id="ec6b9-205">AppConfig</span></span>

* <span data-ttu-id="ec6b9-206">Включена разблокировка с использованием kv set для добавления функции и ссылки на хранилище ключей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-206">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-207">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-207">AppService</span></span>

* <span data-ttu-id="ec6b9-208">az webapp create: устранена проблема с выполнением команды с параметром --runtime.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-208">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="ec6b9-209">az functionapp deployment source config-zip: добавлено сообщение об ошибке, если группа ресурсов или имя функции недействительны или не существуют.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-209">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="ec6b9-210">functionapp create: исправлено сообщение с предупреждением, которое появляется с `functionapp create` и в котором указан флаг `--functions_version`, но в имени флага ошибочно используется `_` вместо `-`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-210">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="ec6b9-211">az functionapp create: обновлен способ настройки linuxFxVersion и имени образа контейнера для приложений с функциями Linux.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-211">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="ec6b9-212">az functionapp deployment source config-zip: устранена проблема, вызванная изменением параметров приложения во время развертывания ZIP, что приводит к ошибкам 5xx во время развертывания.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-212">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="ec6b9-213">Исправление 5720946: не удается задать имя с помощью az webapp backup.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-213">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="ec6b9-214">ARM</span><span class="sxs-lookup"><span data-stu-id="ec6b9-214">ARM</span></span>

* <span data-ttu-id="ec6b9-215">az resource: улучшены примеры для модуля ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-215">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="ec6b9-216">az policy assignment list: Включена поддержка списков назначений политик в области группы управления.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-216">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="ec6b9-217">Добавлены команды `az deployment group` и `az deployment operation group` для развертывания шаблонов в группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-217">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="ec6b9-218">Это дубликат `az group deployment` и `az group deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-218">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="ec6b9-219">Добавлены команды `az deployment sub` и `az deployment operation sub` для развертывания шаблонов в области подписки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-219">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="ec6b9-220">Это дубликат `az deployment` и `az deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-220">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="ec6b9-221">Добавлены команды `az deployment mg` и `az deployment operation mg` для развертывания шаблонов в группах управления.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-221">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="ec6b9-222">Добавлены команды `az deployment tenant` и `az deployment operation tenant` для развертывания шаблонов в области арендатора.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-222">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="ec6b9-223">az policy assignment create: добавлено описание параметра `--location`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-223">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="ec6b9-224">az group deployment create: добавлен параметр `--aux-tenants` для включения поддержки перекрестных арендаторов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-224">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="ec6b9-225">CDN</span><span class="sxs-lookup"><span data-stu-id="ec6b9-225">CDN</span></span>

* <span data-ttu-id="ec6b9-226">Добавлены команды WAF CDN.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-226">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="ec6b9-227">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-227">Compute</span></span>

* <span data-ttu-id="ec6b9-228">az sig image-version: добавлен параметр --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="ec6b9-228">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="ec6b9-229">az ppg show: добавлен параметр --colocation-status, чтобы включить выборку состояния совместного размещения всех ресурсов в группе размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-229">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="ec6b9-230">az vmss create/update: включена поддержка автоматического исправления.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-230">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="ec6b9-231">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] az image template: шаблон переименован в построитель.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-231">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="ec6b9-232">az image builder create: добавлен параметр --image-template.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-232">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="ec6b9-233">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ec6b9-233">Cosmos DB</span></span>

* <span data-ttu-id="ec6b9-234">Добавлены командлеты хранимой процедуры SQL, определяемых пользователем функций и триггеров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-234">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="ec6b9-235">az cosmosdb create: добавлен параметр --key-uri для добавления сведений о шифровании хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-235">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="ec6b9-236">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-236">KeyVault</span></span>

* <span data-ttu-id="ec6b9-237">keyvault create: включена функция обратимого удаления по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-237">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-238">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-238">Monitor</span></span>

* <span data-ttu-id="ec6b9-239">az monitor metrics alert create: включена поддержка `~` в `--condition`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-239">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-240">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-240">Network</span></span>

* <span data-ttu-id="ec6b9-241">az network application-gateway rewrite-rule create: включена поддержка конфигурации URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-241">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="ec6b9-242">az network dns zone import: для параметра --zone-name в будущем можно будет не учитывать регистр.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-242">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="ec6b9-243">az network private-endpoint/private-link-service: удалена метка предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-243">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="ec6b9-244">az network bastion: включена поддержка бастиона.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-244">az network bastion: support bastion</span></span>
* <span data-ttu-id="ec6b9-245">az network vnet list-available-ips: включена поддержка списка доступных IP-адресов в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-245">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="ec6b9-246">az network watcher flow-log create/list/delete/update: добавлены новые команды для управления журналами потоков Наблюдателя и предоставлен параметр --location для явного определения Наблюдателя.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-246">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="ec6b9-247">az network watcher flow-log configure: поддержка прекращена.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-247">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="ec6b9-248">az network watcher flow-log show: включена поддержка параметров --location и --name для получения результатов в формате ARM; поддержка предыдущего форматированного вывода прекращена.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-248">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="ec6b9-249">Политика</span><span class="sxs-lookup"><span data-stu-id="ec6b9-249">Policy</span></span>

* <span data-ttu-id="ec6b9-250">az policy assignment create: исправлена ошибка, из-за которой автоматически генерируемое имя назначения политики превышало предельное значение.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-250">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="ec6b9-251">RBAC</span><span class="sxs-lookup"><span data-stu-id="ec6b9-251">RBAC</span></span>

* <span data-ttu-id="ec6b9-252">az ad group show: исправлено значение --group, обрабатываемое как проблема с регулярными выражениями.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-252">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="ec6b9-253">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ec6b9-253">RDBMS</span></span>

* <span data-ttu-id="ec6b9-254">Обновлена версия пакета SDK azure-mgmt-rdbms до 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-254">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="ec6b9-255">az postgres private-endpoint-connection: включено управление подключениями частных конечных точек Postgres.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-255">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="ec6b9-256">az postgres private-link-resource: включено управление ресурсами частных ссылок Postgres.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-256">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="ec6b9-257">az mysql private-endpoint-connection: включено управление подключениями частных конечных точек MySQL.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-257">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="ec6b9-258">az mysql private-link-resource: включено управление ресурсами частных ссылок MySQL.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-258">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="ec6b9-259">az mariadb private-endpoint-connection: включено управление подключениями частных конечных точек MariaDB.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-259">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="ec6b9-260">az mariadb private-link-resource: включено управление ресурсами частных ссылок MariaDB.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-260">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="ec6b9-261">Обновление тестов частной конечной точки RDBMS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-261">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-262">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-262">SQL</span></span>

* <span data-ttu-id="ec6b9-263">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-263">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="ec6b9-264">(sql server create:) добавлен необязательный флаг включения и отключения доступа к общедоступным сетям в команду создания SQL Server.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-264">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="ec6b9-265">(sql server update:) внесены некоторые изменения для клиентов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-265">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="ec6b9-266">Добавлено свойство minimal_tls_version для MI и SQL DB.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-266">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-267">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-267">Storage</span></span>

* <span data-ttu-id="ec6b9-268">az storage blob delete-batch: исправлено неправильное поведение флага `--dryrun`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-268">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="ec6b9-269">az storage account network-rule add (исправление): добавлено требование того, чтобы операция была идемпотентной.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-269">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="ec6b9-270">az storage account create/update: включена поддержка предпочтения маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-270">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="ec6b9-271">Обновлена версия azure-mgmt-storage до 8.0.0.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-271">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="ec6b9-272">az storage container immutability create: добавлен параметр --allow-protected-append-write.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-272">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="ec6b9-273">az storage account private-link-resource list: включена поддержка вывода списка ресурсов частной ссылки для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-273">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="ec6b9-274">az storage account private-endpoint-connection approve/reject/show/delete: включена поддержка управления подключениями к частным конечным точкам.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-274">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="ec6b9-275">az storage account blob-service-properties update: добавлены параметры --enable-restore-policy и --restore-days.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-275">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="ec6b9-276">az storage blob restore: включена поддержка восстановления диапазонов BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-276">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="ec6b9-277">18 февраля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-277">February 18, 2020</span></span>

<span data-ttu-id="ec6b9-278">Версия 2.1.0</span><span class="sxs-lookup"><span data-stu-id="ec6b9-278">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-279">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-279">ACR</span></span>

* <span data-ttu-id="ec6b9-280">Добавлен новый аргумент `--expose-token` для `az acr login`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-280">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="ec6b9-281">Исправлены неправильные выходные данные `az acr task identity show -n Name -r Registry -o table`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-281">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="ec6b9-282">az acr login: отображение CLIError при наличии ошибок, возвращаемых командой docker.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-282">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-283">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-283">ACS</span></span>

* <span data-ttu-id="ec6b9-284">aks create/update: добавление проверки `--vnet-subnet-id`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-284">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="ec6b9-285">Aladdin</span><span class="sxs-lookup"><span data-stu-id="ec6b9-285">Aladdin</span></span>

* <span data-ttu-id="ec6b9-286">Выполнение синтаксического анализа созданных примеров в _help.py для команд.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-286">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="ec6b9-287">AMS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-287">AMS</span></span>

* <span data-ttu-id="ec6b9-288">az ams теперь предоставляется в общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="ec6b9-288">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="ec6b9-289">AppConfig</span><span class="sxs-lookup"><span data-stu-id="ec6b9-289">AppConfig</span></span>

* <span data-ttu-id="ec6b9-290">Исправлено справочное сообщение, чтобы исключить неподдерживаемый фильтр ключей или меток.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-290">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="ec6b9-291">Удален тег preview для большинства команд, кроме управляемого удостоверения и флагов функций.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-291">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="ec6b9-292">Добавлен управляемый ключ клиента при обновлении магазинов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-292">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-293">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-293">AppService</span></span>

* <span data-ttu-id="ec6b9-294">az webapp list-runtimes: исправлена ошибка для list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-294">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="ec6b9-295">Добавлена команда az webapp|functionapp config ssl create.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-295">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="ec6b9-296">Включена поддержка приложений-функций версии 3 и Node 12.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-296">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="ec6b9-297">ARM</span><span class="sxs-lookup"><span data-stu-id="ec6b9-297">ARM</span></span>

* <span data-ttu-id="ec6b9-298">az policy assignment create: исправлено сообщение об ошибке, если параметр `--policy` является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-298">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="ec6b9-299">az group deployment create: Устранена ошибка stat: path too long for Windows при использовании большого файла parameters.json.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-299">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="ec6b9-300">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="ec6b9-300">Backup</span></span>

* <span data-ttu-id="ec6b9-301">Исправлен поток восстановления на уровне элемента в OLR.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-301">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="ec6b9-302">Включена поддержка восстановления в виде файлов для баз данных SQL и SAP.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-302">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="ec6b9-303">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-303">Compute</span></span>

* <span data-ttu-id="ec6b9-304">vm/vmss/availability-set update: add --ppg: разрешено обновление ProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-304">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="ec6b9-305">vmss create: add --data-disk-iops and --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="ec6b9-305">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="ec6b9-306">az vm host: удален тег preview для `vm host` и `vm host group`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-306">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="ec6b9-307">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправление 10728. `az vm create`: автоматическое создание подсети, если указанные виртуальная сеть и подсеть не существуют.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-307">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="ec6b9-308">Повышена надежность списка образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-308">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="ec6b9-309">Eventhub</span><span class="sxs-lookup"><span data-stu-id="ec6b9-309">Eventhub</span></span>

* <span data-ttu-id="ec6b9-310">Включена поддержка Azure Stack для профиля 2019-03-01-hybrid.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-310">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="ec6b9-311">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-311">KeyVault</span></span>

* <span data-ttu-id="ec6b9-312">az keyvault key create: добавлено новое значение `import` для параметра `--ops`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-312">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="ec6b9-313">az keyvault key list-versions: включена поддержка параметров `--id` для определения ключей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-313">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="ec6b9-314">Включена поддержка подключений к частным конечным точкам.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-314">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-315">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-315">Network</span></span>

* <span data-ttu-id="ec6b9-316">Выполнена активация azure-mgmt-network 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-316">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="ec6b9-317">az network private-link-service update/create: включена поддержка --enable-proxy-protocol.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-317">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="ec6b9-318">Добавлена функция монитора подключения версии 2.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-318">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="ec6b9-319">Упаковка</span><span class="sxs-lookup"><span data-stu-id="ec6b9-319">Packaging</span></span>

* <span data-ttu-id="ec6b9-320">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка Python 2.7.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-320">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="ec6b9-321">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-321">Profile</span></span>

* <span data-ttu-id="ec6b9-322">Предварительный просмотр: В учетные записи подписок добавлены новые атрибуты `homeTenantId` и `managedByTenants`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-322">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="ec6b9-323">Чтобы изменения вступили в силу, повторно выполните команду `az login`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-323">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="ec6b9-324">az login: отображение предупреждения, если подписка связана с несколькими клиентами, но по умолчанию используется с первым из них</span><span class="sxs-lookup"><span data-stu-id="ec6b9-324">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="ec6b9-325">(чтобы выбрать определенный клиент при доступе к этой подписке, включите `--tenant` в `az login`).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-325">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-326">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-326">Role</span></span>

* <span data-ttu-id="ec6b9-327">az role assignment create: исправлена ошибка с кодом HTTP 400, возникающая при присвоении роли субъекту-службе по отображаемому имени.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-327">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-328">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-328">SQL</span></span>

* <span data-ttu-id="ec6b9-329">Обновлен командлет `az sql mi update` Управляемого экземпляра SQL (добавлены два новых параметра: tier и family).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-329">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-330">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-330">Storage</span></span>

* <span data-ttu-id="ec6b9-331">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az storage account create`: Тип учетной записи хранения по умолчанию изменен на StorageV2.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-331">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="ec6b9-332">4 февраля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-332">February 04, 2020</span></span>

<span data-ttu-id="ec6b9-333">Версия 2.0.81</span><span class="sxs-lookup"><span data-stu-id="ec6b9-333">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-334">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-334">ACS</span></span>

* <span data-ttu-id="ec6b9-335">Добавлена возможность задания выделенных исходящих портов и времени ожидания подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-335">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="ec6b9-336">Выполнено обновление до API версии 2019-11-01.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-336">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-337">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-337">ACR</span></span>

* <span data-ttu-id="ec6b9-338">[Критическое изменение] `az acr delete` будет выводить запрос.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-338">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="ec6b9-339">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда az acr task delete будет выводить запрос.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-339">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="ec6b9-340">Добавлена новая группа команд az acr taskrun show/list/delete для управления выполнением задач.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-340">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="ec6b9-341">AKS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-341">AKS</span></span>

* <span data-ttu-id="ec6b9-342">Каждый кластер получает отдельный субъект-службу для улучшения изоляции.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-342">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="ec6b9-343">AppConfig</span><span class="sxs-lookup"><span data-stu-id="ec6b9-343">AppConfig</span></span>

* <span data-ttu-id="ec6b9-344">Поддержка импорта ссылок на хранилище ключей из службы приложений и их экспорта в нее.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-344">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="ec6b9-345">Поддержка импорта и экспорта всех меток между файлами appconfig.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-345">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="ec6b9-346">Проверка имен ключей и функций перед настройкой и импортом.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-346">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="ec6b9-347">Предоставление изменений номера SKU в хранилище конфигураций.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-347">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="ec6b9-348">Новая группа команд для управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-348">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-349">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-349">AppService</span></span>

* <span data-ttu-id="ec6b9-350">Azure Stack: команды поверхности в профиле 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="ec6b9-350">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="ec6b9-351">functionapp: добавлена возможность создавать приложения-функции Java в Linux.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-351">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="ec6b9-352">ARM</span><span class="sxs-lookup"><span data-stu-id="ec6b9-352">ARM</span></span>

* <span data-ttu-id="ec6b9-353">Исправление ошибки 10246: аварийное завершение `az resource tag` в случае, если переданный параметр `--ids` являлся идентификатором группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-353">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="ec6b9-354">Исправление ошибки 11658: команда `az group export` не поддерживала параметры `--query` и `--output`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-354">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="ec6b9-355">Исправление ошибки 10279: код выхода `az group deployment validate` был равен 0, если проверка не пройдена.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-355">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="ec6b9-356">Исправление ошибки 9916: улучшено сообщение об ошибке из-за конфликта между тегом и другими условиями фильтра для команды `az resource list`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-356">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="ec6b9-357">Добавлен новый параметр `--managed-by` для добавления данных managedBy для команды `az group create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-357">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="ec6b9-358">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="ec6b9-358">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="ec6b9-359">Добавлена подгруппа `monitor` для управления мониторингом Log Analytics в кластере Azure Red Hat OpensShift.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-359">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="ec6b9-360">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="ec6b9-360">BotService</span></span>

* <span data-ttu-id="ec6b9-361">Исправление ошибки 11697: команда `az bot create` не являлась идемпотентной.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-361">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="ec6b9-362">Проверки исправления имен изменены для выполнения только в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-362">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="ec6b9-363">CDN</span><span class="sxs-lookup"><span data-stu-id="ec6b9-363">CDN</span></span>

* <span data-ttu-id="ec6b9-364">Добавлена поддержка функции rulesEngine.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-364">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="ec6b9-365">Добавлена новая группа команд cdn endpoint rule для управления правилами.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-365">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="ec6b9-366">Пакет azure-mgmt-cdn обновлен до версии 4.0.0 для использования API версии 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-366">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="ec6b9-367">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="ec6b9-367">Deployment Manager</span></span>

* <span data-ttu-id="ec6b9-368">Добавлена операция вывода списка всех ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-368">Add list operation for all resources.</span></span>
* <span data-ttu-id="ec6b9-369">Улучшен ресурс шага для нового типа шага.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-369">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="ec6b9-370">Пакет azure-mgmt-deploymentmanager обновлен для использования версии 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-370">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="ec6b9-371">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-371">IoT</span></span>

* <span data-ttu-id="ec6b9-372">Команды IoT hub Job объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-372">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="ec6b9-373">IoT Central</span><span class="sxs-lookup"><span data-stu-id="ec6b9-373">IoT Central</span></span>

* <span data-ttu-id="ec6b9-374">Добавлена поддержка создания и обновления приложений с новыми SKU: ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-374">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="ec6b9-375">Key Vault</span><span class="sxs-lookup"><span data-stu-id="ec6b9-375">Key Vault</span></span>

* <span data-ttu-id="ec6b9-376">Добавлена новая команда `az keyvault key download` для скачивания ключей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-376">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="ec6b9-377">Разное</span><span class="sxs-lookup"><span data-stu-id="ec6b9-377">Misc</span></span>

* <span data-ttu-id="ec6b9-378">Исправление ошибки 6371: поддержка завершения имен файлов и переменных среды в Bash.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-378">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-379">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-379">Network</span></span>

* <span data-ttu-id="ec6b9-380">Исправление ошибки 2092: для команды az network dns record-set add/remove добавлено предупреждение, отображаемое, если набор записей не найден.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-380">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="ec6b9-381">В будущем для подтверждения этого автоматического создания будет добавлен дополнительный аргумент.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-381">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="ec6b9-382">Политика</span><span class="sxs-lookup"><span data-stu-id="ec6b9-382">Policy</span></span>

* <span data-ttu-id="ec6b9-383">Добавлена новая команда `az policy metadata` для получения ресурсов метаданных расширенной политики.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-383">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="ec6b9-384">`az policy remediation create`: С помощью параметра `--resource-discovery-mode` можно указать, следует ли повторно оценить соответствие перед исправлением.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-384">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="ec6b9-385">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-385">Profile</span></span>

* <span data-ttu-id="ec6b9-386">`az account get-access-token`: Добавлен параметр `--tenant` для получения маркера для арендатора напрямую, без необходимости указывать подписку.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-386">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="ec6b9-387">RBAC</span><span class="sxs-lookup"><span data-stu-id="ec6b9-387">RBAC</span></span>

* <span data-ttu-id="ec6b9-388">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправление ошибки 11883: `az role assignment create`: пустая область приведет к ошибке.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-388">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="ec6b9-389">Безопасность</span><span class="sxs-lookup"><span data-stu-id="ec6b9-389">Security</span></span>

* <span data-ttu-id="ec6b9-390">Добавлены новые команды `az atp show` и `az atp update` для просмотра и настройки дополнительных параметров защиты от угроз для учетных записей хранения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-390">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-391">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-391">SQL</span></span>

* <span data-ttu-id="ec6b9-392">`sql dw create`: параметры `--zone-redundant` и `--read-replica-count` объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-392">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="ec6b9-393">Эти параметры не применяются к хранилищу данных.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-393">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="ec6b9-394">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql db create`: Значения WideWorldImportersStd и WideWorldImportersFull больше не являются задокументированным допустимыми значениями для команды az sql db create --sample-name.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-394">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="ec6b9-395">Эти примеры базы данных всегда будут приводить к сбою создания.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-395">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="ec6b9-396">Добавлены новые команды `sql db classification show/list/update/delete` и `sql db classification recommendation list/enable/disable` для управления классификациями конфиденциальности баз данных SQL.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-396">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="ec6b9-397">`az sql db audit-policy`: устранены пустые действия аудита и группы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-397">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-398">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-398">Storage</span></span>

* <span data-ttu-id="ec6b9-399">Добавлена новая группа команд `az storage share-rm` для использования поставщика ресурсов Microsoft.Storage в операциях управления файловыми ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-399">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="ec6b9-400">Исправление ошибки 11415: ошибка разрешения для `az storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-400">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="ec6b9-401">Добавлены интеграция AzCopy 10.3.3 и поддержка Win32.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-401">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="ec6b9-402">`az storage copy`: добавлены параметры `--include-path`, `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-402">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="ec6b9-403">`az storage remove`: параметры `--inlcude` и `--exclude` заменены параметрами `--include-path`, `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-403">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="ec6b9-404">`az storage sync`: добавлены параметры `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-404">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="ec6b9-405">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ec6b9-405">ServiceFabric</span></span>

* <span data-ttu-id="ec6b9-406">Добавлены новые команды для управления приложениями и службами.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-406">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="ec6b9-407">13 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-407">January 13, 2020</span></span>

<span data-ttu-id="ec6b9-408">Версия 2.0.80</span><span class="sxs-lookup"><span data-stu-id="ec6b9-408">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="ec6b9-409">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-409">Compute</span></span>

* <span data-ttu-id="ec6b9-410">Обновление диска: добавлены параметры --disk-encryption-set и --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-410">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="ec6b9-411">Создание и обновление моментального снимка: добавлены параметры --disk-encryption-set и --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-411">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-412">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-412">Storage</span></span>

* <span data-ttu-id="ec6b9-413">Обновление azure-mgmt-storage до версии 7.1.0</span><span class="sxs-lookup"><span data-stu-id="ec6b9-413">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="ec6b9-414">`az storage account create`: добавлены параметры `--encryption-key-type-for-table` и `--encryption-key-type-for-queue` для включения поддержки службы шифрования таблиц и очередей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-414">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="ec6b9-415">7 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-415">January 07, 2020</span></span>

<span data-ttu-id="ec6b9-416">Версия 2.0.79</span><span class="sxs-lookup"><span data-stu-id="ec6b9-416">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-417">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-417">ACR</span></span>

* <span data-ttu-id="ec6b9-418">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --os для команд acr build, acr task create/update, acr run и acr pack.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-418">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="ec6b9-419">Вместо этого используется параметр --platform.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-419">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="ec6b9-420">AppConfig</span><span class="sxs-lookup"><span data-stu-id="ec6b9-420">AppConfig</span></span>

* <span data-ttu-id="ec6b9-421">Добавлена поддержка импорта и экспорта флагов функций.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-421">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="ec6b9-422">Добавлена новая команда az appconfig kv set-keyvault для создания ссылки на хранилище ключей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-422">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="ec6b9-423">Добавлена поддержка различных соглашений об именовании при экспорте флагов функций в файл.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-423">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-424">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-424">AppService</span></span>

* <span data-ttu-id="ec6b9-425">Устранена проблема № 7154: обновлена документация по команде <> — теперь в ней используются обратные, а не одинарные кавычки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-425">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="ec6b9-426">Устранена проблема № 11287 (webapp up): по умолчанию для приложения, созданного с использованием этого флага, должен быть включен SSL.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-426">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="ec6b9-427">Устранена проблема № 11592: добавлен флаг az webapp up для статических сайтов HTML.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-427">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="ec6b9-428">ARM</span><span class="sxs-lookup"><span data-stu-id="ec6b9-428">ARM</span></span>

* <span data-ttu-id="ec6b9-429">Исправлена ошибка с командой `az resource tag`: невозможно было обновить теги хранилища Служб восстановления.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-429">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="ec6b9-430">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="ec6b9-430">Backup</span></span>

* <span data-ttu-id="ec6b9-431">Добавлена новая команда backup protection undelete для включения функции обратимого удаления рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-431">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="ec6b9-432">Добавлен новый параметр --soft-delete-feature-state для команды set backup-properties.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-432">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="ec6b9-433">Добавлена поддержка исключения диска для рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-433">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="ec6b9-434">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-434">Compute</span></span>

* <span data-ttu-id="ec6b9-435">Исправлен сбой `vm create` в профиле Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-435">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="ec6b9-436">Добавлена поддержка определений списков и метрик запросов для виртуальной машины (vm monitor metrics tail/list-definitions).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-436">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="ec6b9-437">Добавлено новое действия повторного применения команды az vm</span><span class="sxs-lookup"><span data-stu-id="ec6b9-437">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="ec6b9-438">HDInsight</span><span class="sxs-lookup"><span data-stu-id="ec6b9-438">HDInsight</span></span>

* <span data-ttu-id="ec6b9-439">Включена поддержка создания кластера Kafka с помощью прокси-сервера Kafka RESTful.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-439">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="ec6b9-440">Обновление azure-mgmt-hdinsight до версии 1.3.0</span><span class="sxs-lookup"><span data-stu-id="ec6b9-440">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="ec6b9-441">Прочее</span><span class="sxs-lookup"><span data-stu-id="ec6b9-441">Misc.</span></span>

* <span data-ttu-id="ec6b9-442">Добавлена команда `az version show` предварительного просмотра для отображения версий модулей и расширений Azure CLI в формате JSON по умолчанию или в формате, настроенном с помощью параметра --output</span><span class="sxs-lookup"><span data-stu-id="ec6b9-442">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="ec6b9-443">Центры событий</span><span class="sxs-lookup"><span data-stu-id="ec6b9-443">Event Hubs</span></span>

* <span data-ttu-id="ec6b9-444">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az eventhubs eventhub update и az eventhubs eventhub create.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-444">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="ec6b9-445">Данный параметр недопустим для сущностей концентратора событий.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-445">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="ec6b9-446">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="ec6b9-446">Service Bus</span></span>

* <span data-ttu-id="ec6b9-447">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az servicebus topic create, az servicebus topic update, az servicebus queue create и az servicebus queue update.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-447">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="ec6b9-448">Этот параметр является недопустимым для разделов и очередей служебной шины.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-448">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="ec6b9-449">RBAC</span><span class="sxs-lookup"><span data-stu-id="ec6b9-449">RBAC</span></span>

* <span data-ttu-id="ec6b9-450">Устранена проблема № 11712: команда `az ad app/sp show` не возвращала код выхода 3, если приложение или субъект-служба не существует.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-450">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-451">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-451">Storage</span></span>

* <span data-ttu-id="ec6b9-452">`az storage account create`: удален флаг предварительного просмотра для параметра --enable-hierarchical-namespace.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-452">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="ec6b9-453">Хранилище azure-mgmt-storage обновлено до версии 7.0.0 для использования API версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-453">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="ec6b9-454">Добавлены новые параметры (`--enable-delete-retention` и `--delete-retention-days`) для поддержки управления политикой хранения удаленных свойств службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-454">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="ec6b9-455">17 декабря 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-455">December 17, 2019</span></span>

<span data-ttu-id="ec6b9-456">2.0.78</span><span class="sxs-lookup"><span data-stu-id="ec6b9-456">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-457">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-457">ACR</span></span>

* <span data-ttu-id="ec6b9-458">Добавлена поддержка локального контекста во время выполнения задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-458">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-459">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-459">ACS</span></span>

* <span data-ttu-id="ec6b9-460">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде az openshift create параметр `--workspace-resource-id` переименован на `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-460">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="ec6b9-461">AMS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-461">AMS</span></span>

* <span data-ttu-id="ec6b9-462">Команды show обновлены для возвращения ответа 3, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-462">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="ec6b9-463">AppConfig</span><span class="sxs-lookup"><span data-stu-id="ec6b9-463">AppConfig</span></span>

* <span data-ttu-id="ec6b9-464">Исправлена ошибка, возникающая при добавлении api-version в URL-адрес запроса.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-464">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="ec6b9-465">Имеющееся решение не работает с разбивкой на страницы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-465">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="ec6b9-466">Добавлена поддержка отображения языков, кроме английского, так как наша внутренняя служба поддерживает Юникод для глобализации.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-466">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-467">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-467">AppService</span></span>

* <span data-ttu-id="ec6b9-468">Устранена проблема № 11217 (webapp): теперь команда az webapp config ssl upload поддерживает параметр слота.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-468">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="ec6b9-469">Устранена проблема № 10965. Ошибка: Имя не может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-469">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="ec6b9-470">Разрешено удаление по IP-адресу и подсети.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-470">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="ec6b9-471">Добавлена поддержка импорта сертификатов из хранилища ключей: `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-471">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="ec6b9-472">ARM</span><span class="sxs-lookup"><span data-stu-id="ec6b9-472">ARM</span></span>

* <span data-ttu-id="ec6b9-473">Обновлен пакет ресурсов azure-mgmt-resource для использования версии 6.0.0</span><span class="sxs-lookup"><span data-stu-id="ec6b9-473">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="ec6b9-474">Добавлена межклиентская поддержка команды `az group deployment create` путем добавления нового параметра `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-474">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="ec6b9-475">Добавлен новый параметр `--metadata` для поддержки добавления метаданных определений наборов политик.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-475">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="ec6b9-476">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="ec6b9-476">Backup</span></span>

* <span data-ttu-id="ec6b9-477">Добавлена поддержка резервного копирования для рабочей нагрузки SQL и SAP HANA.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-477">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="ec6b9-478">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="ec6b9-478">BotService</span></span>

* <span data-ttu-id="ec6b9-479">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг --version из предварительной версии команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-479">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="ec6b9-480">Поддерживаются только боты пакетов SDK версии 4.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-480">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="ec6b9-481">Добавлена проверка доступности имени для команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-481">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="ec6b9-482">Добавлена поддержка обновления URL-адреса значка для бота с помощью команды az bot update.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-482">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="ec6b9-483">Добавлена поддержка обновления канала Direct Line с помощью команды az bot directline update.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-483">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="ec6b9-484">Добавлена поддержка флага --enable-enhanced-auth в команде az bot directline create.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-484">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="ec6b9-485">Следующие группы команд предоставляются в общедоступной, а не в предварительной версии: az bot authsetting.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-485">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="ec6b9-486">Следующие команды в az bot предоставляются в общедоступной, а не в предварительной версии: create, prepare-deploy, show, delete и update.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-486">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="ec6b9-487">Устранена проблема с командой az bot prepare-deploy, которая изменяла значение параметра --proj-file-path на нижний регистр (например, с Test.csproj на test.csproj).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-487">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="ec6b9-488">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-488">Compute</span></span>

* <span data-ttu-id="ec6b9-489">vmss create/update: добавлен параметр --scale-on-policy, который определяет, какие виртуальные машины выбираются для удаления при масштабировании VMSS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-489">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="ec6b9-490">vm/vmss update: добавлен параметр --priority.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-490">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="ec6b9-491">vm/vmss update: добавлен параметр --max-price.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-491">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="ec6b9-492">Добавлена группа команд для шифрования дисков (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-492">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="ec6b9-493">disk create: добавлены параметры --encryption-type и --disk-encryption-set.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-493">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="ec6b9-494">vm/vmss create. Добавлены параметры --os-disk-encryption-set и --data-disk-encryption-sets.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-494">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-495">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-495">Core</span></span>

* <span data-ttu-id="ec6b9-496">Удалена поддержка Python версии 3.4.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-496">Removed support for Python 3.4</span></span>
* <span data-ttu-id="ec6b9-497">Подключение к опросу HaTS в нескольких командах.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-497">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="ec6b9-498">DLS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-498">DLS</span></span>

* <span data-ttu-id="ec6b9-499">Обновлена версия пакета SDK для ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-499">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="ec6b9-500">Установка</span><span class="sxs-lookup"><span data-stu-id="ec6b9-500">Install</span></span>

* <span data-ttu-id="ec6b9-501">Добавлена поддержка установки скриптов Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-501">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="ec6b9-502">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-502">IOT</span></span>

* <span data-ttu-id="ec6b9-503">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --failover-region из команды manual-failover.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-503">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="ec6b9-504">Теперь она будет выполнять отработку отказа в назначенный геопарный дополнительный регион.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-504">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="ec6b9-505">Key Vault</span><span class="sxs-lookup"><span data-stu-id="ec6b9-505">Key Vault</span></span>

* <span data-ttu-id="ec6b9-506">Устранена проблема № 8095: (`az keyvault storage remove`): улучшено справочное сообщение.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-506">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="ec6b9-507">Устранена проблема № 8921 (`az keyvault key/secret/certificate list/list-deleted/list-versions`): исправлена ошибка проверки в параметре `--maxresults`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-507">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="ec6b9-508">Устранена проблема № 10512 (`az keyvault set-policy`): улучшено сообщение об ошибке, возвращаемое, если не указан ни один из параметров `--object-id`, `--spn` или `--upn`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-508">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="ec6b9-509">Устранена проблема № 10846 (`az keyvault secret show-deleted`): при указании значения `--id` значение `--name/-n` не требовалось.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-509">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="ec6b9-510">Устранена проблема № 11084: (`az keyvault secret download`): улучшено справочное сообщение параметра `--encoding`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-510">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-511">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-511">Network</span></span>

* <span data-ttu-id="ec6b9-512">az network application-gateway probe: добавлена поддержка параметра --port, позволяющего указать порт, который используется для проверки внутренних серверов при создании и обновлении.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-512">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="ec6b9-513">az network application-gateway url-path-map create/update: исправлена ошибка с `--waf-policy`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-513">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="ec6b9-514">az network application-gateway: добавлена поддержка параметра `--rewrite-rule-set`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-514">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="ec6b9-515">az network list-service-aliases: добавлена поддержка перечисления псевдонимов служб, которые можно использовать для политик конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-515">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="ec6b9-516">az network dns zone import: добавлена поддержка символа .@ в имени записи.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-516">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="ec6b9-517">Упаковка</span><span class="sxs-lookup"><span data-stu-id="ec6b9-517">Packaging</span></span>

* <span data-ttu-id="ec6b9-518">Снова добавлены сборки Edge для установки PIP.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-518">Added back edge builds for pip install</span></span>
* <span data-ttu-id="ec6b9-519">Добавлен пакет Ubuntu eoan.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-519">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="ec6b9-520">Политика</span><span class="sxs-lookup"><span data-stu-id="ec6b9-520">Policy</span></span>

* <span data-ttu-id="ec6b9-521">Добавлена поддержка API Политики версии 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-521">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="ec6b9-522">az policy set-definition: добавлена поддержка группирования в определениях наборов политик с помощью параметра `--definition-groups`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-522">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="ec6b9-523">Redis</span><span class="sxs-lookup"><span data-stu-id="ec6b9-523">Redis</span></span>

* <span data-ttu-id="ec6b9-524">В команду `az redis create` добавлена предварительная версия параметра `--replicas-per-master`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-524">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="ec6b9-525">Обновлена версия azure-mgmt-redis с 6.0.0 на 7.0.0 RC1.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-525">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="ec6b9-526">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ec6b9-526">ServiceFabric</span></span>

* <span data-ttu-id="ec6b9-527">Исправлена логика добавления типа узла, а также устранена проблема № 10963: при добавлении нового типа узла с уровнем устойчивости Gold возникала ошибка CLI.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-527">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="ec6b9-528">Обновлена версия параметра ServiceFabricNodeVmExt до 1.1 в шаблоне создания.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-528">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-529">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-529">SQL</span></span>

* <span data-ttu-id="ec6b9-530">В команды create и update базы данных SQL добавлены параметры --read-scale и --read-replicas для поддержки управления масштабированием операций чтения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-530">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-531">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-531">Storage</span></span>

* <span data-ttu-id="ec6b9-532">Выпущена общедоступная версия больших файловых ресурсов для команды создания и обновления учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-532">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="ec6b9-533">Выпущена общедоступная версия поддержки маркера SAS для делегирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-533">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="ec6b9-534">Добавлены новые команды (`az storage account blob-service-properties show` и `az storage account blob-service-properties update --enable-change-feed`) для управления свойствами службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-534">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="ec6b9-535">[ОЖИДАЕТСЯ КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] `az storage copy`: символ `*` больше не поддерживается в качестве подстановочного знака в URL-адресе. Тем не менее новые параметры--include-pattern и--exclude-pattern будут добавлены с поддержкой подстановочных знаков `*`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-535">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="ec6b9-536">Устранена проблема № 11043: добавлена поддержка удаления всего контейнера или общего ресурса в команде `az storage remove`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-536">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="ec6b9-537">26 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-537">November 26, 2019</span></span>

<span data-ttu-id="ec6b9-538">Версия 2.0.77</span><span class="sxs-lookup"><span data-stu-id="ec6b9-538">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-539">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-539">ACR</span></span>

* <span data-ttu-id="ec6b9-540">Параметр `--branch`, используемый при обновлении или создании задачи ACR, объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-540">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="ec6b9-541">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="ec6b9-541">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="ec6b9-542">Добавлен флаг `--workspace-resource-id` для создания кластера Azure Red Hat Openshift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-542">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="ec6b9-543">Добавлен флаг `monitor_profile` для создания кластера Azure Red Hat OpenShift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-543">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="ec6b9-544">AKS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-544">AKS</span></span>

* <span data-ttu-id="ec6b9-545">Включена поддержка операции смены сертификата кластера с использованием команды az aks rotate-certs.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-545">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="ec6b9-546">AppConfig</span><span class="sxs-lookup"><span data-stu-id="ec6b9-546">AppConfig</span></span>

* <span data-ttu-id="ec6b9-547">Включена поддержка использования символа ":" для разделителя `as az appconfig kv import`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-547">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="ec6b9-548">Исправлена проблема с перечислением значений ключей с несколькими метками, включая метку NULL.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-548">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="ec6b9-549">Обновлен пакет SDK для плоскости управления, azure-mgmt-appconfiguration, до версии 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-549">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="ec6b9-550">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-550">AppService</span></span>

* <span data-ttu-id="ec6b9-551">Исправлена ошибка № 11100. Использование AttributeError для az webapp up при создании плана службы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-551">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="ec6b9-552">az webapp up. При принудительном создании или развертывании сайта для поддерживаемых языков значения по умолчанию не используются.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-552">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="ec6b9-553">Включена поддержка Среды службы приложений: az appservice ase show | list | list-addresses | list-plans | create | update | delete.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-553">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="ec6b9-554">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="ec6b9-554">Backup</span></span>

* <span data-ttu-id="ec6b9-555">Исправлена проблема в команде az backup policy list-associated-items.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-555">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="ec6b9-556">Добавлен необязательный параметр BackupManagementType.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-556">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="ec6b9-557">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-557">Compute</span></span>

* <span data-ttu-id="ec6b9-558">Обновлена версия API вычислений, дисков, моментальных снимков до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-558">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="ec6b9-559">vmss create. Улучшение для --orchestration-mode.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-559">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="ec6b9-560">sig image-definition create. Добавлен параметр --os-state для указания того, являются ли виртуальные машины, созданные в этом образе, универсальными или специализированными.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-560">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="ec6b9-561">sig image-definition create. Добавлен параметр --hyper-v-generation для указания создания гипервизора.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-561">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="ec6b9-562">sig image-version create. Включена поддержка параметров --os-snapshot и --data-snapshots.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-562">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="ec6b9-563">image create. Включена поддержка параметра --data-disk-caching для указания параметра кэширования для дисков данных.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-563">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="ec6b9-564">Обновлена версия пакета SDK для вычислений Python до 10.0.0.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-564">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="ec6b9-565">vm/vmss create. Добавлен фрагмент Spot в свойство перечисления Priority.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-565">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="ec6b9-566">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименование параметра --max-billing в --max-price для виртуальных машин и Масштабируемых наборов виртуальных машин в соответствии с командлетами Swagger и PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-566">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="ec6b9-567">vm monitor log show. Включена поддержка запроса журналов в связанной рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-567">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="ec6b9-568">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-568">IOT</span></span>

* <span data-ttu-id="ec6b9-569">Исправление № 2531. Добавлены вспомогательные аргументы для обновления концентратора.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-569">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="ec6b9-570">Исправление № 8323. Добавлены недостающие параметры для создания пользовательской конечной точки хранилища.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-570">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="ec6b9-571">Исправлена ошибка регрессии. Отменены изменения, переопределяющие конечную точку хранилища по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-571">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="ec6b9-572">Key Vault</span><span class="sxs-lookup"><span data-stu-id="ec6b9-572">Key Vault</span></span>

* <span data-ttu-id="ec6b9-573">Исправление № 11121. При использовании `az keyvault certificate list` для передачи `--include-pending` теперь не требуется значение `true` или `false`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-573">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="ec6b9-574">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="ec6b9-574">NetAppFiles</span></span>

* <span data-ttu-id="ec6b9-575">Обновлена версия azure-mgmt-netapp до 0.7.0, которая включает некоторые дополнительные свойства тома, связанные с предстоящими операциями репликации.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-575">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-576">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-576">Network</span></span>

* <span data-ttu-id="ec6b9-577">application-gateway waf-config. Не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-577">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="ec6b9-578">application-gateway waf-policy. Добавлены управляемые правила подгрупп для контроля управляемых наборов правил и правил исключения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-578">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="ec6b9-579">application-gateway waf-policy. Добавлен параметр политики подгруппы для управления глобальной конфигурацией политики WAF.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-579">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="ec6b9-580">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] application-gateway waf-policy. Переименовано правило подгруппы в пользовательское правило.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-580">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="ec6b9-581">application-gateway http-listener. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-581">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="ec6b9-582">application-gateway url-path-map rule. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-582">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="ec6b9-583">Упаковка</span><span class="sxs-lookup"><span data-stu-id="ec6b9-583">Packaging</span></span>

* <span data-ttu-id="ec6b9-584">Удалена команда az wrapper в Python.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-584">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="ec6b9-585">Включена поддержка Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-585">Added support for Python 3.8</span></span>
* <span data-ttu-id="ec6b9-586">Изменена версия на Python 3 для пакета RPM.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-586">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="ec6b9-587">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-587">Profile</span></span>

* <span data-ttu-id="ec6b9-588">Исправлена ошибка при выполнении `az login -u {} -p {}` с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-588">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="ec6b9-589">Исправлена ошибка с `SSLError` при выполнении `az login` за прокси-сервером с самозаверяющим корневым сертификатом.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-589">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="ec6b9-590">Исправлена ошибка № 10578. `az login` зависает при одновременном запуске нескольких экземпляров в Windows или WSL.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-590">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="ec6b9-591">Исправлена ошибка № 11059. Сбой выполнения `az login --allow-no-subscriptions`, если в клиенте есть подписки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-591">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="ec6b9-592">Исправлена ошибка № 11238. После переименования подписки вход с помощью MSI приведет к тому, что одна и та же подписка появится дважды.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-592">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="ec6b9-593">RBAC</span><span class="sxs-lookup"><span data-stu-id="ec6b9-593">RBAC</span></span>

* <span data-ttu-id="ec6b9-594">Исправлена ошибка № 10996. Исправлена ошибка с `--force-change-password-next-login` в `az ad user update`, если `--password` не указывается.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-594">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="ec6b9-595">Redis</span><span class="sxs-lookup"><span data-stu-id="ec6b9-595">Redis</span></span>

* <span data-ttu-id="ec6b9-596">Исправлена ошибка № 2902. Предотвращена настройка конфигураций памяти при обновлении кэша с номером SKU "Базовый".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-596">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="ec6b9-597">Резервирование</span><span class="sxs-lookup"><span data-stu-id="ec6b9-597">Reservations</span></span>

* <span data-ttu-id="ec6b9-598">Обновлена версия пакета SDK до 0.6.0</span><span class="sxs-lookup"><span data-stu-id="ec6b9-598">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="ec6b9-599">Добавлены сведения о плане выставления счетов после вызова Get-Catalogs.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-599">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="ec6b9-600">Добавлена новая команда `az reservations reservation-order calculate` для вычисления стоимости резервирования.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-600">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="ec6b9-601">Добавлена новая команда `az reservations reservation-order purchase` для приобретения нового резервирования.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-601">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="ec6b9-602">Rest</span><span class="sxs-lookup"><span data-stu-id="ec6b9-602">Rest</span></span>
* <span data-ttu-id="ec6b9-603">Изменена версия `az rest` на общедоступную.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-603">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-604">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-604">SQL</span></span>

* <span data-ttu-id="ec6b9-605">Обновлена версия azure-mgmt-sql до 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-605">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-606">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-606">Storage</span></span>

* <span data-ttu-id="ec6b9-607">storage account create. Добавлен параметр --enable-hierarchical-namespace для включения поддержки семантики файловой системы в службе больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-607">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="ec6b9-608">Удалено несвязанное исключение из сообщения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-608">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="ec6b9-609">Исправлены проблемы, из-за которых появлялось неверное сообщение об отсутствии нужных разрешений на выполнение требуемой операции</span><span class="sxs-lookup"><span data-stu-id="ec6b9-609">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="ec6b9-610">при блокировке правилами сети (AuthenticationFailed).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-610">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="ec6b9-611">4 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-611">November 4, 2019</span></span>

<span data-ttu-id="ec6b9-612">Версия 2.0.76</span><span class="sxs-lookup"><span data-stu-id="ec6b9-612">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-613">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-613">ACR</span></span>

* <span data-ttu-id="ec6b9-614">В команду `az acr pack build` добавлен параметр предварительной версии `--pack-image-tag`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-614">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="ec6b9-615">Добавлена поддержка включения аудита при создании реестра.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-615">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="ec6b9-616">Включена поддержка функции RBAC, распространяющаяся на репозиторий.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-616">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="ec6b9-617">AKS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-617">AKS</span></span>

* <span data-ttu-id="ec6b9-618">В команду `az aks create` добавлены `--enable-cluster-autoscaler`, `--min-count` и `--max-count`, что позволяет автоматически масштабировать кластер для пула узлов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-618">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="ec6b9-619">Добавлены указанные выше флаги, а также `--update-cluster-autoscaler` и `--disable-cluster-autoscaler` в команду `az aks update`, что позволяет обновлять средство автоматического масштабирования кластера.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-619">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="ec6b9-620">AppConfig</span><span class="sxs-lookup"><span data-stu-id="ec6b9-620">AppConfig</span></span>

* <span data-ttu-id="ec6b9-621">Добавлена группа команд функции appconfig для управления флагами функций, хранимыми в Конфигурации приложений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-621">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="ec6b9-622">Исправлена незначительная ошибка команды экспорта в файл appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-622">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="ec6b9-623">Прерывание чтения содержимого конечного файла во время экспорта.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-623">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-624">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-624">AppService</span></span>

* <span data-ttu-id="ec6b9-625">`az appservice plan create`: Добавлена поддержка определения persitescaling при создании плана appservice.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-625">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="ec6b9-626">Исправлена проблема, из-за которой операция webapp config ssl bind удаляла существующие теги из ресурса.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-626">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="ec6b9-627">Добавлен флаг `--build-remote` для `az functionapp deployment source config-zip` для включения поддержки действия удаленной сборки во время развертывания приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-627">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="ec6b9-628">Изменена версия узла по умолчанию для приложений-функций на ~10 для Windows</span><span class="sxs-lookup"><span data-stu-id="ec6b9-628">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="ec6b9-629">В `az functionapp create` добавлено свойство `--runtime-version`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-629">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="ec6b9-630">ARM</span><span class="sxs-lookup"><span data-stu-id="ec6b9-630">ARM</span></span>

* <span data-ttu-id="ec6b9-631">`az deployment/group deployment validate`: В `--handle-extended-json-format` добавлен параметр для включения поддержки многострочности и комментариев в шаблоне JSON при развертывании.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-631">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="ec6b9-632">Версия azure-mgmt-resource обновлена до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-632">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="ec6b9-633">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="ec6b9-633">Backup</span></span>

* <span data-ttu-id="ec6b9-634">Добавлена поддержка резервного копирования AzureFiles.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-634">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="ec6b9-635">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-635">Compute</span></span>

* <span data-ttu-id="ec6b9-636">`az vm create`: Добавлено предупреждение при одновременном определении ускоренной сети и существующей сетевой карты.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-636">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="ec6b9-637">`az vm create`: Добавлен параметр `--vmss` для определения существующего масштабируемого набора виртуальных машин, которому должна быть назначена виртуальная машина.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-637">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="ec6b9-638">`az vm/vmss create`: Добавлена локальная копия файла псевдонима изображения, к которой можно получить доступ в ограниченной сетевой среде.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-638">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="ec6b9-639">`az vmss create`: Добавлен параметр `--orchestration-mode` для определения того, как виртуальные машины управляются масштабируемым набором.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-639">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="ec6b9-640">`az vm/vmss update`: Добавлен параметр `--ultra-ssd-enabled`, чтобы разрешить обновление параметра Ultra SSD.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-640">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="ec6b9-641">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az vm extension set`: Исправлена ошибка, из-за которой пользователям не удавалось определять расширение на виртуальной машине с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-641">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="ec6b9-642">Добавлены новые команды `az vm image terms accept/cancel/show` для управления условиями использования образов Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-642">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="ec6b9-643">Расширение VMAccessForLinux обновлено до версии 1.5.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-643">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ec6b9-644">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ec6b9-644">CosmosDB</span></span>

* <span data-ttu-id="ec6b9-645">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql container create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-645">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="ec6b9-646">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az gremlin graph create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-646">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="ec6b9-647">`az sql container create`: Добавлены команды `--unique-key-policy` и `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-647">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="ec6b9-648">`az sql container create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-648">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="ec6b9-649">`gremlin graph create`: Добавлена команда `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-649">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="ec6b9-650">`gremlin graph create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-650">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="ec6b9-651">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-651">Fixed typo in help message</span></span>
* <span data-ttu-id="ec6b9-652">База данных: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-652">database: Added deprecation information</span></span>
* <span data-ttu-id="ec6b9-653">Коллекция: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-653">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="ec6b9-654">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-654">IoT</span></span>

* <span data-ttu-id="ec6b9-655">Добавлен новый тип источника маршрутизации: DigitalTwinChangeEvents.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-655">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="ec6b9-656">Добавлены отсутствующие компоненты в `az iot hub create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-656">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="ec6b9-657">Key Vault</span><span class="sxs-lookup"><span data-stu-id="ec6b9-657">Key Vault</span></span>

* <span data-ttu-id="ec6b9-658">Исправлена непредвиденная ошибка с отсутствием файла сертификата.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-658">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="ec6b9-659">Исправлена ошибка с неработающей командой `az keyvault recover/purge`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-659">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="ec6b9-660">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="ec6b9-660">NetAppFiles</span></span>

* <span data-ttu-id="ec6b9-661">Пакет azure-mgmt-netapp обновлен до версии 0.6.0 для включения поддержки API версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-661">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="ec6b9-662">Эта новая версия API включает:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-662">This new API version includes:</span></span>

    - <span data-ttu-id="ec6b9-663">При создании тома с использованием `--protocol-types` допускается NFSv4.1 вместо NFSv4.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-663">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="ec6b9-664">Свойство политики экспорта томов теперь называется nfsv41, а не nfsv4.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-664">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="ec6b9-665">Параметр `--creation-token` для тома переименован в `--file-path`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-665">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="ec6b9-666">Дата создания моментального снимка теперь имеет значение Created.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-666">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-667">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-667">Network</span></span>

* <span data-ttu-id="ec6b9-668">`az network private-dns link vnet create/update`: Добавлена поддержка связывания виртуальных сетей между клиентами.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-668">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="ec6b9-669">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az network vnet subnet list`: Параметры `--resource-group` и `--vnet-name` теперь являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-669">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="ec6b9-670">`az network public-ip prefix create`: Включена поддержка определения версии IP-адреса (IPv4, IPv6) при создании.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-670">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="ec6b9-671">Версия azure-mgmt-network обновлена до 7.0.0 и версия api-version до 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-671">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="ec6b9-672">`az network vrouter`: Включена поддержка нового виртуального маршрутизатора службы и пиринга виртуальных маршрутизаторов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-672">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="ec6b9-673">`az network express-route gateway connection`: Добавлена поддержка параметра `--internet-security`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-673">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="ec6b9-674">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-674">Profile</span></span>

* <span data-ttu-id="ec6b9-675">Исправлена ошибка с неработающей командой `az account get-access-token --resource-type ms-graph`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-675">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="ec6b9-676">Удалено предупреждение из `az login`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-676">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="ec6b9-677">RBAC</span><span class="sxs-lookup"><span data-stu-id="ec6b9-677">RBAC</span></span>

* <span data-ttu-id="ec6b9-678">Исправление `az ad app update --id {} --display-name {}` не работает.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-678">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="ec6b9-679">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ec6b9-679">ServiceFabric</span></span>

* <span data-ttu-id="ec6b9-680">`az sf cluster create`: Исправлена проблема путем изменения VMSS для вычислений с использованием файла template.json для Service Fabric Linux и Windows со стандартных дисков на управляемые.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-680">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-681">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-681">SQL</span></span>

* <span data-ttu-id="ec6b9-682">Добавлены параметры `--compute-model`, `--auto-pause-delay` и `--min-capacity` для включения поддержки операций CRUD для нового предложения Базы данных SQL: Модель бессерверных вычислений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-682">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-683">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-683">Storage</span></span>

* <span data-ttu-id="ec6b9-684">`az storage account create/update`: Добавлен параметр --enable-files-adds и группа аргументов свойств Azure Active Directory для включения поддержки аутентификации доменных служб Azure Active Directory для Файлов Azure.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-684">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="ec6b9-685">Расширена команда `az storage account keys list/renew` для включения поддержки перечисления или повторного создания ключей Kerberos для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-685">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="ec6b9-686">15 октября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-686">October 15, 2019</span></span>

<span data-ttu-id="ec6b9-687">Версия 2.0.75</span><span class="sxs-lookup"><span data-stu-id="ec6b9-687">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="ec6b9-688">AKS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-688">AKS</span></span>

* <span data-ttu-id="ec6b9-689">Для параметра `--load-balancer-sku` изменено значение по умолчанию на `standard`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-689">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="ec6b9-690">Для параметра `--vm-set-type` изменено значение по умолчанию на `virtualmachinescalesets`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-690">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="ec6b9-691">AMS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-691">AMS</span></span>

* <span data-ttu-id="ec6b9-692">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя `job start` изменено на `job create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-692">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="ec6b9-693">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В параметре `--ask` команды `content-key-policy create` вместо кодировки UTF8 теперь используется шестнадцатеричная строка из 32 символов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-693">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-694">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-694">AppService</span></span>

* <span data-ttu-id="ec6b9-695">Добавлены команды `webapp config access-restriction show|set|add|remove`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-695">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="ec6b9-696">Улучшена обработка ошибок в `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-696">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="ec6b9-697">Для `appservice plan update` добавлена поддержка номера SKU `Isolated`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-697">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="ec6b9-698">ARM</span><span class="sxs-lookup"><span data-stu-id="ec6b9-698">ARM</span></span>

* <span data-ttu-id="ec6b9-699">В `deployment create` добавлен параметр `--handle-extended-json-format` для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-699">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="ec6b9-700">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-700">Compute</span></span>

* <span data-ttu-id="ec6b9-701">Добавлен параметр `--enable-agent` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-701">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="ec6b9-702">Внесены изменения в `vm create`, позволяющие автоматически использовать номер SKU "Стандартный" для общедоступных IP-адресов при использовании зон.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-702">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="ec6b9-703">Внесены изменения в `vm create`, позволяющие автоматически создавать допустимое имя для виртуальной машины, если оно не задано.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-703">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="ec6b9-704">В `vmss create` добавлен параметр `--computer-name-prefix` для поддержки пользовательского префикса имени для виртуальных машин в VMSS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-704">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="ec6b9-705">В `vm create` добавлен параметр `--workspace` для автоматического включения рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-705">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="ec6b9-706">API коллекций обновлен до версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-706">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-707">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-707">Core</span></span>

* <span data-ttu-id="ec6b9-708">Добавлена проверка синтаксиса для параметра `--set` в универсальной команде обновления.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-708">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="ec6b9-709">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-709">IoT</span></span>

* <span data-ttu-id="ec6b9-710">Исправлена проблема, при которой `iot hub show` неправильно выдавал ошибку "Ресурс не найден".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-710">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-711">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-711">Monitor</span></span>

* <span data-ttu-id="ec6b9-712">В `monitor log-analytics workspace` добавлена поддержка CRUD.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-712">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-713">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-713">Network</span></span>

* <span data-ttu-id="ec6b9-714">В `network private-dns link vnet [create|update]` добавлена поддержка виртуального канала для клиентов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-714">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="ec6b9-715">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для `network vnet subnet list` теперь требуются параметры `--resource-group` и `--vnet-name`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-715">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-716">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-716">SQL</span></span>

* <span data-ttu-id="ec6b9-717">В `sql mi ad-admin` добавлены команды, которые поддерживают назначение администратора AAD в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-717">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-718">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-718">Storage</span></span>

* <span data-ttu-id="ec6b9-719">В `storage copy` добавлен параметр `--preserve-s2s-access-tier`, позволяющий сохранить уровень доступа во время копирования между службами.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-719">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="ec6b9-720">В `storage account [create|update]` добавлен параметр `--enable-large-file-share` для поддержки общих папок большого размера в учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-720">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="ec6b9-721">24 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-721">September 24, 2019</span></span>

<span data-ttu-id="ec6b9-722">Версия 2.0.74</span><span class="sxs-lookup"><span data-stu-id="ec6b9-722">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-723">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-723">ACR</span></span>

* <span data-ttu-id="ec6b9-724">В `acr config retention update` добавлен обязательный параметр `--type`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-724">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="ec6b9-725">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованный параметр `--name -n` изменен на `--registry -r ` для группы команд `acr config`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-725">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="ec6b9-726">AKS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-726">AKS</span></span>

* <span data-ttu-id="ec6b9-727">В команду `aks create` добавлен параметр `--load-balancer-sku`, позволяющий создать кластер AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-727">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="ec6b9-728">В команды `aks [create|update]` добавлены параметры `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` и `--load-balancer-outbound-ip-prefixes`, позволяющие обновлять профиль подсистемы балансировки нагрузки у кластера AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-728">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="ec6b9-729">В команду `aks create` добавлен параметр `--vm-set-type`, позволяющий указывать типы виртуальных машин в кластере AKS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-729">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="ec6b9-730">ARM</span><span class="sxs-lookup"><span data-stu-id="ec6b9-730">ARM</span></span>

* <span data-ttu-id="ec6b9-731">В команду `group deployment create` добавлен параметр `--handle-extended-json-format`, для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-731">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="ec6b9-732">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-732">Compute</span></span>

* <span data-ttu-id="ec6b9-733">В команды `vmss [create|update]` добавлен параметр `--terminate-notification-time`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-733">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="ec6b9-734">В команду `vmss update` добавлен параметр `--enable-terminate-notification`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-734">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="ec6b9-735">В команды `[vm|vmss] create` добавлены параметры `--priority,`, `--eviction-policy,` и `--max-billing`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-735">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="ec6b9-736">Изменена команда `disk create`, которая теперь позволяет указать точный размер отправки на диск.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-736">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="ec6b9-737">В `snapshot create` добавлена поддержка добавочных моментальных снимков для управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-737">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="ec6b9-738">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ec6b9-738">Cosmos DB</span></span>

* <span data-ttu-id="ec6b9-739">В команду `cosmosdb keys list` добавлен параметр `--type <key-type>` для отображения ключей, ключей только для чтения или строк подключения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-739">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="ec6b9-740">Добавлена команда `cosmosdb keys regenerate`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-740">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="ec6b9-741">[УСТАРЕЛО] Команды `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` и `cosmosdb list-read-only-keys` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-741">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="ec6b9-742">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="ec6b9-742">EventGrid</span></span>

* <span data-ttu-id="ec6b9-743">Исправлен текст справки по конечной точке — дана ссылка на правильный параметр.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-743">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="ec6b9-744">Key Vault</span><span class="sxs-lookup"><span data-stu-id="ec6b9-744">Key Vault</span></span>

* <span data-ttu-id="ec6b9-745">Исправлена проблема, из-за которой вход с помощью клиента (`login -t`) мог приводить к сбою `keyvault create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-745">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-746">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-746">Monitor</span></span>

* <span data-ttu-id="ec6b9-747">Исправлена проблема с тем, что символ `:` являлся недопустимым в аргументе `--condition` для `monitor metrics alert create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-747">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="ec6b9-748">Политика</span><span class="sxs-lookup"><span data-stu-id="ec6b9-748">Policy</span></span>

* <span data-ttu-id="ec6b9-749">Добавлена поддержка API Политики версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-749">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="ec6b9-750">В команду `policy assignment create` добавлен параметр `--enforcement-mode`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-750">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-751">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-751">Storage</span></span>

* <span data-ttu-id="ec6b9-752">В команду `az storage copy` добавлен параметр `--blob-type`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-752">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="ec6b9-753">10 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-753">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-754">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-754">ACR</span></span>

* <span data-ttu-id="ec6b9-755">Добавлена группа команд `acr config retention` для настройки политики хранения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-755">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="ec6b9-756">AKS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-756">AKS</span></span>

* <span data-ttu-id="ec6b9-757">Добавлена возможность интеграции ACR с помощью следующих команд:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-757">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="ec6b9-758">В `aks [create|update]` добавлен параметр `--attach-acr` для подключения ACR к кластеру AKS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-758">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="ec6b9-759">В `aks update` добавлен параметр `--detach-acr` для отключения ACR от кластера AKS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-759">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="ec6b9-760">ARM</span><span class="sxs-lookup"><span data-stu-id="ec6b9-760">ARM</span></span>

* <span data-ttu-id="ec6b9-761">Добавлена возможность использования API версии 2019-05-10.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-761">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="ec6b9-762">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-762">Batch</span></span>

* <span data-ttu-id="ec6b9-763">Добавлены новые параметры конфигурации JSON в `--json-file` для `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-763">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="ec6b9-764">Добавлен параметр `MountConfigurations` для подключений файловой системы (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-764">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="ec6b9-765">Добавлено необязательное свойство `publicIPs` в `NetworkConfiguration` для общедоступных IP-адресов в пулах (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-765">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="ec6b9-766">В `--image` добавлена поддержка коллекций общих образов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-766">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="ec6b9-767">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `--start-task-wait-for-success` в `batch pool create` изменено на `true`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-767">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="ec6b9-768">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `Scope` в `AutoUserSpecification` задано как Pool (ранее `Task` на узлах Windows и `Pool` на узлах Linux).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-768">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="ec6b9-769">Этот аргумент можно задать только в конфигурации JSON с помощью `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-769">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="ec6b9-770">HDInsight</span><span class="sxs-lookup"><span data-stu-id="ec6b9-770">HDInsight</span></span>

* <span data-ttu-id="ec6b9-771">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="ec6b9-771">GA release</span></span>
* <span data-ttu-id="ec6b9-772">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--workernode-count/-c` в `az hdinsight resize` теперь является обязательным.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-772">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="ec6b9-773">Key Vault</span><span class="sxs-lookup"><span data-stu-id="ec6b9-773">Key Vault</span></span>

* <span data-ttu-id="ec6b9-774">Исправлена проблема, когда подсети не удавалось удалить из сетевых правил.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-774">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="ec6b9-775">Исправлена проблема, когда дублированные подсети и IP-адреса могли быть добавлены к сетевым правилам.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-775">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-776">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-776">Network</span></span>

* <span data-ttu-id="ec6b9-777">Добавлен параметр `--interval` в `network watcher flow-log` для выбора значения интервала анализа трафика.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-777">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="ec6b9-778">Добавлена команда `network application-gateway identity` для управления удостоверением шлюза.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-778">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="ec6b9-779">Добавлена возможность указать идентификатор Key Vault в команде `network application-gateway ssl-cert`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-779">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="ec6b9-780">Добавлена команда `network express-route peering peer-connection [show|list]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-780">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="ec6b9-781">Политика</span><span class="sxs-lookup"><span data-stu-id="ec6b9-781">Policy</span></span>

* <span data-ttu-id="ec6b9-782">Добавлена возможность использования API версии 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-782">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="ec6b9-783">27 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-783">August 27, 2019</span></span>

<span data-ttu-id="ec6b9-784">Версия 2.0.72</span><span class="sxs-lookup"><span data-stu-id="ec6b9-784">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-785">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-785">ACR</span></span>

* <span data-ttu-id="ec6b9-786">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка SKU `classic`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-786">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="ec6b9-787">Управление API</span><span class="sxs-lookup"><span data-stu-id="ec6b9-787">API Management</span></span>

* <span data-ttu-id="ec6b9-788">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена группа команд `apim`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-788">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-789">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-789">AppService</span></span>

* <span data-ttu-id="ec6b9-790">Исправлена проблема с командой `webapp webjob continuous start` при указании слота.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-790">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="ec6b9-791">Изменена команда `webapp up` для обнаружения и удаления папки `env` из файла, используемого для развертывания.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-791">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="ec6b9-792">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-792">Keyvault</span></span>

* <span data-ttu-id="ec6b9-793">Исправлена ошибка в команде `keyvault secret set`, которая игнорировала аргумент `--expires`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-793">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-794">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-794">Network</span></span>

* <span data-ttu-id="ec6b9-795">Добавлена поддержка IPv6-адресов для аргументов `--private-ip-address-version`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-795">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="ec6b9-796">Добавлены новые команды `network private-endpoint [create|update|list-types]` для управления закрытыми конечными точками.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-796">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="ec6b9-797">Добавлена группа команд для `network private-link-service`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-797">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="ec6b9-798">Добавлены аргументы `--private-endpoint-network-policies` и `--private-link-service-network-policies` для команды `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-798">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="ec6b9-799">RBAC</span><span class="sxs-lookup"><span data-stu-id="ec6b9-799">RBAC</span></span>

* <span data-ttu-id="ec6b9-800">Исправлена проблема с `ad app update --homepage`, когда домашнюю страницу нельзя было обновить.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-800">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="ec6b9-801">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ec6b9-801">ServiceFabric</span></span>

* <span data-ttu-id="ec6b9-802">Добавлена поддержка имен Key Vault в смешанном регистре.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-802">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="ec6b9-803">Исправлена проблема с использованием сертификатов в Key Vault.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-803">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="ec6b9-804">Исправлена проблема с использованием файлов сертификатов PFX.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-804">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="ec6b9-805">Исправлена проблема с `sf cluster certificate add`, когда группа ресурсов Key Vault не была указана.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-805">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="ec6b9-806">Исправлена проблема с неработающей командой `sf cluster set`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-806">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="ec6b9-807">SignalR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-807">SignalR</span></span>

* <span data-ttu-id="ec6b9-808">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-808">Added new commands:</span></span>
  * <span data-ttu-id="ec6b9-809">`signalr cors`: Управление CORS SignalR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-809">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="ec6b9-810">`signalr restart`: Перезапуск службы SignalR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-810">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="ec6b9-811">`signalr update`: Обновление службы SignalR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-811">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="ec6b9-812">Добавлен аргумент `--service-mode` для команды `signalr create`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-812">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-813">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-813">Storage</span></span>

* <span data-ttu-id="ec6b9-814">Добавлена команда `storage account revoke-delegation-keys`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-814">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="ec6b9-815">13 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-815">August 13, 2019</span></span>

<span data-ttu-id="ec6b9-816">Версия 2.0.71</span><span class="sxs-lookup"><span data-stu-id="ec6b9-816">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-817">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-817">AppService</span></span>

* <span data-ttu-id="ec6b9-818">Исправлена проблема, из-за которой выполнение команд `webapp webjob continuous` для слотов завершалось сбоем.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-818">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="ec6b9-819">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="ec6b9-819">BotService</span></span>

* <span data-ttu-id="ec6b9-820">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка создания ботов на основе пакета SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-820">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="ec6b9-821">Cognitive Services:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-821">CognitiveServices</span></span>

* <span data-ttu-id="ec6b9-822">Добавлены команды `cognitiveservices account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-822">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="ec6b9-823">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ec6b9-823">Cosmos DB</span></span>

* <span data-ttu-id="ec6b9-824">Удалено предупреждение при обновлении нескольких расположений для записи.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-824">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="ec6b9-825">Добавлены команды CRUD для ресурсов CosmosDB SQL, MongoDB, Cassandra, Gremlin и ресурсов таблиц, а также пропускной способности ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-825">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="ec6b9-826">HDInsight</span><span class="sxs-lookup"><span data-stu-id="ec6b9-826">HDInsight</span></span>

<span data-ttu-id="ec6b9-827">Этот выпуск содержит большое число критических изменений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-827">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="ec6b9-828">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-828">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="ec6b9-829">Переименование `--storage-default-container` в `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-829">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="ec6b9-830">Переименование `--storage-default-filesystem` в `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-830">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="ec6b9-831">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--name` для `application create`, чтобы представлять имя приложения вместо имени кластера.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-831">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="ec6b9-832">Добавлен аргумент `--cluster-name` для `application create`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-832">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="ec6b9-833">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-833">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="ec6b9-834">Переименование `--application-type` в `--type`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-834">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="ec6b9-835">Переименование `--marketplace-identifier` в `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-835">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="ec6b9-836">Переименование `--https-endpoint-access-mode` в `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-836">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="ec6b9-837">Переименован аргумент `--https-endpoint-destination-port` на `--destination-port`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-837">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="ec6b9-838">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-838">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="ec6b9-839">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Переименован аргумент `--target-instance-count` на `--workernode-count` для `hdinsight resize`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-839">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="ec6b9-840">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены все команды в группе `hdinsight script-action`, чтобы использовать параметр `--name` в качестве имени действия скрипта.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-840">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="ec6b9-841">Добавлен аргумент `--cluster-name` для всех команд `hdinsight script-action`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-841">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="ec6b9-842">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименован аргумент `--script-execution-id` на `--execution-id`для всех команд `hdinsight script-action`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-842">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="ec6b9-843">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `hdinsight script-action show` переименована в `hdinsight script-action show-execution-details`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-843">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="ec6b9-844">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Изменены параметры для `hdinsight script-action execute --roles`, чтобы они разделялись пробелами, а не запятыми.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-844">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="ec6b9-845">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--persisted` для `hdinsight script-action list`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-845">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="ec6b9-846">Изменен параметр `hdinsight create --cluster-configurations`, чтобы принимать путь к локальному файлу JSON или строке JSON.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-846">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="ec6b9-847">Добавлена команда `hdinsight script-action list-execution-history`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-847">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="ec6b9-848">Изменен параметр `hdinsight monitor enable --workspace`, чтобы принимать идентификатор или имя рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-848">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="ec6b9-849">Добавлен аргумент `hdinsight monitor enable --primary-key`, который требуется, если в качестве параметра указан идентификатор рабочей области.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-849">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="ec6b9-850">Добавлены дополнительные примеры и обновленные описания для справочных сообщений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-850">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="ec6b9-851">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="ec6b9-851">Interactive</span></span>

* <span data-ttu-id="ec6b9-852">Исправлена ошибка загрузки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-852">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="ec6b9-853">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="ec6b9-853">Kubernetes</span></span>

* <span data-ttu-id="ec6b9-854">Теперь используется `https`, если порт контейнера панели мониторинга использует `https`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-854">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-855">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-855">Network</span></span>

* <span data-ttu-id="ec6b9-856">Добавлен аргумент `--yes` для `network dns record-set cname delete`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-856">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="ec6b9-857">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-857">Profile</span></span>

* <span data-ttu-id="ec6b9-858">Добавлен аргумент `--resource-type` для `account get-access-token`, чтобы получать маркеры доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-858">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="ec6b9-859">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ec6b9-859">ServiceFabric</span></span>

* <span data-ttu-id="ec6b9-860">Добавлены все поддерживаемые версии ОС для команды sf cluster create.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-860">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="ec6b9-861">Исправлена ошибка проверки основного сертификата.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-861">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-862">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-862">Storage</span></span>

* <span data-ttu-id="ec6b9-863">Добавлена команда `storage copy`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-863">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="ec6b9-864">30 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-864">July 30, 2019</span></span>

<span data-ttu-id="ec6b9-865">Версия 2.0.70</span><span class="sxs-lookup"><span data-stu-id="ec6b9-865">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-866">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-866">ACR</span></span>

* <span data-ttu-id="ec6b9-867">Исправлена проблема № 9952 (регрессия в команде `acr pack build`).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-867">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="ec6b9-868">Удалено имя образа построителя по умолчанию в `acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-868">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-869">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-869">Appservice</span></span>

* <span data-ttu-id="ec6b9-870">Команда `webapp config ssl` изменена для отображения сообщения, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-870">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="ec6b9-871">Исправлена проблема, когда команда `functionapp create` не принимала тип учетной записи хранения `Standard_RAGRS`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-871">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="ec6b9-872">Исправлена проблема, когда команда `webapp up` завершала работу со сбоем в случае выполнения со старой версией Python.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-872">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-873">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-873">Network</span></span>

* <span data-ttu-id="ec6b9-874">Удален недопустимый параметр `--ids` из `network nic ip-config add` (исправление проблемы № 9861).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-874">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="ec6b9-875">Исправлена проблема № 9604.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-875">Fixes #9604.</span></span> <span data-ttu-id="ec6b9-876">Добавлен параметр `--root-certs` в `network application-gateway http-settings [create|update]` для поддержки связанных с пользователем доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-876">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="ec6b9-877">Исправлен аргумент `--subscription` для `network dns record-set ns create` (проблема № 9965).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-877">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="ec6b9-878">RBAC</span><span class="sxs-lookup"><span data-stu-id="ec6b9-878">RBAC</span></span>

* <span data-ttu-id="ec6b9-879">Добавлена команда `user update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-879">Added `user update` command</span></span>
* <span data-ttu-id="ec6b9-880">[УСТАРЕЛО]`--upn-or-object-id` не рекомендуется использовать в связанных с пользователями командах.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-880">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="ec6b9-881">Вместо этого применяйте аргумент `--id`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-881">Use replacement argument `--id`</span></span>
* <span data-ttu-id="ec6b9-882">Добавлен аргумент `--id` в связанные с пользователями команды.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-882">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-883">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-883">SQL</span></span>

* <span data-ttu-id="ec6b9-884">Добавлены команды управления для ключей и предохранителя TDE управляемого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-884">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-885">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-885">Storage</span></span>

* <span data-ttu-id="ec6b9-886">Добавлена команда `storage remove`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-886">Added `storage remove` command</span></span>
* <span data-ttu-id="ec6b9-887">Исправлена проблема с `storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-887">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-888">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-888">VM</span></span>

* <span data-ttu-id="ec6b9-889">Изменена команда `list-skus` для использования новой версии API для вывода сведений о зонах.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-889">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="ec6b9-890">Изменено значение по умолчанию параметра `--single-placement-group` на `false` для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-890">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="ec6b9-891">Добавлена возможность выбирать номера SKU хранилища ZRS для `[snapshot|disk] create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-891">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="ec6b9-892">Добавлена новая группа команд `vm host` для поддержки выделенных узлов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-892">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="ec6b9-893">Добавлены параметры `--host` и `--host-group` в команде `vm create` для указания выделенного узла виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-893">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="ec6b9-894">16 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-894">July 16, 2019</span></span>

<span data-ttu-id="ec6b9-895">Версия 2.0.69</span><span class="sxs-lookup"><span data-stu-id="ec6b9-895">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-896">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-896">Appservice</span></span>

* <span data-ttu-id="ec6b9-897">Изменены команды `webapp identity`. Теперь они возвращают правильное сообщение об ошибке, если параметр ResourceGroupName или имя приложения недопустимы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-897">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="ec6b9-898">Исправлена команда `webapp list`. Теперь она возвращает правильное значение для параметра numberOfSites, если не указан параметр ResourceGroup.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-898">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="ec6b9-899">Исправлены побочные эффекты для команд `appservice plan create` и `webapp create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-899">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-900">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-900">Core</span></span>

* <span data-ttu-id="ec6b9-901">Исправлена ошибка, при которой отображался параметр `--subscription`, хотя он был неприменим.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-901">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="ec6b9-902">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-902">Batch</span></span>

* <span data-ttu-id="ec6b9-903">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `batch pool node-agent-skus list` заменена на `batch pool supported-images list`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-903">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="ec6b9-904">Добавлена поддержка правил безопасности, которые блокируют сетевой доступ к пулу на основе исходного порта трафика при использовании параметра `--json-file` команды `batch pool create network`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-904">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="ec6b9-905">Добавлена поддержка выполнения задачи в рабочей папке контейнера или рабочей папке задачи пакета при использовании параметра `--json-file` команды `batch task create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-905">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="ec6b9-906">Исправлена ошибка в параметре `--application-package-references` команды `batch pool create`, которая позволяла работать только со значениями по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-906">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="ec6b9-907">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="ec6b9-907">Eventhubs</span></span>

* <span data-ttu-id="ec6b9-908">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-908">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="ec6b9-909">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ec6b9-909">RDBMS</span></span>

* <span data-ttu-id="ec6b9-910">Добавлен необязательный параметр для указания номера SKU реплики в команде создания реплики.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-910">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="ec6b9-911">Исправлена ошибка теста CI при создании реплики MySQL.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-911">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="ec6b9-912">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="ec6b9-912">Relay</span></span>

* <span data-ttu-id="ec6b9-913">Исправлена проблема с гибридным подключением при выключенной авторизации клиента ([8775](https://github.com/azure/azure-cli/issues/8775)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-913">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="ec6b9-914">Добавлен параметр `--requires-transport-security` для команды `relay wcfrelay create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-914">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="ec6b9-915">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="ec6b9-915">Servicebus</span></span>

* <span data-ttu-id="ec6b9-916">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-916">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-917">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-917">Storage</span></span>

* <span data-ttu-id="ec6b9-918">Добавлена возможность обновления учетной записи хранения для AADDS в службе "Файлы".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-918">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="ec6b9-919">Устранена проблема, описанная здесь: `storage blob service-properties update --set`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-919">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="ec6b9-920">2 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-920">July 2, 2019</span></span>

<span data-ttu-id="ec6b9-921">Версия 2.0.68</span><span class="sxs-lookup"><span data-stu-id="ec6b9-921">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-922">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-922">Core</span></span>

* <span data-ttu-id="ec6b9-923">Командные модули теперь объединены в один распространяемый пакет Python.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-923">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="ec6b9-924">В результате этого прекращается непосредственное использование множества пакетов `azure-cli-` в PyPI.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-924">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="ec6b9-925">Это также должно уменьшить размер установки и повлияет только на пользователей, которые выполняли установку непосредственно через `pip`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-925">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-926">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-926">ACR</span></span>

* <span data-ttu-id="ec6b9-927">В заданиях добавлена поддержка триггеров таймера.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-927">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-928">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-928">Appservice</span></span>

* <span data-ttu-id="ec6b9-929">Внесены изменения в `functionapp create` для включения Application Insights по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-929">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="ec6b9-930">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена устаревшая команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-930">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="ec6b9-931">Вместо нее используйте новую команду `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-931">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="ec6b9-932">В `functionapp deployment config-zip` добавлена поддержка плана потребления приложения-функции Linux.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-932">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="ec6b9-933">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ec6b9-933">Cosmos DB</span></span>

* <span data-ttu-id="ec6b9-934">Добавлена возможность отключения TTL.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-934">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="ec6b9-935">DLS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-935">DLS</span></span>

* <span data-ttu-id="ec6b9-936">Обновленная версия ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="ec6b9-936">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="ec6b9-937">Отзывы</span><span class="sxs-lookup"><span data-stu-id="ec6b9-937">Feedback</span></span>

* <span data-ttu-id="ec6b9-938">При сообщении о сбое при выполнении команды расширения `az feedback` теперь пытается открыть браузер по URL-адресу репозитория или проекта расширения из индекса.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-938">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="ec6b9-939">HDInsight</span><span class="sxs-lookup"><span data-stu-id="ec6b9-939">HDInsight</span></span>

* <span data-ttu-id="ec6b9-940">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя группы команд `oms` изменилось на `monitor`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-940">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="ec6b9-941">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--http-password/-p` стал обязательным.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-941">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="ec6b9-942">Добавлены средства заполнения для `--cluster-admin-account` и средство заполнения для параметров `cluster-users-group-dns`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-942">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="ec6b9-943">Параметр `cluster-users-group-dns` стал обязательным, если присутствует `—esp`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-943">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="ec6b9-944">Добавлено время ожидания для всех существующих средств автоматического заполнения аргументов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-944">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="ec6b9-945">Добавлено время ожидания для преобразования имени ресурса в идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-945">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="ec6b9-946">Внесены изменения в средства автоматического заполнения для выбора ресурсов из любой группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-946">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="ec6b9-947">Это может быть группа ресурсов, отличная от той, которая указана с помощью `-g`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-947">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="ec6b9-948">Добавлена поддержка параметров `--sub-domain-suffix` и `--disable_gateway_auth` в команде `hdinsight application create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-948">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="ec6b9-949">Управляемые службы</span><span class="sxs-lookup"><span data-stu-id="ec6b9-949">Managed Services</span></span>

* <span data-ttu-id="ec6b9-950">Командный модуль управляемых служб выпущен в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-950">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="ec6b9-951">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-951">Profile</span></span>
* <span data-ttu-id="ec6b9-952">Аргумент `--subscription` подавляется для команды выхода.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-952">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="ec6b9-953">RBAC</span><span class="sxs-lookup"><span data-stu-id="ec6b9-953">RBAC</span></span>

* <span data-ttu-id="ec6b9-954">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален аргумент `--password` для `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-954">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="ec6b9-955">В команду `create` добавлен параметр `--assignee-principal-type` для устранения периодических сбоев из-за задержки репликации сервера AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-955">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="ec6b9-956">Исправлен сбой в `ad signed-in-user` при перечислении собственных объектов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-956">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="ec6b9-957">Исправлена проблема, при которой `ad sp` не удавалось найти нужное приложение в субъекте-службе.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-957">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="ec6b9-958">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ec6b9-958">RDBMS</span></span>

* <span data-ttu-id="ec6b9-959">Добавлена поддержка репликации MariaDB.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-959">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-960">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-960">SQL</span></span>

* <span data-ttu-id="ec6b9-961">Описаны допустимые значения для `sql db create --sample-name`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-961">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-962">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-962">Storage</span></span>

* <span data-ttu-id="ec6b9-963">В `storage blob generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-963">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="ec6b9-964">В `storage container generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-964">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="ec6b9-965">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-965">VM</span></span>

* <span data-ttu-id="ec6b9-966">Исправлена ошибка, при которой команда `vmss create` возвращала сообщение об ошибке при выполнении с `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-966">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="ec6b9-967">Прекращена проверка `vmss create --single-placement-group` на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-967">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="ec6b9-968">Команда не завершается сбоем, если для `--single-placement-group` задано значение `true`, а значение `--instance-count` больше 100 или указаны зоны доступности. Сама проверка теперь выполняется службой вычислений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-968">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="ec6b9-969">Исправлена ошибка, при которой команда `[vm|vmss] extension image list` завершалась сбоем при указании `--latest`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-969">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="ec6b9-970">18 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-970">June 18, 2019</span></span>

<span data-ttu-id="ec6b9-971">Версия 2.0.67</span><span class="sxs-lookup"><span data-stu-id="ec6b9-971">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-972">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-972">Core</span></span>

<span data-ttu-id="ec6b9-973">В этом выпуске добавлен новый тег [Предварительная версия], который яснее дает понять, что группа команд, команда или аргумент находятся в состоянии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-973">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="ec6b9-974">Ранее это указывалось в тексте справки или подразумевалось в номере версии командного модуля.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-974">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="ec6b9-975">В будущем в интерфейсе командной строки номера версий отдельных пакетов не будут указываться.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-975">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="ec6b9-976">Если команда доступна в предварительной версии, это также касается и всех ее аргументов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-976">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="ec6b9-977">Если группа команд помечается как находящаяся в предварительной версии, значит все команды и аргументы также считаются доступными в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-977">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="ec6b9-978">В результате этого изменения несколько групп команд могут "внезапно" оказаться в состоянии предварительной версии в этом выпуске.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-978">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="ec6b9-979">В действительности большинство пакетов, которые находились в состоянии предварительной версии, в этом выпуске будут считаться общедоступными.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-979">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-980">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-980">ACR</span></span>
* <span data-ttu-id="ec6b9-981">Добавлена команда acr check-health.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-981">Added 'acr check-health' command</span></span>
* <span data-ttu-id="ec6b9-982">Улучшена обработка ошибок с маркерами безопасности AAD и ошибок при получении внешних команд.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-982">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-983">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-983">ACS</span></span>
* <span data-ttu-id="ec6b9-984">Устаревшие команды ACS теперь скрыты в тексте справки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-984">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="ec6b9-985">AMS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-985">AMS</span></span>
* <span data-ttu-id="ec6b9-986">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в возврате строк времени ISO 8601 для archive-window-length и key-frame-interval-duration.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-986">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-987">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-987">AppService</span></span>
* <span data-ttu-id="ec6b9-988">Добавлена маршрутизация на основе расположение для `webapp deleted list` и `webapp deleted restore`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-988">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="ec6b9-989">Исправлена проблема, при которой целевой URL-адрес веб-приложения ("Вы можете запустить приложение в...") не был активным в Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-989">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="ec6b9-990">Устранена проблема, при которой создание приложений в некоторых SKU завершалось сбоем с ошибкой AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-990">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="ec6b9-991">Добавлена предварительная проверка в `[appservice|webapp] create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-991">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="ec6b9-992">Исправлено `[webapp|functionapp] traffic-routing` для использования правильного actionHostName.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-992">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="ec6b9-993">Добавлена поддержка слотов для команд `functionapp`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-993">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="ec6b9-994">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-994">Batch</span></span>
* <span data-ttu-id="ec6b9-995">Исправлена регрессия проверки подлинности AAD, которую вызывал чрезмерный поток уведомлений об авторизации с помощью общего ключа.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-995">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="ec6b9-996">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ec6b9-996">BatchAI</span></span>
* <span data-ttu-id="ec6b9-997">Команды BatchAI теперь признаны устаревшими и скрыты.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-997">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="ec6b9-998">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="ec6b9-998">BotService</span></span>
* <span data-ttu-id="ec6b9-999">Добавлены предупреждающие сообщения о прекращении поддержки и режиме обслуживания для команд, которые поддерживают пакет SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-999">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ec6b9-1000">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1000">CosmosDB</span></span>
* <span data-ttu-id="ec6b9-1001">[УСТАРЕЛО] использовать команду `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1001">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="ec6b9-1002">Добавлена команда `cosmosdb keys list`, заменяющая `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1002">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="ec6b9-1003">`cosmsodb create/update`: Добавлен новый формат для --location, который позволяет задавать свойство isZoneRedundant.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1003">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="ec6b9-1004">Нерекомендуемый старый формат.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1004">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="ec6b9-1005">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1005">EventGrid</span></span>
* <span data-ttu-id="ec6b9-1006">Добавлены команды `eventgrid domain` для операций CRUD домена.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1006">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="ec6b9-1007">Добавлены команды `eventgrid domain topic` для операций CRUD разделов домена.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1007">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="ec6b9-1008">В `eventgrid [topic|event-subscription] list` добавлен аргумент `--odata-query` для фильтрации результатов с использованием синтаксиса OData.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1008">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="ec6b9-1009">`event-subscription create/update`: Добавлена ServiceBusQueue в качестве новых значений для параметра `--endpoint-type`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1009">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="ec6b9-1010">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в прекращении поддержки `--included-event-types All` с `eventgrid event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1010">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="ec6b9-1011">HDInsight</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1011">HDInsight</span></span>
* <span data-ttu-id="ec6b9-1012">Добавлена поддержка параметра `--ssh-public-key` в команде `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1012">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="ec6b9-1013">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1013">IoT</span></span>
* <span data-ttu-id="ec6b9-1014">Добавлена поддержка для повторного создания ключей политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1014">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="ec6b9-1015">Добавлен пакет SDK и поддержка для службы подготовки репозитория DigitalTwin.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1015">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1016">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1016">Network</span></span>
* <span data-ttu-id="ec6b9-1017">Добавлена поддержка зон для Шлюза NAT.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1017">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="ec6b9-1018">Добавлена команда `network list-service-tags`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1018">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="ec6b9-1019">Исправлена проблема с `dns zone import`, при которой пользователям не удавалось импортировать записи А с подстановочным знаком.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1019">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="ec6b9-1020">Исправлена проблема с `watcher flow-log configure`, при которой не удавалось включить ведение журнала потоков в определенных регионах.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1020">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-1021">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1021">Resource</span></span>
* <span data-ttu-id="ec6b9-1022">Добавлена команда `az rest` для вызовов REST.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1022">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="ec6b9-1023">Исправлена ошибка, возникавшая при использовании `policy assignment list` с группой ресурсов или уровнем подписки `--scope`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1023">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="ec6b9-1024">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1024">ServiceBus</span></span>
* <span data-ttu-id="ec6b9-1025">Устранена проблема № [9319](https://github.com/azure/azure-cli/issues/9319) с `servicebus topic create --max-size`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1025">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-1026">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1026">SQL</span></span>
* <span data-ttu-id="ec6b9-1027">Параметр `--location` стал необязательным для `sql [server|mi] create`. Если он не указан, используется расположение группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1027">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="ec6b9-1028">Исправлена ошибка "Объект NoneType не подлежит итерации" с `sql db list-editions --available`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1028">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="ec6b9-1029">SQLVm</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1029">SQLVm</span></span>
* <span data-ttu-id="ec6b9-1030">Критическое изменение. Для `sql vm create` теперь требуется параметр `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1030">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="ec6b9-1031">Внесены изменения, позволяющие задавать SKU образа SQL при создании или обновлении виртуальной машины SQL.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1031">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-1032">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1032">Storage</span></span>
* <span data-ttu-id="ec6b9-1033">Исправлена проблема с отсутствующим ключом учетной записи для `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1033">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="ec6b9-1034">Исправлена проблема с `storage blob sync` на платформе Linux.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1034">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-1035">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1035">VM</span></span>
* <span data-ttu-id="ec6b9-1036">[Предварительная версия] Добавлены команды `vm image template` для создания образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1036">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="ec6b9-1037">4 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1037">June 4, 2019</span></span>

<span data-ttu-id="ec6b9-1038">Версия 2.0.66</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1038">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-1039">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1039">Core</span></span>
* <span data-ttu-id="ec6b9-1040">Исправлена ошибка, из-за которой выполнение команды завершалось со сбоем, если параметр `--output yaml` использовался с параметром `--query`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1040">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-1041">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1041">ACR</span></span>
* <span data-ttu-id="ec6b9-1042">Добавлена группа команд acr pack для создания заданий быстрой сборки с помощью пакетов сборок.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1042">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-1043">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1043">ACS</span></span>
* <span data-ttu-id="ec6b9-1044">Разрешено включение и отключение надстройки панели мониторинга Kubernetes для AKS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1044">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="ec6b9-1045">Если подписку нельзя использовать с Azure Red Hat OpenShift, будет отображаться соответствующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1045">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="ec6b9-1046">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1046">Batch</span></span>
* <span data-ttu-id="ec6b9-1047">Улучшена обработка ошибок, если не выполнен вход в учетную запись \[[№ 9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[№ 8978](https://github.com/Azure/azure-cli/issues/8978)\].</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1047">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="ec6b9-1048">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1048">IoT</span></span>
* <span data-ttu-id="ec6b9-1049">Добавлена поддержка для перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1049">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1050">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1050">Network</span></span>
* <span data-ttu-id="ec6b9-1051">Добавлены команды `network application-gateway waf-policy` для поддержки настраиваемых правил WAF.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1051">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="ec6b9-1052">Добавлены аргументы `--waf-policy` и `--max-capacity` для команды `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1052">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="ec6b9-1053">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1053">Resource</span></span>
* <span data-ttu-id="ec6b9-1054">Улучшен вывод сообщения команды `deployment create` при отсутствии TTY.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1054">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-1055">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1055">Role</span></span>
* <span data-ttu-id="ec6b9-1056">Обновлен текст справки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1056">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="ec6b9-1057">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1057">Compute</span></span>
* <span data-ttu-id="ec6b9-1058">Добавлена поддержка команды `vm create` для создания виртуальных машин из управляемого образа с номерами LUN дисков данных, которые не начинаются с 0 или для которых пропущены номера.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1058">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="ec6b9-1059">21 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1059">May 21, 2019</span></span>

<span data-ttu-id="ec6b9-1060">Версия 2.0.65</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1060">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-1061">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1061">Core</span></span>
* <span data-ttu-id="ec6b9-1062">Улучшена функция обратной связи при ошибках аутентификации.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1062">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="ec6b9-1063">Исправлена проблема, из-за которой интерфейс командной строки загружал расширения, которые не были совместимы с его базовой версией.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1063">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="ec6b9-1064">Исправлена проблема с запуском и неисправностью `clouds.config`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1064">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-1065">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1065">ACR</span></span>
* <span data-ttu-id="ec6b9-1066">Добавлена поддержка управляемых удостоверений в Задачи.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1066">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-1067">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1067">ACS</span></span>
* <span data-ttu-id="ec6b9-1068">Исправлена команда `openshift create`, используемая с пользовательским клиентом AAD.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1068">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-1069">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1069">AppService</span></span>
* <span data-ttu-id="ec6b9-1070">[УСТАРЕЛО] Команда `functionapp devops-build` устарела и будет удалена в следующем выпуске.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1070">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="ec6b9-1071">Внесено изменение в `functionapp devops-pipeline` для получения журнала сборки из Azure DevOps в режиме подробного протоколирования.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1071">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="ec6b9-1072">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален неподдерживаемый флаг `--use_local_settings` из команды `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1072">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="ec6b9-1073">Внесено изменение в `webapp up` для возврата выходных данных JSON, если `--logs` не используется.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1073">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="ec6b9-1074">Добавлена поддержка записи ресурсов по умолчанию в локальную конфигурацию для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1074">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="ec6b9-1075">Добавлена поддержка `webapp up` для повторного развертывания приложения без использования аргумента `--location`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1075">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="ec6b9-1076">Устранена проблема, из-за которой нельзя было создать для Linux номер SKU с планом службы приложений "Бесплатный".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1076">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="ec6b9-1077">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1077">BotService</span></span>
* <span data-ttu-id="ec6b9-1078">Внесено изменение для включения поддержки всех регистров в параметрах `--lang` для команд.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1078">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="ec6b9-1079">Обновлено описание модуля команды.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1079">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="ec6b9-1080">Потребление</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1080">Consumption</span></span>
* <span data-ttu-id="ec6b9-1081">Добавлен отсутствующий обязательный параметр при выполнении `consumption usage list --billing-period-name`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1081">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="ec6b9-1082">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1082">IoT</span></span>
* <span data-ttu-id="ec6b9-1083">Добавлена поддержка перечисления всех ключей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1083">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1084">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1084">Network</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="ec6b9-1086">Добавлен аргумент `--nat-gateway` для `network vnet subnet [create|update]` для подключения к шлюзу NAT.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1086">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="ec6b9-1087">Исправлена проблема с `dns zone import`, из-за которой имена записей не сопоставлялись с типом записей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1087">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="ec6b9-1088">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1088">RDBMS</span></span>
* <span data-ttu-id="ec6b9-1089">Добавлена поддержка Postgres и MySQL для георепликации.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1089">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="ec6b9-1090">RBAC</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1090">RBAC</span></span>
* <span data-ttu-id="ec6b9-1091">Добавлена поддержка области группы управления для `role assignment`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1091">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-1092">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1092">Storage</span></span>
* <span data-ttu-id="ec6b9-1093">`storage blob sync`: добавьте команду синхронизации для хранилища BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1093">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="ec6b9-1094">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1094">Compute</span></span>
* <span data-ttu-id="ec6b9-1095">Добавлен параметр `--computer-name` для `vm create` для установки имени виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1095">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="ec6b9-1096">Переименован параметр `--ssh-key-value` в `--ssh-key-values` для `[vm|vmss] create` для приема нескольких значений пути или открытого ключа SSH.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1096">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="ec6b9-1097">__Примечание.__ Это **не** критическое изменение, благодаря которому `--ssh-key-value` будет правильно анализироваться, так как соответствует только `--ssh-key-values`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1097">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="ec6b9-1098">Внесено изменение в аргумент `ppg create` для `--type` — теперь он необязательный.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1098">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="ec6b9-1099">6 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1099">May 6, 2019</span></span>

<span data-ttu-id="ec6b9-1100">Версия 2.0.64</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1100">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-1101">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1101">ACS</span></span>
* <span data-ttu-id="ec6b9-1102">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--fqdn` из команд `openshift`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1102">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="ec6b9-1103">Внесено изменение для использования общедоступной версии API для Azure Red Hat Openshift.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1103">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="ec6b9-1104">Добавлен флаг `customer-admin-group-id` в `openshift create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1104">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="ec6b9-1105">[Общедоступная версия.] `(PREVIEW)` больше не используется для `aks create` в параметре `--network-policy`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1105">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-1106">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1106">Appservice</span></span>
* <span data-ttu-id="ec6b9-1107">[УСТАРЕЛО] Команда `functionapp devops-build` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1107">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="ec6b9-1108">Команда переименована в `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1108">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="ec6b9-1109">Исправлен процесс получения правильного имени пользователя для Cloud Shell, приводивший к ошибке выполнения `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1109">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="ec6b9-1110">Обновлена документация по `appservice plan --sku` в соответствии с поддерживаемыми планами службы приложений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1110">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="ec6b9-1111">Добавлены необязательные аргументы для группы ресурсов и план для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1111">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="ec6b9-1112">Добавлена поддержка `webapp ssh` в соответствии с переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1112">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="ec6b9-1113">Добавлена поддержка `appserviceplan create` для ценовой категории "Бесплатный" в Linux.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1113">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="ec6b9-1114">Внесено изменение в `webapp up` для перевода в спящий режим на 30 с после установки параметра приложения `SCM_DO_BUILD_DURING_DEPLOYMENT=true` для обработки холодного запуска Kudu.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1114">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="ec6b9-1115">Добавлена поддержка среды выполнения `powershell` для `functionapp create` в Windows.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1115">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="ec6b9-1116">Добавлена команда `create-remote-connection`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1116">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="ec6b9-1117">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1117">Batch</span></span>
* <span data-ttu-id="ec6b9-1118">Исправлена ошибка в проверяющем элементе управления для параметров `--application-package-references`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1118">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="ec6b9-1119">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1119">Botservice</span></span>
* <span data-ttu-id="ec6b9-1120">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` для создания пустого бота веб-приложения по умолчанию (т. е. бот не развертывается в Службе приложений).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1120">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="ec6b9-1121">Добавлен флаг `--echo` в `bot create` для использования старого поведения с `-v v4`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1121">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="ec6b9-1122">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено значение по умолчанию `--version` на `v4`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1122">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="ec6b9-1123">__ПРИМЕЧАНИЕ.__ `bot prepare-publish` по-прежнему использует старое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1123">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="ec6b9-1124">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `--lang` — значение `Csharp` больше не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1124">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="ec6b9-1125">Если команда требует `--lang`, который не указан, команда завершит работу с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1125">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="ec6b9-1126">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в аргументы `--appid` и `--password` для `bot create` — теперь они являются обязательными и их можно создать с помощью `ad app create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1126">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="ec6b9-1127">Добавлена проверка `--appid` и `--password`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1127">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="ec6b9-1128">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4`, чтобы не создавать или не использовать учетную запись хранения или Application Insights.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1128">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="ec6b9-1129">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v3`, чтобы требовать регион, где доступна служба Application Insights.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1129">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="ec6b9-1130">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot update`, чтобы влиять только на определенные свойства бота.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1130">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="ec6b9-1131">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в флаг `--lang` для принятия `Javascript` вместо `Node`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1131">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="ec6b9-1132">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`Node` больше не используется как допустимое значение `--lang`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1132">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="ec6b9-1133">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` — значение `SCM_DO_BUILD_DURING_DEPLOYMENT` больше не равно true.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1133">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="ec6b9-1134">Все развертывания через Kudu будут работать в соответствии с поведением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1134">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="ec6b9-1135">Внесено изменение в `bot download` для ботов без файлов `.bot`, чтобы создавать файл конфигурации для определенного языка со значениями из параметров приложения для бота.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1135">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="ec6b9-1136">В команду `bot prepare-deploy` добавлена поддержка параметра `Typescript`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1136">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="ec6b9-1137">Добавлено предупреждающее сообщение в `bot prepare-deploy` для ботов `Javascript` и `Typescript`, когда `--code-dir` не содержит `package.json`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1137">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="ec6b9-1138">Внесено изменение в `bot prepare-deploy` для возврата `true` при успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1138">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="ec6b9-1139">Включено ведение подробного журнала для `bot prepare-deploy`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1139">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="ec6b9-1140">Добавлены более доступные регионы Application Insights для `az bot create -v v3`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1140">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="ec6b9-1141">Configure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1141">Configure</span></span>
* <span data-ttu-id="ec6b9-1142">Добавлена поддержка конфигурации по умолчанию для аргумента на основе папки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1142">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="ec6b9-1143">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1143">Eventhubs</span></span>
* <span data-ttu-id="ec6b9-1144">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1144">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="ec6b9-1145">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1145">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1146">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1146">Network</span></span>
* <span data-ttu-id="ec6b9-1147">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--cache` на `--defer` для `vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1147">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="ec6b9-1148">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1148">Policy Insights</span></span>
* <span data-ttu-id="ec6b9-1149">Добавлена поддержка `--expand PolicyEvaluationDetails` для результатов оценки политики запросов для ресурса.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1149">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-1150">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1150">Role</span></span>
* <span data-ttu-id="ec6b9-1151">[УСТАРЕЛО] Внесено изменение в `create-for-rbac` для скрытия аргумента --password (поддержка прекращается в мае 2019 г.).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1151">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="ec6b9-1152">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1152">Service Bus</span></span>
* <span data-ttu-id="ec6b9-1153">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1153">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="ec6b9-1154">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1154">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="ec6b9-1155">Внесено исправление в `topic [create|update]` — теперь `--max-size` поддерживает значения 10, 20, 40 и 80 ГБ для номера SKU ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1155">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-1156">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1156">SQL</span></span>
* <span data-ttu-id="ec6b9-1157">Добавлены команды `sql virtual-cluster [list|show|delete]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1157">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-1158">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1158">VM</span></span>
* <span data-ttu-id="ec6b9-1159">Добавлены параметры `--protect-from-scale-in` и `--protect-from-scale-set-actions` для `vmss update`, чтобы включать обновления политики защиты для экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1159">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="ec6b9-1160">Добавлены параметры `--instance-id` для `vmss update` для включения общего обновления экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1160">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="ec6b9-1161">Добавлен параметр `--instance-id` для команды `vmss wait`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1161">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="ec6b9-1162">Добавлена новая группа команд `ppg` для управления группами размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1162">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="ec6b9-1163">Добавлен параметр `--ppg` для `[vm|vmss] create` и `vm availability-set create` для управления PPG.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1163">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="ec6b9-1164">Добавлен параметр `--hyper-v-generation` для команды `image create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1164">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="ec6b9-1165">23 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1165">April 23, 2019</span></span>

<span data-ttu-id="ec6b9-1166">Версия 2.0.63</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1166">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-1167">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1167">ACS</span></span>
* <span data-ttu-id="ec6b9-1168">Внесено изменение в `aks get-credentials` для запроса на перезапись повторяющихся значений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1168">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="ec6b9-1169">Удалено описание `(PREVIEW)` из команд Dev Spaces aks use-dev-spaces и aks remove-dev-spaces.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1169">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="ec6b9-1170">AMS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1170">AMS</span></span>
* <span data-ttu-id="ec6b9-1171">Исправлена ошибка с обновлением фильтров ресурсов и учетных записей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1171">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-1172">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1172">AppService</span></span>
* <span data-ttu-id="ec6b9-1173">Добавлена поддержка ASE и времени ожидания для `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1173">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="ec6b9-1174">Добавлена возможность настройки непрерывной интеграции и развертывания в конвейере Azure DevOps из репозитория Github для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1174">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="ec6b9-1175">Добавлен аргумент `--github-pat` для `functionapp devops-build create` для получения личного маркера доступа Github.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1175">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="ec6b9-1176">Добавлен аргумент `--github-repository` для `functionapp devops-build create` для подключения репозитория Github, который содержит исходный код приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1176">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="ec6b9-1177">Исправлена проблема со сбоем `az webapp up --logs` и обновлением .Net Core до версии 2.1 по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1177">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="ec6b9-1178">Удалены ненужные параметры приложения-функции при создании приложения-функции с помощью плана потребления.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1178">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="ec6b9-1179">Внесены изменения в `webapp up`, чтобы строка ASP по умолчанию добавляла номера в конец для создания плана службы приложений на основе параметров SKU.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1179">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="ec6b9-1180">Добавлен параметр `-b` для `webapp up` для запуска приложения в браузере.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1180">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="ec6b9-1181">Внесены изменения в `webapp deployment source config zip` для обработки переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1181">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="ec6b9-1182">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1182">Deployment Manager</span></span>
* <span data-ttu-id="ec6b9-1183">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Создание и администрирование артефактов, которые поддерживают развертывания</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1183">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="ec6b9-1184">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1184">Lab</span></span>
* <span data-ttu-id="ec6b9-1185">Исправлена ошибка, которая приводила к неожиданному завершению работы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1185">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1186">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1186">Network</span></span>
* <span data-ttu-id="ec6b9-1187">Добавлено автоматическое делегирование сервера имен для `dns zone create` в родительском объекте во время создания дочерней зоны.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1187">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-1188">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1188">Resource</span></span>
* <span data-ttu-id="ec6b9-1189">[УСТАРЕЛО] Не рекомендуются к использованию аргументы `--link-id`, `--target-id` и `--filter-string` для `resource link`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1189">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="ec6b9-1190">Используйте вместо них аргументы `--link`, `--target` и `--filter`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1190">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="ec6b9-1191">Исправлена проблема, из-за которой команды `resource link [create|update]` не работали.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1191">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="ec6b9-1192">Исправлена проблема, из-за которой удаление с помощью идентификатора ресурса приводило к сбою или ошибке.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1192">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-1193">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1193">SQL</span></span>
* <span data-ttu-id="ec6b9-1194">Добавлена поддержка пользовательского часового пояса в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1194">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="ec6b9-1195">Внесено изменение, чтобы разрешить использовать имя эластичного пула с `sql db update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1195">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="ec6b9-1196">В команду `sql server [create|update]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1196">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="ec6b9-1197">Добавлена команда `sql server wait`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1197">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-1198">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1198">Storage</span></span>
* <span data-ttu-id="ec6b9-1199">Устранена проблема с двойной кодировкой маркеров SAS в `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1199">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-1200">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1200">VM</span></span>
* <span data-ttu-id="ec6b9-1201">Добавлен флаг `--skip-shutdown` для `vm|vmss stop` для выключения виртуальных машин без завершения работы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1201">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="ec6b9-1202">Добавлен аргумент `--storage-account-type` для `sig image-version create` настройки типа учетной записи профиля публикации.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1202">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="ec6b9-1203">Добавлен аргумент `--target-regions` для `sig image-version create` для указания типов учетных записей хранения, связанных с регионами.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1203">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="ec6b9-1204">9 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1204">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-1205">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1205">Core</span></span>
* <span data-ttu-id="ec6b9-1206">Исправлена проблема, из-за которой для некоторых расширений отображалась версия `Unknown` и ее невозможно было обновить.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1206">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-1207">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1207">ACR</span></span>
* <span data-ttu-id="ec6b9-1208">Добавлена поддержка запуска образа без контекста.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1208">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="ec6b9-1209">AMS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1209">AMS</span></span>
* [УСТАРЕЛО]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="ec6b9-1212">Добавлена поддержка новых параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1212">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="ec6b9-1213">Добавлен новый параметр `--filters` для `ams streaming-locator create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1213">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-1214">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1214">AppService</span></span>
* <span data-ttu-id="ec6b9-1215">В команду `webapp up` добавлена поддержка параметра `--logs`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1215">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="ec6b9-1216">Исправлены ошибки в команде `functionapp devops-build create` при создании файла `azure-pipelines.yml`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1216">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="ec6b9-1217">Улучшена обработка и индикаторы ошибок с `unctionapp devops-build create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1217">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="ec6b9-1218">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--local-git` для команды `devops-build`. Обнаружение и обработка локального репозитория Git являются обязательными для создания конвейеров DevOps в Azure.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1218">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="ec6b9-1219">Добавлена поддержка создания плана функций Linux.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1219">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="ec6b9-1220">Добавлена возможность менять план для приложения-функции с помощью `functionapp update --plan`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1220">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="ec6b9-1221">Добавлена поддержка параметров горизонтального увеличения масштаба плана "Премиум" для Функций Azure.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1221">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="ec6b9-1222">CDN</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1222">CDN</span></span>
* <span data-ttu-id="ec6b9-1223">Добавлена поддержка `Microsoft_Standard` и `Standard_ChinaCdn`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1223">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="ec6b9-1224">Отзывы</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1224">Feedback</span></span>
* <span data-ttu-id="ec6b9-1225">Внесены изменения в `feedback` для отображения метаданных недавно выполненных команд.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1225">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="ec6b9-1226">Внесены изменения в `feedback`. Теперь при регистрации проблемы отображается запрос, в соответствии с которым пользователь должен открыть браузер и воспользоваться шаблоном проблемы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1226">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="ec6b9-1227">Внесены изменения в `feedback`. Теперь текст проблемы выводится при запуске с параметром --verbose.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1227">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-1228">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1228">Monitor</span></span>
* <span data-ttu-id="ec6b9-1229">Исправлена проблема, из-за которой у параметра count было недопустимое значение в `metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1229">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="ec6b9-1230">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1230">Network</span></span>
* <span data-ttu-id="ec6b9-1231">Исправлен формат таблицы, которая не отображалась с помощью `vnet-gateway list-bgp-peer-status`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1231">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="ec6b9-1232">Добавлены команды `list-request-headers` и `list-response-headers` для `application-gateway rewrite-rule`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1232">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="ec6b9-1233">Добавлена команда `list-server-variables` для `application-gateway rewrite-rule condition`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1233">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="ec6b9-1234">Исправлена проблема, из-за которой обновление состояния соединения на порту ExpressRoute вызывало неизвестное исключение атрибута `express-route port update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1234">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="ec6b9-1235">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1235">PrivateDNS</span></span>
* <span data-ttu-id="ec6b9-1236">Добавлена команда `network private-dns` для частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1236">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-1237">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1237">Resource</span></span>
* <span data-ttu-id="ec6b9-1238">Исправлена проблема с `deployment create` и `group deployment create`, из-за которой файл параметров с пустым набором параметров не работал.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1238">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-1239">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1239">Role</span></span>
* <span data-ttu-id="ec6b9-1240">Внесены исправления в `create-for-rbac`. Теперь `--years` обрабатывается правильно.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1240">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="ec6b9-1241">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `role assignment delete`. Теперь появляется запрос при удалении всех назначений в рамках подписки без дополнительных условий.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1241">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-1242">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1242">SQL</span></span>
* <span data-ttu-id="ec6b9-1243">Команда `sql mi [create|update]` обновлена с помощью свойств proxyOverride и publicDataEndpointEnabled.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1243">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-1244">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1244">Storage</span></span>
* <span data-ttu-id="ec6b9-1245">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален результат выполнения `storage blob delete`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1245">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="ec6b9-1246">В команду `storage blob generate-sas` добавлен параметр `--full-uri` для создания полного URI большого двоичного объекта с помощью SAS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1246">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="ec6b9-1247">В команду `storage file copy start` добавлен параметр `--file-snapshot` для копирования файла из моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1247">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="ec6b9-1248">Внесены изменения в `storage blob copy cancel`. Теперь вместо исключения для NoPendingCopyOperation отображается только сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1248">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="ec6b9-1249">26 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1249">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="ec6b9-1250">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1250">Core</span></span>
* <span data-ttu-id="ec6b9-1251">Устранены проблемы с несовместимостью расширений для разработки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1251">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="ec6b9-1252">Функция обработки ошибок теперь указывает клиентам на страницу проблем.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1252">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="ec6b9-1253">Cloud</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1253">Cloud</span></span>
* <span data-ttu-id="ec6b9-1254">Исправлена ошибка с сообщением о не найденной подписке в `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1254">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-1255">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1255">ACR</span></span>
* <span data-ttu-id="ec6b9-1256">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1256">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="ec6b9-1257">Добавлено `--auth-mode` в команды `acr build`, `acr run`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1257">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="ec6b9-1258">Добавлена команда acr task credential для управления учетными данными для задачи.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1258">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="ec6b9-1259">Добавлено --no-wait в команду `acr build`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1259">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-1260">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1260">AppService</span></span>
* <span data-ttu-id="ec6b9-1261">Исправлена ошибка с `webapp up`, из-за которой нельзя было правильно выполнить запуск из пустого каталога или скрипта неизвестного кода.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1261">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="ec6b9-1262">Исправлена ошибка, из-за которой не работали слоты для `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1262">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="ec6b9-1263">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1263">BOT Service</span></span>
* <span data-ttu-id="ec6b9-1264">Добавлено `bot prepare-deploy` для подготовки к развертыванию ботов с помощью `webapp`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1264">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="ec6b9-1265">Изменено `bot create --kind registration` для отображения пароля, если пароль не указан.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1265">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="ec6b9-1266">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--endpoint` в `bot create --kind registration` на пустую строку (по умолчанию) вместо запрашиваемой.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1266">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="ec6b9-1267">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1267">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="ec6b9-1268">CDN</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1268">CDN</span></span>
* <span data-ttu-id="ec6b9-1269">Добавлена поддержка параметра `--no-wait` в команде `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1269">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="ec6b9-1270">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено поведение кэширования строки запроса `cdn endpoint create` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1270">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="ec6b9-1271">IgnoreQueryString больше не используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1271">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="ec6b9-1272">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1272">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ec6b9-1273">Сosmos DB</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1273">Cosmosdb</span></span>
* <span data-ttu-id="ec6b9-1274">Добавлена поддержка `--enable-multiple-write-locations` для обновления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1274">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="ec6b9-1275">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1275">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="ec6b9-1276">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1276">Interactive</span></span>
* <span data-ttu-id="ec6b9-1277">Исправлена несовместимость с интерактивным расширением, установленным с помощью azdev.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1277">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-1278">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1278">Monitor</span></span>
* <span data-ttu-id="ec6b9-1279">Внесено изменение, разрешающее использовать значение измерения `*` для `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1279">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1280">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1280">Network</span></span>
* <span data-ttu-id="ec6b9-1281">Добавлена группа команд `rewrite-rule` для `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1281">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="ec6b9-1282">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1282">Profile</span></span>
* <span data-ttu-id="ec6b9-1283">Включена поддержка учетной записи уровня клиентов для управляемого удостоверения службы для `login`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1283">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="ec6b9-1284">Postgres</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1284">Postgres</span></span> 
* <span data-ttu-id="ec6b9-1285">Добавлены команды postgresql `replica` и команда `restart server`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1285">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="ec6b9-1286">Внесены изменения для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1286">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-1287">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1287">Resource</span></span>
* <span data-ttu-id="ec6b9-1288">Улучшены табличные выходные данные для `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1288">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="ec6b9-1289">Исправлена проблема с `deployment [create|validate]`, из-за которой secureObject типа не распознавался.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1289">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="ec6b9-1290">График</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1290">Graph</span></span>
* <span data-ttu-id="ec6b9-1291">Добавлена поддержка параметра `--end-date` в команде `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1291">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="ec6b9-1292">Добавлена поддержка разрешений для `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1292">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="ec6b9-1293">Исправлена проблема с `ad app permission list`, из-за которой отсутствовали разрешения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1293">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="ec6b9-1294">Изменено `ad sp delete` для пропуска удаления назначения роли, если текущая учетная запись не содержит подписок.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1294">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="ec6b9-1295">Изменено `ad app create` для использования `--identifier-uris` пустого списка (по умолчанию), если список не указан.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1295">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-1296">носителей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1296">storage</span></span>
* <span data-ttu-id="ec6b9-1297">Добавлено `--snapshot` для `storage file download-batch` для скачивания из моментального снимка общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1297">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="ec6b9-1298">Изменен индикатор выполнения `storage blob [download-batch|upload-batch]`, чтобы обобщить сведения и указать текущий большой двоичный объект.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1298">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="ec6b9-1299">Исправлена проблема с `storage account update` при обновлении параметров шифрования.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1299">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="ec6b9-1300">Исправлена проблема со сбоем `storage blob show` при использовании OAuth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1300">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-1301">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1301">VM</span></span>
* <span data-ttu-id="ec6b9-1302">Добавлена команда `image update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1302">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="ec6b9-1303">12 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1303">March 12, 2019</span></span>

<span data-ttu-id="ec6b9-1304">Версия 2.0.60</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1304">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-1305">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1305">Core</span></span>

* <span data-ttu-id="ec6b9-1306">Исправлена недопустимая ошибка в `cloud set` о том, что подписка не найдена.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1306">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-1307">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1307">ACR</span></span>

* <span data-ttu-id="ec6b9-1308">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1308">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-1309">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1309">ACS</span></span>

* <span data-ttu-id="ec6b9-1310">Внесены изменения, в соответствии с которыми параметр `--listen-address` для `aks browse` игнорируется, если он не поддерживается kubectl.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1310">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="ec6b9-1311">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1311">AppService</span></span>

* <span data-ttu-id="ec6b9-1312">Добавлено `[webapp|functionapp] deployment list-publishing-credentials` для получения URL-адреса публикации Kudu и связанных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1312">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="ec6b9-1313">Удалена ошибочная инструкция печати для `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1313">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="ec6b9-1314">Исправлено `functionapp` для настройки правильного образа для среды выполнения в планах службы приложений Linux.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1314">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="ec6b9-1315">Удален тег предварительной версии для `webapp up` и добавлены усовершенствования в команду.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1315">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="ec6b9-1316">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1316">Botservice</span></span>

* <span data-ttu-id="ec6b9-1317">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1317">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="ec6b9-1318">Добавлено `Microsoft-BotFramework-AppId` и `Microsoft-BotFramework-AppPassword` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1318">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="ec6b9-1319">Удалены одинарные кавычки из выходных данных команды `bot publish` в конце `bot create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1319">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="ec6b9-1320">Изменено `bot publish` для включения поддержки асинхронных операций.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1320">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="ec6b9-1321">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1321">Container</span></span>

* <span data-ttu-id="ec6b9-1322">Добавлен аргумент `--no-wait` для команды `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1322">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="ec6b9-1323">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1323">EventHub</span></span>

* <span data-ttu-id="ec6b9-1324">Добавлен флаг `--skip-empty-archives` для `eventhub create|update` для включения поддержки пустых архивов при записи.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1324">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="ec6b9-1325">Поиск</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1325">Find</span></span>

* <span data-ttu-id="ec6b9-1326">Основные обновления функций</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1326">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="ec6b9-1327">HDInsight</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1327">HDInsight</span></span>

* <span data-ttu-id="ec6b9-1328">Добавлен параметр `--storage-account-managed-identity` для `hdinsight create` для включения поддержки MSI ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1328">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1329">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1329">Network</span></span>

* <span data-ttu-id="ec6b9-1330">Исправлена проблема с `vpn-connection update`, когда обновление VPN-подключения между шлюзами в разных подписках завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1330">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="ec6b9-1331">Rdbms</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1331">Rdbms</span></span>

* <span data-ttu-id="ec6b9-1332">Незначительные исправления для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1332">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-1333">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1333">Role</span></span>

* <span data-ttu-id="ec6b9-1334">Исправлено `role definition update` для использования идентификатора для правильного разрешения определения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1334">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="ec6b9-1335">Изменено `ad app credential reset` для исключения предположения о том, что субъект-служба приложения всегда существует.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1335">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ec6b9-1336">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1336">Service Fabric</span></span>

* <span data-ttu-id="ec6b9-1337">Исправлена проблема с `sf cluster list` и невозможностью итерации.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1337">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="ec6b9-1338">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1338">February 26, 2019</span></span>

<span data-ttu-id="ec6b9-1339">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1339">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-1340">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1340">Core</span></span>

* <span data-ttu-id="ec6b9-1341">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1341">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-1342">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1342">ACR</span></span>

* <span data-ttu-id="ec6b9-1343">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1343">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="ec6b9-1344">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1344">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-1345">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1345">ACS</span></span>

* <span data-ttu-id="ec6b9-1346">Добавлен параметр `--listen-address` для команды `aks port-forward`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1346">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-1347">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1347">AppService</span></span>

* <span data-ttu-id="ec6b9-1348">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1348">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="ec6b9-1349">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1349">Batch</span></span>
* <span data-ttu-id="ec6b9-1350">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1350">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="ec6b9-1351">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1351">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="ec6b9-1352">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1352">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="ec6b9-1353">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1353">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="ec6b9-1354">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1354">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="ec6b9-1355">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1355">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ec6b9-1356">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1356">CosmosDB</span></span>

* <span data-ttu-id="ec6b9-1357">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1357">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="ec6b9-1358">Kusto</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1358">Kusto</span></span>

* <span data-ttu-id="ec6b9-1359">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1359">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1360">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1360">Network</span></span>

* <span data-ttu-id="ec6b9-1361">Добавлен аргумент `--express-route-gateway-bypass` для команды `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1361">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="ec6b9-1362">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1362">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="ec6b9-1363">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1363">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="ec6b9-1364">Добавлен аргумент `--legacy-mode` в команду `express-route peering [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1364">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="ec6b9-1365">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1365">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="ec6b9-1366">Добавлен аргумент `--gateway-default-site` для команды `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1366">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="ec6b9-1367">Добавлены команды `ipsec-policy` для `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1367">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-1368">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1368">Resource</span></span>

* <span data-ttu-id="ec6b9-1369">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1369">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="ec6b9-1370">Добавлена поддержка файла параметров на основе URI для `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1370">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="ec6b9-1371">Добавлена поддержка определений и параметров на основе URI для `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1371">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="ec6b9-1372">Исправлена обработка параметров и правил для `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1372">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="ec6b9-1373">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1373">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-1374">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1374">Role</span></span>

* <span data-ttu-id="ec6b9-1375">Добавлена поддержка ролей приложений для `ad app [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1375">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-1376">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1376">VM</span></span>

* <span data-ttu-id="ec6b9-1377">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1377">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="ec6b9-1378">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1378">February 12, 2019</span></span>

<span data-ttu-id="ec6b9-1379">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1379">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-1380">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1380">Core</span></span>

* <span data-ttu-id="ec6b9-1381">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1381">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="ec6b9-1382">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1382">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-1383">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1383">ACR</span></span>
* <span data-ttu-id="ec6b9-1384">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1384">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="ec6b9-1385">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1385">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-1386">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1386">ACS</span></span>
* <span data-ttu-id="ec6b9-1387">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1387">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="ec6b9-1388">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1388">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="ec6b9-1389">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1389">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="ec6b9-1390">AMS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1390">AMS</span></span>
* <span data-ttu-id="ec6b9-1391">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1391">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="ec6b9-1392">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1392">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-1393">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1393">Appservice</span></span>
* <span data-ttu-id="ec6b9-1394">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1394">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="ec6b9-1395">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1395">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="ec6b9-1396">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1396">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="ec6b9-1397">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1397">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="ec6b9-1398">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1398">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="ec6b9-1399">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1399">Botservice</span></span>
* <span data-ttu-id="ec6b9-1400">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1400">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="ec6b9-1401">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1401">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="ec6b9-1402">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1402">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="ec6b9-1403">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1403">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="ec6b9-1404">[УСТАРЕЛО] Аргумент `--proj-name` не рекомендуется к использованию. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1404">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="ec6b9-1405">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1405">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="ec6b9-1406">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1406">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="ec6b9-1407">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1407">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="ec6b9-1408">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1408">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="ec6b9-1409">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1409">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="ec6b9-1410">Key Vault</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1410">Key Vault</span></span>
* <span data-ttu-id="ec6b9-1411">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1411">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-1412">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1412">Monitor</span></span>
* <span data-ttu-id="ec6b9-1413">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1413">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1414">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1414">Network</span></span>
* <span data-ttu-id="ec6b9-1415">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1415">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="ec6b9-1416">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1416">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="ec6b9-1417">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1417">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="ec6b9-1418">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1418">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="ec6b9-1419">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1419">Policy Insights</span></span>
* <span data-ttu-id="ec6b9-1420">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1420">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="ec6b9-1421">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1421">RDBMS</span></span>
* <span data-ttu-id="ec6b9-1422">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1422">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="ec6b9-1423">Redis</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1423">Redis</span></span>
* <span data-ttu-id="ec6b9-1424">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1424">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="ec6b9-1425">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1425">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="ec6b9-1426">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1426">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="ec6b9-1427">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1427">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="ec6b9-1428">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1428">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="ec6b9-1429">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1429">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="ec6b9-1430">[УСТАРЕЛО] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1430">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-1431">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1431">Role</span></span>
* <span data-ttu-id="ec6b9-1432">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1432">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="ec6b9-1433">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1433">SQL VM</span></span>
* <span data-ttu-id="ec6b9-1434">[УСТАРЕЛО] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1434">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-1435">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1435">VM</span></span>
* <span data-ttu-id="ec6b9-1436">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1436">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="ec6b9-1437">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1437">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="ec6b9-1438">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1438">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="ec6b9-1439">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1439">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="ec6b9-1440">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1440">January 31, 2019</span></span>

<span data-ttu-id="ec6b9-1441">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1441">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-1442">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1442">Core</span></span>

* <span data-ttu-id="ec6b9-1443">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1443">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="ec6b9-1444">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1444">January 28, 2019</span></span>

<span data-ttu-id="ec6b9-1445">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1445">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-1446">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1446">ACR</span></span>
* <span data-ttu-id="ec6b9-1447">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1447">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-1448">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1448">ACS</span></span>
* <span data-ttu-id="ec6b9-1449">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1449">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="ec6b9-1450">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1450">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="ec6b9-1451">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1451">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="ec6b9-1452">AMS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1452">AMS</span></span>
* <span data-ttu-id="ec6b9-1453">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1453">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="ec6b9-1454">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1454">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-1455">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1455">Appservice</span></span>
* <span data-ttu-id="ec6b9-1456">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1456">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="ec6b9-1457">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1457">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="ec6b9-1458">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1458">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="ec6b9-1459">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1459">Container</span></span>
* <span data-ttu-id="ec6b9-1460">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1460">Added `container start` command</span></span>
* <span data-ttu-id="ec6b9-1461">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1461">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="ec6b9-1462">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1462">EventGrid</span></span>
* <span data-ttu-id="ec6b9-1463">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1463">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="ec6b9-1464">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1464">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="ec6b9-1465">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1465">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="ec6b9-1466">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1466">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="ec6b9-1467">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1467">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="ec6b9-1468">HDInsight</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1468">HDInsight</span></span>
* <span data-ttu-id="ec6b9-1469">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1469">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="ec6b9-1470">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1470">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="ec6b9-1471">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1471">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="ec6b9-1472">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1472">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="ec6b9-1473">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1473">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="ec6b9-1474">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1474">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="ec6b9-1475">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1475">IoT</span></span>
* <span data-ttu-id="ec6b9-1476">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1476">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="ec6b9-1477">Kusto</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1477">Kusto</span></span>
* <span data-ttu-id="ec6b9-1478">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1478">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-1479">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1479">Monitor</span></span>
* <span data-ttu-id="ec6b9-1480">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1480">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="ec6b9-1481">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1481">Profile</span></span>
* <span data-ttu-id="ec6b9-1482">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1482">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1483">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1483">Network</span></span>
* <span data-ttu-id="ec6b9-1484">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1484">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="ec6b9-1485">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1485">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-1486">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1486">Resource</span></span>
* <span data-ttu-id="ec6b9-1487">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1487">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="ec6b9-1488">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1488">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="ec6b9-1489">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1489">SQL Virtual Machine</span></span>
* <span data-ttu-id="ec6b9-1490">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1490">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-1491">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1491">Storage</span></span>
* <span data-ttu-id="ec6b9-1492">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1492">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="ec6b9-1493">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1493">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-1494">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1494">VM</span></span>
* <span data-ttu-id="ec6b9-1495">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1495">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="ec6b9-1496">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1496">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="ec6b9-1497">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1497">January 15, 2019</span></span>

<span data-ttu-id="ec6b9-1498">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1498">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-1499">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1499">ACR</span></span>
* <span data-ttu-id="ec6b9-1500">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1500">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="ec6b9-1501">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1501">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="ec6b9-1502">[УСТАРЕЛО] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1502">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="ec6b9-1503">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1503">ACS</span></span>
* <span data-ttu-id="ec6b9-1504">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1504">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-1505">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1505">Appservice</span></span>
* <span data-ttu-id="ec6b9-1506">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1506">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="ec6b9-1507">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1507">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="ec6b9-1508">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1508">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="ec6b9-1509">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1509">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="ec6b9-1510">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1510">Botservice</span></span>
* <span data-ttu-id="ec6b9-1511">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1511">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="ec6b9-1512">Configure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1512">Configure</span></span>
* <span data-ttu-id="ec6b9-1513">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1513">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ec6b9-1514">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1514">CosmosDB</span></span>
* <span data-ttu-id="ec6b9-1515">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1515">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="ec6b9-1516">HDInsight</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1516">HDInsight</span></span>
* <span data-ttu-id="ec6b9-1517">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1517">Added commands for managing applications</span></span>
* <span data-ttu-id="ec6b9-1518">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1518">Added commands for managing script actions</span></span>
* <span data-ttu-id="ec6b9-1519">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1519">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="ec6b9-1520">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1520">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="ec6b9-1521">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1521">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1522">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1522">Network</span></span>
* <span data-ttu-id="ec6b9-1523">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1523">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="ec6b9-1524">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1524">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="ec6b9-1525">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1525">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="ec6b9-1526">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1526">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-1527">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1527">Role</span></span>
* <span data-ttu-id="ec6b9-1528">[УСТАРЕЛО] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1528">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="ec6b9-1529">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1529">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="ec6b9-1530">Безопасность</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1530">Security</span></span>
* <span data-ttu-id="ec6b9-1531">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1531">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-1532">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1532">Storage</span></span>
* <span data-ttu-id="ec6b9-1533">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1533">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="ec6b9-1534">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1534">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="ec6b9-1535">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1535">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="ec6b9-1536">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1536">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="ec6b9-1537">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1537">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-1538">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1538">VM</span></span>
* <span data-ttu-id="ec6b9-1539">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1539">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="ec6b9-1540">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1540">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="ec6b9-1541">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1541">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="ec6b9-1542">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1542">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="ec6b9-1543">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1543">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="ec6b9-1544">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1544">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="ec6b9-1545">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1545">December 20, 2018</span></span>

<span data-ttu-id="ec6b9-1546">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1546">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="ec6b9-1547">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1547">Appservice</span></span>
* <span data-ttu-id="ec6b9-1548">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1548">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="ec6b9-1549">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1549">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="ec6b9-1550">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1550">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="ec6b9-1551">IoT Central</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1551">IoTCentral</span></span>
* <span data-ttu-id="ec6b9-1552">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1552">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-1553">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1553">Role</span></span>
* <span data-ttu-id="ec6b9-1554">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1554">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-1555">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1555">SQL</span></span>
* <span data-ttu-id="ec6b9-1556">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1556">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-1557">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1557">VM</span></span>
* <span data-ttu-id="ec6b9-1558">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1558">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="ec6b9-1559">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1559">December 18, 2018</span></span>

<span data-ttu-id="ec6b9-1560">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1560">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="ec6b9-1561">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1561">ACR</span></span>
* <span data-ttu-id="ec6b9-1562">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1562">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="ec6b9-1563">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1563">Condensed the table layout for task list</span></span>
* <span data-ttu-id="ec6b9-1564">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1564">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-1565">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1565">ACS</span></span>
* <span data-ttu-id="ec6b9-1566">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1566">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="ec6b9-1567">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1567">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="ec6b9-1568">[УСТАРЕЛО] Команды `az acs` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1568">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="ec6b9-1569">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1569">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="ec6b9-1570">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1570">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="ec6b9-1571">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1571">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-1572">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1572">Appservice</span></span>
* <span data-ttu-id="ec6b9-1573">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1573">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="ec6b9-1574">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1574">Botservice</span></span>
* <span data-ttu-id="ec6b9-1575">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1575">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="ec6b9-1576">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1576">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="ec6b9-1577">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1577">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="ec6b9-1578">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1578">Reduced Kudu network calls</span></span>
* <span data-ttu-id="ec6b9-1579">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1579">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="ec6b9-1580">Потребление</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1580">Consumption</span></span>
* <span data-ttu-id="ec6b9-1581">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1581">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ec6b9-1582">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1582">CosmosDB</span></span>
* <span data-ttu-id="ec6b9-1583">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1583">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="ec6b9-1584">Maps</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1584">Maps</span></span>
* <span data-ttu-id="ec6b9-1585">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1585">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1586">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1586">Network</span></span>
* <span data-ttu-id="ec6b9-1587">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1587">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="ec6b9-1588">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1588">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-1589">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1589">Resource</span></span>
* <span data-ttu-id="ec6b9-1590">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1590">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="ec6b9-1591">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1591">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-1592">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1592">Storage</span></span>
*  <span data-ttu-id="ec6b9-1593">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1593">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-1594">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1594">VM</span></span>
* <span data-ttu-id="ec6b9-1595">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1595">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="ec6b9-1596">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1596">December 4, 2018</span></span>

<span data-ttu-id="ec6b9-1597">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1597">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="ec6b9-1598">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1598">Core</span></span>
* <span data-ttu-id="ec6b9-1599">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1599">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="ec6b9-1600">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1600">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-1601">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1601">Appservice</span></span>
* <span data-ttu-id="ec6b9-1602">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1602">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="ec6b9-1603">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1603">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1604">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1604">Network</span></span>
* <span data-ttu-id="ec6b9-1605">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1605">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-1606">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1606">Role</span></span>
* <span data-ttu-id="ec6b9-1607">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1607">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="ec6b9-1608">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1608">VM</span></span>
* <span data-ttu-id="ec6b9-1609">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1609">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="ec6b9-1610">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1610">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="ec6b9-1611">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1611">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="ec6b9-1612">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1612">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="ec6b9-1613">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1613">November 20, 2018</span></span>

<span data-ttu-id="ec6b9-1614">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1614">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="ec6b9-1615">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1615">Core</span></span>
* <span data-ttu-id="ec6b9-1616">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1616">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-1617">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1617">ACR</span></span>
* <span data-ttu-id="ec6b9-1618">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1618">Added context token to task step</span></span>
* <span data-ttu-id="ec6b9-1619">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1619">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="ec6b9-1620">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1620">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-1621">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1621">Appservice</span></span>
* <span data-ttu-id="ec6b9-1622">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1622">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="ec6b9-1623">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1623">Updated the default `node_version`.</span></span> <span data-ttu-id="ec6b9-1624">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1624">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="ec6b9-1625">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1625">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="ec6b9-1626">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1626">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="ec6b9-1627">IotCentral</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1627">IotCentral</span></span>
* <span data-ttu-id="ec6b9-1628">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1628">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="ec6b9-1629">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1629">KeyVault</span></span>
* <span data-ttu-id="ec6b9-1630">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1630">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1631">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1631">Network</span></span>
* <span data-ttu-id="ec6b9-1632">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1632">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="ec6b9-1633">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1633">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="ec6b9-1634">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1634">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="ec6b9-1635">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1635">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="ec6b9-1636">Rdbms</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1636">Rdbms</span></span>
* <span data-ttu-id="ec6b9-1637">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1637">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="ec6b9-1638">RBAC:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1638">Rbac</span></span>
* <span data-ttu-id="ec6b9-1639">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1639">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="ec6b9-1640">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1640">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="ec6b9-1641">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1641">Storage</span></span>
* <span data-ttu-id="ec6b9-1642">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1642">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="ec6b9-1643">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1643">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="ec6b9-1644">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1644">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="ec6b9-1645">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1645">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-1646">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1646">VM</span></span>
* <span data-ttu-id="ec6b9-1647">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1647">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="ec6b9-1648">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1648">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="ec6b9-1649">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1649">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="ec6b9-1650">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1650">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="ec6b9-1651">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1651">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="ec6b9-1652">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1652">Added `snapshot wait` command</span></span>
* <span data-ttu-id="ec6b9-1653">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1653">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="ec6b9-1654">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1654">November 6, 2018</span></span>

<span data-ttu-id="ec6b9-1655">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1655">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-1656">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1656">Core</span></span>
* <span data-ttu-id="ec6b9-1657">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1657">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-1658">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1658">ACR</span></span>
* <span data-ttu-id="ec6b9-1659">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1659">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="ec6b9-1660">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1660">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-1661">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1661">ACS</span></span>
* <span data-ttu-id="ec6b9-1662">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1662">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="ec6b9-1663">Помощник</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1663">Advisor</span></span>
* <span data-ttu-id="ec6b9-1664">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1664">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="ec6b9-1665">AMS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1665">AMS</span></span>
* <span data-ttu-id="ec6b9-1666">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1666">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="ec6b9-1667">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1667">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="ec6b9-1668">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1668">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="ec6b9-1669">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1669">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="ec6b9-1670">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1670">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="ec6b9-1671">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1671">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="ec6b9-1672">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1672">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="ec6b9-1673">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1673">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="ec6b9-1674">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1674">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="ec6b9-1675">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1675">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="ec6b9-1676">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1676">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="ec6b9-1677">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1677">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="ec6b9-1678">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1678">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="ec6b9-1679">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1679">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="ec6b9-1680">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1680">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="ec6b9-1681">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1681">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="ec6b9-1682">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1682">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-1683">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1683">AppService</span></span>
* <span data-ttu-id="ec6b9-1684">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1684">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="ec6b9-1685">Configure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1685">Configure</span></span>
* <span data-ttu-id="ec6b9-1686">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1686">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="ec6b9-1687">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1687">Container</span></span>
* <span data-ttu-id="ec6b9-1688">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1688">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="ec6b9-1689">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1689">EventHub</span></span>
* <span data-ttu-id="ec6b9-1690">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1690">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="ec6b9-1691">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1691">Interactive</span></span>
* <span data-ttu-id="ec6b9-1692">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1692">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-1693">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1693">Monitor</span></span>
* <span data-ttu-id="ec6b9-1694">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1694">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1695">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1695">Network</span></span>
* <span data-ttu-id="ec6b9-1696">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1696">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="ec6b9-1697">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1697">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="ec6b9-1698">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1698">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="ec6b9-1699">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1699">Profile</span></span>
* <span data-ttu-id="ec6b9-1700">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1700">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="ec6b9-1701">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1701">RDBMS</span></span>
* <span data-ttu-id="ec6b9-1702">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1702">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-1703">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1703">Resource</span></span>
* <span data-ttu-id="ec6b9-1704">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1704">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-1705">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1705">Role</span></span>
* <span data-ttu-id="ec6b9-1706">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1706">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="ec6b9-1707">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1707">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="ec6b9-1708">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1708">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-1709">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1709">Storage</span></span>
* <span data-ttu-id="ec6b9-1710">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1710">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-1711">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1711">VM</span></span>
* <span data-ttu-id="ec6b9-1712">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1712">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="ec6b9-1713">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1713">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="ec6b9-1714">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1714">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="ec6b9-1715">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1715">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="ec6b9-1716">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1716">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="ec6b9-1717">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1717">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="ec6b9-1718">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1718">October 23, 2018</span></span>

<span data-ttu-id="ec6b9-1719">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1719">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-1720">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1720">Core</span></span>
* <span data-ttu-id="ec6b9-1721">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1721">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="ec6b9-1722">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1722">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-1723">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1723">ACR</span></span>
* <span data-ttu-id="ec6b9-1724">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1724">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="ec6b9-1725">CDN</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1725">CDN</span></span>
* <span data-ttu-id="ec6b9-1726">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1726">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="ec6b9-1727">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1727">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="ec6b9-1728">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1728">Container</span></span>
* <span data-ttu-id="ec6b9-1729">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1729">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="ec6b9-1730">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1730">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="ec6b9-1731">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1731">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="ec6b9-1732">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1732">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="ec6b9-1733">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1733">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="ec6b9-1734">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1734">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="ec6b9-1735">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1735">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ec6b9-1736">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1736">CosmosDB</span></span>
* <span data-ttu-id="ec6b9-1737">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1737">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="ec6b9-1738">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1738">Interactive</span></span>
* <span data-ttu-id="ec6b9-1739">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1739">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="ec6b9-1740">IoT Central</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1740">IoT Central</span></span>
* <span data-ttu-id="ec6b9-1741">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1741">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="ec6b9-1742">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1742">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-1743">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1743">Monitor</span></span>
* <span data-ttu-id="ec6b9-1744">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1744">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="ec6b9-1745">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1745">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="ec6b9-1746">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1746">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="ec6b9-1747">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1747">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="ec6b9-1748">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1748">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="ec6b9-1749">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1749">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="ec6b9-1750">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1750">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="ec6b9-1751">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1751">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="ec6b9-1752">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1752">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="ec6b9-1753">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1753">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1754">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1754">Network</span></span>
* <span data-ttu-id="ec6b9-1755">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1755">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="ec6b9-1756">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1756">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="ec6b9-1757">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1757">ServiceBus</span></span>
* <span data-ttu-id="ec6b9-1758">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1758">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-1759">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1759">SQL</span></span>
* <span data-ttu-id="ec6b9-1760">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1760">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-1761">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1761">Storage</span></span>
* <span data-ttu-id="ec6b9-1762">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1762">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="ec6b9-1763">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1763">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-1764">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1764">VM</span></span>
* <span data-ttu-id="ec6b9-1765">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1765">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="ec6b9-1766">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1766">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="ec6b9-1767">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1767">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="ec6b9-1768">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1768">October 16, 2018</span></span>

<span data-ttu-id="ec6b9-1769">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1769">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-1770">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1770">VM</span></span>
* <span data-ttu-id="ec6b9-1771">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1771">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="ec6b9-1772">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1772">October 9, 2018</span></span>

<span data-ttu-id="ec6b9-1773">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1773">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-1774">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1774">Core</span></span>
* <span data-ttu-id="ec6b9-1775">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1775">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-1776">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1776">ACR</span></span>
* <span data-ttu-id="ec6b9-1777">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1777">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-1778">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1778">ACS</span></span>
* <span data-ttu-id="ec6b9-1779">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1779">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="ec6b9-1780">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1780">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="ec6b9-1781">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1781">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="ec6b9-1782">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1782">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="ec6b9-1783">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1783">Container</span></span>
* <span data-ttu-id="ec6b9-1784">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1784">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="ec6b9-1785">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1785">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="ec6b9-1786">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1786">Event Hub</span></span>
* <span data-ttu-id="ec6b9-1787">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1787">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="ec6b9-1788">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1788">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="ec6b9-1789">Модули</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1789">Extensions</span></span>
* <span data-ttu-id="ec6b9-1790">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1790">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="ec6b9-1791">HDInsight</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1791">HDInsight</span></span>
* <span data-ttu-id="ec6b9-1792">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1792">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="ec6b9-1793">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1793">IoT</span></span>
* <span data-ttu-id="ec6b9-1794">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1794">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="ec6b9-1795">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1795">KeyVault</span></span>
* <span data-ttu-id="ec6b9-1796">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1796">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1797">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1797">Network</span></span>
* <span data-ttu-id="ec6b9-1798">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1798">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="ec6b9-1799">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1799">See #6052</span></span>
* <span data-ttu-id="ec6b9-1800">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1800">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="ec6b9-1801">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1801">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="ec6b9-1802">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1802">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="ec6b9-1803">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1803">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="ec6b9-1804">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1804">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="ec6b9-1805">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1805">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-1806">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1806">Role</span></span>
* <span data-ttu-id="ec6b9-1807">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1807">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="ec6b9-1808">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1808">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="ec6b9-1809">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1809">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="ec6b9-1810">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1810">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="ec6b9-1811">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1811">Service Bus</span></span>
* <span data-ttu-id="ec6b9-1812">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1812">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-1813">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1813">VM</span></span>
* <span data-ttu-id="ec6b9-1814">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1814">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="ec6b9-1815">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1815">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="ec6b9-1816">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1816">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="ec6b9-1817">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1817">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="ec6b9-1818">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1818">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="ec6b9-1819">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1819">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="ec6b9-1820">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1820">September 21, 2018</span></span>

<span data-ttu-id="ec6b9-1821">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1821">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-1822">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1822">ACR</span></span>
* <span data-ttu-id="ec6b9-1823">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1823">Added ACR Task commands</span></span>
* <span data-ttu-id="ec6b9-1824">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1824">Added quick run command</span></span>
* <span data-ttu-id="ec6b9-1825">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1825">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="ec6b9-1826">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1826">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="ec6b9-1827">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1827">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="ec6b9-1828">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1828">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-1829">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1829">ACS</span></span>
* <span data-ttu-id="ec6b9-1830">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1830">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="ec6b9-1831">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1831">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-1832">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1832">AppService</span></span>

* <span data-ttu-id="ec6b9-1833">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1833">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="ec6b9-1834">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1834">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="ec6b9-1835">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1835">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="ec6b9-1836">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1836">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="ec6b9-1837">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1837">Batch</span></span>
* <span data-ttu-id="ec6b9-1838">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1838">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="ec6b9-1839">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1839">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="ec6b9-1840">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1840">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="ec6b9-1841">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1841">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ec6b9-1842">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1842">Batch AI</span></span> 
* <span data-ttu-id="ec6b9-1843">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1843">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ec6b9-1844">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1844">Cognitive Services</span></span>
* <span data-ttu-id="ec6b9-1845">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1845">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="ec6b9-1846">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1846">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="ec6b9-1847">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1847">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="ec6b9-1848">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1848">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="ec6b9-1849">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1849">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="ec6b9-1850">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1850">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="ec6b9-1851">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1851">Container</span></span>
* <span data-ttu-id="ec6b9-1852">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1852">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="ec6b9-1853">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1853">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="ec6b9-1854">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1854">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="ec6b9-1855">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1855">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="ec6b9-1856">Data Lake</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1856">Datalake</span></span>
* <span data-ttu-id="ec6b9-1857">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1857">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="ec6b9-1858">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1858">Interactive Shell</span></span>
* <span data-ttu-id="ec6b9-1859">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1859">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="ec6b9-1860">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1860">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="ec6b9-1861">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1861">IoT</span></span>
* <span data-ttu-id="ec6b9-1862">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1862">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="ec6b9-1863">Key Vault</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1863">Key Vault</span></span>
* <span data-ttu-id="ec6b9-1864">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1864">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1865">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1865">Network</span></span>
* <span data-ttu-id="ec6b9-1866">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1866">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="ec6b9-1867">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1867">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="ec6b9-1868">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1868">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="ec6b9-1869">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1869">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="ec6b9-1870">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1870">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="ec6b9-1871">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1871">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="ec6b9-1872">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1872">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="ec6b9-1873">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1873">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="ec6b9-1874">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1874">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="ec6b9-1875">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1875">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="ec6b9-1876">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1876">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="ec6b9-1877">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1877">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="ec6b9-1878">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1878">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="ec6b9-1879">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1879">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="ec6b9-1880">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1880">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="ec6b9-1881">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1881">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="ec6b9-1882">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1882">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="ec6b9-1883">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1883">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="ec6b9-1884">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1884">RDBMS</span></span>
* <span data-ttu-id="ec6b9-1885">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1885">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="ec6b9-1886">резервирование.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1886">Reservation</span></span>
* <span data-ttu-id="ec6b9-1887">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1887">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="ec6b9-1888">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1888">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="ec6b9-1889">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1889">Manage App</span></span>
* <span data-ttu-id="ec6b9-1890">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1890">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="ec6b9-1891">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1891">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-1892">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1892">Role</span></span>
* <span data-ttu-id="ec6b9-1893">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1893">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="ec6b9-1894">SignalR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1894">SignalR</span></span>
* <span data-ttu-id="ec6b9-1895">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1895">First release</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-1896">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1896">Storage</span></span>
* <span data-ttu-id="ec6b9-1897">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1897">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="ec6b9-1898">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1898">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-1899">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1899">VM</span></span>
* <span data-ttu-id="ec6b9-1900">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1900">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="ec6b9-1901">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1901">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="ec6b9-1902">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1902">August 28, 2018</span></span>

<span data-ttu-id="ec6b9-1903">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1903">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-1904">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1904">Core</span></span>

* <span data-ttu-id="ec6b9-1905">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1905">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="ec6b9-1906">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1906">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-1907">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1907">ACR</span></span>

* <span data-ttu-id="ec6b9-1908">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1908">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="ec6b9-1909">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1909">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-1910">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1910">ACS</span></span>

* <span data-ttu-id="ec6b9-1911">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1911">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="ec6b9-1912">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1912">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-1913">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1913">AppService</span></span>

* <span data-ttu-id="ec6b9-1914">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1914">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="ec6b9-1915">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1915">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="ec6b9-1916">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1916">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="ec6b9-1917">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1917">Backup</span></span>

* <span data-ttu-id="ec6b9-1918">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1918">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="ec6b9-1919">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1919">Bot Service</span></span>

* <span data-ttu-id="ec6b9-1920">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1920">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ec6b9-1921">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1921">Cognitive Services</span></span>

* <span data-ttu-id="ec6b9-1922">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1922">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="ec6b9-1923">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1923">IoT</span></span>

* <span data-ttu-id="ec6b9-1924">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1924">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-1925">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1925">Monitor</span></span>

* <span data-ttu-id="ec6b9-1926">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1926">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="ec6b9-1927">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1927">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1928">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1928">Network</span></span>

* <span data-ttu-id="ec6b9-1929">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1929">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-1930">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1930">Resource</span></span>

* <span data-ttu-id="ec6b9-1931">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1931">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-1932">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1932">Storage</span></span>

* <span data-ttu-id="ec6b9-1933">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1933">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-1934">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1934">VM</span></span>

* <span data-ttu-id="ec6b9-1935">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1935">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="ec6b9-1936">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1936">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="ec6b9-1937">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1937">Auguest 14, 2018</span></span>

<span data-ttu-id="ec6b9-1938">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1938">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-1939">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1939">Core</span></span>

* <span data-ttu-id="ec6b9-1940">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1940">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="ec6b9-1941">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1941">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="ec6b9-1942">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1942">Telemetry</span></span>

* <span data-ttu-id="ec6b9-1943">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1943">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-1944">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1944">ACR</span></span>

* <span data-ttu-id="ec6b9-1945">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1945">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="ec6b9-1946">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1946">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-1947">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1947">ACS</span></span>

* <span data-ttu-id="ec6b9-1948">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1948">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="ec6b9-1949">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1949">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="ec6b9-1950">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1950">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="ec6b9-1951">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1951">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="ec6b9-1952">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1952">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="ec6b9-1953">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1953">AppService</span></span>

* <span data-ttu-id="ec6b9-1954">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1954">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="ec6b9-1955">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1955">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="ec6b9-1956">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1956">BatchAI</span></span>

* <span data-ttu-id="ec6b9-1957">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1957">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="ec6b9-1958">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1958">Container</span></span>

* <span data-ttu-id="ec6b9-1959">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1959">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="ec6b9-1960">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1960">IoT</span></span>

* <span data-ttu-id="ec6b9-1961">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1961">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="ec6b9-1962">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1962">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="ec6b9-1963">IoT Central</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1963">Iot Central</span></span>

* <span data-ttu-id="ec6b9-1964">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1964">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="ec6b9-1965">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1965">KeyVault</span></span>


* <span data-ttu-id="ec6b9-1966">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1966">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="ec6b9-1967">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1967">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="ec6b9-1968">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1968">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="ec6b9-1969">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1969">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="ec6b9-1970">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1970">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="ec6b9-1971">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1971">Relay</span></span>

* <span data-ttu-id="ec6b9-1972">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1972">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-1973">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1973">Sql</span></span>

* <span data-ttu-id="ec6b9-1974">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1974">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-1975">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1975">Storage</span></span>

* <span data-ttu-id="ec6b9-1976">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1976">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="ec6b9-1977">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1977">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="ec6b9-1978">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1978">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="ec6b9-1979">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1979">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="ec6b9-1980">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1980">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-1981">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1981">VM</span></span>

* <span data-ttu-id="ec6b9-1982">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1982">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="ec6b9-1983">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1983">July 31, 2018</span></span>

<span data-ttu-id="ec6b9-1984">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1984">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-1985">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1985">ACR</span></span>

* <span data-ttu-id="ec6b9-1986">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1986">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="ec6b9-1987">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1987">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-1988">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1988">ACS</span></span>

* <span data-ttu-id="ec6b9-1989">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1989">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="ec6b9-1990">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1990">Batch</span></span>

* <span data-ttu-id="ec6b9-1991">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1991">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="ec6b9-1992">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1992">Container</span></span>

* <span data-ttu-id="ec6b9-1993">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1993">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-1994">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1994">Network</span></span>

* <span data-ttu-id="ec6b9-1995">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1995">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="ec6b9-1996">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1996">Resource</span></span>

* <span data-ttu-id="ec6b9-1997">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1997">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="ec6b9-1998">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1998">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-1999">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-1999">Role</span></span>

* <span data-ttu-id="ec6b9-2000">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2000">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="ec6b9-2001">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2001">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="ec6b9-2002">Поиск</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2002">Search</span></span>

* <span data-ttu-id="ec6b9-2003">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2003">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="ec6b9-2004">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2004">Service Bus</span></span>

* <span data-ttu-id="ec6b9-2005">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2005">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="ec6b9-2006">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2006">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="ec6b9-2007">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2007">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="ec6b9-2008">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2008">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-2009">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2009">Storage</span></span>

* <span data-ttu-id="ec6b9-2010">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2010">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="ec6b9-2011">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2011">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2012">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2012">VM</span></span>

* <span data-ttu-id="ec6b9-2013">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2013">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="ec6b9-2014">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2014">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="ec6b9-2015">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2015">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="ec6b9-2016">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2016">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="ec6b9-2017">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2017">July 18, 2018</span></span>

<span data-ttu-id="ec6b9-2018">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2018">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-2019">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2019">Core</span></span>

* <span data-ttu-id="ec6b9-2020">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2020">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="ec6b9-2021">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2021">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="ec6b9-2022">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2022">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-2023">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2023">ACR</span></span>

* <span data-ttu-id="ec6b9-2024">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2024">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="ec6b9-2025">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2025">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="ec6b9-2026">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2026">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="ec6b9-2027">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2027">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-2028">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2028">ACS</span></span>

* <span data-ttu-id="ec6b9-2029">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2029">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-2030">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2030">AppService</span></span>

* <span data-ttu-id="ec6b9-2031">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2031">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="ec6b9-2032">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2032">Batch</span></span>

* <span data-ttu-id="ec6b9-2033">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2033">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="ec6b9-2034">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2034">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ec6b9-2035">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2035">Batch AI</span></span>

* <span data-ttu-id="ec6b9-2036">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2036">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="ec6b9-2037">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2037">Container</span></span>

* <span data-ttu-id="ec6b9-2038">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2038">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="ec6b9-2039">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2039">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-2040">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2040">Network</span></span>

* <span data-ttu-id="ec6b9-2041">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2041">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="ec6b9-2042">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2042">Added `network nic wait`</span></span>
* <span data-ttu-id="ec6b9-2043">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2043">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="ec6b9-2044">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2044">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="ec6b9-2045">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2045">Resource</span></span>

* <span data-ttu-id="ec6b9-2046">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2046">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="ec6b9-2047">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2047">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="ec6b9-2048">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2048">Added `deployment wait` command</span></span>
* <span data-ttu-id="ec6b9-2049">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2049">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-2050">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2050">SQL</span></span>

* <span data-ttu-id="ec6b9-2051">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2051">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="ec6b9-2052">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2052">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="ec6b9-2053">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2053">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-2054">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2054">Storage</span></span>

* <span data-ttu-id="ec6b9-2055">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2055">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2056">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2056">VM</span></span>

* <span data-ttu-id="ec6b9-2057">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2057">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="ec6b9-2058">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2058">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="ec6b9-2059">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2059">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="ec6b9-2060">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2060">July 3, 2018</span></span>

<span data-ttu-id="ec6b9-2061">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2061">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="ec6b9-2062">AKS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2062">AKS</span></span>

* <span data-ttu-id="ec6b9-2063">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2063">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="ec6b9-2064">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2064">July 3, 2018</span></span>

<span data-ttu-id="ec6b9-2065">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2065">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-2066">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2066">Core</span></span>

* <span data-ttu-id="ec6b9-2067">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2067">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-2068">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2068">ACR</span></span>

* <span data-ttu-id="ec6b9-2069">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2069">Added polling build status</span></span>
* <span data-ttu-id="ec6b9-2070">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2070">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="ec6b9-2071">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2071">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-2072">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2072">ACS</span></span>

* <span data-ttu-id="ec6b9-2073">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2073">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="ec6b9-2074">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2074">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="ec6b9-2075">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2075">Updated options for `aks browse` command.</span></span> <span data-ttu-id="ec6b9-2076">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2076">Added `--listen-port` support</span></span>
* <span data-ttu-id="ec6b9-2077">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2077">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="ec6b9-2078">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2078">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="ec6b9-2079">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2079">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-2080">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2080">AppService</span></span>

* <span data-ttu-id="ec6b9-2081">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2081">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="ec6b9-2082">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2082">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="ec6b9-2083">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2083">Backup</span></span>

* <span data-ttu-id="ec6b9-2084">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2084">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="ec6b9-2085">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2085">BatchAI</span></span>

* <span data-ttu-id="ec6b9-2086">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2086">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="ec6b9-2087">Cloud</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2087">Cloud</span></span>

* <span data-ttu-id="ec6b9-2088">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2088">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="ec6b9-2089">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2089">Container</span></span>

* <span data-ttu-id="ec6b9-2090">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2090">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="ec6b9-2091">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2091">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="ec6b9-2092">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2092">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="ec6b9-2093">Расширение</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2093">Extension</span></span>

* <span data-ttu-id="ec6b9-2094">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2094">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-2095">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2095">Network</span></span>

* <span data-ttu-id="ec6b9-2096">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2096">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="ec6b9-2097">Rdbms</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2097">Rdbms</span></span>

* <span data-ttu-id="ec6b9-2098">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2098">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-2099">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2099">Resource</span></span>

* <span data-ttu-id="ec6b9-2100">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2100">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2101">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2101">VM</span></span>

* <span data-ttu-id="ec6b9-2102">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2102">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="ec6b9-2103">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2103">June 25, 2018</span></span>

<span data-ttu-id="ec6b9-2104">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2104">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="ec6b9-2105">CLI</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2105">CLI</span></span>

* <span data-ttu-id="ec6b9-2106">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2106">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="ec6b9-2107">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2107">June 19, 2018</span></span>

<span data-ttu-id="ec6b9-2108">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2108">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-2109">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2109">Core</span></span>

* <span data-ttu-id="ec6b9-2110">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2110">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-2111">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2111">ACR</span></span>

* <span data-ttu-id="ec6b9-2112">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2112">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="ec6b9-2113">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2113">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-2114">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2114">ACS</span></span>

* <span data-ttu-id="ec6b9-2115">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2115">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="ec6b9-2116">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2116">Added `--update` support</span></span>
* <span data-ttu-id="ec6b9-2117">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2117">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="ec6b9-2118">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2118">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="ec6b9-2119">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2119">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="ec6b9-2120">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2120">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="ec6b9-2121">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2121">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="ec6b9-2122">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2122">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-2123">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2123">AppService</span></span>

* <span data-ttu-id="ec6b9-2124">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2124">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="ec6b9-2125">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2125">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="ec6b9-2126">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2126">Batch</span></span>

* <span data-ttu-id="ec6b9-2127">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2127">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ec6b9-2128">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2128">Batch AI</span></span>

* <span data-ttu-id="ec6b9-2129">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2129">Added support for workspaces.</span></span> <span data-ttu-id="ec6b9-2130">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2130">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="ec6b9-2131">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2131">Added support for experiments.</span></span> <span data-ttu-id="ec6b9-2132">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2132">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="ec6b9-2133">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2133">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="ec6b9-2134">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2134">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="ec6b9-2135">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2135">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="ec6b9-2136">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2136">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="ec6b9-2137">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2137">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="ec6b9-2138">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2138">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="ec6b9-2139">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2139">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="ec6b9-2140">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2140">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="ec6b9-2141">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2141">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="ec6b9-2142">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2142">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="ec6b9-2143">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2143">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="ec6b9-2144">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2144">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="ec6b9-2145">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2145">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="ec6b9-2146">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2146">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="ec6b9-2147">[`--config`, `-c`] переименовано в [`--config-file`, `-f`].</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2147">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="ec6b9-2148">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2148">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="ec6b9-2149">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2149">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="ec6b9-2150">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2150">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="ec6b9-2151">Maps</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2151">Maps</span></span>

* <span data-ttu-id="ec6b9-2152">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2152">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-2153">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2153">Network</span></span>

* <span data-ttu-id="ec6b9-2154">Добавлена поддержка `https` в `network lb probe create` ([№ 6571](https://github.com/Azure/azure-cli/issues/6571)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2154">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="ec6b9-2155">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2155">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="ec6b9-2156">#6502</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2156">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="ec6b9-2157">Резервирование</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2157">Reservations</span></span>

* <span data-ttu-id="ec6b9-2158">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2158">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="ec6b9-2159">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2159">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="ec6b9-2160">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2160">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="ec6b9-2161">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2161">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="ec6b9-2162">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2162">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="ec6b9-2163">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2163">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-2164">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2164">Role</span></span>

* <span data-ttu-id="ec6b9-2165">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2165">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-2166">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2166">SQL</span></span>

* <span data-ttu-id="ec6b9-2167">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2167">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-2168">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2168">Storage</span></span>

* <span data-ttu-id="ec6b9-2169">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2169">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2170">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2170">VM</span></span>

* <span data-ttu-id="ec6b9-2171">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2171">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="ec6b9-2172">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2172">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="ec6b9-2173">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2173">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="ec6b9-2174">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2174">June 13, 2018</span></span>

<span data-ttu-id="ec6b9-2175">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2175">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-2176">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2176">Core</span></span>

* <span data-ttu-id="ec6b9-2177">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2177">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="ec6b9-2178">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2178">June 13, 2018</span></span>

<span data-ttu-id="ec6b9-2179">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2179">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="ec6b9-2180">AKS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2180">AKS</span></span>

* <span data-ttu-id="ec6b9-2181">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2181">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="ec6b9-2182">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2182">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="ec6b9-2183">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2183">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="ec6b9-2184">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2184">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="ec6b9-2185">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2185">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-2186">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2186">AppService</span></span>

* <span data-ttu-id="ec6b9-2187">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2187">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="ec6b9-2188">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2188">June 5, 2018</span></span>

<span data-ttu-id="ec6b9-2189">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2189">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="ec6b9-2190">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2190">Interactive</span></span>

* <span data-ttu-id="ec6b9-2191">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2191">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="ec6b9-2192">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2192">June 5, 2018</span></span>

<span data-ttu-id="ec6b9-2193">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2193">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-2194">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2194">Core</span></span>

* <span data-ttu-id="ec6b9-2195">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2195">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="ec6b9-2196">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2196">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-2197">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2197">ACR</span></span>

* <span data-ttu-id="ec6b9-2198">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2198">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="ec6b9-2199">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2199">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="ec6b9-2200">AKS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2200">AKS</span></span>

* <span data-ttu-id="ec6b9-2201">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2201">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="ec6b9-2202">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2202">Batch</span></span>

* <span data-ttu-id="ec6b9-2203">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2203">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="ec6b9-2204">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2204">IOT</span></span>

* <span data-ttu-id="ec6b9-2205">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2205">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-2206">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2206">Network</span></span>

* <span data-ttu-id="ec6b9-2207">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2207">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="ec6b9-2208">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2208">Policy Insights</span></span>

* <span data-ttu-id="ec6b9-2209">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2209">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="ec6b9-2210">ARM</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2210">ARM</span></span>

* <span data-ttu-id="ec6b9-2211">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2211">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-2212">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2212">SQL</span></span>

* <span data-ttu-id="ec6b9-2213">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2213">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="ec6b9-2214">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2214">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="ec6b9-2215">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2215">Storage</span></span>

* <span data-ttu-id="ec6b9-2216">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2216">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2217">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2217">VM</span></span>

* <span data-ttu-id="ec6b9-2218">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2218">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="ec6b9-2219">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2219">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="ec6b9-2220">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2220">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="ec6b9-2221">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2221">May 22, 2018</span></span>

<span data-ttu-id="ec6b9-2222">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2222">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-2223">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2223">Core</span></span>

* <span data-ttu-id="ec6b9-2224">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2224">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-2225">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2225">ACS</span></span>

* <span data-ttu-id="ec6b9-2226">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2226">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="ec6b9-2227">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2227">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-2228">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2228">AppService</span></span>

* <span data-ttu-id="ec6b9-2229">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2229">Improved generic update commands</span></span>
* <span data-ttu-id="ec6b9-2230">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2230">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="ec6b9-2231">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2231">Container</span></span>

* <span data-ttu-id="ec6b9-2232">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2232">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="ec6b9-2233">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2233">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="ec6b9-2234">Расширение</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2234">Extension</span></span>

* <span data-ttu-id="ec6b9-2235">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2235">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="ec6b9-2236">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2236">Interactive</span></span>

* <span data-ttu-id="ec6b9-2237">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2237">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="ec6b9-2238">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2238">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="ec6b9-2239">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2239">KeyVault</span></span>

* <span data-ttu-id="ec6b9-2240">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2240">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-2241">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2241">Network</span></span>

* <span data-ttu-id="ec6b9-2242">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2242">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="ec6b9-2243">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2243">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-2244">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2244">SQL</span></span>

* <span data-ttu-id="ec6b9-2245">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2245">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="ec6b9-2246">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2246">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="ec6b9-2247">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2247">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="ec6b9-2248">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2248">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="ec6b9-2249">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2249">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="ec6b9-2250">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2250">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="ec6b9-2251">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2251">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="ec6b9-2252">`edition`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2252">`edition`.</span></span> <span data-ttu-id="ec6b9-2253">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2253">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="ec6b9-2254">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2254">`elasticPoolName`.</span></span> <span data-ttu-id="ec6b9-2255">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2255">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="ec6b9-2256">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2256">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="ec6b9-2257">`edition`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2257">`edition`.</span></span> <span data-ttu-id="ec6b9-2258">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2258">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="ec6b9-2259">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2259">`dtu`.</span></span> <span data-ttu-id="ec6b9-2260">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2260">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="ec6b9-2261">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2261">`databaseDtuMin`.</span></span> <span data-ttu-id="ec6b9-2262">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2262">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="ec6b9-2263">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2263">`databaseDtuMax`.</span></span> <span data-ttu-id="ec6b9-2264">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2264">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="ec6b9-2265">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2265">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="ec6b9-2266">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2266">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-2267">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2267">Storage</span></span>

* <span data-ttu-id="ec6b9-2268">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2268">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="ec6b9-2269">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2269">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2270">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2270">VM</span></span>

* <span data-ttu-id="ec6b9-2271">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2271">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="ec6b9-2272">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2272">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="ec6b9-2273">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2273">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="ec6b9-2274">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2274">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="ec6b9-2275">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2275">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="ec6b9-2276">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2276">May 7, 2018</span></span>

<span data-ttu-id="ec6b9-2277">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2277">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-2278">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2278">Core</span></span>

* <span data-ttu-id="ec6b9-2279">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2279">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="ec6b9-2280">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2280">Added limited support for positional arguments</span></span>
* <span data-ttu-id="ec6b9-2281">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2281">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="ec6b9-2282">#5591</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2282">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="ec6b9-2283">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2283">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="ec6b9-2284">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2284">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="ec6b9-2285">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2285">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="ec6b9-2286">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2286">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="ec6b9-2287">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2287">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-2288">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2288">ACR</span></span>

* <span data-ttu-id="ec6b9-2289">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2289">Added ACR Build commands</span></span>
* <span data-ttu-id="ec6b9-2290">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2290">Improved resource not found error messages</span></span>
* <span data-ttu-id="ec6b9-2291">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2291">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="ec6b9-2292">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2292">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="ec6b9-2293">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2293">Improved repository commands error messages</span></span>
* <span data-ttu-id="ec6b9-2294">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2294">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-2295">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2295">ACS</span></span>

* <span data-ttu-id="ec6b9-2296">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2296">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="ec6b9-2297">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2297">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="ec6b9-2298">AMS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2298">AMS</span></span>

* <span data-ttu-id="ec6b9-2299">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2299">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-2300">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2300">Appservice</span></span>

* <span data-ttu-id="ec6b9-2301">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2301">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="ec6b9-2302">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2302">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="ec6b9-2303">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2303">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="ec6b9-2304">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2304">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ec6b9-2305">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2305">Batch AI</span></span>

* <span data-ttu-id="ec6b9-2306">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2306">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ec6b9-2307">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2307">Cognitive Services</span></span>

* <span data-ttu-id="ec6b9-2308">Исправлена опечатка в примере для `cognitiveservices account create` ([№ 5603](https://github.com/Azure/azure-cli/issues/5603)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2308">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="ec6b9-2309">Потребление</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2309">Consumption</span></span>

* <span data-ttu-id="ec6b9-2310">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2310">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="ec6b9-2311">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2311">Container</span></span>

* <span data-ttu-id="ec6b9-2312">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2312">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="ec6b9-2313">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2313">Cosmos DB</span></span>

* <span data-ttu-id="ec6b9-2314">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2314">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="ec6b9-2315">DMS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2315">DMS</span></span>

* <span data-ttu-id="ec6b9-2316">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2316">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="ec6b9-2317">Расширение</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2317">Extension</span></span>

* <span data-ttu-id="ec6b9-2318">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2318">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="ec6b9-2319">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2319">Interactive</span></span>

* <span data-ttu-id="ec6b9-2320">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2320">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="ec6b9-2321">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2321">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="ec6b9-2322">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2322">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="ec6b9-2323">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2323">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="ec6b9-2324">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2324">Lab</span></span>

* <span data-ttu-id="ec6b9-2325">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2325">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-2326">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2326">Network</span></span>

* <span data-ttu-id="ec6b9-2327">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2327">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="ec6b9-2328">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2328">Profile</span></span>

* <span data-ttu-id="ec6b9-2329">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2329">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="ec6b9-2330">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2330">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="ec6b9-2331">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2331">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="ec6b9-2332">Redis</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2332">Redis</span></span>

* <span data-ttu-id="ec6b9-2333">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2333">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="ec6b9-2334">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2334">Deprecated `redis list-all`.</span></span> <span data-ttu-id="ec6b9-2335">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2335">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="ec6b9-2336">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2336">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="ec6b9-2337">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2337">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-2338">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2338">Role</span></span>

* <span data-ttu-id="ec6b9-2339">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2339">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-2340">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2340">Storage</span></span>

* <span data-ttu-id="ec6b9-2341">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2341">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="ec6b9-2342">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2342">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="ec6b9-2343">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2343">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="ec6b9-2344">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2344">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="ec6b9-2345">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2345">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2346">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2346">VM</span></span>

* <span data-ttu-id="ec6b9-2347">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2347">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="ec6b9-2348">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2348">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="ec6b9-2349">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2349">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="ec6b9-2350">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2350">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="ec6b9-2351">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2351">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="ec6b9-2352">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2352">Added write accelerator support</span></span>
* <span data-ttu-id="ec6b9-2353">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2353">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="ec6b9-2354">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2354">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="ec6b9-2355">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2355">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="ec6b9-2356">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2356">April 10, 2018</span></span>

<span data-ttu-id="ec6b9-2357">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2357">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-2358">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2358">ACR</span></span>

* <span data-ttu-id="ec6b9-2359">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2359">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-2360">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2360">ACS</span></span>

* <span data-ttu-id="ec6b9-2361">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2361">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-2362">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2362">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="ec6b9-2364">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2364">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="ec6b9-2365">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2365">BatchAI</span></span>

* <span data-ttu-id="ec6b9-2366">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2366">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="ec6b9-2367">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2367">Job level mounting</span></span>
  - <span data-ttu-id="ec6b9-2368">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2368">Environment variables with secret values</span></span>
  - <span data-ttu-id="ec6b9-2369">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2369">Performance counters settings</span></span>
  - <span data-ttu-id="ec6b9-2370">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2370">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="ec6b9-2371">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2371">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="ec6b9-2372">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2372">Usage and limits reporting</span></span>
  - <span data-ttu-id="ec6b9-2373">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2373">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="ec6b9-2374">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2374">Support for custom images</span></span>
  - <span data-ttu-id="ec6b9-2375">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2375">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="ec6b9-2376">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2376">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="ec6b9-2377">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2377">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="ec6b9-2378">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2378">National clouds are supported</span></span>
* <span data-ttu-id="ec6b9-2379">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2379">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="ec6b9-2380">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2380">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="ec6b9-2381">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2381">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="ec6b9-2382">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2382">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="ec6b9-2383">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2383">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="ec6b9-2384">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2384">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="ec6b9-2385">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2385">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="ec6b9-2386">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2386">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="ec6b9-2387">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2387">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="ec6b9-2388">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2388">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="ec6b9-2389">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2389">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="ec6b9-2390">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2390">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="ec6b9-2391">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2391">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="ec6b9-2392">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2392">Billing</span></span>

* <span data-ttu-id="ec6b9-2393">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2393">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="ec6b9-2394">Потребление</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2394">Consumption</span></span>

* <span data-ttu-id="ec6b9-2395">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2395">Added `marketplace` commands</span></span>
* <span data-ttu-id="ec6b9-2396">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2396">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="ec6b9-2397">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2397">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="ec6b9-2398">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2398">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="ec6b9-2399">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2399">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="ec6b9-2400">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2400">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="ec6b9-2401">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2401">Container</span></span>

* <span data-ttu-id="ec6b9-2402">Добавлены параметры подключения тома репозитория Git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2402">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="ec6b9-2403">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2403">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="ec6b9-2404">Расширение</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2404">Extension</span></span>

* <span data-ttu-id="ec6b9-2405">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2405">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="ec6b9-2406">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2406">Interactive</span></span>

* <span data-ttu-id="ec6b9-2407">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2407">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="ec6b9-2408">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2408">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="ec6b9-2409">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2409">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-2410">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2410">Network</span></span>

* <span data-ttu-id="ec6b9-2411">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2411">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="ec6b9-2412">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2412">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="ec6b9-2413">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2413">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="ec6b9-2414">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2414">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="ec6b9-2415">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2415">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="ec6b9-2416">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2416">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="ec6b9-2417">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2417">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="ec6b9-2418">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2418">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="ec6b9-2419">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2419">Profile</span></span>

* <span data-ttu-id="ec6b9-2420">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2420">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="ec6b9-2421">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi` & `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2421">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="ec6b9-2422">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2422">RDBMS</span></span>

* <span data-ttu-id="ec6b9-2423">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2423">Added `georestore` command</span></span>
* <span data-ttu-id="ec6b9-2424">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2424">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-2425">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2425">Resource</span></span>

* <span data-ttu-id="ec6b9-2426">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2426">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="ec6b9-2427">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2427">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-2428">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2428">SQL</span></span>

* <span data-ttu-id="ec6b9-2429">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2429">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-2430">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2430">Storage</span></span>

* <span data-ttu-id="ec6b9-2431">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2431">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2432">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2432">VM</span></span>

* <span data-ttu-id="ec6b9-2433">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2433">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="ec6b9-2434">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2434">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="ec6b9-2436">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2436">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="ec6b9-2437">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2437">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="ec6b9-2438">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2438">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="ec6b9-2439">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2439">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="ec6b9-2440">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2440">March 27, 2018</span></span>

<span data-ttu-id="ec6b9-2441">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2441">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-2442">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2442">Core</span></span>

* <span data-ttu-id="ec6b9-2443">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2443">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-2444">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2444">ACS</span></span>

* <span data-ttu-id="ec6b9-2445">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2445">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-2446">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2446">Appservice</span></span>

* <span data-ttu-id="ec6b9-2447">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2447">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="ec6b9-2448">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2448">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="ec6b9-2449">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2449">Backup</span></span>

* <span data-ttu-id="ec6b9-2450">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2450">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="ec6b9-2451">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2451">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="ec6b9-2452">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2452">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="ec6b9-2453">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2453">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="ec6b9-2454">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2454">Container</span></span>

* <span data-ttu-id="ec6b9-2455">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2455">Added `container exec` command.</span></span> <span data-ttu-id="ec6b9-2456">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2456">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="ec6b9-2457">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2457">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="ec6b9-2458">Расширение</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2458">Extension</span></span>

* <span data-ttu-id="ec6b9-2459">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2459">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="ec6b9-2460">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2460">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="ec6b9-2461">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2461">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="ec6b9-2462">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2462">Interactive</span></span>

* <span data-ttu-id="ec6b9-2463">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2463">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="ec6b9-2464">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2464">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="ec6b9-2465">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2465">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="ec6b9-2466">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2466">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="ec6b9-2467">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2467">Lab</span></span>

* <span data-ttu-id="ec6b9-2468">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2468">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-2469">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2469">Monitor</span></span>

* <span data-ttu-id="ec6b9-2470">Добавлена поддержка аргументов `--top`, `--orderby` и `--namespace` для `metrics list` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2470">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="ec6b9-2471">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2471">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="ec6b9-2472">Добавлена поддержка `--namespace` для `metrics list-definitions` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2472">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-2473">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2473">Network</span></span>

* <span data-ttu-id="ec6b9-2474">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2474">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="ec6b9-2475">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2475">Profile</span></span>

* <span data-ttu-id="ec6b9-2476">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2476">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="ec6b9-2477">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2477">RDBMS</span></span>

* <span data-ttu-id="ec6b9-2478">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2478">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-2479">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2479">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="ec6b9-2481">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2481">Role</span></span>

* <span data-ttu-id="ec6b9-2482">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2482">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="ec6b9-2483">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2483">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="ec6b9-2484">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2484">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="ec6b9-2485">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2485">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="ec6b9-2486">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2486">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-2487">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2487">Storage</span></span>

* <span data-ttu-id="ec6b9-2488">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2488">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="ec6b9-2489">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2489">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2490">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2490">VM</span></span>

* <span data-ttu-id="ec6b9-2491">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2491">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="ec6b9-2492">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2492">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="ec6b9-2493">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2493">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="ec6b9-2494">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2494">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="ec6b9-2495">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2495">March 13, 2018</span></span>

<span data-ttu-id="ec6b9-2496">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2496">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-2497">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2497">ACR</span></span>

* <span data-ttu-id="ec6b9-2498">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2498">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="ec6b9-2499">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2499">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="ec6b9-2500">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2500">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-2501">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2501">ACS</span></span>

* <span data-ttu-id="ec6b9-2502">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2502">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="ec6b9-2503">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2503">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="ec6b9-2504">Помощник</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2504">Advisor</span></span>

* <span data-ttu-id="ec6b9-2505">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2505">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="ec6b9-2506">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2506">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="ec6b9-2507">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2507">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="ec6b9-2508">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2508">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="ec6b9-2509">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2509">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-2510">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2510">Appservice</span></span>

* <span data-ttu-id="ec6b9-2511">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2511">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="ec6b9-2512">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2512">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="ec6b9-2513">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2513">Eventhubs</span></span>

* <span data-ttu-id="ec6b9-2514">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2514">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="ec6b9-2515">Расширение</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2515">Extension</span></span>

* <span data-ttu-id="ec6b9-2516">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2516">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="ec6b9-2517">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2517">Interactive</span></span>

* <span data-ttu-id="ec6b9-2518">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2518">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="ec6b9-2519">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2519">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="ec6b9-2520">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2520">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="ec6b9-2521">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2521">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-2522">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2522">Monitor</span></span>

* <span data-ttu-id="ec6b9-2523">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2523">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="ec6b9-2524">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2524">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="ec6b9-2525">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2525">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="ec6b9-2526">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2526">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-2527">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2527">Network</span></span>

* <span data-ttu-id="ec6b9-2528">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2528">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="ec6b9-2529">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2529">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="ec6b9-2530">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2530">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="ec6b9-2531">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2531">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="ec6b9-2532">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2532">Profile</span></span>

* <span data-ttu-id="ec6b9-2533">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2533">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="ec6b9-2534">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2534">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="ec6b9-2535">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2535">RDBMS</span></span>

* <span data-ttu-id="ec6b9-2536">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2536">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="ec6b9-2537">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2537">Service Bus</span></span>

* <span data-ttu-id="ec6b9-2538">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2538">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-2539">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2539">Storage</span></span>

* <span data-ttu-id="ec6b9-2540">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2540">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="ec6b9-2541">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2541">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2542">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2542">VM</span></span>

* <span data-ttu-id="ec6b9-2543">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2543">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="ec6b9-2544">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2544">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="ec6b9-2545">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2545">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="ec6b9-2546">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2546">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="ec6b9-2547">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2547">February 27, 2018</span></span>

<span data-ttu-id="ec6b9-2548">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2548">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-2549">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2549">Core</span></span>

* <span data-ttu-id="ec6b9-2550">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2550">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="ec6b9-2551">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2551">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="ec6b9-2552">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2552">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-2553">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2553">ACS</span></span>

* <span data-ttu-id="ec6b9-2554">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2554">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="ec6b9-2555">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2555">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="ec6b9-2556">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2556">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="ec6b9-2557">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2557">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-2558">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2558">Appservice</span></span>

* <span data-ttu-id="ec6b9-2559">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2559">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="ec6b9-2560">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2560">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ec6b9-2561">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2561">Cognitive Services</span></span>

* <span data-ttu-id="ec6b9-2562">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2562">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="ec6b9-2563">Потребление</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2563">Consumption</span></span>

* <span data-ttu-id="ec6b9-2564">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2564">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="ec6b9-2565">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2565">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="ec6b9-2566">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2566">Container</span></span>

* <span data-ttu-id="ec6b9-2567">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2567">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-2568">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2568">Network</span></span>

* <span data-ttu-id="ec6b9-2569">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2569">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-2570">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2570">Resource</span></span>

* <span data-ttu-id="ec6b9-2571">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2571">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-2572">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2572">Role</span></span>

* <span data-ttu-id="ec6b9-2573">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2573">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-2574">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2574">SQL</span></span>

* <span data-ttu-id="ec6b9-2575">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2575">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-2576">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2576">Storage</span></span>

* <span data-ttu-id="ec6b9-2577">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2577">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2578">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2578">VM</span></span>

* <span data-ttu-id="ec6b9-2579">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2579">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="ec6b9-2580">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2580">February 13, 2018</span></span>

<span data-ttu-id="ec6b9-2581">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2581">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-2582">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2582">Core</span></span>

* <span data-ttu-id="ec6b9-2583">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2583">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-2584">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2584">ACS</span></span>

* <span data-ttu-id="ec6b9-2585">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2585">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="ec6b9-2586">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2586">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="ec6b9-2587">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2587">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="ec6b9-2588">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2588">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="ec6b9-2589">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2589">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="ec6b9-2590">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2590">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="ec6b9-2591">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2591">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="ec6b9-2592">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2592">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-2593">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2593">Appservice</span></span>

* <span data-ttu-id="ec6b9-2594">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2594">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="ec6b9-2595">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2595">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="ec6b9-2596">CDN</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2596">CDN</span></span>

* <span data-ttu-id="ec6b9-2597">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2597">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="ec6b9-2598">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2598">Container</span></span>

* <span data-ttu-id="ec6b9-2599">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2599">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="ec6b9-2600">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2600">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ec6b9-2601">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2601">CosmosDB</span></span>

* <span data-ttu-id="ec6b9-2602">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2602">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="ec6b9-2603">Расширение</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2603">Extension</span></span>

* <span data-ttu-id="ec6b9-2604">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2604">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="ec6b9-2605">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2605">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="ec6b9-2606">Отзывы</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2606">Feedback</span></span>

* <span data-ttu-id="ec6b9-2607">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2607">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="ec6b9-2608">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2608">Interactive</span></span>

* <span data-ttu-id="ec6b9-2609">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2609">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="ec6b9-2610">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2610">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="ec6b9-2611">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2611">IoT</span></span>

* <span data-ttu-id="ec6b9-2612">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2612">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="ec6b9-2613">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2613">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="ec6b9-2614">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2614">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="ec6b9-2615">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2615">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-2616">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2616">Monitor</span></span>

* <span data-ttu-id="ec6b9-2617">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2617">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-2618">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2618">Network</span></span>

* <span data-ttu-id="ec6b9-2619">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2619">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="ec6b9-2620">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2620">Profile</span></span>

* <span data-ttu-id="ec6b9-2621">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2621">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-2622">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2622">Resource</span></span>

* <span data-ttu-id="ec6b9-2623">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2623">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-2624">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2624">Role</span></span>

* <span data-ttu-id="ec6b9-2625">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2625">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-2626">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2626">SQL</span></span>

* <span data-ttu-id="ec6b9-2627">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2627">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="ec6b9-2628">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2628">Added `sql db rename`</span></span>
* <span data-ttu-id="ec6b9-2629">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2629">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-2630">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2630">Storage</span></span>

* <span data-ttu-id="ec6b9-2631">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2631">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2632">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2632">VM</span></span>

* <span data-ttu-id="ec6b9-2633">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2633">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="ec6b9-2634">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2634">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="ec6b9-2635">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2635">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="ec6b9-2636">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2636">January 31, 2018</span></span>

<span data-ttu-id="ec6b9-2637">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2637">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-2638">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2638">Core</span></span>

* <span data-ttu-id="ec6b9-2639">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2639">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="ec6b9-2640">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2640">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="ec6b9-2641">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2641">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="ec6b9-2642">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2642">Use `--verbose` to see</span></span>
* <span data-ttu-id="ec6b9-2643">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2643">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-2644">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2644">ACS</span></span>

* <span data-ttu-id="ec6b9-2645">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2645">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="ec6b9-2646">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2646">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-2647">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2647">Appservice</span></span>

* <span data-ttu-id="ec6b9-2648">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2648">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="ec6b9-2649">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2649">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="ec6b9-2650">CDN</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2650">CDN</span></span>

* <span data-ttu-id="ec6b9-2651">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2651">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ec6b9-2652">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2652">CosmosDB</span></span>

* <span data-ttu-id="ec6b9-2653">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2653">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="ec6b9-2654">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2654">Interactive</span></span>

* <span data-ttu-id="ec6b9-2655">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2655">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-2656">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2656">Network</span></span>

* <span data-ttu-id="ec6b9-2657">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2657">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="ec6b9-2658">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2658">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="ec6b9-2659">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2659">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="ec6b9-2660">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2660">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="ec6b9-2661">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2661">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="ec6b9-2662">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2662">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="ec6b9-2663">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2663">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="ec6b9-2664">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2664">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="ec6b9-2665">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2665">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="ec6b9-2666">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2666">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="ec6b9-2667">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2667">Profile</span></span>

* <span data-ttu-id="ec6b9-2668">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2668">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-2669">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2669">Resource</span></span>

* <span data-ttu-id="ec6b9-2670">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2670">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-2671">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2671">Storage</span></span>

* <span data-ttu-id="ec6b9-2672">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2672">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="ec6b9-2673">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2673">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="ec6b9-2674">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2674">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="ec6b9-2675">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2675">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="ec6b9-2676">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2676">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2677">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2677">VM</span></span>

* <span data-ttu-id="ec6b9-2678">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2678">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="ec6b9-2679">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2679">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="ec6b9-2680">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2680">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="ec6b9-2681">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2681">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="ec6b9-2682">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2682">January 17, 2018</span></span>

<span data-ttu-id="ec6b9-2683">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2683">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-2684">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2684">ACR</span></span>

* <span data-ttu-id="ec6b9-2685">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2685">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="ec6b9-2686">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2686">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-2687">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2687">ACS</span></span>

* <span data-ttu-id="ec6b9-2688">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2688">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="ec6b9-2689">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2689">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-2690">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2690">Appservice</span></span>

* <span data-ttu-id="ec6b9-2691">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2691">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="ec6b9-2692">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2692">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="ec6b9-2693">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2693">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="ec6b9-2694">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2694">Backup</span></span>

* <span data-ttu-id="ec6b9-2695">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2695">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="ec6b9-2696">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2696">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="ec6b9-2697">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2697">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="ec6b9-2698">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2698">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="ec6b9-2699">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2699">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="ec6b9-2700">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2700">Batch</span></span>

* <span data-ttu-id="ec6b9-2701">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2701">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="ec6b9-2702">Cloud</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2702">Cloud</span></span>

* <span data-ttu-id="ec6b9-2703">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2703">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="ec6b9-2704">Потребление</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2704">Consumption</span></span>

* <span data-ttu-id="ec6b9-2705">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2705">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="ec6b9-2706">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2706">Event Grid</span></span>

* <span data-ttu-id="ec6b9-2707">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2707">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="ec6b9-2708">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2708">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="ec6b9-2709">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2709">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="ec6b9-2710">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2710">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="ec6b9-2711">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2711">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="ec6b9-2712">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2712">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="ec6b9-2713">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2713">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="ec6b9-2714">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2714">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="ec6b9-2715">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2715">Interactive</span></span>

* <span data-ttu-id="ec6b9-2716">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2716">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="ec6b9-2717">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2717">Fixed errors on startup</span></span>
* <span data-ttu-id="ec6b9-2718">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2718">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="ec6b9-2719">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2719">IoT</span></span>

* <span data-ttu-id="ec6b9-2720">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2720">Added support for device provisioning service</span></span>
* <span data-ttu-id="ec6b9-2721">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2721">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="ec6b9-2722">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2722">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-2723">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2723">Monitor</span></span>

* <span data-ttu-id="ec6b9-2724">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2724">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="ec6b9-2725">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2725">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="ec6b9-2726">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2726">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-2727">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2727">Network</span></span>

* <span data-ttu-id="ec6b9-2728">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2728">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="ec6b9-2729">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2729">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="ec6b9-2730">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2730">Profile</span></span>

* <span data-ttu-id="ec6b9-2731">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2731">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-2732">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2732">Role</span></span>

* <span data-ttu-id="ec6b9-2733">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2733">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ec6b9-2734">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2734">Service Fabric</span></span>

* <span data-ttu-id="ec6b9-2735">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2735">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="ec6b9-2736">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2736">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2737">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2737">VM</span></span>

* <span data-ttu-id="ec6b9-2738">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2738">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="ec6b9-2739">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2739">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="ec6b9-2740">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2740">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="ec6b9-2741">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2741">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="ec6b9-2742">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2742">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="ec6b9-2743">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2743">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="ec6b9-2744">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2744">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="ec6b9-2745">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2745">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="ec6b9-2746">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2746">December 19, 2017</span></span>

<span data-ttu-id="ec6b9-2747">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2747">Version 2.0.23</span></span>

* <span data-ttu-id="ec6b9-2748">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2748">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="ec6b9-2749">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2749">Container</span></span>

* <span data-ttu-id="ec6b9-2750">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2750">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-2751">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2751">Network</span></span>

* <span data-ttu-id="ec6b9-2752">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2752">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="ec6b9-2753">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2753">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-2754">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2754">Storage</span></span>

* <span data-ttu-id="ec6b9-2755">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2755">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2756">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2756">VM</span></span>

* <span data-ttu-id="ec6b9-2757">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2757">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="ec6b9-2758">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2758">December 5, 2017</span></span>

<span data-ttu-id="ec6b9-2759">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2759">Version 2.0.22</span></span>

* <span data-ttu-id="ec6b9-2760">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2760">Removed `az component` commands.</span></span> <span data-ttu-id="ec6b9-2761">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2761">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-2762">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2762">Core</span></span>
* <span data-ttu-id="ec6b9-2763">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2763">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="ec6b9-2764">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2764">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-2765">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2765">ACS</span></span>

* <span data-ttu-id="ec6b9-2766">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2766">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="ec6b9-2767">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2767">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="ec6b9-2768">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2768">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="ec6b9-2769">Помощник</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2769">Advisor</span></span>

* <span data-ttu-id="ec6b9-2770">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2770">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-2771">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2771">Appservice</span></span>

* <span data-ttu-id="ec6b9-2772">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2772">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="ec6b9-2773">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2773">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="ec6b9-2774">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2774">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="ec6b9-2775">Потребление</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2775">Consumption</span></span>

* <span data-ttu-id="ec6b9-2776">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2776">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="ec6b9-2777">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2777">Container</span></span>

* <span data-ttu-id="ec6b9-2778">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2778">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-2779">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2779">Monitor</span></span>

* <span data-ttu-id="ec6b9-2780">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2780">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-2781">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2781">Resource</span></span>

* <span data-ttu-id="ec6b9-2782">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2782">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-2783">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2783">Role</span></span>

* <span data-ttu-id="ec6b9-2784">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2784">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="ec6b9-2785">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2785">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="ec6b9-2786">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2786">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-2787">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2787">SQL</span></span>

* <span data-ttu-id="ec6b9-2788">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2788">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="ec6b9-2789">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2789">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2790">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2790">VM</span></span>

* <span data-ttu-id="ec6b9-2791">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2791">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="ec6b9-2792">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2792">November 14, 2017</span></span>

<span data-ttu-id="ec6b9-2793">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2793">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-2794">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2794">ACR</span></span>

* <span data-ttu-id="ec6b9-2795">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2795">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="ec6b9-2796">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2796">ACS</span></span>

* <span data-ttu-id="ec6b9-2797">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2797">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="ec6b9-2798">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2798">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="ec6b9-2799">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2799">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="ec6b9-2800">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2800">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="ec6b9-2801">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2801">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-2802">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2802">Appservice</span></span>

* <span data-ttu-id="ec6b9-2803">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2803">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="ec6b9-2804">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2804">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="ec6b9-2805">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2805">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="ec6b9-2806">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2806">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="ec6b9-2807">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2807">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="ec6b9-2808">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2808">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="ec6b9-2809">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2809">Batch</span></span>

* <span data-ttu-id="ec6b9-2810">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2810">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="ec6b9-2811">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2811">Batchai</span></span>

* <span data-ttu-id="ec6b9-2812">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2812">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="ec6b9-2813">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2813">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="ec6b9-2814">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2814">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="ec6b9-2815">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2815">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="ec6b9-2816">Cloud</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2816">Cloud</span></span>

* <span data-ttu-id="ec6b9-2817">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2817">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="ec6b9-2818">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2818">Container</span></span>

* <span data-ttu-id="ec6b9-2819">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2819">Added support to open multiple ports</span></span>
* <span data-ttu-id="ec6b9-2820">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2820">Added container group restart policy</span></span>
* <span data-ttu-id="ec6b9-2821">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2821">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="ec6b9-2822">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2822">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ec6b9-2823">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2823">Data Lake Analytics</span></span>

* <span data-ttu-id="ec6b9-2824">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2824">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ec6b9-2825">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2825">Data Lake Store</span></span>

* <span data-ttu-id="ec6b9-2826">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2826">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="ec6b9-2827">Расширение</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2827">Extension</span></span>

* <span data-ttu-id="ec6b9-2828">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2828">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="ec6b9-2829">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2829">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="ec6b9-2830">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2830">IoT</span></span>

* <span data-ttu-id="ec6b9-2831">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2831">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-2832">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2832">Monitor</span></span>

* <span data-ttu-id="ec6b9-2833">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2833">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-2834">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2834">Network</span></span>

* <span data-ttu-id="ec6b9-2835">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2835">Added support for CAA DNS records</span></span>
* <span data-ttu-id="ec6b9-2836">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2836">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="ec6b9-2837">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2837">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="ec6b9-2838">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2838">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="ec6b9-2839">Резервирование</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2839">Reservations</span></span>

* <span data-ttu-id="ec6b9-2840">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2840">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-2841">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2841">Resource</span></span>

* <span data-ttu-id="ec6b9-2842">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2842">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-2843">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2843">SQL</span></span>

* <span data-ttu-id="ec6b9-2844">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2844">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-2845">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2845">Storage</span></span>

* <span data-ttu-id="ec6b9-2846">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2846">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="ec6b9-2847">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2847">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="ec6b9-2848">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2848">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="ec6b9-2849">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2849">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="ec6b9-2850">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2850">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="ec6b9-2851">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2851">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="ec6b9-2852">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2852">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2853">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2853">VM</span></span>

* <span data-ttu-id="ec6b9-2854">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2854">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="ec6b9-2855">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2855">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="ec6b9-2856">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2856">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="ec6b9-2857">Переименование `vm format-secret` в `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2857">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="ec6b9-2858">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2858">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="ec6b9-2859">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2859">October 24, 2017</span></span>

<span data-ttu-id="ec6b9-2860">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2860">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-2861">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2861">Core</span></span>

* <span data-ttu-id="ec6b9-2862">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2862">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-2863">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2863">ACR</span></span>

* <span data-ttu-id="ec6b9-2864">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2864">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="ec6b9-2865">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2865">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="ec6b9-2866">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2866">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-2867">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2867">ACS</span></span>

* <span data-ttu-id="ec6b9-2868">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2868">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="ec6b9-2869">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2869">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-2870">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2870">Appservice</span></span>

* <span data-ttu-id="ec6b9-2871">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2871">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="ec6b9-2872">Компонент</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2872">Component</span></span>

* <span data-ttu-id="ec6b9-2873">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2873">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-2874">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2874">Monitor</span></span>

* <span data-ttu-id="ec6b9-2875">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2875">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-2876">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2876">Resource</span></span>

* <span data-ttu-id="ec6b9-2877">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2877">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="ec6b9-2878">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2878">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2879">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2879">VM</span></span>

* <span data-ttu-id="ec6b9-2880">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2880">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="ec6b9-2881">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2881">October 9, 2017</span></span>

<span data-ttu-id="ec6b9-2882">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2882">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-2883">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2883">Core</span></span>

* <span data-ttu-id="ec6b9-2884">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2884">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-2885">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2885">Appservice</span></span>

* <span data-ttu-id="ec6b9-2886">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2886">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="ec6b9-2887">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2887">Batch</span></span>

* <span data-ttu-id="ec6b9-2888">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2888">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="ec6b9-2889">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2889">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="ec6b9-2890">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2890">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="ec6b9-2891">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2891">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="ec6b9-2892">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2892">Batchai</span></span>

* <span data-ttu-id="ec6b9-2893">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2893">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="ec6b9-2894">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2894">Keyvault</span></span>

* <span data-ttu-id="ec6b9-2895">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2895">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="ec6b9-2896">(#4448)</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2896">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="ec6b9-2897">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2897">Network</span></span>

* <span data-ttu-id="ec6b9-2898">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2898">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="ec6b9-2899">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2899">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-2900">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2900">Resource</span></span>

* <span data-ttu-id="ec6b9-2901">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2901">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="ec6b9-2902">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2902">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="ec6b9-2903">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2903">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="ec6b9-2904">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2904">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-2905">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2905">Sql</span></span>

* <span data-ttu-id="ec6b9-2906">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2906">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="ec6b9-2907">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2907">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="ec6b9-2908">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2908">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-2909">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2909">Storage</span></span>

* <span data-ttu-id="ec6b9-2910">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2910">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2911">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2911">Vm</span></span>

* <span data-ttu-id="ec6b9-2912">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2912">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="ec6b9-2913">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2913">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="ec6b9-2914">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2914">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="ec6b9-2915">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2915">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="ec6b9-2916">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2916">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="ec6b9-2917">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2917">September 22, 2017</span></span>

<span data-ttu-id="ec6b9-2918">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2918">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-2919">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2919">Resource</span></span>

* <span data-ttu-id="ec6b9-2920">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2920">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="ec6b9-2921">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2921">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="ec6b9-2922">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2922">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="ec6b9-2923">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2923">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-2924">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2924">Network</span></span>

* <span data-ttu-id="ec6b9-2925">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2925">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="ec6b9-2926">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2926">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="ec6b9-2927">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2927">Added `asg` application security group commands</span></span>
* <span data-ttu-id="ec6b9-2928">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2928">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="ec6b9-2929">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2929">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="ec6b9-2930">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2930">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="ec6b9-2931">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2931">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-2932">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2932">Storage</span></span>

* <span data-ttu-id="ec6b9-2933">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2933">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="ec6b9-2934">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2934">Eventgrid</span></span>

* <span data-ttu-id="ec6b9-2935">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2935">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-2936">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2936">SQL</span></span>

* <span data-ttu-id="ec6b9-2937">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2937">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="ec6b9-2938">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2938">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="ec6b9-2939">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2939">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="ec6b9-2940">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2940">Keyvault</span></span>

* <span data-ttu-id="ec6b9-2941">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2941">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2942">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2942">VM</span></span>

* <span data-ttu-id="ec6b9-2943">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2943">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="ec6b9-2944">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2944">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="ec6b9-2945">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2945">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="ec6b9-2946">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2946">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="ec6b9-2947">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2947">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="ec6b9-2948">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2948">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-2949">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2949">ACS</span></span>

* <span data-ttu-id="ec6b9-2950">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2950">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-2951">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2951">Appservice</span></span>

* <span data-ttu-id="ec6b9-2952">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2952">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="ec6b9-2953">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2953">Backup</span></span>

* <span data-ttu-id="ec6b9-2954">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2954">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="ec6b9-2955">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2955">September 11, 2017</span></span>

<span data-ttu-id="ec6b9-2956">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2956">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="ec6b9-2957">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2957">Core</span></span>

* <span data-ttu-id="ec6b9-2958">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2958">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="ec6b9-2959">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2959">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-2960">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2960">Acs</span></span>

* <span data-ttu-id="ec6b9-2961">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2961">Added `acs list-locations` command</span></span>
* <span data-ttu-id="ec6b9-2962">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2962">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-2963">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2963">Appservice</span></span>

* <span data-ttu-id="ec6b9-2964">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2964">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="ec6b9-2965">CDN</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2965">CDN</span></span>

* <span data-ttu-id="ec6b9-2966">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2966">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="ec6b9-2967">Расширение</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2967">Extension</span></span>

* <span data-ttu-id="ec6b9-2968">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2968">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="ec6b9-2969">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2969">Keyvault</span></span>

* <span data-ttu-id="ec6b9-2970">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2970">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-2971">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2971">Network</span></span>

* <span data-ttu-id="ec6b9-2972">Переименование `vnet list-private-access-services` в `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2972">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="ec6b9-2973">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2973">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="ec6b9-2974">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2974">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="ec6b9-2975">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2975">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="ec6b9-2976">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2976">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-2977">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2977">Resource</span></span>

* <span data-ttu-id="ec6b9-2978">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2978">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="ec6b9-2979">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2979">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="ec6b9-2980">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2980">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="ec6b9-2981">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2981">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-2982">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2982">SQL</span></span>

* <span data-ttu-id="ec6b9-2983">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2983">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-2984">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2984">VM</span></span>

* <span data-ttu-id="ec6b9-2985">Исправлено: Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2985">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="ec6b9-2986">Исправлено: Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2986">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="ec6b9-2987">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2987">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="ec6b9-2988">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2988">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="ec6b9-2989">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2989">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="ec6b9-2990">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2990">August 31, 2017</span></span>

<span data-ttu-id="ec6b9-2991">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2991">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="ec6b9-2992">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2992">Keyvault</span></span>

* <span data-ttu-id="ec6b9-2993">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2993">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="ec6b9-2994">Sf</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2994">Sf</span></span>

* <span data-ttu-id="ec6b9-2995">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2995">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-2996">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2996">Storage</span></span>

* <span data-ttu-id="ec6b9-2997">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2997">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="ec6b9-2998">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2998">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="ec6b9-2999">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-2999">August 28, 2017</span></span>

<span data-ttu-id="ec6b9-3000">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3000">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="ec6b9-3001">CLI</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3001">CLI</span></span>

* <span data-ttu-id="ec6b9-3002">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3002">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-3003">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3003">ACS</span></span>

* <span data-ttu-id="ec6b9-3004">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3004">Corrected preview regions</span></span>
* <span data-ttu-id="ec6b9-3005">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3005">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="ec6b9-3006">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3006">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-3007">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3007">Appservice</span></span>

* <span data-ttu-id="ec6b9-3008">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3008">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="ec6b9-3009">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3009">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="ec6b9-3010">Предоставлен параметр `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3010">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="ec6b9-3011">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3011">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="ec6b9-3012">Исправлено: Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3012">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="ec6b9-3013">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3013">IoT</span></span>

* <span data-ttu-id="ec6b9-3014">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3014">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-3015">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3015">Network</span></span>

* <span data-ttu-id="ec6b9-3016">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3016">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="ec6b9-3017">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3017">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="ec6b9-3018">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3018">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="ec6b9-3019">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3019">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="ec6b9-3020">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3020">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="ec6b9-3021">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3021">Profile</span></span>

* <span data-ttu-id="ec6b9-3022">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3022">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ec6b9-3023">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3023">Service Fabric</span></span>

* <span data-ttu-id="ec6b9-3024">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3024">Preview release</span></span>
* <span data-ttu-id="ec6b9-3025">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3025">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="ec6b9-3026">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3026">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="ec6b9-3027">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3027">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-3028">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3028">Storage</span></span>

* <span data-ttu-id="ec6b9-3029">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3029">Enabled setting blob tier</span></span>
* <span data-ttu-id="ec6b9-3030">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3030">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="ec6b9-3031">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3031">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="ec6b9-3032">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3032">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="ec6b9-3033">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3033">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="ec6b9-3034">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3034">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-3035">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3035">VM</span></span>

* <span data-ttu-id="ec6b9-3036">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3036">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="ec6b9-3037">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3037">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="ec6b9-3038">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3038">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="ec6b9-3039">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3039">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="ec6b9-3040">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3040">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="ec6b9-3041">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3041">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="ec6b9-3042">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3042">August 15, 2017</span></span>

<span data-ttu-id="ec6b9-3043">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3043">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-3044">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3044">ACS</span></span>

* <span data-ttu-id="ec6b9-3045">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3045">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-3046">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3046">Appservice</span></span>

* <span data-ttu-id="ec6b9-3047">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3047">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="ec6b9-3048">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3048">Event Grid</span></span>

* <span data-ttu-id="ec6b9-3049">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3049">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="ec6b9-3050">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3050">August 11, 2017</span></span>

<span data-ttu-id="ec6b9-3051">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3051">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-3052">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3052">ACS</span></span>

* <span data-ttu-id="ec6b9-3053">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3053">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="ec6b9-3054">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3054">Batch</span></span>

* <span data-ttu-id="ec6b9-3055">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3055">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="ec6b9-3056">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3056">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="ec6b9-3057">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3057">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="ec6b9-3058">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3058">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="ec6b9-3059">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3059">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="ec6b9-3060">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3060">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="ec6b9-3061">Компонент</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3061">Component</span></span>

* <span data-ttu-id="ec6b9-3062">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3062">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="ec6b9-3063">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3063">Container</span></span>

* <span data-ttu-id="ec6b9-3064">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3064">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="ec6b9-3065">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3065">Data Lake Store</span></span>

* <span data-ttu-id="ec6b9-3066">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3066">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="ec6b9-3067">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3067">Event Grid</span></span>

* <span data-ttu-id="ec6b9-3068">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3068">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-3069">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3069">Network</span></span>

* <span data-ttu-id="ec6b9-3070">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3070">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="ec6b9-3071">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3071">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="ec6b9-3072">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3072">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="ec6b9-3073">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3073">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="ec6b9-3074">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3074">Profile</span></span>

* <span data-ttu-id="ec6b9-3075">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3075">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-3076">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3076">Storage</span></span>

* <span data-ttu-id="ec6b9-3077">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3077">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-3078">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3078">VM</span></span>

* <span data-ttu-id="ec6b9-3079">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3079">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="ec6b9-3080">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3080">Exposed `list-skus` command</span></span>
* <span data-ttu-id="ec6b9-3081">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3081">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="ec6b9-3082">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3082">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="ec6b9-3083">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3083">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="ec6b9-3084">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3084">July 28, 2017</span></span>

<span data-ttu-id="ec6b9-3085">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3085">Version 2.0.12</span></span>

* <span data-ttu-id="ec6b9-3086">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3086">Added container commands</span></span>
* <span data-ttu-id="ec6b9-3087">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3087">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="ec6b9-3088">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3088">Core</span></span>

* <span data-ttu-id="ec6b9-3089">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3089">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="ec6b9-3090">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3090">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="ec6b9-3091">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3091">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="ec6b9-3092">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3092">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="ec6b9-3093">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3093">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="ec6b9-3094">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3094">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="ec6b9-3095">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3095">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="ec6b9-3096">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3096">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="ec6b9-3097">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3097">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="ec6b9-3098">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3098">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="ec6b9-3099">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3099">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="ec6b9-3100">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3100">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="ec6b9-3101">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3101">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="ec6b9-3102">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3102">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="ec6b9-3103">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3103">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="ec6b9-3104">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3104">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="ec6b9-3105">ACR</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3105">ACR</span></span>

* <span data-ttu-id="ec6b9-3106">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3106">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="ec6b9-3107">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3107">Support SKU update for managed registries</span></span>
* <span data-ttu-id="ec6b9-3108">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3108">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="ec6b9-3109">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3109">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="ec6b9-3110">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3110">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="ec6b9-3111">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3111">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-3112">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3112">ACS</span></span>

* <span data-ttu-id="ec6b9-3113">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3113">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-3114">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3114">Appservice</span></span>

* <span data-ttu-id="ec6b9-3115">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3115">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="ec6b9-3116">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3116">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="ec6b9-3117">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3117">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="ec6b9-3118">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3118">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="ec6b9-3119">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3119">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="ec6b9-3120">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3120">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="ec6b9-3121">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3121">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="ec6b9-3122">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3122">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="ec6b9-3123">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3123">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="ec6b9-3124">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3124">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="ec6b9-3125">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3125">Batch</span></span>

* <span data-ttu-id="ec6b9-3126">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3126">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="ec6b9-3127">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3127">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="ec6b9-3128">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3128">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="ec6b9-3129">CDN</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3129">CDN</span></span>

* <span data-ttu-id="ec6b9-3130">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3130">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="ec6b9-3131">Cloud</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3131">Cloud</span></span>

* <span data-ttu-id="ec6b9-3132">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3132">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="ec6b9-3133">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3133">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="ec6b9-3134">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3134">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="ec6b9-3135">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3135">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="ec6b9-3136">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3136">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ec6b9-3137">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3137">CosmosDB</span></span>

* <span data-ttu-id="ec6b9-3138">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3138">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="ec6b9-3139">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3139">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ec6b9-3140">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3140">Data Lake Analytics</span></span>

* <span data-ttu-id="ec6b9-3141">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3141">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="ec6b9-3142">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3142">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="ec6b9-3143">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3143">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ec6b9-3144">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3144">Data Lake Store</span></span>

* <span data-ttu-id="ec6b9-3145">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3145">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="ec6b9-3146">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3146">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="ec6b9-3147">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3147">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="ec6b9-3148">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3148">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="ec6b9-3149">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3149">Interactive</span></span>

* <span data-ttu-id="ec6b9-3150">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3150">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="ec6b9-3151">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3151">Increased test coverage</span></span>
* <span data-ttu-id="ec6b9-3152">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3152">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="ec6b9-3153">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3153">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="ec6b9-3154">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3154">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="ec6b9-3155">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3155">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="ec6b9-3156">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3156">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="ec6b9-3157">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3157">Added `--progress` flag</span></span>
* <span data-ttu-id="ec6b9-3158">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3158">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="ec6b9-3159">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3159">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="ec6b9-3160">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3160">IoT</span></span>

* <span data-ttu-id="ec6b9-3161">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3161">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="ec6b9-3162">(3934).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3162">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="ec6b9-3163">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3163">Key vault</span></span>

* <span data-ttu-id="ec6b9-3164">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3164">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="ec6b9-3165">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3165">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="ec6b9-3166">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3166">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="ec6b9-3167">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3167">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="ec6b9-3168">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3168">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="ec6b9-3169">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3169">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="ec6b9-3170">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3170">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="ec6b9-3171">(3307).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3171">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="ec6b9-3172">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3172">Lab</span></span>

* <span data-ttu-id="ec6b9-3173">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3173">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="ec6b9-3174">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3174">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-3175">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3175">Monitor</span></span>

* <span data-ttu-id="ec6b9-3176">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3176">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="ec6b9-3177">Переименование `monitor alert-rule-incidents list` в `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3177">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="ec6b9-3178">Переименование `monitor alert-rule-incidents show` в `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3178">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="ec6b9-3179">Переименование `monitor metric-defintions list` в `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3179">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="ec6b9-3180">Переименование `monitor alert-rules` в `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3180">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="ec6b9-3181">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3181">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="ec6b9-3182">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3182">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="ec6b9-3183">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3183">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="ec6b9-3184">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3184">`location` no longer required</span></span>
  * <span data-ttu-id="ec6b9-3185">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3185">Add name and ID support for target</span></span>
  * <span data-ttu-id="ec6b9-3186">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3186">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="ec6b9-3187">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3187">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="ec6b9-3188">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3188">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="ec6b9-3189">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3189">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="ec6b9-3190">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3190">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="ec6b9-3191">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3191">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-3192">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3192">Network</span></span>

* <span data-ttu-id="ec6b9-3193">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3193">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="ec6b9-3194">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3194">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="ec6b9-3195">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3195">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="ec6b9-3196">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3196">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="ec6b9-3197">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3197">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="ec6b9-3198">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3198">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="ec6b9-3199">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3199">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="ec6b9-3200">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3200">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="ec6b9-3201">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3201">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="ec6b9-3202">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3202">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="ec6b9-3203">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3203">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="ec6b9-3204">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3204">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="ec6b9-3205">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3205">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="ec6b9-3206">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3206">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="ec6b9-3207">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3207">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="ec6b9-3208">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3208">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="ec6b9-3209">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3209">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="ec6b9-3210">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3210">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="ec6b9-3211">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3211">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="ec6b9-3212">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3212">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="ec6b9-3213">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3213">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="ec6b9-3214">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3214">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="ec6b9-3215">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3215">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="ec6b9-3216">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3216">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="ec6b9-3217">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3217">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="ec6b9-3218">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3218">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="ec6b9-3219">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3219">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="ec6b9-3220">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3220">Profile</span></span>

* <span data-ttu-id="ec6b9-3221">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3221">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="ec6b9-3222">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3222">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="ec6b9-3223">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3223">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="ec6b9-3224">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3224">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="ec6b9-3225">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3225">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="ec6b9-3226">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3226">RDBMS</span></span>

* <span data-ttu-id="ec6b9-3227">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3227">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="ec6b9-3228">Исправлена проблема с обработкой `%s` из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3228">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="ec6b9-3229">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3229">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="ec6b9-3230">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3230">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-3231">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3231">Resource</span></span>

* <span data-ttu-id="ec6b9-3232">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3232">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="ec6b9-3233">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3233">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="ec6b9-3234">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3234">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="ec6b9-3235">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3235">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="ec6b9-3236">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3236">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="ec6b9-3237">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3237">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="ec6b9-3238">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3238">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="ec6b9-3239">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3239">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-3240">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3240">Role</span></span>

* <span data-ttu-id="ec6b9-3241">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3241">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="ec6b9-3242">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3242">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="ec6b9-3243">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3243">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="ec6b9-3244">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3244">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="ec6b9-3245">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3245">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ec6b9-3246">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3246">Service Fabric</span></span>
* <span data-ttu-id="ec6b9-3247">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3247">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="ec6b9-3248">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3248">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="ec6b9-3249">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3249">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-3250">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3250">SQL</span></span>

* <span data-ttu-id="ec6b9-3251">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3251">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="ec6b9-3252">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3252">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="ec6b9-3253">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3253">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-3254">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3254">Storage</span></span>

* <span data-ttu-id="ec6b9-3255">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3255">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="ec6b9-3256">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3256">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="ec6b9-3257">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3257">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="ec6b9-3258">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3258">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="ec6b9-3259">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3259">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="ec6b9-3260">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3260">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-3261">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3261">VM</span></span>

* <span data-ttu-id="ec6b9-3262">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3262">Support configuring nsg</span></span>
* <span data-ttu-id="ec6b9-3263">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3263">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="ec6b9-3264">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3264">Support managed service identities</span></span>
* <span data-ttu-id="ec6b9-3265">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3265">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="ec6b9-3266">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3266">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="ec6b9-3267">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3267">May 10, 2017</span></span>

<span data-ttu-id="ec6b9-3268">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3268">Version 2.0.6</span></span>

* <span data-ttu-id="ec6b9-3269">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3269">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="ec6b9-3270">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3270">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="ec6b9-3271">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3271">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="ec6b9-3272">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3272">Include Cognitive Services module</span></span>
* <span data-ttu-id="ec6b9-3273">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3273">Include Service Fabric module</span></span>
* <span data-ttu-id="ec6b9-3274">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3274">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="ec6b9-3275">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3275">Add support for CDN commands</span></span>
* <span data-ttu-id="ec6b9-3276">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3276">Remove Container module</span></span>
* <span data-ttu-id="ec6b9-3277">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3277">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="ec6b9-3278">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3278">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="ec6b9-3279">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3279">Core</span></span>

* <span data-ttu-id="ec6b9-3280">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3280">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="ec6b9-3281">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([#2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3281">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="ec6b9-3282">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3282">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="ec6b9-3283">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3283">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="ec6b9-3284">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3284">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="ec6b9-3285">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3285">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="ec6b9-3286">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3286">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="ec6b9-3287">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3287">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="ec6b9-3288">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3288">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="ec6b9-3289">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3289">core: Improved performance</span></span>
* <span data-ttu-id="ec6b9-3290">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3290">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="ec6b9-3291">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3291">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-3292">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3292">ACS</span></span>

* <span data-ttu-id="ec6b9-3293">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3293">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="ec6b9-3294">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3294">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="ec6b9-3295">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3295">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="ec6b9-3296">Удален профиль Windows перед вызовом метода PUT для команды scale ([#2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3296">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-3297">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3297">AppService</span></span>

* <span data-ttu-id="ec6b9-3298">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3298">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="ec6b9-3299">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3299">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="ec6b9-3300">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3300">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="ec6b9-3301">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3301">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="ec6b9-3302">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3302">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="ec6b9-3303">Включена поддержка настройки строк подключения ([#2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3303">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="ec6b9-3304">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3304">support slot swap with preview</span></span>
* <span data-ttu-id="ec6b9-3305">Устранены ошибки из команд службы приложений ([#2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3305">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="ec6b9-3306">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([#2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3306">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ec6b9-3307">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3307">CosmosDB</span></span>

* <span data-ttu-id="ec6b9-3308">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3308">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="ec6b9-3309">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3309">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="ec6b9-3310">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3310">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="ec6b9-3311">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3311">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ec6b9-3312">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3312">Data Lake Analytics</span></span>

* <span data-ttu-id="ec6b9-3313">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3313">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="ec6b9-3314">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3314">Add support for new catalog item type: package.</span></span> <span data-ttu-id="ec6b9-3315">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3315">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="ec6b9-3316">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3316">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="ec6b9-3317">Таблица</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3317">Table</span></span>
  * <span data-ttu-id="ec6b9-3318">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3318">Table valued function</span></span>
  * <span data-ttu-id="ec6b9-3319">Представление</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3319">View</span></span>
  * <span data-ttu-id="ec6b9-3320">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3320">Table Statistics.</span></span> <span data-ttu-id="ec6b9-3321">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3321">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ec6b9-3322">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3322">Data Lake Store</span></span>

* <span data-ttu-id="ec6b9-3323">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3323">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="ec6b9-3324">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3324">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="ec6b9-3325">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3325">missed help for access show.</span></span> <span data-ttu-id="ec6b9-3326">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3326">adding it.</span></span> <span data-ttu-id="ec6b9-3327">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3327">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="ec6b9-3328">Поиск</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3328">Find</span></span>

* <span data-ttu-id="ec6b9-3329">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3329">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="ec6b9-3330">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3330">KeyVault</span></span>

* <span data-ttu-id="ec6b9-3331">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3331">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="ec6b9-3332">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3332">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="ec6b9-3333">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3333">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="ec6b9-3334">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3334">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="ec6b9-3335">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3335">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="ec6b9-3336">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3336">Lab</span></span>

* <span data-ttu-id="ec6b9-3337">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3337">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="ec6b9-3338">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3338">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="ec6b9-3339">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3339">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="ec6b9-3340">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3340">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="ec6b9-3341">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3341">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="ec6b9-3342">Монитор</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3342">Monitor</span></span>

* <span data-ttu-id="ec6b9-3343">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3343">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="ec6b9-3344">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3344">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="ec6b9-3345">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3345">Network</span></span>

* <span data-ttu-id="ec6b9-3346">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3346">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="ec6b9-3347">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3347">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="ec6b9-3348">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3348">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="ec6b9-3349">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3349">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="ec6b9-3350">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3350">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="ec6b9-3351">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3351">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="ec6b9-3352">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3352">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="ec6b9-3353">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3353">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="ec6b9-3354">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3354">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="ec6b9-3355">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3355">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="ec6b9-3356">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3356">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="ec6b9-3357">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3357">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="ec6b9-3358">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3358">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="ec6b9-3359">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3359">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="ec6b9-3360">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3360">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="ec6b9-3361">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3361">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="ec6b9-3362">Профиль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3362">Profile</span></span>

* <span data-ttu-id="ec6b9-3363">Включена поддержка входа при отсутствии подписок ([#2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3363">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="ec6b9-3364">Включена поддержка сокращенных имен параметров в команде az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3364">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="ec6b9-3365">Redis</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3365">Redis</span></span>

* <span data-ttu-id="ec6b9-3366">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3366">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="ec6b9-3367">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3367">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="ec6b9-3368">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3368">Resource</span></span>

* <span data-ttu-id="ec6b9-3369">Добавлены команды определения managedapp и managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3369">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="ec6b9-3370">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3370">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="ec6b9-3371">Включена поддержка создания универсального ресурса ([#2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3371">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="ec6b9-3372">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3372">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="ec6b9-3373">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3373">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="ec6b9-3374">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3374">Add docs for az lock update.</span></span> <span data-ttu-id="ec6b9-3375">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3375">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="ec6b9-3376">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3376">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="ec6b9-3377">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3377">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="ec6b9-3378">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3378">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="ec6b9-3379">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3379">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="ec6b9-3380">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([#2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3380">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="ec6b9-3381">Роль</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3381">Role</span></span>

* <span data-ttu-id="ec6b9-3382">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([#2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3382">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="ec6b9-3383">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3383">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="ec6b9-3384">Роль: устранены проблемы при обновлении определения роли ([#2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3384">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="ec6b9-3385">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3385">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="ec6b9-3386">SQL</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3386">SQL</span></span>

* <span data-ttu-id="ec6b9-3387">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3387">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="ec6b9-3388">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3388">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="ec6b9-3389">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3389">Storage</span></span>

* <span data-ttu-id="ec6b9-3390">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3390">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="ec6b9-3391">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3391">Add support for incremental blob copy</span></span>
* <span data-ttu-id="ec6b9-3392">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3392">Add support for large block blob upload</span></span>
* <span data-ttu-id="ec6b9-3393">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3393">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-3394">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3394">VM</span></span>

* <span data-ttu-id="ec6b9-3395">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3395">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="ec6b9-3396">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3396">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="ec6b9-3397">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3397">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="ec6b9-3398">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3398">az vm/vmss disk</span></span>
  3. <span data-ttu-id="ec6b9-3399">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3399">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="ec6b9-3400">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3400">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="ec6b9-3401">vm/vmss: добавлена поддержка создания из образа Marketplace, для которого требуются сведения о плане ([#1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3401">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="ec6b9-3402">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3402">April 3, 2017</span></span>

<span data-ttu-id="ec6b9-3403">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3403">Version 2.0.2</span></span>

<span data-ttu-id="ec6b9-3404">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3404">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="ec6b9-3405">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3405">Core</span></span>

* <span data-ttu-id="ec6b9-3406">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3406">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="ec6b9-3407">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3407">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="ec6b9-3408">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3408">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="ec6b9-3409">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3409">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ec6b9-3410">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3410">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="ec6b9-3411">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3411">Add prompting for missing template parameters.</span></span> <span data-ttu-id="ec6b9-3412">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3412">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="ec6b9-3413">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3413">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="ec6b9-3414">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3414">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="ec6b9-3415">ACS</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3415">ACS</span></span>

* <span data-ttu-id="ec6b9-3416">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3416">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="ec6b9-3417">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3417">Add support for ssh key password prompting.</span></span> <span data-ttu-id="ec6b9-3418">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3418">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="ec6b9-3419">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3419">Add support for windows clusters.</span></span> <span data-ttu-id="ec6b9-3420">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3420">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="ec6b9-3421">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3421">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="ec6b9-3422">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3422">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="ec6b9-3423">AppService</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3423">AppService</span></span>

* <span data-ttu-id="ec6b9-3424">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3424">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="ec6b9-3425">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3425">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="ec6b9-3426">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3426">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="ec6b9-3427">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3427">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="ec6b9-3428">Data Lake</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3428">DataLake</span></span>

* <span data-ttu-id="ec6b9-3429">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3429">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="ec6b9-3430">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3430">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="ec6b9-3431">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3431">DocuemntDB</span></span>

* <span data-ttu-id="ec6b9-3432">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3432">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="ec6b9-3433">ВМ</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3433">VM</span></span>

* <span data-ttu-id="ec6b9-3434">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3434">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="ec6b9-3435">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3435">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="ec6b9-3436">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3436">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="ec6b9-3437">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3437">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ec6b9-3438">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3438">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="ec6b9-3439">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3439">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="ec6b9-3440">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3440">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="ec6b9-3441">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3441">February 27, 2017</span></span>

<span data-ttu-id="ec6b9-3442">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3442">Version 2.0.0</span></span>

<span data-ttu-id="ec6b9-3443">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3443">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="ec6b9-3444">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3444">Container Service (acs)</span></span>
- <span data-ttu-id="ec6b9-3445">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3445">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="ec6b9-3446">Сеть</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3446">Networking</span></span>
- <span data-ttu-id="ec6b9-3447">Память</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3447">Storage</span></span>

<span data-ttu-id="ec6b9-3448">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3448">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="ec6b9-3449">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3449">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="ec6b9-3450">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3450">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="ec6b9-3451">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3451">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="ec6b9-3452">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3452">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="ec6b9-3453">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3453">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="ec6b9-3454">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3454">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="ec6b9-3455">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3455">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="ec6b9-3456">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="ec6b9-3456">Provide feedback from the command line with the `az feedback` command</span></span>

